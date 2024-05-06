# Comparing `tmp/mkt-retv-1.415.tar.gz` & `tmp/mkt-retv-1.416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.415.tar", last modified: Sun May  5 13:46:53 2024, max compression
+gzip compressed data, was "mkt-retv-1.416.tar", last modified: Sun May  5 14:01:20 2024, max compression
```

## Comparing `mkt-retv-1.415.tar` & `mkt-retv-1.416.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.812066 mkt-retv-1.415/
--rw-rw-rw-   0        0        0      697 2024-05-05 13:46:53.807612 mkt-retv-1.415/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.415/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.698839 mkt-retv-1.415/market_research/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.707695 mkt-retv-1.415/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.415/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.415/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.415/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.415/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.415/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.716244 mkt-retv-1.415/market_research/scraper/
--rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.415/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.415/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.415/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.716244 mkt-retv-1.415/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.716244 mkt-retv-1.415/market_research/scraper/models/lge/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/lge/__init__.py
--rw-rw-rw-   0        0        0    12830 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/lge/spec_l.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.726100 mkt-retv-1.415/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6868 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12938 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.734269 mkt-retv-1.415/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.415/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5267 2024-05-05 05:49:12.000000 mkt-retv-1.415/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10590 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12370 2024-05-05 13:45:10.000000 mkt-retv-1.415/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.415/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.734269 mkt-retv-1.415/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.415/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.415/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.415/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.415/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.744319 mkt-retv-1.415/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.415/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.415/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.415/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.415/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.415/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:46:53.791961 mkt-retv-1.415/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 13:46:53.000000 mkt-retv-1.415/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 13:46:53.812066 mkt-retv-1.415/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-05 13:46:48.000000 mkt-retv-1.415/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.959855 mkt-retv-1.416/
+-rw-rw-rw-   0        0        0      697 2024-05-05 14:01:20.959855 mkt-retv-1.416/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.416/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.886365 mkt-retv-1.416/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.416/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.887573 mkt-retv-1.416/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.416/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.416/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.416/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.416/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.416/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.896081 mkt-retv-1.416/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.416/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.416/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.416/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.896081 mkt-retv-1.416/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.416/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.896081 mkt-retv-1.416/market_research/scraper/models/lge/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.416/market_research/scraper/models/lge/__init__.py
+-rw-rw-rw-   0        0        0    12835 2024-05-05 13:58:54.000000 mkt-retv-1.416/market_research/scraper/models/lge/spec_l.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.909089 mkt-retv-1.416/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.416/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6873 2024-05-05 13:58:54.000000 mkt-retv-1.416/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12943 2024-05-05 13:58:54.000000 mkt-retv-1.416/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.912128 mkt-retv-1.416/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.416/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5267 2024-05-05 05:49:12.000000 mkt-retv-1.416/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10614 2024-05-05 14:00:38.000000 mkt-retv-1.416/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12393 2024-05-05 14:00:38.000000 mkt-retv-1.416/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.416/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.928600 mkt-retv-1.416/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.416/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.416/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.416/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.416/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.938151 mkt-retv-1.416/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.416/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.416/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.416/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.416/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.416/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:01:20.959855 mkt-retv-1.416/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-05 14:01:20.000000 mkt-retv-1.416/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-05-05 14:01:20.000000 mkt-retv-1.416/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 14:01:20.000000 mkt-retv-1.416/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-05 14:01:20.000000 mkt-retv-1.416/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-05 14:01:20.000000 mkt-retv-1.416/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 14:01:20.000000 mkt-retv-1.416/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 14:01:20.959855 mkt-retv-1.416/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-05 14:01:10.000000 mkt-retv-1.416/setup.py
```

### Comparing `mkt-retv-1.415/PKG-INFO` & `mkt-retv-1.416/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.415
+Version: 1.416
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.415/README.md` & `mkt-retv-1.416/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.416/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/analysis/imgemanger.py` & `mkt-retv-1.416/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.416/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/analysis/textmanager.py` & `mkt-retv-1.416/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/__init__.py` & `mkt-retv-1.416/market_research/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.416/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/models/lge/spec_l.py` & `mkt-retv-1.416/market_research/scraper/models/lge/spec_l.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 try:
                     dict_info = self._get_model_info(url_model)
                     dict_models[key] = dict_info
                     dict_spec = self._get_global_spec(url=url_model)
                     dict_models[key].update(dict_spec)
                     visit_url_dict[key] = url_model
                 except Exception as e:
