# Comparing `tmp/mkt-retv-1.419.tar.gz` & `tmp/mkt-retv-1.420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.419.tar", last modified: Mon May  6 09:01:54 2024, max compression
+gzip compressed data, was "mkt-retv-1.420.tar", last modified: Mon May  6 12:09:13 2024, max compression
```

## Comparing `mkt-retv-1.419.tar` & `mkt-retv-1.420.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.695435 mkt-retv-1.419/
--rw-rw-rw-   0        0        0      697 2024-05-06 09:01:54.695435 mkt-retv-1.419/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.419/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.569528 mkt-retv-1.419/market_research/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.419/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.569528 mkt-retv-1.419/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.419/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.419/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.419/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.419/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.419/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.586594 mkt-retv-1.419/market_research/scraper/
--rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.419/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.419/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.419/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.586594 mkt-retv-1.419/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.419/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.586594 mkt-retv-1.419/market_research/scraper/models/lge/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.419/market_research/scraper/models/lge/__init__.py
--rw-rw-rw-   0        0        0    12835 2024-05-05 13:58:54.000000 mkt-retv-1.419/market_research/scraper/models/lge/spec_l.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.600609 mkt-retv-1.419/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.419/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6873 2024-05-05 13:58:54.000000 mkt-retv-1.419/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12943 2024-05-05 13:58:54.000000 mkt-retv-1.419/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.618679 mkt-retv-1.419/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.419/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5356 2024-05-06 08:36:11.000000 mkt-retv-1.419/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10614 2024-05-05 14:00:38.000000 mkt-retv-1.419/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12393 2024-05-05 14:00:38.000000 mkt-retv-1.419/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4392 2024-05-06 09:01:29.000000 mkt-retv-1.419/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.618679 mkt-retv-1.419/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.419/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.419/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.419/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.419/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.632189 mkt-retv-1.419/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.419/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.419/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.419/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.419/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.419/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:01:54.686804 mkt-retv-1.419/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-06 09:01:54.000000 mkt-retv-1.419/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-05-06 09:01:54.000000 mkt-retv-1.419/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:01:54.000000 mkt-retv-1.419/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-06 09:01:54.000000 mkt-retv-1.419/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-06 09:01:54.000000 mkt-retv-1.419/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 09:01:54.000000 mkt-retv-1.419/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 09:01:54.695435 mkt-retv-1.419/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-06 09:01:51.000000 mkt-retv-1.419/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.257893 mkt-retv-1.420/
+-rw-rw-rw-   0        0        0      697 2024-05-06 12:09:13.255893 mkt-retv-1.420/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2024-05-06 09:02:26.000000 mkt-retv-1.420/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.135205 mkt-retv-1.420/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.420/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.146205 mkt-retv-1.420/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.420/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.420/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.420/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.420/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.420/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.153203 mkt-retv-1.420/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.420/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.420/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.420/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.155203 mkt-retv-1.420/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.420/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.159204 mkt-retv-1.420/market_research/scraper/models/lge/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.420/market_research/scraper/models/lge/__init__.py
+-rw-rw-rw-   0        0        0    12973 2024-05-06 12:08:02.000000 mkt-retv-1.420/market_research/scraper/models/lge/spec_l.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.165205 mkt-retv-1.420/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.420/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6873 2024-05-05 13:58:54.000000 mkt-retv-1.420/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12943 2024-05-05 13:58:54.000000 mkt-retv-1.420/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.177208 mkt-retv-1.420/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.420/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5356 2024-05-06 08:36:11.000000 mkt-retv-1.420/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10614 2024-05-05 14:00:38.000000 mkt-retv-1.420/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12529 2024-05-06 12:05:21.000000 mkt-retv-1.420/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4392 2024-05-06 09:01:29.000000 mkt-retv-1.420/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.184220 mkt-retv-1.420/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.420/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.420/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.420/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.420/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.199375 mkt-retv-1.420/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.420/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.420/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.420/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.420/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.420/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:09:13.254894 mkt-retv-1.420/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-06 12:09:12.000000 mkt-retv-1.420/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-05-06 12:09:12.000000 mkt-retv-1.420/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:09:12.000000 mkt-retv-1.420/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-06 12:09:12.000000 mkt-retv-1.420/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-06 12:09:12.000000 mkt-retv-1.420/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 12:09:12.000000 mkt-retv-1.420/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 12:09:13.257893 mkt-retv-1.420/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-06 12:08:12.000000 mkt-retv-1.420/setup.py
```

### Comparing `mkt-retv-1.419/PKG-INFO` & `mkt-retv-1.420/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.419
+Version: 1.420
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.419/README.md` & `mkt-retv-1.420/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 이 프로젝트는 웹사이트에서 제품 모델 사양을 가져오고 분석하는 기능을 제공합니다.
 
 ## 실행 데모
 이 프로젝트는 웹사이트에서 제품 정보를 수집하고 분석 합니다.
 사용법은 아래의 note를 참고 하세요.
 > **Demo Note book**  
