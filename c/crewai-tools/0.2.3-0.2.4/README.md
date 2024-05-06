# Comparing `tmp/crewai_tools-0.2.3.tar.gz` & `tmp/crewai_tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.2.3.tar", max compression
+gzip compressed data, was "crewai_tools-0.2.4.tar", max compression
```

## Comparing `crewai_tools-0.2.3.tar` & `crewai_tools-0.2.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.2.3/LICENSE
--rw-r--r--   0        0        0     3478 2024-05-02 06:04:48.741505 crewai_tools-0.2.3/README.md
--rw-r--r--   0        0        0      509 2024-05-02 05:49:21.488653 crewai_tools-0.2.3/crewai_tools/__init__.py
--rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.2.3/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.2.3/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1541 2024-05-02 06:53:53.439980 crewai_tools-0.2.3/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.2.3/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0      931 2024-05-02 05:36:37.312858 crewai_tools-0.2.3/crewai_tools/tools/browserbase_load_tool/README.md
--rw-r--r--   0        0        0     1166 2024-05-02 06:55:55.945860 crewai_tools-0.2.3/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py
--rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.2.3/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.2.3/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.2.3/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.2.3/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.2.3/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.2.3/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.2.3/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.2.3/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.2.3/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1642 2024-04-10 14:50:04.965572 crewai_tools-0.2.3/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1472 2024-05-02 05:50:40.176058 crewai_tools-0.2.3/crewai_tools/tools/exa_tools/README.md
--rw-r--r--   0        0        0     1044 2024-05-02 07:12:25.534945 crewai_tools-0.2.3/crewai_tools/tools/exa_tools/exa_base_tool.py
--rw-r--r--   0        0        0      650 2024-05-03 01:31:40.048347 crewai_tools-0.2.3/crewai_tools/tools/exa_tools/exa_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.2.3/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1350 2024-05-02 05:36:37.313883 crewai_tools-0.2.3/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.2.3/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.2.3/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.2.3/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.2.3/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.2.3/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.2.3/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.2.3/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.2.3/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.2.3/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.2.3/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.2.3/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.2.3/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.2.3/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.2.3/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.2.3/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.2.3/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.2.3/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2504 2024-05-02 06:04:48.748764 crewai_tools-0.2.3/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.2.3/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1447 2024-05-02 05:48:30.482467 crewai_tools-0.2.3/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.2.3/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.2.3/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.2.3/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.2.3/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.2.3/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.2.3/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.2.3/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.2.3/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.2.3/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.2.3/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      730 2024-05-03 01:31:51.246836 crewai_tools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 crewai_tools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3478 2024-05-02 06:04:48.741505 crewai_tools-0.2.4/README.md
+-rw-r--r--   0        0        0      509 2024-05-02 05:49:21.488653 crewai_tools-0.2.4/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.2.4/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.2.4/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1541 2024-05-02 06:53:53.439980 crewai_tools-0.2.4/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.2.4/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0      931 2024-05-02 05:36:37.312858 crewai_tools-0.2.4/crewai_tools/tools/browserbase_load_tool/README.md
+-rw-r--r--   0        0        0     1166 2024-05-02 06:55:55.945860 crewai_tools-0.2.4/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.2.4/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.2.4/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.2.4/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.2.4/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.2.4/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.2.4/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.2.4/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.2.4/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.2.4/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1983 2024-05-06 16:45:13.581028 crewai_tools-0.2.4/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1472 2024-05-02 05:50:40.176058 crewai_tools-0.2.4/crewai_tools/tools/exa_tools/README.md
+-rw-r--r--   0        0        0     1044 2024-05-02 07:12:25.534945 crewai_tools-0.2.4/crewai_tools/tools/exa_tools/exa_base_tool.py
+-rw-r--r--   0        0        0      650 2024-05-03 01:31:40.048347 crewai_tools-0.2.4/crewai_tools/tools/exa_tools/exa_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.2.4/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1350 2024-05-02 05:36:37.313883 crewai_tools-0.2.4/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.2.4/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.2.4/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.2.4/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.2.4/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.2.4/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.2.4/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.2.4/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.2.4/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.2.4/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.2.4/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.2.4/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.2.4/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.2.4/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.2.4/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.2.4/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.2.4/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.2.4/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2504 2024-05-02 06:04:48.748764 crewai_tools-0.2.4/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.2.4/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1447 2024-05-02 05:48:30.482467 crewai_tools-0.2.4/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.2.4/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.2.4/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.2.4/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.2.4/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.2.4/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.2.4/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.2.4/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.2.4/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.2.4/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.2.4/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      748 2024-05-06 16:44:21.607301 crewai_tools-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 crewai_tools-0.2.4/PKG-INFO
```

### Comparing `crewai_tools-0.2.3/LICENSE` & `crewai_tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/README.md` & `crewai_tools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/adapters/embedchain_adapter.py` & `crewai_tools-0.2.4/crewai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.2.4/crewai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/__init__.py` & `crewai_tools-0.2.4/crewai_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/base_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/browserbase_load_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/browserbase_load_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/code_docs_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/code_docs_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/csv_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/csv_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/csv_search_tool/csv_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/csv_search_tool/csv_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/directory_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/directory_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/directory_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/docx_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/docx_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/docx_search_tool/docx_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 
 from embedchain.models.data_type import DataType
 from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
