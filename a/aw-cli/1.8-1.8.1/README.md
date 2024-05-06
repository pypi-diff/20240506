# Comparing `tmp/aw-cli-1.8.tar.gz` & `tmp/aw-cli-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aw-cli-1.8.tar", last modified: Sun Mar  3 20:04:53 2024, max compression
+gzip compressed data, was "aw-cli-1.8.1.tar", last modified: Mon May  6 15:36:48 2024, max compression
```

## Comparing `aw-cli-1.8.tar` & `aw-cli-1.8.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-03-03 20:04:53.746349 aw-cli-1.8/
--rw-r--r--   0 fexh      (1000) fexh      (1000)    35149 2024-03-03 20:04:32.000000 aw-cli-1.8/LICENSE
--rw-r--r--   0 fexh      (1000) fexh      (1000)     5437 2024-03-03 20:04:53.746349 aw-cli-1.8/PKG-INFO
--rw-r--r--   0 fexh      (1000) fexh      (1000)     5046 2024-03-03 20:04:32.000000 aw-cli-1.8/README.md
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-03-03 20:04:53.746349 aw-cli-1.8/aw_cli.egg-info/
--rw-r--r--   0 fexh      (1000) fexh      (1000)     5437 2024-03-03 20:04:53.000000 aw-cli-1.8/aw_cli.egg-info/PKG-INFO
--rw-r--r--   0 fexh      (1000) fexh      (1000)      389 2024-03-03 20:04:53.000000 aw-cli-1.8/aw_cli.egg-info/SOURCES.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)        1 2024-03-03 20:04:53.000000 aw-cli-1.8/aw_cli.egg-info/dependency_links.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)       42 2024-03-03 20:04:53.000000 aw-cli-1.8/aw_cli.egg-info/entry_points.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)       40 2024-03-03 20:04:53.000000 aw-cli-1.8/aw_cli.egg-info/requires.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)        6 2024-03-03 20:04:53.000000 aw-cli-1.8/aw_cli.egg-info/top_level.txt
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-03-03 20:04:53.746349 aw-cli-1.8/awcli/
--rw-r--r--   0 fexh      (1000) fexh      (1000)        0 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/__init__.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     4424 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/anilist.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     3874 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/anime.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2930 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/arg_parser.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)    26940 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/run.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     9319 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/utilities.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)       16 2024-03-03 20:04:32.000000 aw-cli-1.8/awcli/version.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)       38 2024-03-03 20:04:53.746349 aw-cli-1.8/setup.cfg
--rw-r--r--   0 fexh      (1000) fexh      (1000)      752 2024-03-03 20:04:32.000000 aw-cli-1.8/setup.py
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-03-03 20:04:53.746349 aw-cli-1.8/tests/
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2025 2024-03-03 20:04:32.000000 aw-cli-1.8/tests/test_anime.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)      500 2024-03-03 20:04:32.000000 aw-cli-1.8/tests/test_run.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     3585 2024-03-03 20:04:32.000000 aw-cli-1.8/tests/test_utilities.py
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-05-06 15:36:48.088442 aw-cli-1.8.1/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    35149 2024-05-06 15:36:03.000000 aw-cli-1.8.1/LICENSE
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     5439 2024-05-06 15:36:48.088442 aw-cli-1.8.1/PKG-INFO
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     5046 2024-05-06 15:36:03.000000 aw-cli-1.8.1/README.md
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-05-06 15:36:48.085109 aw-cli-1.8.1/aw_cli.egg-info/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     5439 2024-05-06 15:36:48.000000 aw-cli-1.8.1/aw_cli.egg-info/PKG-INFO
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      389 2024-05-06 15:36:48.000000 aw-cli-1.8.1/aw_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        1 2024-05-06 15:36:48.000000 aw-cli-1.8.1/aw_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       42 2024-05-06 15:36:48.000000 aw-cli-1.8.1/aw_cli.egg-info/entry_points.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       40 2024-05-06 15:36:48.000000 aw-cli-1.8.1/aw_cli.egg-info/requires.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        6 2024-05-06 15:36:48.000000 aw-cli-1.8.1/aw_cli.egg-info/top_level.txt
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-05-06 15:36:48.085109 aw-cli-1.8.1/awcli/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        0 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/__init__.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     4424 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/anilist.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     3874 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/anime.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2930 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/arg_parser.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    27145 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/run.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     9327 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/utilities.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       18 2024-05-06 15:36:03.000000 aw-cli-1.8.1/awcli/version.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       38 2024-05-06 15:36:48.088442 aw-cli-1.8.1/setup.cfg
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      754 2024-05-06 15:36:03.000000 aw-cli-1.8.1/setup.py
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2024-05-06 15:36:48.085109 aw-cli-1.8.1/tests/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2025 2024-05-06 15:36:03.000000 aw-cli-1.8.1/tests/test_anime.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      500 2024-05-06 15:36:03.000000 aw-cli-1.8.1/tests/test_run.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     3585 2024-05-06 15:36:03.000000 aw-cli-1.8.1/tests/test_utilities.py
```

### Comparing `aw-cli-1.8/LICENSE` & `aw-cli-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aw-cli-1.8/PKG-INFO` & `aw-cli-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aw-cli
-Version: 1.8
+Version: 1.8.1
 Summary: guarda anime dal terminale e molto altro!
 Home-page: https://github.com/fexh10/aw-cli
 Author: fexh10
 License: GPL-3.0
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aw-cli Version: 1.8 Summary: guarda anime dal
+Metadata-Version: 2.1 Name: aw-cli Version: 1.8.1 Summary: guarda anime dal
 terminale e molto altro! Home-page: https://github.com/fexh10/aw-cli Author:
 fexh10 License: GPL-3.0 Requires-Python: >3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: bs4 Requires-Dist: requests
 Requires-Dist: lxml Requires-Dist: pySmartDL Requires-Dist: wheel Requires-
 Dist: regex # aw-cli
                 ******** GGuuaarrddaa aanniimmee ddaall tteerrmmiinnaallee ee mmoollttoo aallttrroo!!
                   GGllii aanniimmee vveennggoonnoo pprreessii ddaa _AA_nn_ii_mm_ee_WW_oo_rr_ll_dd ********