-> [market model information](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quick_guide_market_models.ipynb)  
-> [model scores & measurement](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quick_guide_market_rtings.ipynb)  
-> [text analysis](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quick_guide_textanalysis.ipynb)  
-> [image analysis](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quick_guide_imganalysis.ipynb)
+> [market model information](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quickguide_market_models.ipynb)  
+> [model scores & measurement](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quickguide_market_rtings.ipynb)  
+> [text analysis](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quickguide_textanalysis.ipynb)  
+> [image analysis](https://colab.research.google.com/github/xikest/research_market_tv/blob/main/quickguide_imganalysis.ipynb)
 
 
 
 ## 주의사항
 Selenium을 사용하여 웹 스크래핑을 수행하므로 Chrome 웹 드라이버가 필요합니다.   
 Chrome 웹 드라이버를 설치하고 경로를 올바르게 설정해야 합니다.
```

### Comparing `mkt-retv-1.419/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.420/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/analysis/imgemanger.py` & `mkt-retv-1.420/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.420/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/analysis/textmanager.py` & `mkt-retv-1.420/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/__init__.py` & `mkt-retv-1.420/market_research/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.420/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/models/lge/spec_l.py` & `mkt-retv-1.420/market_research/scraper/models/lge/spec_l.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,39 +71,40 @@
         Get the series URLs by scrolling down the main page.
         """
         url = "https://www.lg.com/us/tvs"
         prefix = "https://www.lg.com/"
         step = 200
         url_series = set()
         try_total = 5
-        for _ in range(try_total):
-            driver = self.web_driver.get_chrome()
-            try:
-                driver.get(url=url)
-                time.sleep(self.wait_time)
-                scroll_distance_total = self.web_driver.get_scroll_distance_total()
-                scroll_distance = 0
+        for _ in range(2): #page_checker
+            for _ in range(try_total):
+                driver = self.web_driver.get_chrome()
+                try:
+                    driver.get(url=url)
+                    time.sleep(self.wait_time)
+                    scroll_distance_total = self.web_driver.get_scroll_distance_total()
+                    scroll_distance = 0
 
-                while scroll_distance < scroll_distance_total:
-                    for _ in range(2):
-                        html = driver.page_source
-                        soup = BeautifulSoup(html, 'html.parser')
-                        elements = soup.find_all('a', class_="css-11xg6yi")
-                        for element in elements:
-                            url_series.add(prefix + element['href'].strip())
-                        driver.execute_script(f"window.scrollBy(0, {step});")
-                        time.sleep(self.wait_time)
-                        scroll_distance += step
-                driver.quit()
-                break
-            except Exception as e:
-                driver.quit()
-                if self.tracking_log:
-                    print(f"Try collecting {_ + 1}/{try_total}")
-                    print(e)
+                    while scroll_distance < scroll_distance_total:
+                        for _ in range(2):
+                            html = driver.page_source
+                            soup = BeautifulSoup(html, 'html.parser')
+                            elements = soup.find_all('a', class_="css-11xg6yi")
+                            for element in elements:
+                                url_series.add(prefix + element['href'].strip())
+                            driver.execute_script(f"window.scrollBy(0, {step});")
+                            time.sleep(self.wait_time)
+                            scroll_distance += step
+                    driver.quit()
+                    break
+                except Exception as e:
+                    driver.quit()
+                    if self.tracking_log:
+                        print(f"Try collecting {_ + 1}/{try_total}")
+                        print(e)
         print("The website scan has been completed.")
         print(f"number of total series: {len(url_series)}")
         return url_series
 
     def _get_models(self, url: str, prefix="https://www.lg.com/", static_mode=True) -> dict:
         """
         Extract all model URLs from a given series URL.
```

### Comparing `mkt-retv-1.419/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.420/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.420/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.420/market_research/scraper/models/sony/cleanup_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.420/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.420/market_research/scraper/models/sony/spec_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,38 +70,40 @@
         Get the series URLs by scrolling down the main page.
         """
         url = "https://electronics.sony.com/tv-video/televisions/c/all-tvs/"
         prefix = "https://electronics.sony.com/"
         step = 200
         url_series = set()
         try_total = 5
-        for _ in range(try_total):
-            driver = self.web_driver.get_chrome()
-            try:
-                driver.get(url=url)
-                time.sleep(self.wait_time)
-                scroll_distance_total = self.web_driver.get_scroll_distance_total()
-                scroll_distance = 0
+        for _ in range(2): #page_checker
+            for _ in range(try_total):
+                driver = self.web_driver.get_chrome()
+                try:
+                    driver.get(url=url)
+                    time.sleep(self.wait_time)
+                    scroll_distance_total = self.web_driver.get_scroll_distance_total()
+                    scroll_distance = 0
+
+                    while scroll_distance < scroll_distance_total:
+                        for _ in range(2):
+                            html = driver.page_source
+                            soup = BeautifulSoup(html, 'html.parser')
+                            elements = soup.find_all('a', class_="custom-product-grid-item__product-name")
+                            for element in elements:
+                                url_series.add(prefix + element['href'].strip())
+                            driver.execute_script(f"window.scrollBy(0, {step});")
+                            time.sleep(self.wait_time)
+                            scroll_distance += step
+                    driver.quit()
+                    break
+                except Exception as e:
+                    driver.quit()
+                    print(f"Try collecting {_ + 1}/{try_total}")
+                    # print(e)
 
-                while scroll_distance < scroll_distance_total:
-                    for _ in range(2):
-                        html = driver.page_source
-                        soup = BeautifulSoup(html, 'html.parser')
-                        elements = soup.find_all('a', class_="custom-product-grid-item__product-name")
-                        for element in elements:
-                            url_series.add(prefix + element['href'].strip())
-                        driver.execute_script(f"window.scrollBy(0, {step});")
-                        time.sleep(self.wait_time)
-                        scroll_distance += step
-                driver.quit()
-                break
-            except Exception as e:
-                driver.quit()
-                print(f"Try collecting {_ + 1}/{try_total}")
-                # print(e)
         print("The website scan has been completed.")
         print(f"number of total series: {len(url_series)}")
         return url_series
 
     def _get_models(self, url: str, prefix="https://electronics.sony.com/", static_mode=True) -> dict:
         """
         Extract all model URLs from a given series URL.
```

### Comparing `mkt-retv-1.419/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.420/market_research/scraper/models/sony/visualizer_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.420/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.420/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.420/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/tools/aimanager.py` & `mkt-retv-1.420/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/tools/filemanager.py` & `mkt-retv-1.420/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/tools/installer.py` & `mkt-retv-1.420/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/market_research/tools/webdriver.py` & `mkt-retv-1.420/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.420/mkt_retv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.419
+Version: 1.420
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.419/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.420/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.419/setup.py` & `mkt-retv-1.420/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.419',
+    version='1.420',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

