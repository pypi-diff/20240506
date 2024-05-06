# Comparing `tmp/scrapegraphai-0.9.0b5.tar.gz` & `tmp/scrapegraphai-0.9.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.9.0b5.tar", max compression
+gzip compressed data, was "scrapegraphai-0.9.0b6.tar", max compression
```

## Comparing `scrapegraphai-0.9.0b5.tar` & `scrapegraphai-0.9.0b6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1065 2024-05-06 07:53:56.108501 scrapegraphai-0.9.0b5/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-06 07:53:56.108501 scrapegraphai-0.9.0b5/README.md
--rw-r--r--   0        0        0     1792 2024-05-06 07:54:14.396428 scrapegraphai-0.9.0b5/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      491 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    12385 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2440 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3359 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3738 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3628 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3585 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3513 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4297 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3502 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     2068 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      369 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      479 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/claude.py
--rw-r--r--   0        0        0      487 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      835 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8591 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3721 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     7038 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6462 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7038 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     7014 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     6670 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3537 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     3041 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     1980 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3902 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     2709 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4495 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5664 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3932 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6292 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2342 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     2140 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-06 07:53:56.140500 scrapegraphai-0.9.0b5/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-06 10:31:12.315757 scrapegraphai-0.9.0b6/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-06 10:31:12.315757 scrapegraphai-0.9.0b6/README.md
+-rw-r--r--   0        0        0     1792 2024-05-06 10:31:31.563793 scrapegraphai-0.9.0b6/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      491 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    12862 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2440 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3359 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3628 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3569 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3513 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4297 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3502 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      369 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-06 10:31:12.343757 scrapegraphai-0.9.0b6/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      479 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/claude.py
+-rw-r--r--   0        0        0      487 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      835 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8591 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3721 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     7038 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6462 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7038 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     7014 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     6670 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3537 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     3041 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     1980 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3902 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     2709 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4495 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5664 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3948 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6307 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2342 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     2140 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-06 10:31:12.347757 scrapegraphai-0.9.0b6/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b6/PKG-INFO
```

### Comparing `scrapegraphai-0.9.0b5/LICENSE` & `scrapegraphai-0.9.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/README.md` & `scrapegraphai-0.9.0b6/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/pyproject.toml` & `scrapegraphai-0.9.0b6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.9.0b5"
+version = "0.9.0b6"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.9.0b6/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/abstract_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def __init__(self, prompt: str, config: dict, source: Optional[str] = None):
 
         self.prompt = prompt
         self.source = source
         self.config = config
         self.llm_model = self._create_llm(config["llm"], chat=True)
