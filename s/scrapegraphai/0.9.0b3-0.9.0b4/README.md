# Comparing `tmp/scrapegraphai-0.9.0b3.tar.gz` & `tmp/scrapegraphai-0.9.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.9.0b3.tar", max compression
+gzip compressed data, was "scrapegraphai-0.9.0b4.tar", max compression
```

## Comparing `scrapegraphai-0.9.0b3.tar` & `scrapegraphai-0.9.0b4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1065 2024-05-05 00:19:51.770133 scrapegraphai-0.9.0b3/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-05 00:19:51.770133 scrapegraphai-0.9.0b3/README.md
--rw-r--r--   0        0        0     1792 2024-05-05 00:20:18.554206 scrapegraphai-0.9.0b3/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      449 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    11402 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3594 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3738 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     2068 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      369 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      479 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/claude.py
--rw-r--r--   0        0        0      487 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      736 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6987 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6431 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6987 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6987 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     6639 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4464 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     2140 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-05 15:57:07.774541 scrapegraphai-0.9.0b4/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-05 15:57:07.774541 scrapegraphai-0.9.0b4/README.md
+-rw-r--r--   0        0        0     1792 2024-05-05 15:57:28.602352 scrapegraphai-0.9.0b4/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      449 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    12384 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2440 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3359 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3628 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3379 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3513 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4297 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3502 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     2068 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      369 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      479 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/claude.py
+-rw-r--r--   0        0        0      487 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      736 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8591 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3721 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     7011 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6437 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7011 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6987 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     6645 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4470 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5611 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3713 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6267 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     2140 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b4/PKG-INFO
```

### Comparing `scrapegraphai-0.9.0b3/LICENSE` & `scrapegraphai-0.9.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/README.md` & `scrapegraphai-0.9.0b4/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/pyproject.toml` & `scrapegraphai-0.9.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.9.0b3"
+version = "0.9.0b4"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.9.0b4/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/abstract_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 AbstractGraph Module
 """
-
 from abc import ABC, abstractmethod
 from typing import Optional
-
-from langchain_aws.embeddings.bedrock import BedrockEmbeddings
-from langchain_community.embeddings import HuggingFaceHubEmbeddings, OllamaEmbeddings
 from langchain_openai import AzureOpenAIEmbeddings, OpenAIEmbeddings
-
+from langchain_community.embeddings import HuggingFaceHubEmbeddings, OllamaEmbeddings
 from ..helpers import models_tokens
 from ..models import AzureOpenAI, Bedrock, Gemini, Groq, HuggingFace, Ollama, OpenAI, Claude
+from langchain_aws.embeddings.bedrock import BedrockEmbeddings
+from langchain_google_genai import GoogleGenerativeAIEmbeddings
 
 
 class AbstractGraph(ABC):
     """
     Scaffolding class for creating a graph representation and executing it.
 
     Attributes:
@@ -48,32 +46,49 @@
         self.source = source
         self.config = config
         self.llm_model = self._create_llm(config["llm"], chat=True)
         self.embedder_model = self._create_default_embedder(
         ) if "embeddings" not in config else self._create_embedder(
             config["embeddings"])
 
+        # Create the graph
+        self.graph = self._create_graph()
+        self.final_state = None
+        self.execution_info = None
+
         # Set common configuration parameters
         self.verbose = True if config is None else config.get("verbose", False)
         self.headless = True if config is None else config.get(
             "headless", True)
+        common_params = {"headless": self.headless,
+                         "verbose": self.verbose,
+                         "llm_model": self.llm_model,
+                         "embedder_model": self.embedder_model}
+        self.set_common_params(common_params, overwrite=False)
 
-        # Create the graph
-        self.graph = self._create_graph()
-        self.final_state = None
-        self.execution_info = None
+
+    def set_common_params(self, params: dict, overwrite=False):
+        """
+        Pass parameters to every node in the graph unless otherwise defined in the graph.
+        
+        Args:
+            params (dict): Common parameters and their values.
+        """
+
+        for node in self.graph.nodes:
+            node.update_config(params, overwrite)
 
     def _set_model_token(self, llm):
 
         if 'Azure' in str(type(llm)):
             try:
                 self.model_token = models_tokens["azure"][llm.model_name]
             except KeyError:
                 raise KeyError("Model not supported")
