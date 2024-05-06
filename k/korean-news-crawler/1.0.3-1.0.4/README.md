# Comparing `tmp/korean_news_crawler-1.0.3.tar.gz` & `tmp/korean_news_crawler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "korean_news_crawler-1.0.3.tar", last modified: Mon May  6 09:22:32 2024, max compression
+gzip compressed data, was "korean_news_crawler-1.0.4.tar", last modified: Mon May  6 09:26:42 2024, max compression
```

## Comparing `korean_news_crawler-1.0.3.tar` & `korean_news_crawler-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/
--rw-rw-rw-   0        0        0    22931 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    22391 2024-05-06 08:26:28.000000 korean_news_crawler-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/korean_news_crawler.egg-info/
--rw-rw-rw-   0        0        0    22931 2024-05-06 09:22:32.000000 korean_news_crawler-1.0.3/korean_news_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/korean_news_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/korean_news_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/korean_news_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/korean_news_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-10-27 04:01:28.000000 korean_news_crawler-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      909 2024-05-06 09:22:12.000000 korean_news_crawler-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:22:34.000000 korean_news_crawler-1.0.3/src/
--rw-rw-rw-   0        0        0      526 2024-05-06 09:22:08.000000 korean_news_crawler-1.0.3/src/__init__.py
--rw-rw-rw-   0        0        0       21 2024-05-06 09:22:20.000000 korean_news_crawler-1.0.3/src/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/
+-rw-rw-rw-   0        0        0    22931 2024-05-06 09:26:44.000000 korean_news_crawler-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    22391 2024-05-06 08:26:28.000000 korean_news_crawler-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/korean_news_crawler.egg-info/
+-rw-rw-rw-   0        0        0    22931 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/korean_news_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/korean_news_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/korean_news_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/korean_news_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:26:42.000000 korean_news_crawler-1.0.4/korean_news_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-10-27 04:01:28.000000 korean_news_crawler-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-06 09:26:44.000000 korean_news_crawler-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      909 2024-05-06 09:26:36.000000 korean_news_crawler-1.0.4/setup.py
```

### Comparing `korean_news_crawler-1.0.3/PKG-INFO` & `korean_news_crawler-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: korean_news_crawler
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Library for Crawling Top 10 Korean News and Providing Synonym Dictionary
 Home-page: https://github.com/Indigo-Coder-github/Korean_News_Crawler
 Author: Indigo-Coder
 Author-email: hjs40111@gmail.com
 Project-URL: Bug Tracker, https://github.com/Indigo-Coder-github/Korean_News_Crawler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: korean_news_crawler Version: 1.0.3 Summary: Python
+Metadata-Version: 2.1 Name: korean_news_crawler Version: 1.0.4 Summary: Python
 Library for Crawling Top 10 Korean News and Providing Synonym Dictionary Home-
 page: https://github.com/Indigo-Coder-github/Korean_News_Crawler Author:
 Indigo-Coder Author-email: hjs40111@gmail.com Project-URL: Bug Tracker, https:/
 /github.com/Indigo-Coder-github/Korean_News_Crawler/issues Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_P_I_ _1_._0_._1_-
```

### Comparing `korean_news_crawler-1.0.3/README.md` & `korean_news_crawler-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `korean_news_crawler-1.0.3/korean_news_crawler.egg-info/PKG-INFO` & `korean_news_crawler-1.0.4/korean_news_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: korean-news-crawler
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Library for Crawling Top 10 Korean News and Providing Synonym Dictionary
 Home-page: https://github.com/Indigo-Coder-github/Korean_News_Crawler
 Author: Indigo-Coder
 Author-email: hjs40111@gmail.com
 Project-URL: Bug Tracker, https://github.com/Indigo-Coder-github/Korean_News_Crawler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: korean-news-crawler Version: 1.0.3 Summary: Python
+Metadata-Version: 2.1 Name: korean-news-crawler Version: 1.0.4 Summary: Python
 Library for Crawling Top 10 Korean News and Providing Synonym Dictionary Home-
 page: https://github.com/Indigo-Coder-github/Korean_News_Crawler Author:
 Indigo-Coder Author-email: hjs40111@gmail.com Project-URL: Bug Tracker, https:/
 /github.com/Indigo-Coder-github/Korean_News_Crawler/issues Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_P_I_ _1_._0_._1_-
```

### Comparing `korean_news_crawler-1.0.3/setup.py` & `korean_news_crawler-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="korean_news_crawler",
-    version="1.0.3",
+    version="1.0.4",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Python Library for Crawling Top 10 Korean News and Providing Synonym Dictionary",
     author="Indigo-Coder",
     author_email="hjs40111@gmail.com",
     url="https://github.com/Indigo-Coder-github/Korean_News_Crawler",
     install_requires=[
```