-        self.embedder_model = self._create_default_embedder(
+        self.embedder_model = self._create_default_embedder(llm_config=config["llm"]
         ) if "embeddings" not in config else self._create_embedder(
             config["embeddings"])
 
         # Create the graph
         self.graph = self._create_graph()
         self.final_state = None
         self.execution_info = None
@@ -87,14 +87,21 @@
 
         elif 'HuggingFaceEndpoint' in str(type(llm)):
             if 'mistral' in llm.repo_id:
                 try:
                     self.model_token = models_tokens['mistral'][llm.repo_id]
                 except KeyError:
                     raise KeyError("Model not supported")
+                
+        elif 'Google' in str(type(llm)):
+            try:
+                if 'gemini' in llm.model:
+                    self.model_token = models_tokens['gemini'][llm.model]
+            except KeyError:
+                raise KeyError("Model not supported")
 
     def _create_llm(self, llm_config: dict, chat=False) -> object:
         """
         Create a large language model instance based on the configuration provided.
 
         Args:
             llm_config (dict): Configuration parameters for the language model.
@@ -193,24 +200,26 @@
                     "temperature": llm_params["temperature"],
                 }
             })
         else:
             raise ValueError(
                 "Model provided by the configuration not supported")
 
-    def _create_default_embedder(self) -> object:
+    def _create_default_embedder(self, llm_config=None) -> object:
         """
         Create an embedding model instance based on the chosen llm model.
 
         Returns:
             object: An instance of the embedding model client.
 
         Raises:
             ValueError: If the model is not supported.
         """
+        if isinstance(self.llm_model, Gemini):
+            return GoogleGenerativeAIEmbeddings(google_api_key=llm_config['api_key'], model="models/embedding-001")
         if isinstance(self.llm_model, OpenAI):
             return OpenAIEmbeddings(api_key=self.llm_model.openai_api_key)
         elif isinstance(self.llm_model, AzureOpenAIEmbeddings):
             return self.llm_model
         elif isinstance(self.llm_model, AzureOpenAI):
             return AzureOpenAIEmbeddings()
         elif isinstance(self.llm_model, Ollama):
@@ -237,15 +246,14 @@
 
         Returns:
             object: An instance of the embedding model client.
 
         Raises:
             KeyError: If the model is not supported.
         """
-
         if 'model_instance' in embedder_config:
             return embedder_config['model_instance']
         # Instantiate the embedding model based on the model name
         if "openai" in embedder_config["model"]:
             return OpenAIEmbeddings(api_key=embedder_config["api_key"])
         elif "azure" in embedder_config["model"]:
             return AzureOpenAIEmbeddings()
```

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/search_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,15 @@
             ],
             entry_point=search_internet_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping and searching process.
-        
+
         Returns:
             str: The answer to the prompt.
         """
-        
         inputs = {"user_prompt": self.prompt}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.9.0b6/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.9.0b6/scrapegraphai/helpers/models_tokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "azure": {
         "gpt-3.5-turbo": 4096,
         "gpt-4": 8192,
         "gpt-4-32k": 32768
     },
     "gemini": {
         "gemini-pro": 128000,
+        "models/embedding-001": 2048
     },
 
     "ollama": {
         "llama2": 4096,
         "llama3": 8192,
         "mistral": 8192,
         "codellama": 16000,
```

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.9.0b6/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.9.0b6/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.9.0b6/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.9.0b6/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.9.0b6/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/search_internet_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "SearchInternet".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
                  node_name: str = "SearchInternet"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.llm_model = node_config["llm_model"]
-        self.verbose = True if node_config is None else node_config.get("verbose", False)
+        self.verbose = True if node_config is None else node_config.get(
+            "verbose", False)
         self.max_results = node_config.get("max_results", 3)
 
     def execute(self, state: dict) -> dict:
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
 
@@ -81,16 +82,17 @@
 
         # Execute the chain to get the search query
         search_answer = search_prompt | self.llm_model | output_parser
         search_query = search_answer.invoke({"user_prompt": user_prompt})[0]
 
         if self.verbose:
             print(f"Search Query: {search_query}")
-            
-        answer = search_on_web(query=search_query, max_results=self.max_results)
+
+        answer = search_on_web(
+            query=search_query, max_results=self.max_results)
 
         if len(answer) == 0:
             # raise an exception if no answer is found
             raise ValueError("Zero results found for the search query.")
 
         # Update the state with the generated answer
         state.update({self.output[0]: answer})
```

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/search_link_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,21 @@
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: Optional[dict]=None,
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
                  node_name: str = "GenerateLinks"):
         super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.llm_model = node_config["llm_model"]
-        self.verbose = True if node_config is None else node_config.get("verbose", False)
+        self.verbose = True if node_config is None else node_config.get(
+            "verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Generates a list of links by extracting them from the provided HTML content.
         First, it tries to extract the links using classical methods, if it fails it uses the LLM to extract the links.
 
         Args:
@@ -69,18 +70,19 @@
         try:
             links = []
             for elem in doc:
                 soup = BeautifulSoup(elem.content, 'html.parser')
                 links.append(soup.find_all("a"))
             state.update({self.output[0]: {elem for elem in links}})
 
-        except Exception as e:
+        except Exception:
             if self.verbose:
-                print("Error extracting links using classical methods. Using LLM to extract links.")
-                
+                print(
+                    "Error extracting links using classical methods. Using LLM to extract links.")
+
             output_parser = JsonOutputParser()
 
             template_chunks = """
             You are a website scraper and you have just scraped the
             following content from a website.
             You are now asked to find all the links inside this page.\n 
             The website is big so I am giving you one chunk at the time to be merged later with the other chunks.\n
```

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.9.0b6/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/remover.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.9.0b6/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b5/PKG-INFO` & `scrapegraphai-0.9.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.9.0b5
+Version: 0.9.0b6
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

