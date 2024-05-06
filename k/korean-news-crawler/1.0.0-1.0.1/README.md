# Comparing `tmp/korean_news_crawler-1.0.0.tar.gz` & `tmp/korean_news_crawler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "korean_news_crawler-1.0.0.tar", last modified: Mon May  6 07:35:06 2024, max compression
+gzip compressed data, was "korean_news_crawler-1.0.1.tar", last modified: Mon May  6 07:54:41 2024, max compression
```

## Comparing `korean_news_crawler-1.0.0.tar` & `korean_news_crawler-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/
--rw-rw-rw-   0        0        0      538 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    22211 2024-05-06 07:28:04.000000 korean_news_crawler-1.0.0/README.md
--rw-rw-rw-   0        0        0      108 2023-10-27 04:01:28.000000 korean_news_crawler-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-05-06 05:52:56.000000 korean_news_crawler-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/korean_news_crawler.egg-info/
--rw-rw-rw-   0        0        0      538 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/korean_news_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/korean_news_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/korean_news_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/korean_news_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 07:35:08.000000 korean_news_crawler-1.0.0/src/korean_news_crawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/
+-rw-rw-rw-   0        0        0    22751 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    22211 2024-05-06 07:28:04.000000 korean_news_crawler-1.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-10-27 04:01:28.000000 korean_news_crawler-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-06 07:52:14.000000 korean_news_crawler-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/korean_news_crawler.egg-info/
+-rw-rw-rw-   0        0        0    22751 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/korean_news_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/korean_news_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/korean_news_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/korean_news_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:54:42.000000 korean_news_crawler-1.0.1/src/korean_news_crawler.egg-info/top_level.txt
```

### Comparing `korean_news_crawler-1.0.0/README.md` & `korean_news_crawler-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `korean_news_crawler-1.0.0/setup.py` & `korean_news_crawler-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import setuptools
 
+with open("README.md", "r", encoding="UTF-8") as f:
+    long_description = f.read()
+
 setuptools.setup(
     name="korean_news_crawler",
-    version="1.0.0",
+    version="1.0.1",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    description="Python Library for Crawling Top 10 Korean News and Providing Synonym Dictionary",
     author="Indigo-Coder",
     author_email="hjs40111@gmail.com",
-    description="Python Library for Crawling Top 10 Korean News and Providing Synonym Dictionary",
-    long_description_content_type="text/markdown",
     url="https://github.com/Indigo-Coder-github/Korean_News_Crawler",
     install_requires=[
         "BeautifulSoup4",
         "selenium"
     ],
     project_urls={
         "Bug Tracker": "https://github.com/Indigo-Coder-github/Korean_News_Crawler/issues",
```

