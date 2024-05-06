# Comparing `tmp/mkt-retv-1.417.tar.gz` & `tmp/mkt-retv-1.418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.417.tar", last modified: Mon May  6 06:52:03 2024, max compression
+gzip compressed data, was "mkt-retv-1.418.tar", last modified: Mon May  6 08:37:38 2024, max compression
```

## Comparing `mkt-retv-1.417.tar` & `mkt-retv-1.418.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.792027 mkt-retv-1.417/
--rw-rw-rw-   0        0        0      697 2024-05-06 06:52:03.790027 mkt-retv-1.417/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.417/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.672140 mkt-retv-1.417/market_research/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.417/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.684141 mkt-retv-1.417/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.417/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.417/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.417/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.417/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.417/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.692153 mkt-retv-1.417/market_research/scraper/
--rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.417/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.417/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.417/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.694141 mkt-retv-1.417/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.417/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.698142 mkt-retv-1.417/market_research/scraper/models/lge/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.417/market_research/scraper/models/lge/__init__.py
--rw-rw-rw-   0        0        0    12835 2024-05-05 13:58:54.000000 mkt-retv-1.417/market_research/scraper/models/lge/spec_l.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.705142 mkt-retv-1.417/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.417/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6873 2024-05-05 13:58:54.000000 mkt-retv-1.417/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12943 2024-05-05 13:58:54.000000 mkt-retv-1.417/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.714146 mkt-retv-1.417/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.417/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     7554 2024-05-06 06:51:26.000000 mkt-retv-1.417/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10614 2024-05-05 14:00:38.000000 mkt-retv-1.417/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12393 2024-05-05 14:00:38.000000 mkt-retv-1.417/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4387 2024-05-05 00:51:17.000000 mkt-retv-1.417/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.724735 mkt-retv-1.417/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.417/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.417/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.417/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.417/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.734735 mkt-retv-1.417/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.417/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.417/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.417/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.417/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.417/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:03.789028 mkt-retv-1.417/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-06 06:52:03.000000 mkt-retv-1.417/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-05-06 06:52:03.000000 mkt-retv-1.417/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:52:03.000000 mkt-retv-1.417/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-06 06:52:03.000000 mkt-retv-1.417/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-06 06:52:03.000000 mkt-retv-1.417/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 06:52:03.000000 mkt-retv-1.417/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 06:52:03.792027 mkt-retv-1.417/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-06 06:51:38.000000 mkt-retv-1.417/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:38.149214 mkt-retv-1.418/
+-rw-rw-rw-   0        0        0      697 2024-05-06 08:37:38.149214 mkt-retv-1.418/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.418/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.513424 mkt-retv-1.418/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.418/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.622979 mkt-retv-1.418/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.418/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.418/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.418/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.418/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.418/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.686070 mkt-retv-1.418/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.418/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.418/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.418/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.686070 mkt-retv-1.418/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.418/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.726293 mkt-retv-1.418/market_research/scraper/models/lge/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.418/market_research/scraper/models/lge/__init__.py
+-rw-rw-rw-   0        0        0    12835 2024-05-05 13:58:54.000000 mkt-retv-1.418/market_research/scraper/models/lge/spec_l.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.773736 mkt-retv-1.418/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.418/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6873 2024-05-05 13:58:54.000000 mkt-retv-1.418/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12943 2024-05-05 13:58:54.000000 mkt-retv-1.418/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.836360 mkt-retv-1.418/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.418/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5356 2024-05-06 08:36:11.000000 mkt-retv-1.418/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10614 2024-05-05 14:00:38.000000 mkt-retv-1.418/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12393 2024-05-05 14:00:38.000000 mkt-retv-1.418/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4393 2024-05-06 08:33:42.000000 mkt-retv-1.418/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:37.930130 mkt-retv-1.418/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.418/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.418/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.418/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.418/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:38.070973 mkt-retv-1.418/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.418/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.418/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.418/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.418/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.418/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:37:38.133574 mkt-retv-1.418/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-06 08:37:37.000000 mkt-retv-1.418/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-05-06 08:37:37.000000 mkt-retv-1.418/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:37:37.000000 mkt-retv-1.418/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-06 08:37:37.000000 mkt-retv-1.418/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-06 08:37:37.000000 mkt-retv-1.418/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 08:37:37.000000 mkt-retv-1.418/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:37:38.149214 mkt-retv-1.418/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-06 08:36:57.000000 mkt-retv-1.418/setup.py
```

### Comparing `mkt-retv-1.417/PKG-INFO` & `mkt-retv-1.418/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.417
+Version: 1.418
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.417/README.md` & `mkt-retv-1.418/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.418/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/analysis/imgemanger.py` & `mkt-retv-1.418/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.418/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/analysis/textmanager.py` & `mkt-retv-1.418/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/__init__.py` & `mkt-retv-1.418/market_research/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.418/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/models/lge/spec_l.py` & `mkt-retv-1.418/market_research/scraper/models/lge/spec_l.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.418/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.418/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.418/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.418/market_research/scraper/models/sony/spec_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.418/market_research/scraper/models/sony/visualizer_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 from .cleanup_s import DataCleanup_s
 from market_research.scraper._visualizer_scheme import Visualizer
-class Visualizer_s(Visualizer):
+class Visualizer_s1(Visualizer):
 
     def __init__(self, df, output_folder_path="results", style="whitegrid", cleaning_mask:list=None):
 
         """
         cleaning_mask에 삭제할 column의 키워드를 리스트로 전달하세요.
         기본 값으로는 사전 정의된 값을 사용합니다.
         """
@@ -71,15 +71,15 @@
 
         data_df = self.dc.get_df_cleaned()
         data_df = data_df[col_selected]
         if display_types is not None:
             condition = data_df.index.get_level_values('display type').str.contains('|'.join(display_types), case=False, na=False)
             data_df = data_df[condition]
         data_df = data_df.mask(data_df == '-', 0)
-        data_df = data_df.map(lambda x: len(x.split(",")) if isinstance(x, str) else x)
+        data_df = data_df.applymap(lambda x: len(x.split(",")) if isinstance(x, str) else x)
         data_df = data_df.fillna(0)
         idx_names = data_df.index.names
         data_df = data_df.reset_index().drop_duplicates()
         data_df = data_df.set_index(idx_names)
         data_df = data_df.sort_index(ascending=True)
         # Use plt.subplots to get the axis for colorbar
         self.data_df = data_df
```

### Comparing `mkt-retv-1.417/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.418/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.418/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.418/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/tools/aimanager.py` & `mkt-retv-1.418/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/tools/filemanager.py` & `mkt-retv-1.418/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/tools/installer.py` & `mkt-retv-1.418/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/market_research/tools/webdriver.py` & `mkt-retv-1.418/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.418/mkt_retv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.417
+Version: 1.418
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.417/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.418/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.417/setup.py` & `mkt-retv-1.418/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.417',
+    version='1.418',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

