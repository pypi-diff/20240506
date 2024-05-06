# Comparing `tmp/scrapegraphai-0.9.0b4.tar.gz` & `tmp/scrapegraphai-0.9.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.9.0b4.tar", max compression
+gzip compressed data, was "scrapegraphai-0.9.0b5.tar", max compression
```

## Comparing `scrapegraphai-0.9.0b4.tar` & `scrapegraphai-0.9.0b5.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0     1065 2024-05-05 15:57:07.774541 scrapegraphai-0.9.0b4/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-05 15:57:07.774541 scrapegraphai-0.9.0b4/README.md
--rw-r--r--   0        0        0     1792 2024-05-05 15:57:28.602352 scrapegraphai-0.9.0b4/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      449 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    12384 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2440 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3359 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3738 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3628 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3379 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3513 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4297 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3502 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     2068 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      369 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      479 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/claude.py
--rw-r--r--   0        0        0      487 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      736 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8591 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3721 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     7011 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6437 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7011 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6987 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     6645 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4470 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5611 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3713 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6267 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     2140 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-05 15:57:07.806541 scrapegraphai-0.9.0b4/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-06 07:53:56.108501 scrapegraphai-0.9.0b5/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-06 07:53:56.108501 scrapegraphai-0.9.0b5/README.md
+-rw-r--r--   0        0        0     1792 2024-05-06 07:54:14.396428 scrapegraphai-0.9.0b5/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      491 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    12385 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2440 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3359 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3628 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3585 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3513 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4297 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3502 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     2068 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      369 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      479 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/claude.py
+-rw-r--r--   0        0        0      487 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      835 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8591 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3721 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     7038 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6462 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7038 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     7014 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     6670 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3537 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     3041 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     1980 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3902 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     2709 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4495 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5664 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3932 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6292 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2342 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     2140 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b5/PKG-INFO
```

### Comparing `scrapegraphai-0.9.0b4/LICENSE` & `scrapegraphai-0.9.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/README.md` & `scrapegraphai-0.9.0b5/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/pyproject.toml` & `scrapegraphai-0.9.0b5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.9.0b4"
+version = "0.9.0b5"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.9.0b5/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/abstract_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         # Create the graph
         self.graph = self._create_graph()
         self.final_state = None
         self.execution_info = None
 
         # Set common configuration parameters
-        self.verbose = True if config is None else config.get("verbose", False)
+        self.verbose = False if config is None else config.get("verbose", False)
         self.headless = True if config is None else config.get(
             "headless", True)
         common_params = {"headless": self.headless,
                          "verbose": self.verbose,
                          "llm_model": self.llm_model,
                          "embedder_model": self.embedder_model}
         self.set_common_params(common_params, overwrite=False)
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/search_graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """ 
 SearchGraph Module
 """
 
 from .base_graph import BaseGraph
 from ..nodes import (
     SearchInternetNode,
-    FetchNode,
-    ParseNode,
-    RAGNode,
-    GenerateAnswerNode
+    GraphIteratorNode,
+    MergeAnswersNode
 )
 from .abstract_graph import AbstractGraph
+from .smart_scraper_graph import SmartScraperGraph
 
 
 class SearchGraph(AbstractGraph):
     """ 
     SearchGraph is a scraping pipeline that searches the internet for answers to a given prompt.
     It only requires a user prompt to search the internet and generate an answer.
 
@@ -34,69 +33,74 @@
         >>> search_graph = SearchGraph(
         ...     "What is Chioggia famous for?",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
         >>> result = search_graph.run()
     """
 