```

### Comparing `aw-cli-1.8/README.md` & `aw-cli-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aw-cli-1.8/aw_cli.egg-info/PKG-INFO` & `aw-cli-1.8.1/aw_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aw-cli
-Version: 1.8
+Version: 1.8.1
 Summary: guarda anime dal terminale e molto altro!
 Home-page: https://github.com/fexh10/aw-cli
 Author: fexh10
 License: GPL-3.0
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aw-cli Version: 1.8 Summary: guarda anime dal
+Metadata-Version: 2.1 Name: aw-cli Version: 1.8.1 Summary: guarda anime dal
 terminale e molto altro! Home-page: https://github.com/fexh10/aw-cli Author:
 fexh10 License: GPL-3.0 Requires-Python: >3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: bs4 Requires-Dist: requests
 Requires-Dist: lxml Requires-Dist: pySmartDL Requires-Dist: wheel Requires-
 Dist: regex # aw-cli
                 ******** GGuuaarrddaa aanniimmee ddaall tteerrmmiinnaallee ee mmoollttoo aallttrroo!!
                   GGllii aanniimmee vveennggoonnoo pprreessii ddaa _AA_nn_ii_mm_ee_WW_oo_rr_ll_dd ********
```

### Comparing `aw-cli-1.8/awcli/anilist.py` & `aw-cli-1.8.1/awcli/anilist.py`

 * *Files identical despite different names*

### Comparing `aw-cli-1.8/awcli/anime.py` & `aw-cli-1.8.1/awcli/anime.py`

 * *Files identical despite different names*

### Comparing `aw-cli-1.8/awcli/arg_parser.py` & `aw-cli-1.8.1/awcli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `aw-cli-1.8/awcli/run.py` & `aw-cli-1.8.1/awcli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         nome_video (str): il nome dell'episodio.
     """
 
     if syncplay_path == "Syncplay: None":
         my_print("Aggiornare il path di syncplay nella configurazione tramite: aw-cli -a", color="rosso")
         safeExit()
 
-    os.system(f''''{syncplay_path}' "{url_ep}" media-title="{nome_video}" --language it > /dev/null 2>&1''')
+    os.system(f''''{syncplay_path}' "{url_ep}" force-media-title="{nome_video}" --language it > /dev/null 2>&1''')
 
 
 def openMPV(url_ep: str, nome_video: str):
     """
     Apre MPV per riprodurre il video.
 
     Args:
@@ -533,15 +533,19 @@
     delete = my_input("", check_yes)
 
     if delete:
         if anilist.dropAnilist:
             drop = my_input(f"Droppare \"{anime.name}\" su AniList? (s/N)", check_yes)
 
             if drop:
-                updateAnilist(anime.ep_corrente, True)
+                if anime.id_anilist == 0:
+                    my_print("Impossibile droppare su AniList: id anime non trovato!", color="rosso")
+                    sleep(1)
+                else:
+                    updateAnilist(anime.ep_corrente, True)
 
         log.pop(number)
 
         printAnimeNames(getCronologia())
 
         def check_str(s: str):
             s.lower()
```

### Comparing `aw-cli-1.8/awcli/utilities.py` & `aw-cli-1.8.1/awcli/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
         anilist.tokenAnilist = lines[1].strip()
         anilist.ratingAnilist = True if lines[2].strip() == "ratingAnilist: True" else False
         anilist.preferitoAnilist = True if lines[3].strip() == "preferitoAnilist: True" else False
         anilist.dropAnilist = True if lines[4].strip() == "dropAnilist: True" else False
         anilist.user_id = int(lines[5])
 
-        syncplay_path = lines[6]
+        syncplay_path = lines[6].strip()
 
     return mpv, player_path, syncplay_path
 
 
 headers = {
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
 }
```

### Comparing `aw-cli-1.8/setup.py` & `aw-cli-1.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         "pySmartDL",
         "wheel",
         "regex",]
 
 setup(
     name="aw-cli",
     packages=find_packages(include=["awcli"]),
-    version="1.8",
+    version="1.8.1",
     python_requires=">3.10",
     description="guarda anime dal terminale e molto altro!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="fexh10",
     url="https://github.com/fexh10/aw-cli",
     license="GPL-3.0",
```

### Comparing `aw-cli-1.8/tests/test_anime.py` & `aw-cli-1.8.1/tests/test_anime.py`

 * *Files identical despite different names*

### Comparing `aw-cli-1.8/tests/test_utilities.py` & `aw-cli-1.8.1/tests/test_utilities.py`

 * *Files identical despite different names*