-                    if cnt == cnt_loop:
+                    if cnt == cnt_loop - 1 :
                         print(f"\nFailed to get info from {key}")
                         print(e)
                     pass
             break
         print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
```

### Comparing `mkt-retv-1.415/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.416/market_research/scraper/models/pana/spec_p.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     # print(model,":", url)
                     modelspec = self._get_spec_global(url=url)
                     modelspec["url"] = url
                     dictModels[model] = modelspec
 
                     visit_url_dict[model] = url
                 except Exception as e:
-                    if cnt == cnt_loop:
+                    if cnt == cnt_loop - 1 :
                         print(f"\nFailed to get info from {model}")
                         print(e)
                     pass
             break
         print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
         # print("Number of all Series:", len(dictModels))
```

### Comparing `mkt-retv-1.415/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.416/market_research/scraper/models/pana/spec_pjp.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         for cnt in range(cnt_loop):#main try
             for model, url in tqdm(specs_dict.items()):
                 try:
                     visit_url_dict[model] = url
                     modelspec = self._get_spec(model = model, url=url)
                     models_dict[model] = modelspec
                 except Exception as e:
-                    if cnt == cnt_loop:
+                    if cnt == cnt_loop - 1 :
                         print(f"\nFailed to get info from {model}")
                         print(e)
                     pass
             break
         print("\n")
         for model, url in visit_url_dict.items(): print(f"{model}: {url}")
```

### Comparing `mkt-retv-1.415/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.416/market_research/scraper/models/sony/cleanup_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.416/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,19 @@
             for model, url in tqdm(url_series_dict.items()):
                 try:
                     # print(f"{model}: {url}")
                     modelspec = self._get_spec(url=url)
                     models_dict.update(modelspec)
                     visit_url_dict[model] = url
                 except Exception as e:
-                    if cnt == cnt_loop:
+                    if cnt == cnt_loop - 1 :
                         print(f"\nFailed to get info from {model}")
                         print(e)
                     pass
+            break
         print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
         # print("Number of all Series:", len(models_dict))
 
         if foramt_output == "df":
             df_models = pd.DataFrame.from_dict(models_dict).T
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na", mode='w')
```

### Comparing `mkt-retv-1.415/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.416/market_research/scraper/models/sony/spec_s.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,18 +43,19 @@
                 try:
                     dict_info = self._get_model_info(url_model)
                     dict_models[key] = dict_info
                     dict_spec = self._get_global_spec(url=url_model)
                     dict_models[key].update(dict_spec)
                     visit_url_dict[key] = url_model
                 except Exception as e:
-                    if cnt == cnt_loop:
+                    if cnt == cnt_loop - 1:
                         print(f"\nFailed to get info from {key}")
                         print(e)
                     pass
+            break
         print("\n")
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
 
         if format_df:
             df_models = pd.DataFrame.from_dict(dict_models).T
             if temporary_year_marking:
                 df_models['year'] = df_models['year'].fillna("2024") ## 임시
```

### Comparing `mkt-retv-1.415/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.416/market_research/scraper/models/sony/visualizer_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.416/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.416/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.416/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/tools/aimanager.py` & `mkt-retv-1.416/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/tools/filemanager.py` & `mkt-retv-1.416/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/tools/installer.py` & `mkt-retv-1.416/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/market_research/tools/webdriver.py` & `mkt-retv-1.416/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.416/mkt_retv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.415
+Version: 1.416
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.415/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.416/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.415/setup.py` & `mkt-retv-1.416/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.415',
+    version='1.416',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