-                
+
         elif 'HuggingFaceEndpoint' in str(type(llm)):
             if 'mistral' in llm.repo_id:
                 try:
                     self.model_token = models_tokens['mistral'][llm.repo_id]
                 except KeyError:
                     raise KeyError("Model not supported")
 
@@ -225,37 +240,38 @@
 
         Raises:
             KeyError: If the model is not supported.
         """
 
         if 'model_instance' in embedder_config:
             return embedder_config['model_instance']
-        
         # Instantiate the embedding model based on the model name
         if "openai" in embedder_config["model"]:
             return OpenAIEmbeddings(api_key=embedder_config["api_key"])
-
         elif "azure" in embedder_config["model"]:
             return AzureOpenAIEmbeddings()
-
         elif "ollama" in embedder_config["model"]:
             embedder_config["model"] = embedder_config["model"].split("/")[-1]
             try:
                 models_tokens["ollama"][embedder_config["model"]]
             except KeyError as exc:
                 raise KeyError("Model not supported") from exc
             return OllamaEmbeddings(**embedder_config)
-
         elif "hugging_face" in embedder_config["model"]:
             try:
                 models_tokens["hugging_face"][embedder_config["model"]]
             except KeyError as exc:
                 raise KeyError("Model not supported")from exc
             return HuggingFaceHubEmbeddings(model=embedder_config["model"])
-
+        elif "gemini" in embedder_config["model"]:
+            try:
+                models_tokens["gemini"][embedder_config["model"]]
+            except KeyError as exc:
+                raise KeyError("Model not supported")from exc
+            return GoogleGenerativeAIEmbeddings(model=embedder_config["model"])
         elif "bedrock" in embedder_config["model"]:
             embedder_config["model"] = embedder_config["model"].split("/")[-1]
             try:
                 models_tokens["bedrock"][embedder_config["model"]]
             except KeyError as exc:
                 raise KeyError("Model not supported") from exc
             return BedrockEmbeddings(client=None, model_id=embedder_config["model"])
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,42 +28,35 @@
     def _create_graph(self):
         """
         Creates the graph of nodes representing the workflow for web scraping.
         """
         fetch_node = FetchNode(
             input="csv_dir",
             output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
                 "chunk_size": self.model_token,
-                "verbose": self.verbose
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
+                "llm_model": self.llm_model,
                 "embedder_model": self.embedder_model,
-                "verbose": self.verbose
             }
         )
         generate_answer_node = GenerateAnswerCSVNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model,
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
                 parse_node,
@@ -81,8 +74,8 @@
     def run(self) -> str:
         """
         Executes the web scraping process and returns the answer to the prompt.
         """
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 """
-JSONScraperGraph Module
+PDFScraperGraph Module
 """
 
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
 
-class JSONScraperGraph(AbstractGraph):
+class PDFScraperGraph(AbstractGraph):
     """
-    JSONScraperGraph defines a scraping pipeline for JSON files.
+    PDFScraperGraph is a scraping pipeline that extracts information from pdf files using a natural
+    language model to interpret and answer prompts.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         llm_model: An instance of a language model client, configured for generating answers.
         embedder_model: An instance of an embedding model client, 
         configured for generating embeddings.
         verbose (bool): A flag indicating whether to show print statements during execution.
         headless (bool): A flag indicating whether to run the graph in headless mode.
+        model_token (int): The token limit for the language model.
 
     Args:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
 
     Example:
-        >>> json_scraper = JSONScraperGraph(
+        >>> pdf_scraper = PDFScraperGraph(
         ...     "List me all the attractions in Chioggia.",
-        ...     "data/chioggia.json",
+        ...     "data/chioggia.pdf",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
-        >>> result = json_scraper.run()
+        >>> result = pdf_scraper.run()
     """
 
     def __init__(self, prompt: str, source: str, config: dict):
         super().__init__(prompt, config, source)
 
-        self.input_key = "json" if source.endswith("json") else "json_dir"
+        self.input_key = "pdf" if source.endswith("pdf") else "pdf_dir"
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
 
         fetch_node = FetchNode(
-            input="json_dir",
+            input="pdf_dir",
             output=["doc"],
             node_config={
                 "headless": self.headless,
                 "verbose": self.verbose
             }
         )
         parse_node = ParseNode(
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-PDFScraperGraph Module
+XMLScraperGraph Module
 """
 
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
 
-class PDFScraperGraph(AbstractGraph):
+class XMLScraperGraph(AbstractGraph):
     """
-    PDFScraperGraph is a scraping pipeline that extracts information from pdf files using a natural
+    XMLScraperGraph is a scraping pipeline that extracts information from XML files using a natural
     language model to interpret and answer prompts.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         llm_model: An instance of a language model client, configured for generating answers.
@@ -30,66 +30,59 @@
 
     Args:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
 
     Example:
-        >>> pdf_scraper = PDFScraperGraph(
+        >>> xml_scraper = XMLScraperGraph(
         ...     "List me all the attractions in Chioggia.",
-        ...     "data/chioggia.pdf",
+        ...     "data/chioggia.xml",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
-        >>> result = pdf_scraper.run()
+        >>> result = xml_scraper.run()
     """
 
     def __init__(self, prompt: str, source: str, config: dict):
         super().__init__(prompt, config, source)
 
-        self.input_key = "pdf" if source.endswith("pdf") else "pdf_dir"
+        self.input_key = "xml" if source.endswith("xml") else "xml_dir"
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
 
         fetch_node = FetchNode(
-            input="pdf_dir",
-            output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
+            input="xml_dir",
+            output=["doc"]
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
-                "chunk_size": self.model_token,
-                "verbose": self.verbose
+                "chunk_size": self.model_token
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
-                "embedder_model": self.embedder_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model,
+                "embedder_model": self.embedder_model
             }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
                 parse_node,
@@ -111,8 +104,8 @@
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/script_creator_graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,40 +57,33 @@
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
 
         fetch_node = FetchNode(
             input="url | local_dir",
             output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={"chunk_size": self.model_token,
-                         "verbose": self.verbose
                          }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
-                "embedder_model": self.embedder_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model,
+                "embedder_model": self.embedder_model
             }
         )
         generate_scraper_node = GenerateScraperNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
-            node_config={"llm": self.llm_model,
-                         "verbose": self.verbose},
+            node_config={"llm_model": self.llm_model},
             library=self.library,
             website=self.source
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
@@ -113,8 +106,8 @@
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/search_graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,49 +46,41 @@
             BaseGraph: A graph instance representing the web scraping and searching workflow.
         """
 
         search_internet_node = SearchInternetNode(
             input="user_prompt",
             output=["url"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model
             }
         )
         fetch_node = FetchNode(
             input="url | local_dir",
-            output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
+            output=["doc"]
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
-                "chunk_size": self.model_token,
-                "verbose": self.verbose
+                "chunk_size": self.model_token
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
-                "embedder_model": self.embedder_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model,
+                "embedder_model": self.embedder_model
             }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model
             }
         )
 
         return BaseGraph(
             nodes=[
                 search_internet_node,
                 fetch_node,
@@ -112,8 +104,8 @@
         Returns:
             str: The answer to the prompt.
         """
         
         inputs = {"user_prompt": self.prompt}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,43 +53,36 @@
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
         fetch_node = FetchNode(
             input="url | local_dir",
-            output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
+            output=["doc"]
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
-                "chunk_size": self.model_token,
-                "verbose": self.verbose
+                "chunk_size": self.model_token
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
-                "embedder_model": self.embedder_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model,
+                "embedder_model": self.embedder_model
             }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
                 parse_node,
@@ -111,8 +104,8 @@
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/speech_graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,51 +52,42 @@
 
         Returns:
             BaseGraph: A graph instance representing the web scraping and audio generation workflow.
         """
 
         fetch_node = FetchNode(
             input="url | local_dir",
-            output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
+            output=["doc"]
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
-                "chunk_size": self.model_token,
-                "verbose": self.verbose
+                "chunk_size": self.model_token
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
-                "embedder_model": self.embedder_model,
-                "verbose": self.verbose
-            }
+                "llm_model": self.llm_model,
+                "embedder_model": self.embedder_model            }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model
             }
         )
         text_to_speech_node = TextToSpeechNode(
             input="answer",
             output=["audio"],
             node_config={
-                "tts_model": OpenAITextToSpeech(self.config["tts_model"]),
-                "verbose": self.verbose
+                "tts_model": OpenAITextToSpeech(self.config["tts_model"])
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
                 parse_node,
@@ -127,8 +118,8 @@
         audio = self.final_state.get("audio", None)
         if not audio:
             raise ValueError("No audio generated from the text.")
         save_audio_from_bytes(audio, self.config.get(
             "output_path", "output.mp3"))
         print(f"Audio saved to {self.config.get('output_path', 'output.mp3')}")
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.9.0b4/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,86 @@
 """
-XMLScraperGraph Module
+JSONScraperGraph Module
 """
 
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
 
-class XMLScraperGraph(AbstractGraph):
+class JSONScraperGraph(AbstractGraph):
     """
-    XMLScraperGraph is a scraping pipeline that extracts information from XML files using a natural
-    language model to interpret and answer prompts.
+    JSONScraperGraph defines a scraping pipeline for JSON files.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         llm_model: An instance of a language model client, configured for generating answers.
         embedder_model: An instance of an embedding model client, 
         configured for generating embeddings.
         verbose (bool): A flag indicating whether to show print statements during execution.
         headless (bool): A flag indicating whether to run the graph in headless mode.
-        model_token (int): The token limit for the language model.
 
     Args:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
 
     Example:
-        >>> xml_scraper = XMLScraperGraph(
+        >>> json_scraper = JSONScraperGraph(
         ...     "List me all the attractions in Chioggia.",
-        ...     "data/chioggia.xml",
+        ...     "data/chioggia.json",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
-        >>> result = xml_scraper.run()
+        >>> result = json_scraper.run()
     """
 
     def __init__(self, prompt: str, source: str, config: dict):
         super().__init__(prompt, config, source)
 
-        self.input_key = "xml" if source.endswith("xml") else "xml_dir"
+        self.input_key = "json" if source.endswith("json") else "json_dir"
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
 
         fetch_node = FetchNode(
-            input="xml_dir",
+            input="json_dir",
             output=["doc"],
-            node_config={
-                "headless": self.headless,
-                "verbose": self.verbose
-            }
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
-                "chunk_size": self.model_token,
-                "verbose": self.verbose
+                "chunk_size": self.model_token
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
-                "llm": self.llm_model,
-                "embedder_model": self.embedder_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model,
+                "embedder_model": self.embedder_model
             }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
-                "llm": self.llm_model,
-                "verbose": self.verbose
+                "llm_model": self.llm_model
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
                 parse_node,
@@ -111,8 +102,8 @@
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.9.0b4/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.9.0b4/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.9.0b4/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.9.0b4/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.9.0b4/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.9.0b4/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/base_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,29 @@
 
         Returns:
             dict: The updated state after executing the node's logic.
         """
 
         pass
 
+    def update_config(self, params: dict, overwrite: bool = False):
+        """
+        Updates the node_config dictionary as well as attributes with same key.
+
+        Args:
+            param (dict): The dictionary to update node_config with.
+            overwrite (bool): Flag indicating if the values of node_config should be overwritten if their value is not None.
+        """
+        if self.node_config is None:
+            self.node_config = {}
+        for key, val in params.items():
+            if hasattr(self, key) and (key not in self.node_config or overwrite):
+                self.node_config[key] = val
+                setattr(self, key, val)
+
     def get_input_keys(self, state: dict) -> List[str]:
         """
         Determines the necessary state keys based on the input specification.
 
         Args:
             state (dict): The current state of the graph used to parse input keys.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/fetch_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (Optional[dict]): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "Fetch".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: Optional[dict], node_name: str = "Fetch"):
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None, node_name: str = "Fetch"):
         super().__init__(node_name, "node", input, output, 1)
 
         self.headless = True if node_config is None else node_config.get("headless", True)
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state):
         """
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,41 +18,41 @@
     """
     A node that generates an answer using a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
 
     Attributes:
-        llm: An instance of a language model client, configured for generating answers.
+        llm_model: An instance of a language model client, configured for generating answers.
         node_name (str): The unique identifier name for the node, defaulting 
         to "GenerateAnswerNodeCsv".
         node_type (str): The type of the node, set to "node" indicating a 
         standard operational node.
 
     Args:
-        llm: An instance of the language model client (e.g., ChatOpenAI) used 
+        llm_model: An instance of the language model client (e.g., ChatOpenAI) used 
         for generating answers.
         node_name (str, optional): The unique identifier name for the node. 
         Defaults to "GenerateAnswerNodeCsv".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNodeCsv with a language model client and a node name.
         Args:
-            llm: An instance of the OpenAIImageToText class.
+            llm_model: An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
         super().__init__(node_name, "node", input, output, 2, node_config)
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get(
             "verbose", False)
 
     def execute(self, state):
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  node_name: str = "GenerateAnswer"):
         super().__init__(node_name, "node", input, output, 2, node_config)
         
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,41 +18,41 @@
     """
     A node that generates an answer using a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
 
     Attributes:
-        llm: An instance of a language model client, configured for generating answers.
+        llm_model: An instance of a language model client, configured for generating answers.
         node_name (str): The unique identifier name for the node, defaulting 
         to "GenerateAnswerNodeCsv".
         node_type (str): The type of the node, set to "node" indicating a 
         standard operational node.
 
     Args:
-        llm: An instance of the language model client (e.g., ChatOpenAI) used 
+        llm_model: An instance of the language model client (e.g., ChatOpenAI) used 
         for generating answers.
         node_name (str, optional): The unique identifier name for the node. 
         Defaults to "GenerateAnswerNodeCsv".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNodeCsv with a language model client and a node name.
         Args:
-            llm: An instance of the OpenAIImageToText class.
+            llm_model: An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
         super().__init__(node_name, "node", input, output, 2, node_config)
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get(
             "verbose", False)
 
     def execute(self, state):
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  library: str, website: str, node_name: str = "GenerateAnswer"):
         super().__init__(node_name, "node", input, output, 2, node_config)
 
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.library = library
         self.source = website
 
     def execute(self, state: dict) -> dict:
         """
         Generates a python script for scraping a website using the specified library.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/rag_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "Parse".
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "RAG"):
         super().__init__(node_name, "node", input, output, 2, node_config)
 
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.embedder_model = node_config.get("embedder_model", None)
         self.verbose = True if node_config is None else node_config.get(
             "verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Executes the node's logic to implement RAG (Retrieval-Augmented Generation).
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/robots_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         node_name (str): The unique identifier name for the node, defaulting to "Robots".
     """
 
     def __init__(self, input: str, output: List[str],  node_config: dict, force_scraping=True,
                  node_name: str = "Robots"):
         super().__init__(node_name, "node", input, output, 1)
 
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.force_scraping = force_scraping
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Checks if a website is scrapeable based on the robots.txt file and updates the state
         with the scrapeability status. The method constructs a prompt for the language model,
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_internet_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         node_name (str): The unique identifier name for the node, defaulting to "SearchInternet".
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  node_name: str = "SearchInternet"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_link_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict,
                  node_name: str = "GenerateLinks"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
-        self.llm_model = node_config["llm"]
+        self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Generates a list of links by extracting them from the provided HTML content.
         First, it tries to extract the links using classical methods, if it fails it uses the LLM to extract the links.
```

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.9.0b4/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/remover.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.9.0b4/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b3/PKG-INFO` & `scrapegraphai-0.9.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.9.0b3
+Version: 0.9.0b4
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