-class FixedDOCXSearchToolSchema(BaseModel):
-    """Input for DOCXSearchTool."""
+class FixedMDXSearchToolSchema(BaseModel):
+    """Input for MDXSearchTool."""
 
     search_query: str = Field(
         ...,
-        description="Mandatory search query you want to use to search the DOCX's content",
+        description="Mandatory search query you want to use to search the MDX's content",
     )
 
 
-class DOCXSearchToolSchema(FixedDOCXSearchToolSchema):
-    """Input for DOCXSearchTool."""
+class MDXSearchToolSchema(FixedMDXSearchToolSchema):
+    """Input for MDXSearchTool."""
 
-    docx: str = Field(..., description="Mandatory docx path you want to search")
+    mdx: str = Field(..., description="Mandatory mdx path you want to search")
 
 
-class DOCXSearchTool(RagTool):
-    name: str = "Search a DOCX's content"
+class MDXSearchTool(RagTool):
+    name: str = "Search a MDX's content"
     description: str = (
-        "A tool that can be used to semantic search a query from a DOCX's content."
+        "A tool that can be used to semantic search a query from a MDX's content."
     )
-    args_schema: Type[BaseModel] = DOCXSearchToolSchema
+    args_schema: Type[BaseModel] = MDXSearchToolSchema
 