+    def __init__(self, prompt: str, config: dict):
+
+        self.max_results = config.get("max_results", 3)
+        super().__init__(prompt, config)
+
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping and searching.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping and searching workflow.
         """
 
+        # ************************************************
+        # Create a SmartScraperGraph instance
+        # ************************************************
+
+        smart_scraper_instance = SmartScraperGraph(
+            prompt="",
+            source="",
+            config=self.config
+        )
+
+        # ************************************************
+        # Define the graph nodes
+        # ************************************************
+
         search_internet_node = SearchInternetNode(
             input="user_prompt",
-            output=["url"],
+            output=["urls"],
             node_config={
-                "llm_model": self.llm_model
-            }
-        )
-        fetch_node = FetchNode(
-            input="url | local_dir",
-            output=["doc"]
-        )
-        parse_node = ParseNode(
-            input="doc",
-            output=["parsed_doc"],
-            node_config={
-                "chunk_size": self.model_token
+                "llm_model": self.llm_model,
+                "max_results": self.max_results
             }
         )
-        rag_node = RAGNode(
-            input="user_prompt & (parsed_doc | doc)",
-            output=["relevant_chunks"],
+        graph_iterator_node = GraphIteratorNode(
+            input="user_prompt & urls",
+            output=["results"],
             node_config={
-                "llm_model": self.llm_model,
-                "embedder_model": self.embedder_model
+                "graph_instance": smart_scraper_instance,
             }
         )
-        generate_answer_node = GenerateAnswerNode(
-            input="user_prompt & (relevant_chunks | parsed_doc | doc)",
+
+        merge_answers_node = MergeAnswersNode(
+            input="user_prompt & results",
             output=["answer"],
             node_config={
-                "llm_model": self.llm_model
+                "llm_model": self.llm_model,
             }
         )
 
         return BaseGraph(
             nodes=[
                 search_internet_node,
-                fetch_node,
-                parse_node,
-                rag_node,
-                generate_answer_node,
+                graph_iterator_node,
+                merge_answers_node
             ],
             edges=[
-                (search_internet_node, fetch_node),
-                (fetch_node, parse_node),
-                (parse_node, rag_node),
-                (rag_node, generate_answer_node)
+                (search_internet_node, graph_iterator_node),
+                (graph_iterator_node, merge_answers_node)
             ],
             entry_point=search_internet_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping and searching process.
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.9.0b5/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.9.0b5/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.9.0b5/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.9.0b5/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.9.0b5/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.9.0b5/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.9.0b5/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 from .image_to_text_node import ImageToTextNode
 from .search_internet_node import SearchInternetNode
 from .generate_scraper_node import GenerateScraperNode
 from .search_link_node import SearchLinkNode
 from .robots_node import RobotsNode
 from .generate_answer_csv_node import GenerateAnswerCSVNode
 from .generate_answer_pdf_node import GenerateAnswerPDFNode
+from .graph_iterator_node import GraphIteratorNode
+from .merge_answers_node import MergeAnswersNode
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module for generating the answer node
 """
 # Imports from standard library
-from typing import List
+from typing import List, Optional
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.runnables import RunnableParallel
 
@@ -35,15 +35,15 @@
         Defaults to "GenerateAnswerNodeCsv".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
                  node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNodeCsv with a language model client and a node name.
         Args:
             llm_model: An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 GenerateAnswerNode Module
 """
 
 # Imports from standard library
-from typing import List
+from typing import List, Optional
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.runnables import RunnableParallel
 
@@ -29,15 +29,15 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None,
                  node_name: str = "GenerateAnswer"):
         super().__init__(node_name, "node", input, output, 2, node_config)
         
         self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module for generating the answer node
 """
 # Imports from standard library
-from typing import List
+from typing import List, Optional
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.runnables import RunnableParallel
 
@@ -35,15 +35,15 @@
         Defaults to "GenerateAnswerNodeCsv".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
                  node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNodeCsv with a language model client and a node name.
         Args:
             llm_model: An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module for generating the answer node
 """
 # Imports from standard library
-from typing import List
+from typing import List, Optional
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.runnables import RunnableParallel
 
@@ -35,15 +35,15 @@
         Defaults to "GenerateAnswerNodePDF".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
                  node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNodePDF with a language model client and a node name.
         Args:
             llm: An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 GenerateScraperNode Module
 """
 
 # Imports from standard library
-from typing import List
+from typing import List, Optional
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.runnables import RunnableParallel
 
@@ -32,16 +32,16 @@
         node_config (dict): Additional configuration for the node.
         library (str): The python library to use for scraping the website.
         website (str): The website to scrape.
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
 
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
-                 library: str, website: str, node_name: str = "GenerateAnswer"):
+    def __init__(self, input: str, output: List[str], library: str, website: str,
+                 node_config: Optional[dict]=None, node_name: str = "GenerateAnswer"):
         super().__init__(node_name, "node", input, output, 2, node_config)
 
         self.llm_model = node_config["llm_model"]
         self.library = library
         self.source = website
 
     def execute(self, state: dict) -> dict:
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 GetProbableTagsNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from langchain.output_parsers import CommaSeparatedListOutputParser
 from langchain.prompts import PromptTemplate
 from .base_node import BaseNode
 
 
 class GetProbableTagsNode(BaseNode):
     """
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/image_to_text_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 ImageToTextNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from .base_node import BaseNode
 
 
 class ImageToTextNode(BaseNode):
     """
     Retrieve an image from an URL and convert it to text using an ImageToText model.
 
@@ -17,15 +17,15 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "ImageToText".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None,
                  node_name: str = "ImageToText"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/parse_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 ParseNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_community.document_transformers import Html2TextTransformer
 from .base_node import BaseNode
 
 
 class ParseNode(BaseNode):
     """
@@ -22,15 +22,15 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "Parse".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "Parse"):
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None, node_name: str = "Parse"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self,  state: dict) -> dict:
         """
         Executes the node's logic to parse the HTML document content and split it into chunks.
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/rag_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 RAGNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from langchain.docstore.document import Document
 from langchain.retrievers import ContextualCompressionRetriever
 from langchain.retrievers.document_compressors import EmbeddingsFilter, DocumentCompressorPipeline
 from langchain_community.document_transformers import EmbeddingsRedundantFilter
 from langchain_community.vectorstores import FAISS
 
 from .base_node import BaseNode
