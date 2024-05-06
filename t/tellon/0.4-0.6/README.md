# Comparing `tmp/tellon-0.4.tar.gz` & `tmp/tellon-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellon-0.4.tar", last modified: Sat May  4 22:55:20 2024, max compression
+gzip compressed data, was "tellon-0.6.tar", last modified: Mon May  6 20:47:05 2024, max compression
```

## Comparing `tellon-0.4.tar` & `tellon-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 22:55:20.388554 tellon-0.4/
--rw-rw-rw-   0        0        0      100 2024-05-04 22:49:28.000000 tellon-0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      374 2024-05-04 22:55:20.382561 tellon-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-04 22:55:20.388554 tellon-0.4/setup.cfg
--rw-rw-rw-   0        0        0      463 2024-05-04 22:53:35.000000 tellon-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 22:55:20.296620 tellon-0.4/tellon/
--rw-rw-rw-   0        0        0     1004 2024-05-04 22:53:56.000000 tellon-0.4/tellon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 22:55:20.378563 tellon-0.4/tellon.egg-info/
--rw-rw-rw-   0        0        0      374 2024-05-04 22:55:19.000000 tellon-0.4/tellon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-04 22:55:19.000000 tellon-0.4/tellon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 22:55:19.000000 tellon-0.4/tellon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-04 22:55:19.000000 tellon-0.4/tellon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 22:55:19.000000 tellon-0.4/tellon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 20:47:05.202171 tellon-0.6/
+-rw-rw-rw-   0        0        0      100 2024-05-04 22:49:28.000000 tellon-0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      374 2024-05-06 20:47:05.195190 tellon-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-06 20:47:05.202171 tellon-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      463 2024-05-06 20:44:48.000000 tellon-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 20:47:05.101303 tellon-0.6/tellon/
+-rw-rw-rw-   0        0        0     1208 2024-05-06 20:46:37.000000 tellon-0.6/tellon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 20:47:05.188184 tellon-0.6/tellon.egg-info/
+-rw-rw-rw-   0        0        0      374 2024-05-06 20:47:03.000000 tellon-0.6/tellon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-06 20:47:03.000000 tellon-0.6/tellon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 20:47:03.000000 tellon-0.6/tellon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-06 20:47:03.000000 tellon-0.6/tellon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 20:47:03.000000 tellon-0.6/tellon.egg-info/top_level.txt
```

### Comparing `tellon-0.4/tellon/__init__.py` & `tellon-0.6/tellon/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import os
 try:
- import cloudscraper
+ import cloudscraper,random
+ 
 except:
  os.system('pip install cloudscraper')
 
+proxy_list =  open('proxy.txt','r').read().splitlines()
+prox = random.choice(proxy_list)
+proxy = {"https://" : prox, "http://" : prox}
 whisper = cloudscraper.create_scraper( 
     browser={ 
         'browser': 'chrome', 
         'platform': 'windows', 
         'desktop': True 
     } 
 )
 
 def Search_Tellonym(Query:str):
- response=whisper.get(f'https://api.tellonym.me/search/users?searchString={Query}&term={Query}&limit=25').json()
+ response=whisper.get(f'https://api.tellonym.me/search/users?searchString={Query}&term={Query}&limit=25',proxies=proxy).json()
  return response
 
 
 def Check_Tellonym_User(User:str):
- res = whisper.get(f'https://api.tellonym.me/accounts/check?username={User}&limit=25').json()
+ res = whisper.get(f'https://api.tellonym.me/accounts/check?username={User}&limit=25',proxies=proxy).json()
  return res
  
 
 def Check_Tellonym_Email(email:str):
  e1 = email.split('@')[0]
  e2 = email.split('@')[1]
  whis = cloudscraper.create_scraper(browser={ 'browser': 'chrome', 'platform': 'windows', 'desktop': True })
- res = whis.get(f'https://api.tellonym.me/accounts/check?email={e1}%40{e2}&limit=13').json()
+ res = whis.get(f'https://api.tellonym.me/accounts/check?email={e1}%40{e2}&limit=13',proxies=proxy).json()
  return res 
  
 
 def Info_Account(User:str):
- r = whisper.get(f'https://api.tellonym.me/profiles/name/{User}?limit=13').json()
+ r = whisper.get(f'https://api.tellonym.me/profiles/name/{User}?limit=13',proxies=proxy).json()
  return r
```