-    def __init__(self, docx: Optional[str] = None, **kwargs):
+    def __init__(self, mdx: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
-        if docx is not None:
-            self.add(docx)
-            self.description = f"A tool that can be used to semantic search a query the {docx} DOCX's content."
-            self.args_schema = FixedDOCXSearchToolSchema
+        if mdx is not None:
+            self.add(mdx)
+            self.description = f"A tool that can be used to semantic search a query the {mdx} MDX's content."
+            self.args_schema = FixedMDXSearchToolSchema
             self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        kwargs["data_type"] = DataType.DOCX
+        kwargs["data_type"] = DataType.MDX
         super().add(*args, **kwargs)
 
     def _before_run(
         self,
         query: str,
         **kwargs: Any,
     ) -> Any:
-        if "docx" in kwargs:
-            self.add(kwargs["docx"])
+        if "mdx" in kwargs:
+            self.add(kwargs["mdx"])
 
     def _run(
         self,
         search_query: str,
         **kwargs: Any,
     ) -> Any:
         return super()._run(query=search_query)
```

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/exa_tools/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/exa_tools/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/exa_tools/exa_base_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/exa_tools/exa_base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/exa_tools/exa_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/exa_tools/exa_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/github_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/json_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/json_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/json_search_tool/json_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/json_search_tool/json_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/mdx_seach_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/mdx_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 
 from embedchain.models.data_type import DataType
 from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
-class FixedMDXSearchToolSchema(BaseModel):
-    """Input for MDXSearchTool."""
+class FixedTXTSearchToolSchema(BaseModel):
+    """Input for TXTSearchTool."""
 
     search_query: str = Field(
         ...,
-        description="Mandatory search query you want to use to search the MDX's content",
+        description="Mandatory search query you want to use to search the txt's content",
     )
 
 
-class MDXSearchToolSchema(FixedMDXSearchToolSchema):
-    """Input for MDXSearchTool."""
+class TXTSearchToolSchema(FixedTXTSearchToolSchema):
+    """Input for TXTSearchTool."""
 
-    mdx: str = Field(..., description="Mandatory mdx path you want to search")
+    txt: str = Field(..., description="Mandatory txt path you want to search")
 
 
-class MDXSearchTool(RagTool):
-    name: str = "Search a MDX's content"
+class TXTSearchTool(RagTool):
+    name: str = "Search a txt's content"
     description: str = (
-        "A tool that can be used to semantic search a query from a MDX's content."
+        "A tool that can be used to semantic search a query from a txt's content."
     )
-    args_schema: Type[BaseModel] = MDXSearchToolSchema
+    args_schema: Type[BaseModel] = TXTSearchToolSchema
 
-    def __init__(self, mdx: Optional[str] = None, **kwargs):
+    def __init__(self, txt: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
-        if mdx is not None:
-            self.add(mdx)
-            self.description = f"A tool that can be used to semantic search a query the {mdx} MDX's content."
-            self.args_schema = FixedMDXSearchToolSchema
+        if txt is not None:
+            self.add(txt)
+            self.description = f"A tool that can be used to semantic search a query the {txt} txt's content."
+            self.args_schema = FixedTXTSearchToolSchema
             self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        kwargs["data_type"] = DataType.MDX
+        kwargs["data_type"] = DataType.TEXT_FILE
         super().add(*args, **kwargs)
 
     def _before_run(
         self,
         query: str,
         **kwargs: Any,
     ) -> Any:
-        if "mdx" in kwargs:
-            self.add(kwargs["mdx"])
+        if "txt" in kwargs:
+            self.add(kwargs["txt"])
 
     def _run(
         self,
         search_query: str,
         **kwargs: Any,
     ) -> Any:
         return super()._run(query=search_query)
```

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/pdf_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/pdf_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/pg_seach_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/pg_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/pg_seach_tool/pg_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/pg_seach_tool/pg_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/rag/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/rag/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/rag/rag_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/rag/rag_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.2.4/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/txt_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/txt_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/xml_search_tool/xml_search_tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 
 from embedchain.models.data_type import DataType
 from pydantic.v1 import BaseModel, Field
 
 from ..rag.rag_tool import RagTool
 
 
-class FixedTXTSearchToolSchema(BaseModel):
-    """Input for TXTSearchTool."""
+class FixedXMLSearchToolSchema(BaseModel):
+    """Input for XMLSearchTool."""
 
     search_query: str = Field(
         ...,
-        description="Mandatory search query you want to use to search the txt's content",
+        description="Mandatory search query you want to use to search the XML's content",
     )
 
 
-class TXTSearchToolSchema(FixedTXTSearchToolSchema):
-    """Input for TXTSearchTool."""
+class XMLSearchToolSchema(FixedXMLSearchToolSchema):
+    """Input for XMLSearchTool."""
 
-    txt: str = Field(..., description="Mandatory txt path you want to search")
+    xml: str = Field(..., description="Mandatory xml path you want to search")
 
 
-class TXTSearchTool(RagTool):
-    name: str = "Search a txt's content"
+class XMLSearchTool(RagTool):
+    name: str = "Search a XML's content"
     description: str = (
-        "A tool that can be used to semantic search a query from a txt's content."
+        "A tool that can be used to semantic search a query from a XML's content."
     )
-    args_schema: Type[BaseModel] = TXTSearchToolSchema
+    args_schema: Type[BaseModel] = XMLSearchToolSchema
 
-    def __init__(self, txt: Optional[str] = None, **kwargs):
+    def __init__(self, xml: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
-        if txt is not None:
-            self.add(txt)
-            self.description = f"A tool that can be used to semantic search a query the {txt} txt's content."
-            self.args_schema = FixedTXTSearchToolSchema
+        if xml is not None:
+            self.add(xml)
+            self.description = f"A tool that can be used to semantic search a query the {xml} XML's content."
+            self.args_schema = FixedXMLSearchToolSchema
             self._generate_description()
 
     def add(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        kwargs["data_type"] = DataType.TEXT_FILE
+        kwargs["data_type"] = DataType.XML
         super().add(*args, **kwargs)
 
     def _before_run(
         self,
         query: str,
         **kwargs: Any,
     ) -> Any:
-        if "txt" in kwargs:
-            self.add(kwargs["txt"])
+        if "xml" in kwargs:
+            self.add(kwargs["xml"])
 
     def _run(
         self,
         search_query: str,
         **kwargs: Any,
     ) -> Any:
         return super()._run(query=search_query)
```

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/website_search/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/website_search/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/xml_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/xml_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/youtube_channel_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/youtube_channel_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/youtube_video_search_tool/README.md` & `crewai_tools-0.2.4/crewai_tools/tools/youtube_video_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py` & `crewai_tools-0.2.4/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.3/pyproject.toml` & `crewai_tools-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.2.3"
+version = "0.2.4"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
@@ -15,14 +15,15 @@
 embedchain = {extras = ["github", "youtube"], version = "^0.1.85"}
 chromadb = "^0.4.22"
 pyright = "^1.1.350"
 pytube = "^15.0.0"
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.3"
 selenium = "^4.18.1"
+docx2txt = "^0.8"
 
 [tool.poetry.urls]
 Homepage = "https://crewai.com"
 Repository = "https://github.com/joaomdmoura/crewAI-tools"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `crewai_tools-0.2.3/PKG-INFO` & `crewai_tools-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: chromadb (>=0.4.22,<0.5.0)
+Requires-Dist: docx2txt (>=0.8,<0.9)
 Requires-Dist: embedchain[github,youtube] (>=0.1.85,<0.2.0)
 Requires-Dist: lancedb (>=0.5.4,<0.6.0)
 Requires-Dist: langchain (>=0.1.4,<0.2.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pyright (>=1.1.350,<2.0.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
```