@@ -27,15 +27,15 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "Parse".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "RAG"):
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None, node_name: str = "RAG"):
         super().__init__(node_name, "node", input, output, 2, node_config)
 
         self.llm_model = node_config["llm_model"]
         self.embedder_model = node_config.get("embedder_model", None)
         self.verbose = True if node_config is None else node_config.get(
             "verbose", False)
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/robots_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 RobotsNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from urllib.parse import urlparse
-from langchain_community.document_loaders import AsyncHtmlLoader
+from langchain_community.document_loaders import AsyncChromiumLoader
 from langchain.prompts import PromptTemplate
 from langchain.output_parsers import CommaSeparatedListOutputParser
 from .base_node import BaseNode
 from ..helpers import robots_dictionary
 
 
 class RobotsNode(BaseNode):
@@ -30,15 +30,15 @@
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         force_scraping (bool): A flag indicating whether scraping should be enforced even
                                  if disallowed by robots.txt. Defaults to True.
         node_name (str): The unique identifier name for the node, defaulting to "Robots".
     """
 
-    def __init__(self, input: str, output: List[str],  node_config: dict, force_scraping=True,
+    def __init__(self, input: str, output: List[str],  node_config: Optional[dict]=None, force_scraping=True,
                  node_name: str = "Robots"):
         super().__init__(node_name, "node", input, output, 1)
 
         self.llm_model = node_config["llm_model"]
         self.force_scraping = force_scraping
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
@@ -89,19 +89,19 @@
         if not source.startswith("http"):
             raise ValueError(
                 "Operation not allowed")
 
         else:
             parsed_url = urlparse(source)
             base_url = f"{parsed_url.scheme}://{parsed_url.netloc}"
-            loader = AsyncHtmlLoader(f"{base_url}/robots.txt")
+            loader = AsyncChromiumLoader(f"{base_url}/robots.txt")
             document = loader.load()
-            if "ollama" in self.llm_model.model:
-                self.llm_model.model = self.llm_model.model.split("/")[-1]
-                model = self.llm_model.model.split("/")[-1]
+            if "ollama" in self.llm_model.model_name:
+                self.llm_model.model_name = self.llm_model.model_name.split("/")[-1]
+                model = self.llm_model.model_name.split("/")[-1]
 
             else:
                 model = self.llm_model.model_name
             try:
                 agent = robots_dictionary[model]
 
             except KeyError:
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_internet_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 SearchInternetNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from langchain.output_parsers import CommaSeparatedListOutputParser
 from langchain.prompts import PromptTemplate
 from ..utils.research_web import search_on_web
 from .base_node import BaseNode
 
 
 class SearchInternetNode(BaseNode):
@@ -23,20 +23,21 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "SearchInternet".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None,
                  node_name: str = "SearchInternet"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
+        self.max_results = node_config.get("max_results", 3)
 
     def execute(self, state: dict) -> dict:
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
 
         The method updates the state with the generated answer.
@@ -81,13 +82,16 @@
         # Execute the chain to get the search query
         search_answer = search_prompt | self.llm_model | output_parser
         search_query = search_answer.invoke({"user_prompt": user_prompt})[0]
 
         if self.verbose:
             print(f"Search Query: {search_query}")
             
-        # TODO: handle multiple URLs
-        answer = search_on_web(query=search_query, max_results=1)[0]
+        answer = search_on_web(query=search_query, max_results=self.max_results)
+
+        if len(answer) == 0:
+            # raise an exception if no answer is found
+            raise ValueError("Zero results found for the search query.")
 
         # Update the state with the generated answer
         state.update({self.output[0]: answer})
         return state
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_link_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 SearchLinkNode Module
 """
 
 # Imports from standard library
-from typing import List
+from typing import List, Optional
 from tqdm import tqdm
 from bs4 import BeautifulSoup
 
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
@@ -29,15 +29,15 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: dict,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None,
                  node_name: str = "GenerateLinks"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.llm_model = node_config["llm_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.9.0b5/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 TextToSpeechNode Module
 """
 
-from typing import List
+from typing import List, Optional
 from .base_node import BaseNode
 
 
 class TextToSpeechNode(BaseNode):
     """
     Converts text to speech using the specified text-to-speech model.
 
@@ -18,15 +18,15 @@
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "TextToSpeech".
     """
 
     def __init__(self, input: str, output: List[str],
-                 node_config: dict, node_name: str = "TextToSpeech"):
+                 node_config: Optional[dict]=None, node_name: str = "TextToSpeech"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.tts_model = node_config["tts_model"]
         self.verbose = True if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
```

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/remover.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.9.0b5/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b4/PKG-INFO` & `scrapegraphai-0.9.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.9.0b4
+Version: 0.9.0b5
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

