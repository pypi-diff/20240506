# Comparing `tmp/semantic_kernel-0.9.6b1.tar.gz` & `tmp/semantic_kernel-0.9.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.9.6b1.tar", max compression
+gzip compressed data, was "semantic_kernel-0.9.7b1.tar", max compression
```

## Comparing `semantic_kernel-0.9.6b1.tar` & `semantic_kernel-0.9.7b1.tar`

### file list

```diff
@@ -1,227 +1,222 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.6b1/pip/README.md
--rw-r--r--   0        0        0     5363 2024-04-16 13:30:52.646626 semantic_kernel-0.9.6b1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3592 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      417 2024-03-13 15:37:17.045380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1746 2024-03-13 15:37:17.045380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10227 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     3822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     2229 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1122 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6673 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2094 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8390 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3968 2024-03-20 18:24:28.763758 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1804 2024-03-20 18:24:28.763758 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2580 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/__init__.py
--rw-r--r--   0        0        0     1510 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/azure_chat_message_content.py
--rw-r--r--   0        0        0     4442 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/azure_streaming_chat_message_content.py
--rw-r--r--   0        0        0     1992 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
--rw-r--r--   0        0        0     3027 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_chat_message_content.py
--rw-r--r--   0        0        0     4256 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_streaming_chat_message_content.py
--rw-r--r--   0        0        0      844 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/contents/tool_calls.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     3972 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    14685 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    18930 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6335 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0      820 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py
--rw-r--r--   0        0        0     6935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/utils.py
--rw-r--r--   0        0        0     3653 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1652 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6364 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0     9405 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      937 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0     7409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14863 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    13477 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.6b1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      641 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0    12644 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0     3360 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0     3278 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/chat_message_content_base.py
--rw-r--r--   0        0        0      211 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/contents/chat_role.py
--rw-r--r--   0        0        0      600 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0      515 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0     3326 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      564 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2602 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     1144 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      747 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4084 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2489 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     3495 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2673 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8045 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1804 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/events/__init__.py
--rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/events/function_invoked_event_args.py
--rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/events/function_invoking_event_args.py
--rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/events/kernel_events_args.py
--rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2445 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1542 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0     9393 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     5257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     7579 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    17627 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1877 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0      541 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    23093 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      769 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      225 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    36028 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6273 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3548 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     1310 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      126 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/action_planner/__init__.py
--rw-r--r--   0        0        0    11352 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/action_planner/action_planner.py
--rw-r--r--   0        0        0      392 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/action_planner/action_planner_config.py
--rw-r--r--   0        0        0      409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/action_planner/skprompt.txt
--rw-r--r--   0        0        0     8152 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/basic_planner.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    11033 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1676 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      886 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      622 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5924 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4729 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      881 2024-03-13 15:37:17.055380 semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json
--rw-r--r--   0        0        0     2847 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
--rw-r--r--   0        0        0      243 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/__init__.py
--rw-r--r--   0        0        0    16330 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py
--rw-r--r--   0        0        0      982 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py
--rw-r--r--   0        0        0      371 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/system_step.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      644 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4128 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4670 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     7935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     4762 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4521 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2412 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.6b1/semantic_kernel/py.typed
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2555 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7402 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0    11160 2024-04-16 13:30:52.656626 semantic_kernel-0.9.6b1/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.6b1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 semantic_kernel-0.9.6b1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.7b1/pip/README.md
+-rw-r--r--   0        0        0     5404 2024-05-06 13:16:31.745032 semantic_kernel-0.9.7b1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3223 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0     9646 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     3821 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     2191 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6662 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8403 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3962 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     4031 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    16094 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    18726 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6342 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0      820 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py
+-rw-r--r--   0        0        0     6935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/utils.py
+-rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1720 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    10299 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14863 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    13518 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.7b1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    13781 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12276 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     3729 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     3913 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    11084 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     1957 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      747 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/events/__init__.py
+-rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoked_event_args.py
+-rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoking_event_args.py
+-rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/events/kernel_events_args.py
+-rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1601 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0     9539 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     5517 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0     7585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    17580 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1912 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    23557 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      791 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    38918 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     1310 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/__init__.py
+-rw-r--r--   0        0        0    11352 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/action_planner.py
+-rw-r--r--   0        0        0      392 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/action_planner_config.py
+-rw-r--r--   0        0        0      409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/skprompt.txt
+-rw-r--r--   0        0        0     8152 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/basic_planner.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    11240 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1676 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      886 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      622 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5924 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4729 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      881 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json
+-rw-r--r--   0        0        0     2847 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
+-rw-r--r--   0        0        0      243 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    16330 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py
+-rw-r--r--   0        0        0      982 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py
+-rw-r--r--   0        0        0      371 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/system_step.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4128 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4670 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     7935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     4762 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2476 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2555 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7402 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0    12327 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5107 1970-01-01 00:00:00.000000 semantic_kernel-0.9.7b1/PKG-INFO
```

### Comparing `semantic_kernel-0.9.6b1/pip/README.md` & `semantic_kernel-0.9.7b1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/pyproject.toml` & `semantic_kernel-0.9.7b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.9.6b1"
+version = "0.9.7b1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.13"
+python = "^3.10,<3.13"
 aiohttp = "^3.8"
 numpy = [
     { version = "^1.24", python = "3.8" },
     { version = ">=1.25", python = ">=3.9,<3.12" },
     { version = ">=1.26", python = ">=3.12" },
 ]
 scipy = [
@@ -66,20 +66,20 @@
 usearch = { version = "^2.9", optional = true}
 pyarrow = { version = ">=12.0.1,<16.0.0", optional = true}
 
 # Groups are for development only (installed through Poetry)
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.5"
 black = "^24.2.0"
-ruff = "^0.3.2"
+ruff = ">=0.3.2,<0.5.0"
 ipykernel = "^6.29.3"
 pytest = "^8.1.1"
-pytest-asyncio = "^0.23.5.post1"
+pytest-asyncio = "^0.23.6"
 snoop = "^0.4.3"
-pytest-cov = ">=4.1.0"
+pytest-cov = ">=5.0.0"
 mypy = ">=1.9.0"
 types-PyYAML = "^6.0.12.20240311"
 
 [tool.poetry.group.unit-tests]
 optional = true
 
 [tool.poetry.group.unit-tests.dependencies]
@@ -114,27 +114,28 @@
 psycopg = { version="^3.1.9", extras=["binary","pool"]}
 redis = "^4.6.0"
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
 azure-core = "^1.28.0"
 azure-identity = "^1.13.0"
 usearch = "^2.9"
 pyarrow = ">=12.0.1,<16.0.0"
+msgraph-sdk = "^1.2.0"
 
 # Extras are exposed to pip, this allows a user to easily add the right dependencies to their environment
 [tool.poetry.extras]
 google = ["google-generativeai", "grpcio-status"]
 hugging_face = ["transformers", "sentence-transformers", "torch"]
 qdrant = ["qdrant-client"]
 chromadb = ["chromadb"]
 milvus = ["pymilvus", "milvus"]
 weaviate = ["weaviate-client"]
 pinecone = ["pinecone-client"]
 postgres = ["psycopg"]
 redis = ["redis"]
-azure = ["azure-search-documents", "azure-core", "azure-identity"]
+azure = ["azure-search-documents", "azure-core", "azure-identity", "msgraph-sdk"]
 usearch = ["usearch", "pyarrow"]
 notebooks = ["ipykernel"]
 all = ["google-generativeai", "grpcio-status", "transformers", "sentence-transformers", "torch", "qdrant-client", "chromadb", "pymilvus", "milvus", "weaviate-client", "pinecone-client", "psycopg", "redis", "azure-search-documents", "azure-core", "azure-identity", "usearch", "pyarrow", "ipykernel"]
 
 [tool.ruff]
 lint.select = ["E", "F", "I"]
 line-length = 120
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, AsyncGenerator
 
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
     from semantic_kernel.contents.chat_history import ChatHistory
     from semantic_kernel.contents.chat_message_content import ChatMessageContent
     from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
 
 
 class ChatCompletionClientBase(AIServiceClientBase, ABC):
-    def get_chat_message_content_type(self) -> str:
-        """Get the chat message content types used by a class, default is 'ChatMessageContent'."""
-        return "ChatMessageContent"
-
     @abstractmethod
     async def complete_chat(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
-    ) -> List["ChatMessageContent"]:
+    ) -> list["ChatMessageContent"]:
         """
         This is the method that is called from the kernel to get a response from a chat-optimized LLM.
 
         Arguments:
             chat_history {ChatHistory} -- A list of chats in a chat_history object, that can be
                 rendered into messages from system, user, assistant and tools.
             settings {PromptExecutionSettings} -- Settings for the request.
@@ -35,52 +32,49 @@
 
         Returns:
             Union[str, List[str]] -- A string or list of strings representing the response(s) from the LLM.
         """
         pass
 
     @abstractmethod
-    async def complete_chat_stream(
+    def complete_chat_stream(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
-    ) -> AsyncIterable[List["StreamingChatMessageContent"]]:
+    ) -> AsyncGenerator[list["StreamingChatMessageContent"], Any]:
         """
         This is the method that is called from the kernel to get a stream response from a chat-optimized LLM.
 
         Arguments:
             chat_history {ChatHistory} -- A list of chat chat_history, that can be rendered into a
                 set of chat_history, from system, user, assistant and function.
             settings {PromptExecutionSettings} -- Settings for the request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
 
         Yields:
             A stream representing the response(s) from the LLM.
         """
-        pass
+        ...
 
     def _prepare_chat_history_for_request(
         self,
         chat_history: "ChatHistory",
-    ) -> List[Dict[str, Optional[str]]]:
+        role_key: str = "role",
+        content_key: str = "content",
+    ) -> list[dict[str, str | None]]:
         """
         Prepare the chat history for a request, allowing customization of the key names for role/author,
         and optionally overriding the role.
 
         ChatRole.TOOL messages need to be formatted different than system/user/assistant messages:
             They require a "tool_call_id" and (function) "name" key, and the "metadata" key should
             be removed. The "encoding" key should also be removed.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to prepare.
 
         Returns:
             List[Dict[str, Optional[str]]] -- The prepared chat history.
         """
-        return [self._chat_message_content_to_dict(message) for message in chat_history.messages]
-
-    def _chat_message_content_to_dict(self, message: "ChatMessageContent") -> Dict[str, Optional[str]]:
-        """can be overridden to customize the serialization of the chat message content"""
-        msg = message.model_dump(include=["role", "content"])
-        return msg
+        return [message.to_dict(role_key=role_key, content_key=content_key) for message in chat_history.messages]
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 from pydantic import Field, model_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.exceptions import ServiceInvalidExecutionSettingsError
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import sys
-from typing import Any, Dict, List, Optional, Tuple
-
-from semantic_kernel.contents.chat_message_content import ChatMessageContent
-from semantic_kernel.contents.text_content import TextContent
-from semantic_kernel.exceptions import ServiceInvalidRequestError, ServiceResponseException
+from typing import Any, List, Optional, Tuple
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 import google.generativeai as palm
@@ -20,20 +16,23 @@
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.google_palm.gp_prompt_execution_settings import (
     GooglePalmChatPromptExecutionSettings,
     GooglePalmPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_history import ChatHistory
-from semantic_kernel.contents.chat_role import ChatRole
+from semantic_kernel.contents.chat_message_content import ChatMessageContent
+from semantic_kernel.contents.text_content import TextContent
+from semantic_kernel.exceptions import ServiceInvalidRequestError, ServiceResponseException
 
 logger: logging.Logger = logging.getLogger(__name__)
 
-int_to_role = {1: ChatRole.USER, 2: ChatRole.SYSTEM, 3: ChatRole.ASSISTANT, 4: ChatRole.TOOL}
+int_to_role = {1: AuthorRole.USER, 2: AuthorRole.SYSTEM, 3: AuthorRole.ASSISTANT, 4: AuthorRole.TOOL}
 
 
 class GooglePalmChatCompletion(ChatCompletionClientBase, TextCompletionClientBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
     _message_history: Optional[ChatHistory] = PrivateAttr()
     service_id: Optional[str] = None
 
@@ -73,15 +72,15 @@
                 set of messages, from system, user, assistant and function.
             settings {GooglePalmPromptExecutionSettings} -- Settings for the request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
         Returns:
             List[ChatMessageContent] -- A list of ChatMessageContent objects representing the response(s) from the LLM.
         """
-        settings.messages = self._prepare_chat_history_for_request(chat_history)
+        settings.messages = self._prepare_chat_history_for_request(chat_history, role_key="author")
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         response = await self._send_chat_request(settings)
         return [
             self._create_chat_message_content(response, candidate, index)
             for index, candidate in enumerate(response.candidates)
         ]
@@ -224,22 +223,7 @@
                 ex,
             ) from ex
         return response
 
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return GooglePalmChatPromptExecutionSettings
-
-    def _prepare_chat_history_for_request(
-        self,
-        chat_history: ChatHistory,
-    ) -> List[Dict[str, Optional[str]]]:
-        """
-        Prepare the chat history for a request, allowing customization of the key names for role/author,
-        and optionally overriding the role.
-        """
-        standard_out = super()._prepare_chat_history_for_request(chat_history)
-        for message in standard_out:
-            message["author"] = message.pop("role")
-        # The last message should always be from the user
-        standard_out[-1]["author"] = "user"
-        return standard_out
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import sys
 from typing import List
 
-from semantic_kernel.contents.text_content import TextContent
-from semantic_kernel.exceptions import ServiceResponseException
-
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 import google.generativeai as palm
 from google.generativeai.types import Completion
 from google.generativeai.types.text_types import TextCompletion
 from pydantic import StringConstraints
 
 from semantic_kernel.connectors.ai.google_palm.gp_prompt_execution_settings import GooglePalmTextPromptExecutionSettings
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.contents.text_content import TextContent
+from semantic_kernel.exceptions import ServiceResponseException
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class GooglePalmTextCompletion(TextCompletionClientBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 import sys
-from typing import List
+from typing import Any, List
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 import google.generativeai as palm
 from numpy import array, ndarray
 from pydantic import StringConstraints
 
-from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
-    EmbeddingGeneratorBase,
-)
+from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.exceptions import ServiceInvalidAuthError, ServiceResponseException
 
 
 class GooglePalmTextEmbedding(EmbeddingGeneratorBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
 
     def __init__(self, ai_model_id: str, api_key: str) -> None:
@@ -30,15 +28,15 @@
             ai_model_id {str} -- GooglePalm model name, see
             https://developers.generativeai.google/models/language
             api_key {str} -- GooglePalm API key, see
             https://developers.generativeai.google/products/palm
         """
         super().__init__(ai_model_id=ai_model_id, api_key=api_key)
 
-    async def generate_embeddings(self, texts: List[str]) -> ndarray:
+    async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
             texts {List[str]} -- Texts to generate embeddings for.
 
         Returns:
@@ -50,18 +48,15 @@
             raise ServiceInvalidAuthError(
                 "Google PaLM service failed to configure. Invalid API key provided.",
                 ex,
             ) from ex
         embeddings = []
         for text in texts:
             try:
-                response = palm.generate_embeddings(
-                    model=self.ai_model_id,
-                    text=text,
-                )
+                response = palm.generate_embeddings(model=self.ai_model_id, text=text, **kwargs)
                 embeddings.append(array(response["embedding"]))
             except Exception as ex:
                 raise ServiceResponseException(
                     "Google PaLM service failed to generate the embedding.",
                     ex,
                 ) from ex
         return array(embeddings)
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 class HuggingFacePromptExecutionSettings(PromptExecutionSettings):
     do_sample: bool = True
     max_new_tokens: int = 256
     num_return_sequences: int = 1
     stop_sequences: Any = None
     pad_token_id: int = 50256
-    temperature: float = 0.0
+    eos_token_id: int = 50256
+    temperature: float = 1.0
     top_p: float = 1.0
 
     def get_generation_config(self) -> GenerationConfig:
         return GenerationConfig(
             **self.model_dump(
-                include={"max_new_tokens", "pad_token_id", "temperature", "top_p"},
-                exclude_unset=True,
+                include={"max_new_tokens", "pad_token_id", "eos_token_id", "temperature", "top_p"},
+                exclude_unset=False,
                 exclude_none=True,
                 by_alias=True,
             )
         )
 
     def prepare_settings_dict(self, **kwargs) -> Dict[str, Any]:
         gen_config = self.get_generation_config()
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from threading import Thread
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Literal, Optional
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Literal, Optional
 
 import torch
 from transformers import AutoTokenizer, TextIteratorStreamer, pipeline
 
-from semantic_kernel.connectors.ai.hugging_face.hf_prompt_execution_settings import (
-    HuggingFacePromptExecutionSettings,
-)
-from semantic_kernel.connectors.ai.text_completion_client_base import (
-    TextCompletionClientBase,
-)
+from semantic_kernel.connectors.ai.hugging_face.hf_prompt_execution_settings import HuggingFacePromptExecutionSettings
+from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import ServiceInvalidExecutionSettingsError, ServiceResponseException
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 
@@ -107,15 +103,15 @@
             text=candidate["summary_text" if self.task == "summarization" else "generated_text"],
         )
 
     async def complete_stream(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
-    ) -> AsyncIterable[List[StreamingTextContent]]:
+    ) -> AsyncGenerator[List[StreamingTextContent], Any]:
         """
         Streams a text completion using a Hugging Face model.
         Note that this method does not support multiple responses.
 
         Arguments:
             prompt {str} -- Prompt to complete.
             settings {HuggingFacePromptExecutionSettings} -- Request settings.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,23 +38,23 @@
         super().__init__(
             ai_model_id=ai_model_id,
             service_id=service_id,
             device=resolved_device,
             generator=sentence_transformers.SentenceTransformer(model_name_or_path=ai_model_id, device=resolved_device),
         )
 
-    async def generate_embeddings(self, texts: List[str]) -> ndarray:
+    async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
             texts {List[str]} -- Texts to generate embeddings for.
 
         Returns:
             ndarray -- Embeddings for the texts.
         """
         try:
             logger.info(f"Generating embeddings for {len(texts)} texts")
-            embeddings = self.generator.encode(texts)
+            embeddings = self.generator.encode(texts, **kwargs)
             return array(embeddings)
         except Exception as e:
             raise ServiceResponseException("Hugging Face embeddings failed", e) from e
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
-from typing import Any, AsyncIterable, List, Optional
+from typing import Any, AsyncGenerator, List, Optional
 
 import aiohttp
 from pydantic import HttpUrl
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.ollama.ollama_prompt_execution_settings import OllamaChatPromptExecutionSettings
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
@@ -71,15 +71,15 @@
                 ]
 
     async def complete_chat_stream(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
-    ) -> AsyncIterable[List[StreamingChatMessageContent]]:
+    ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses.
 
         Arguments:
             chat_history {ChatHistory} -- A chat history that contains a list of chat messages,
                 that can be rendered into a set of messages, from system, user, assistant and function.
@@ -98,19 +98,19 @@
                 response.raise_for_status()
                 async for line in response.content:
                     body = json.loads(line)
                     if body.get("done") and body.get("message", {}).get("content") is None:
                         break
                     yield [
                         StreamingChatMessageContent(
+                            role="assistant",
                             choice_index=0,
                             inner_content=body,
                             ai_model_id=self.ai_model_id,
                             content=body.get("message", {"content": None}).get("content", None),
-                            role="assistant",
                         )
                     ]
                     if body.get("done"):
                         break
 
     async def complete(
         self,
@@ -143,15 +143,15 @@
                     )
                 ]
 
     async def complete_stream(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
-    ) -> AsyncIterable[List[StreamingTextContent]]:
+    ) -> AsyncGenerator[List[StreamingTextContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses.
 
         Arguments:
             prompt {str} -- A chat history that contains the prompt to complete.
             settings {OllamaChatPromptExecutionSettings} -- Request settings.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
-from typing import AsyncIterable, List, Optional
+from typing import Any, AsyncGenerator, List, Optional
 
 import aiohttp
 from pydantic import HttpUrl
 
-from semantic_kernel.connectors.ai.ollama.ollama_prompt_execution_settings import (
-    OllamaTextPromptExecutionSettings,
-)
+from semantic_kernel.connectors.ai.ollama.ollama_prompt_execution_settings import OllamaTextPromptExecutionSettings
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
-from semantic_kernel.connectors.ai.text_completion_client_base import (
-    TextCompletionClientBase,
-)
+from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OllamaTextCompletion(TextCompletionClientBase):
@@ -60,15 +56,15 @@
                 text = inner_content["response"]
                 return [TextContent(inner_content=inner_content, ai_model_id=self.ai_model_id, text=text)]
 
     async def complete_stream(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
-    ) -> AsyncIterable[List[StreamingTextContent]]:
+    ) -> AsyncGenerator[List[StreamingTextContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses,
         but the result will be a list anyway.
 
         Arguments:
             prompt {str} -- Prompt to complete.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List, Optional
+from typing import Any, List, Optional
 
 import aiohttp
 from numpy import array, ndarray
 from pydantic import HttpUrl
 
-from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
-    EmbeddingGeneratorBase,
-)
+from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OllamaTextEmbedding(EmbeddingGeneratorBase):
     """Ollama embeddings client.
@@ -25,15 +23,15 @@
         url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/embeddings
         session {Optional[aiohttp.ClientSession]} -- Optional client session to use for requests.
     """
 
     url: HttpUrl = "http://localhost:11434/api/embeddings"
     session: Optional[aiohttp.ClientSession] = None
 
-    async def generate_embeddings(self, texts: List[str], **kwargs) -> ndarray:
+    async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
             texts {List[str]} -- Texts to generate embeddings for.
 
         Returns:
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,7 +78,8 @@
     ai_model_id: Optional[str] = Field(None, serialization_alias="model")
     encoding_format: Optional[Literal["float", "base64"]] = None
     user: Optional[str] = None
     extra_headers: Optional[Dict] = None
     extra_query: Optional[Dict] = None
     extra_body: Optional[Dict] = None
     timeout: Optional[float] = None
+    dimensions: Optional[int] = Field(None, gt=0, le=3072)
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # Copyright (c) Microsoft. All rights reserved.
 import json
 import logging
+from copy import deepcopy
 from typing import Any, Dict, Mapping, Optional, Union, overload
+from uuid import uuid4
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION
-from semantic_kernel.connectors.ai.open_ai.contents import AzureChatMessageContent, AzureStreamingChatMessageContent
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.azure_chat_prompt_execution_settings import (
     AzureChatPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import AzureOpenAIConfigBase
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion_base import OpenAIChatCompletionBase
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIModelTypes
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import OpenAITextCompletionBase
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
-from semantic_kernel.contents.chat_role import ChatRole
+from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.finish_reason import FinishReason
+from semantic_kernel.contents.function_call_content import FunctionCallContent
+from semantic_kernel.contents.function_result_content import FunctionResultContent
+from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
+from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.kernel_pydantic import HttpsUrl
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class AzureChatCompletion(AzureOpenAIConfigBase, OpenAIChatCompletionBase, OpenAITextCompletionBase):
     """Azure Chat completion class."""
@@ -240,58 +245,77 @@
 
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return AzureChatPromptExecutionSettings
 
     def _create_chat_message_content(
         self, response: ChatCompletion, choice: Choice, response_metadata: Dict[str, Any]
-    ) -> AzureChatMessageContent:
+    ) -> ChatMessageContent:
         """Create a Azure chat message content object from a choice."""
-        metadata = self._get_metadata_from_chat_choice(choice)
-        metadata.update(response_metadata)
-        return AzureChatMessageContent(
-            inner_content=response,
-            ai_model_id=self.ai_model_id,
-            metadata=metadata,
-            role=ChatRole(choice.message.role) if choice.message.role is not None else None,
-            content=choice.message.content,
-            function_call=self._get_function_call_from_chat_choice(choice),
-            tool_calls=self._get_tool_calls_from_chat_choice(choice),
-            tool_message=self._get_tool_message_from_chat_choice(choice),
-        )
+        content = super()._create_chat_message_content(response, choice, response_metadata)
+        return self._add_tool_message_to_chat_message_content(content, choice)
 
     def _create_streaming_chat_message_content(
         self,
         chunk: ChatCompletionChunk,
         choice: ChunkChoice,
         chunk_metadata: Dict[str, Any],
-    ):
+    ) -> "StreamingChatMessageContent":
         """Create a Azure streaming chat message content object from a choice."""
-        metadata = self._get_metadata_from_chat_choice(choice)
-        metadata.update(chunk_metadata)
-        return AzureStreamingChatMessageContent(
-            choice_index=choice.index,
-            inner_content=chunk,
-            ai_model_id=self.ai_model_id,
-            metadata=metadata,
-            role=ChatRole(choice.delta.role) if choice.delta.role else ChatRole.ASSISTANT,
-            content=choice.delta.content,
-            finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason is not None else None,
-            function_call=self._get_function_call_from_chat_choice(choice),
-            tool_calls=self._get_tool_calls_from_chat_choice(choice),
-            tool_message=self._get_tool_message_from_chat_choice(choice),
-        )
+        content = super()._create_streaming_chat_message_content(chunk, choice, chunk_metadata)
+        return self._add_tool_message_to_chat_message_content(content, choice)
+
+    def _add_tool_message_to_chat_message_content(
+        self, content: ChatMessageContent | StreamingChatMessageContent, choice: Choice
+    ) -> "ChatMessageContent | StreamingChatMessageContent":
+        if tool_message := self._get_tool_message_from_chat_choice(choice=choice):
+            try:
+                tool_message_dict = json.loads(tool_message)
+            except json.JSONDecodeError:
+                logger.error("Failed to parse tool message JSON: %s", tool_message)
+                tool_message_dict = {"citations": tool_message}
+
+            function_call = FunctionCallContent(
+                id=str(uuid4()),
+                name="Azure-OnYourData",
+                arguments=json.dumps({"query": tool_message_dict.get("intent", [])}),
+            )
+            result = FunctionResultContent.from_function_call_content_and_result(
+                result=tool_message_dict["citations"], function_call_content=function_call
+            )
+            content.items.insert(0, function_call)
+            content.items.insert(1, result)
+        return content
 
     def _get_tool_message_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> Optional[str]:
         """Get the tool message from a choice."""
         if isinstance(choice, Choice):
             content = choice.message
         else:
             content = choice.delta
         if content.model_extra is not None and "context" in content.model_extra:
             return json.dumps(content.model_extra["context"])
 
         return None
 
-    def get_chat_message_content_type(self) -> str:
-        """Get the chat message content types used by a class, default is 'ChatMessageContent'."""
-        return "AzureChatMessageContent"
+    @staticmethod
+    def split_message(message: "ChatMessageContent") -> list["ChatMessageContent"]:
+        """Split a Azure On Your Data response into separate ChatMessageContents.
+
+        If the message does not have three contents, and those three are one each of:
+        FunctionCallContent, FunctionResultContent, and TextContent,
+        it will not return three messages, potentially only one or two.
+
+        The order of the returned messages is as expected by OpenAI.
+        """
+        if len(message.items) != 3:
+            return [message]
+        messages = {"tool_call": deepcopy(message), "tool_result": deepcopy(message), "assistant": deepcopy(message)}
+        for key, msg in messages.items():
+            if key == "tool_call":
+                msg.items = [item for item in msg.items if isinstance(item, FunctionCallContent)]
+                msg.finish_reason = FinishReason.FUNCTION_CALL
+            if key == "tool_result":
+                msg.items = [item for item in msg.items if isinstance(item, FunctionResultContent)]
+            if key == "assistant":
+                msg.items = [item for item in msg.items if isinstance(item, TextContent)]
+        return [messages["tool_call"], messages["tool_result"], messages["assistant"]]
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from copy import copy
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Optional, Tuple, Union
 
 from openai import AsyncStream
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.connectors.ai.open_ai.contents import OpenAIChatMessageContent, OpenAIStreamingChatMessageContent
-from semantic_kernel.connectors.ai.open_ai.contents.function_call import FunctionCall
-from semantic_kernel.connectors.ai.open_ai.contents.tool_calls import ToolCall
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
     OpenAIPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.open_ai.services.tool_call_behavior import ToolCallBehavior
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
-from semantic_kernel.contents.chat_role import ChatRole
 from semantic_kernel.contents.finish_reason import FinishReason
+from semantic_kernel.contents.function_call_content import FunctionCallContent
+from semantic_kernel.contents.function_result_content import FunctionResultContent
+from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
+from semantic_kernel.contents.streaming_text_content import StreamingTextContent
+from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import (
     FunctionCallInvalidArgumentsException,
     ServiceInvalidExecutionSettingsError,
     ServiceInvalidResponseError,
 )
 from semantic_kernel.utils.chat import store_results
 
@@ -45,69 +47,67 @@
     # most of the methods are overridden from the ChatCompletionClientBase class, otherwise it is mentioned
 
     # override from AIServiceClientBase
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return OpenAIChatPromptExecutionSettings
 
-    def get_chat_message_content_type(self) -> str:
-        """Get the chat message content types used by a class, default is 'ChatMessageContent'."""
-        return "OpenAIChatMessageContent"
-
     async def complete_chat(
         self,
         chat_history: ChatHistory,
         settings: OpenAIPromptExecutionSettings,
         **kwargs: Any,
-    ) -> List[OpenAIChatMessageContent]:
+    ) -> List["ChatMessageContent"]:
         """Executes a chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
         Returns:
-            List[OpenAIChatMessageContent | AzureChatMessageContent] -- The completion result(s).
+            List[ChatMessageContent] -- The completion result(s).
         """
         tool_call_behavior = self._get_tool_call_behavior(settings)
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
         if tool_call_behavior.auto_invoke_kernel_functions and (kernel is None or arguments is None):
             raise ServiceInvalidExecutionSettingsError(
                 "The kernel argument and arguments are required for OpenAI tool calling."
             )
 
         for _ in range(tool_call_behavior.max_auto_invoke_attempts):
             settings = self._prepare_settings(settings, chat_history, stream_request=False)
             completions = await self._send_chat_request(settings)
-            if self._should_return_completions_response(completions=completions, tool_call_behavior=tool_call_behavior):
+            if not tool_call_behavior.auto_invoke_kernel_functions or all(
+                not isinstance(item, FunctionCallContent) for completion in completions for item in completion.items
+            ):
                 return completions
             await self._process_chat_response_with_tool_call(
                 completions=completions, chat_history=chat_history, kernel=kernel, arguments=arguments
             )
 
     async def complete_chat_stream(
         self,
         chat_history: ChatHistory,
         settings: OpenAIPromptExecutionSettings,
         **kwargs: Any,
-    ) -> AsyncIterable[List[OpenAIStreamingChatMessageContent]]:
+    ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
         """Executes a streaming chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
         Yields:
-            List[OpenAIStreamingChatMessageContent | AzureStreamingChatMessageContent] -- A stream of
-                OpenAIStreamingChatMessages or AzureStreamingChatMessageContent when using Azure.
+            List[StreamingChatMessageContent] -- A stream of
+                StreamingChatMessageContent when using Azure.
         """
         tool_call_behavior = self._get_tool_call_behavior(settings)
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
         if tool_call_behavior.auto_invoke_kernel_functions and (kernel is None or arguments is None):
             raise ServiceInvalidExecutionSettingsError(
                 "The kernel argument and arguments are required for OpenAI tool calling."
@@ -120,19 +120,20 @@
             async for content, finish_reason in self._process_chat_stream_response(
                 response=response,
                 chat_history=chat_history,
                 kernel=kernel,
                 tool_call_behavior=tool_call_behavior,
                 arguments=arguments,
             ):
-                yield content
+                if content:
+                    yield content
             if finish_reason != FinishReason.TOOL_CALLS:
                 break
 
-    def _chat_message_content_to_dict(self, message: ChatMessageContent) -> Dict[str, Optional[str]]:
+    def _chat_message_content_to_dict(self, message: "ChatMessageContent") -> Dict[str, Optional[str]]:
         msg = super()._chat_message_content_to_dict(message)
         if message.role == "assistant":
             if tool_calls := getattr(message, "tool_calls", None):
                 msg["tool_calls"] = [tool_call.model_dump() for tool_call in tool_calls]
             if function_call := getattr(message, "function_call", None):
                 msg["function_call"] = function_call.model_dump_json()
         if message.role == "tool":
@@ -141,15 +142,15 @@
             if message.metadata and "function" in message.metadata:
                 msg["name"] = message.metadata["function_name"]
         return msg
 
     # endregion
     # region internal handlers
 
-    async def _send_chat_request(self, settings: OpenAIChatPromptExecutionSettings) -> List[OpenAIChatMessageContent]:
+    async def _send_chat_request(self, settings: OpenAIChatPromptExecutionSettings) -> List["ChatMessageContent"]:
         """Send the chat request"""
         response = await self._send_request(request_settings=settings)
         response_metadata = self._get_metadata_from_chat_response(response)
         completions = [
             self._create_chat_message_content(response, choice, response_metadata) for choice in response.choices
         ]
         return completions
@@ -159,15 +160,15 @@
         response = await self._send_request(request_settings=settings)
         if not isinstance(response, AsyncStream):
             raise ServiceInvalidResponseError("Expected an AsyncStream[ChatCompletionChunk] response.")
         return response
 
     async def _process_chat_response_with_tool_call(
         self,
-        completions: List[OpenAIChatMessageContent],
+        completions: List["ChatMessageContent"],
         chat_history: ChatHistory,
         kernel: "Kernel",
         arguments: "KernelArguments",
     ) -> None:
         """Process the completions in the chat response"""
         for result in completions:
             # An assistant message needs to be followed be a tool call response
@@ -177,79 +178,94 @@
     async def _process_chat_stream_response(
         self,
         response: AsyncStream,
         chat_history: ChatHistory,
         tool_call_behavior: ToolCallBehavior,
         kernel: Optional["Kernel"] = None,
         arguments: Optional["KernelArguments"] = None,
-    ) -> AsyncIterable[Tuple[List[OpenAIStreamingChatMessageContent], Optional[FinishReason]]]:
+    ) -> AsyncGenerator[Tuple[List["StreamingChatMessageContent"], Optional["FinishReason"]], Any]:
         """Process the chat stream response and handle tool calls if applicable."""
         full_content = None
         async for chunk in response:
             if len(chunk.choices) == 0:
                 continue
 
             chunk_metadata = self._get_metadata_from_streaming_chat_response(chunk)
             contents = [
                 self._create_streaming_chat_message_content(chunk, choice, chunk_metadata) for choice in chunk.choices
             ]
+            if not contents:
+                continue
             if not tool_call_behavior.auto_invoke_kernel_functions:
                 yield contents, None
                 continue
-            finish_reason = getattr(contents[0], "finish_reason", None)
+
             full_content = contents[0] if full_content is None else full_content + contents[0]
-            if not contents[0].tool_calls or finish_reason not in (FinishReason.STOP, FinishReason.TOOL_CALLS, None):
+            finish_reason = getattr(full_content, "finish_reason", None)
+            if not any(isinstance(item, FunctionCallContent) for item in full_content.items) or finish_reason not in (
+                FinishReason.STOP,
+                FinishReason.TOOL_CALLS,
+                None,
+            ):
                 yield contents, finish_reason
 
             if finish_reason == FinishReason.STOP:
                 tool_call_behavior.auto_invoke_kernel_functions = False
                 break
             if finish_reason == FinishReason.TOOL_CALLS:
                 chat_history.add_message(message=full_content)
                 await self._process_tool_calls(full_content, kernel, chat_history, arguments)
-                break
+                yield None, finish_reason
 
     # endregion
     # region content creation
 
     def _create_chat_message_content(
         self, response: ChatCompletion, choice: Choice, response_metadata: Dict[str, Any]
-    ) -> OpenAIChatMessageContent:
+    ) -> "ChatMessageContent":
         """Create a chat message content object from a choice."""
         metadata = self._get_metadata_from_chat_choice(choice)
         metadata.update(response_metadata)
-        return OpenAIChatMessageContent(
+
+        items: list[Any] = self._get_tool_calls_from_chat_choice(choice)
+        items.extend(self._get_function_call_from_chat_choice(choice))
+        if choice.message.content:
+            items.append(TextContent(text=choice.message.content))
+
+        return ChatMessageContent(
             inner_content=response,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
-            role=ChatRole(choice.message.role),
-            content=choice.message.content,
-            function_call=self._get_function_call_from_chat_choice(choice),
-            tool_calls=self._get_tool_calls_from_chat_choice(choice),
+            role=AuthorRole(choice.message.role),
+            items=items,
+            finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason else None,
         )
 
     def _create_streaming_chat_message_content(
         self,
         chunk: ChatCompletionChunk,
         choice: ChunkChoice,
         chunk_metadata: Dict[str, Any],
-    ):
+    ) -> StreamingChatMessageContent | None:
         """Create a streaming chat message content object from a choice."""
         metadata = self._get_metadata_from_chat_choice(choice)
         metadata.update(chunk_metadata)
-        return OpenAIStreamingChatMessageContent(
+
+        items: list[Any] = self._get_tool_calls_from_chat_choice(choice)
+        items.extend(self._get_function_call_from_chat_choice(choice))
+        if choice.delta.content is not None:
+            items.append(StreamingTextContent(choice_index=choice.index, text=choice.delta.content))
+        return StreamingChatMessageContent(
             choice_index=choice.index,
             inner_content=chunk,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
-            role=ChatRole(choice.delta.role) if choice.delta.role else ChatRole.ASSISTANT,
-            content=choice.delta.content,
+            role=AuthorRole(choice.delta.role) if choice.delta.role else AuthorRole.ASSISTANT,
             finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason else None,
-            function_call=self._get_function_call_from_chat_choice(choice),
-            tool_calls=self._get_tool_calls_from_chat_choice(choice),
+            items=items,
         )
 
     def _get_metadata_from_chat_response(self, response: ChatCompletion) -> Dict[str, Any]:
         """Get metadata from a chat response."""
         return {
             "id": response.id,
             "created": response.created,
@@ -267,40 +283,45 @@
 
     def _get_metadata_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> Dict[str, Any]:
         """Get metadata from a chat choice."""
         return {
             "logprobs": getattr(choice, "logprobs", None),
         }
 
-    def _get_tool_calls_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> Optional[List[ToolCall]]:
+    def _get_tool_calls_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> List[FunctionCallContent]:
         """Get tool calls from a chat choice."""
         if isinstance(choice, Choice):
             content = choice.message
         else:
             content = choice.delta
         if content.tool_calls is None:
-            return None
+            return []
         return [
-            ToolCall(
+            FunctionCallContent(
                 id=tool.id,
-                type=tool.type,
-                function=FunctionCall(name=tool.function.name, arguments=tool.function.arguments),
+                index=getattr(tool, "index", None),
+                name=tool.function.name,
+                arguments=tool.function.arguments,
             )
             for tool in content.tool_calls
         ]
 
-    def _get_function_call_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> Optional[FunctionCall]:
+    def _get_function_call_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> List[FunctionCallContent]:
         """Get a function call from a chat choice."""
         if isinstance(choice, Choice):
             content = choice.message
         else:
             content = choice.delta
         if content.function_call is None:
-            return None
-        return FunctionCall(name=content.function_call.name, arguments=content.function_call.arguments)
+            return []
+        return [
+            FunctionCallContent(
+                id="legacy_function_call", name=content.function_call.name, arguments=content.function_call.arguments
+            )
+        ]
 
     def _get_tool_call_behavior(self, execution_settings: OpenAIPromptExecutionSettings) -> ToolCallBehavior:
         """Gets the auto invoke and max iterations settings through ToolCallBehavior."""
         auto_invoke_kernel_functions = False
         max_auto_invoke_attempts = 1
         if isinstance(execution_settings, OpenAIChatPromptExecutionSettings):
             if execution_settings.auto_invoke_kernel_functions is not None:
@@ -342,63 +363,47 @@
         return settings
 
     # endregion
     # region tool calling
 
     async def _process_tool_calls(
         self,
-        result: Union[OpenAIChatMessageContent, OpenAIStreamingChatMessageContent],
+        result: ChatMessageContent,
         kernel: "Kernel",
         chat_history: ChatHistory,
         arguments: "KernelArguments",
     ) -> None:
         """Processes the tool calls in the result and return it as part of the chat history."""
-        logger.info(f"processing {len(result.tool_calls)} tool calls")
+        logger.info(f"processing {len(result.items)} tool calls")
         args_cloned = copy(arguments)
-        for tool_call in result.tool_calls:
-            if tool_call.function is None:
+        for function_call in result.items:
+            if not isinstance(function_call, FunctionCallContent):
                 continue
             try:
-                func_args = tool_call.function.parse_arguments()
-                args_cloned.update(func_args)
+                func_args = function_call.parse_arguments()
+                if func_args:
+                    args_cloned.update(func_args)
             except FunctionCallInvalidArgumentsException as exc:
                 logger.exception(
-                    f"Received invalid arguments for function {tool_call.function.name}: {exc}. Trying tool call again."
+                    f"Received invalid arguments for function {function_call.name}: {exc}. Trying tool call again."
                 )
-                msg = OpenAIChatMessageContent(
-                    role=ChatRole.TOOL,
-                    content="The tool call arguments are malformed, please try again.",
-                    tool_call_id=tool_call.id,
-                    metadata={"function_name": tool_call.function.name},
+                frc = FunctionResultContent.from_function_call_content_and_result(
+                    function_call_content=function_call,
+                    result="The tool call arguments are malformed, please try again.",
                 )
-                chat_history.add_message(message=msg)
+                chat_history.add_message(message=frc.to_chat_message_content())
                 continue
-            logger.info(f"Calling {tool_call.function.name} function with args: {tool_call.function.arguments}")
+            logger.info(f"Calling {function_call.name} function with args: {function_call.arguments}")
             try:
-                func_result = await kernel.invoke(**tool_call.function.split_name_dict(), arguments=args_cloned)
+                func_result = await kernel.invoke(**function_call.split_name_dict(), arguments=args_cloned)
             except Exception as exc:
-                logger.exception(f"Error occurred while invoking function {tool_call.function.name}")
+                logger.exception(f"Error occurred while invoking function {function_call.name}")
                 raise ServiceInvalidResponseError(
-                    f"Error occurred while invoking function {tool_call.function.name}"
+                    f"Error occurred while invoking function {function_call.name}"
                 ) from exc
-            msg = OpenAIChatMessageContent(
-                role=ChatRole.TOOL,
-                content=str(func_result),
-                tool_call_id=tool_call.id,
-                metadata={"function_name": tool_call.function.name, "function_arguments": func_result.metadata},
+            frc = FunctionResultContent.from_function_call_content_and_result(
+                function_call_content=function_call, result=func_result
             )
-            chat_history.add_message(message=msg)
-
-    def _should_return_completions_response(
-        self,
-        completions: Union[List[OpenAIChatMessageContent], List[OpenAIStreamingChatMessageContent]],
-        tool_call_behavior: ToolCallBehavior,
-    ) -> bool:
-        """Determines if the completions should be returned."""
-        return (
-            not tool_call_behavior.auto_invoke_kernel_functions
-            or any(not isinstance(completion, OpenAIChatMessageContent) for completion in completions)
-            or any(not hasattr(completion, "tool_calls") or not completion.tool_calls for completion in completions)
-        )
+            chat_history.add_message(message=frc.to_chat_message_content())
 
 
 # endregion
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Union
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Union
 
 from openai import AsyncStream
 from openai.types import Completion, CompletionChoice
 from openai.types.chat.chat_completion import Choice as ChatCompletionChoice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
@@ -72,15 +72,15 @@
             metadata=choice_metadata,
         )
 
     async def complete_stream(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
-    ) -> AsyncIterable[List["StreamingTextContent"]]:
+    ) -> AsyncGenerator[List["StreamingTextContent"], Any]:
         """
         Executes a completion request and streams the result.
         Supports both chat completion and text completion.
 
         Arguments:
             prompt {str} -- The prompt to use for the completion request.
             settings {OpenAITextPromptExecutionSettings} -- The settings to use for the completion request.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/open_ai/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import Any, Dict, Optional
+# Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
+
+from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class PromptExecutionSettings(KernelBaseModel):
@@ -17,51 +20,56 @@
         service_id (str): The service ID to use for the request.
         extension_data (Dict[str, Any], optional): Any additional data to send with the request. Defaults to None.
         kwargs (Any): Additional keyword arguments,
             these are attempted to parse into the keys of the specific prompt execution settings.
     Methods:
         prepare_settings_dict: Prepares the settings as a dictionary for sending to the AI service.
         update_from_prompt_execution_settings: Update the keys from another prompt execution settings object.
-        from_prompt_execution_settings: Create a prompt execution settings from another prompt execution settings object.
-    """  # noqa: E501
+        from_prompt_execution_settings: Create a prompt execution settings from another prompt execution settings.
+    """
 
-    service_id: Optional[str] = Field(None, min_length=1)
-    extension_data: Dict[str, Any] = Field(default_factory=dict)
+    service_id: str | None = Field(None, min_length=1)
+    extension_data: dict[str, Any] = Field(default_factory=dict)
 
-    def __init__(self, service_id: Optional[str] = None, **kwargs: Any):
+    def __init__(self, service_id: str | None = None, **kwargs: Any):
         extension_data = kwargs.pop("extension_data", {})
         extension_data.update(kwargs)
         super().__init__(service_id=service_id, extension_data=extension_data)
         self.unpack_extension_data()
 
     @property
     def keys(self):
         """Get the keys of the prompt execution settings."""
         return self.model_fields.keys()
 
-    def prepare_settings_dict(self, **kwargs) -> Dict[str, Any]:
+    def prepare_settings_dict(self, **kwargs) -> dict[str, Any]:
+        """Prepare the settings as a dictionary for sending to the AI service.
+
+        By default, this method excludes the service_id and extension_data fields.
+        As well as any fields that are None.
+        """
         return self.model_dump(
             exclude={
                 "service_id",
                 "extension_data",
             },
             exclude_none=True,
             by_alias=True,
         )
 
-    def update_from_prompt_execution_settings(self, config: "PromptExecutionSettings") -> None:
+    def update_from_prompt_execution_settings(self, config: PromptExecutionSettings) -> None:
         """Update the prompt execution settings from a completion config."""
         if config.service_id is not None:
             self.service_id = config.service_id
         config.pack_extension_data()
         self.extension_data.update(config.extension_data)
         self.unpack_extension_data()
 
     @classmethod
-    def from_prompt_execution_settings(cls, config: "PromptExecutionSettings") -> "PromptExecutionSettings":
+    def from_prompt_execution_settings(cls, config: PromptExecutionSettings) -> PromptExecutionSettings:
         """Create a prompt execution settings from a completion config."""
         config.pack_extension_data()
         return cls(
             service_id=config.service_id,
             extension_data=config.extension_data,
         )
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
-
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, AsyncIterable, List
+from typing import TYPE_CHECKING, Any, AsyncGenerator
 
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
     from semantic_kernel.contents import StreamingTextContent, TextContent
 
@@ -15,35 +15,36 @@
     """Base class for text completion AI services."""
 
     @abstractmethod
     async def complete(
         self,
         prompt: str,
         settings: "PromptExecutionSettings",
-    ) -> List["TextContent"]:
+    ) -> list["TextContent"]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
         Arguments:
             prompt {str} -- The prompt to send to the LLM.
             settings {PromptExecutionSettings} -- Settings for the request.
 
             Returns:
-                Union[str, List[str]] -- A string or list of strings representing the response(s) from the LLM.
+            list[TextContent] -- A string or list of strings representing the response(s) from the LLM.
         """
 
     @abstractmethod
-    async def complete_stream(
+    def complete_stream(
         self,
         prompt: str,
         settings: "PromptExecutionSettings",
-    ) -> AsyncIterable[List["StreamingTextContent"]]:
+    ) -> AsyncGenerator[list["StreamingTextContent"], Any]:
         """
         This is the method that is called from the kernel to get a stream response from a text-optimized LLM.
 
         Arguments:
             prompt {str} -- The prompt to send to the LLM.
             settings {PromptExecutionSettings} -- Settings for the request.
 
         Yields:
-            A stream representing the response(s) from the LLM.
+            list[StreamingTextContent] -- A stream representing the response(s) from the LLM.
         """
+        ...
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import json
 from typing import Dict, List, Optional
 
 import aiohttp
 
 from semantic_kernel.connectors.memory.astradb.utils import AsyncSession
+from semantic_kernel.connectors.telemetry import APP_INFO
 from semantic_kernel.exceptions import ServiceResponseException
 
+ASTRA_CALLER_IDENTITY: str
+SEMANTIC_KERNEL_VERSION = APP_INFO.get("Semantic-Kernel-Version")
+if SEMANTIC_KERNEL_VERSION:
+    ASTRA_CALLER_IDENTITY = f"semantic-kernel/{SEMANTIC_KERNEL_VERSION}"
+else:
+    ASTRA_CALLER_IDENTITY = "semantic-kernel"
+
 
 class AstraClient:
     def __init__(
         self,
         astra_id: str,
         astra_region: str,
         astra_application_token: str,
@@ -27,14 +35,15 @@
 
         self.request_base_url = (
             f"https://{self.astra_id}-{self.astra_region}.apps.astra.datastax.com/api/json/v1/{self.keyspace_name}"
         )
         self.request_header = {
             "x-cassandra-token": self.astra_application_token,
             "Content-Type": "application/json",
+            "User-Agent": ASTRA_CALLER_IDENTITY,
         }
         self._session = session
 
     async def _run_query(self, request_url: str, query: Dict):
         async with AsyncSession(self._session) as session:
             async with session.post(request_url, data=json.dumps(query), headers=self.request_header) as response:
                 if response.status == 200:
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
-
 from typing import List, Tuple
 
 from numpy import ndarray
 
 from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmos_db_store_api import AzureCosmosDBStoreApi
-from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import get_mongodb_search_client
+from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import (
+    CosmosDBSimilarityType,
+    CosmosDBVectorSearchType,
+    get_mongodb_search_client,
+)
 from semantic_kernel.connectors.memory.azure_cosmosdb.mongo_vcore_store_api import MongoStoreApi
 from semantic_kernel.exceptions import ServiceInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
 
 class AzureCosmosDBMemoryStore(MemoryStoreBase):
@@ -22,73 +25,98 @@
     mongodb_client = None
     database = None
     index_name = None
     vector_dimensions = None
     num_lists = None
     similarity = None
     collection_name = None
+    kind = None
+    m = None
+    ef_construction = None
+    ef_search = None
 
     def __init__(
         self,
         cosmosStore: AzureCosmosDBStoreApi,
         database_name: str,
         index_name: str,
         vector_dimensions: int,
-        num_lists: int,
-        similarity: str,
+        num_lists: int = 100,
+        similarity: CosmosDBSimilarityType = CosmosDBSimilarityType.COS,
+        kind: CosmosDBVectorSearchType = CosmosDBVectorSearchType.VECTOR_HNSW,
+        m: int = 16,
+        ef_construction: int = 64,
+        ef_search: int = 40,
     ):
         if vector_dimensions <= 0:
             raise ServiceInitializationError("Vector dimensions must be a positive number.")
         # if connection_string is None:
         #     raise ValueError("Connection String cannot be empty.")
         if database_name is None:
             raise ServiceInitializationError("Database Name cannot be empty.")
         if index_name is None:
             raise ServiceInitializationError("Index Name cannot be empty.")
 
         self.cosmosStore = cosmosStore
         self.index_name = index_name
         self.num_lists = num_lists
         self.similarity = similarity
+        self.kind = kind
+        self.m = m
+        self.ef_construction = ef_construction
+        self.ef_search = ef_search
 
     @staticmethod
     async def create(
         cosmos_connstr,
+        application_name,
         cosmos_api,
         database_name,
         collection_name,
         index_name,
         vector_dimensions,
         num_lists,
         similarity,
+        kind,
+        m,
+        ef_construction,
+        ef_search,
     ) -> MemoryStoreBase:
         """Creates the underlying data store based on the API definition"""
         # Right now this only supports Mongo, but set up to support more later.
         apiStore: AzureCosmosDBStoreApi = None
         if cosmos_api == "mongo-vcore":
-            mongodb_client = get_mongodb_search_client(cosmos_connstr)
+            mongodb_client = get_mongodb_search_client(cosmos_connstr, application_name)
             database = mongodb_client[database_name]
             apiStore = MongoStoreApi(
-                collection_name,
-                index_name,
-                vector_dimensions,
-                num_lists,
-                similarity,
-                database,
+                collection_name=collection_name,
+                index_name=index_name,
+                vector_dimensions=vector_dimensions,
+                num_lists=num_lists,
+                similarity=similarity,
+                database=database,
+                kind=kind,
+                m=m,
+                ef_construction=ef_construction,
+                ef_search=ef_search,
             )
         else:
             raise NotImplementedError(f"API type {cosmos_api} is not supported.")
 
         store = AzureCosmosDBMemoryStore(
             apiStore,
             database_name,
             index_name,
             vector_dimensions,
             num_lists,
             similarity,
+            kind,
+            m,
+            ef_construction,
+            ef_search,
         )
         await store.create_collection(collection_name)
         return store
 
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection in the data store.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,17 @@
     openapi_runner = OpenApiRunner(parsed_openapi_document=parsed_doc, auth_callback=auth_callback)
 
     return [
         _create_function_from_operation(openapi_runner, operation, plugin_name) for operation in operations.values()
     ]
 
 
-def _create_function_from_operation(runner: OpenApiRunner, operation: RestApiOperation, plugin_name: str | None = None):
+def _create_function_from_operation(
+    runner: OpenApiRunner, operation: RestApiOperation, plugin_name: str | None = None
+) -> KernelFunctionFromMethod:
     logger.info(f"Registering OpenAPI operation: {plugin_name}.{operation.id}")
 
     @kernel_function(
         description=operation.summary if operation.summary else operation.description,
         name=operation.id,
     )
     async def run_openapi_operation(
@@ -356,8 +358,8 @@
             headers=json.loads(headers) if isinstance(headers, str) else headers if headers else None,
             request_body=(
                 json.loads(request_body) if isinstance(request_body, str) else request_body if request_body else None
             ),
         )
         return response
 
-    return KernelFunctionFromMethod(run_openapi_operation, plugin_name=plugin_name)
+    return KernelFunctionFromMethod(method=run_openapi_operation, plugin_name=plugin_name)
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-0.9.7b1/semantic_kernel/connectors/utils/document_loader.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
-from typing import Any, Iterator, List
+from functools import singledispatchmethod
+from typing import Any, Generator
 from xml.etree.ElementTree import Element, tostring
 
 from defusedxml.ElementTree import XML, ParseError
 from pydantic import field_validator
 
+from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
-from semantic_kernel.contents.chat_message_content_base import ChatMessageContentBase
-from semantic_kernel.contents.chat_role import ChatRole
-from semantic_kernel.contents.const import (
-    CHAT_MESSAGE_CONTENT,
-    ROOT_KEY_HISTORY,
-    ROOT_KEY_MESSAGE,
-    TYPES_CHAT_MESSAGE_CONTENT,
-)
+from semantic_kernel.contents.const import CHAT_HISTORY_TAG, CHAT_MESSAGE_CONTENT_TAG
+from semantic_kernel.contents.kernel_content import KernelContent
 from semantic_kernel.exceptions import ContentInitializationError, ContentSerializationError
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 logger = logging.getLogger(__name__)
 
 
 class ChatHistory(KernelBaseModel):
@@ -32,15 +28,14 @@
     as a keyword argument, but not be part of the class definition.
 
     Attributes:
         messages (List[ChatMessageContent]): The list of chat messages in the history.
     """
 
     messages: list[ChatMessageContent]
-    message_type: TYPES_CHAT_MESSAGE_CONTENT = CHAT_MESSAGE_CONTENT
 
     def __init__(self, **data: Any):
         """
         Initializes a new instance of the ChatHistory class, optionally incorporating a message and/or
         a system message at the beginning of the chat history.
 
         This constructor allows for flexible initialization with chat messages and an optional messages or a
@@ -57,99 +52,131 @@
                 included at the start of the chat history.
 
         Note: The 'system_message' is not retained as part of the class's attributes; it's used during
         initialization and then discarded. The rest of the keyword arguments are passed to the superclass
         constructor and handled according to the Pydantic model's behavior.
         """
         system_message_content = data.pop("system_message", None)
-        message_type = data.get("message_type", CHAT_MESSAGE_CONTENT)
 
         if system_message_content:
-            system_message = ChatMessageContentBase.from_fields(
-                role=ChatRole.SYSTEM, content=system_message_content, type=message_type
-            )
+            system_message = ChatMessageContent(role=AuthorRole.SYSTEM, content=system_message_content)
 
             if "messages" in data:
                 data["messages"] = [system_message] + data["messages"]
             else:
                 data["messages"] = [system_message]
         if "messages" not in data:
             data["messages"] = []
         super().__init__(**data)
 
     @field_validator("messages", mode="before")
     @classmethod
-    def _validate_messages(cls, messages: List[ChatMessageContent]) -> List[ChatMessageContent]:
+    def _validate_messages(cls, messages: list[ChatMessageContent]) -> list[ChatMessageContent]:
         if not messages:
             return messages
-        out_msgs: List[ChatMessageContent] = []
+        out_msgs: list[ChatMessageContent] = []
         for message in messages:
             if isinstance(message, dict):
-                out_msgs.append(ChatMessageContentBase.from_dict(message))
+                out_msgs.append(ChatMessageContent.model_validate(message))
             else:
                 out_msgs.append(message)
         return out_msgs
 
-    def add_system_message(self, content: str, **kwargs: Any) -> None:
+    @singledispatchmethod
+    def add_system_message(self, content: str | list[KernelContent], **kwargs) -> None:
         """Add a system message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.SYSTEM, content, **kwargs))
+        raise NotImplementedError
 
-    def add_user_message(self, content: str, **kwargs: Any) -> None:
+    @add_system_message.register
+    def add_system_message_str(self, content: str, **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.SYSTEM, content=content, **kwargs))
+
+    @add_system_message.register(list)
+    def add_system_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.SYSTEM, items=content, **kwargs))
+
+    @singledispatchmethod
+    def add_user_message(self, content: str | list[KernelContent], **kwargs: Any) -> None:
         """Add a user message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.USER, content, **kwargs))
+        raise NotImplementedError
+
+    @add_user_message.register
+    def add_user_message_str(self, content: str, **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.USER, content=content, **kwargs))
+
+    @add_user_message.register(list)
+    def add_user_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.USER, items=content, **kwargs))
 
-    def add_assistant_message(self, content: str, **kwargs: Any) -> None:
+    @singledispatchmethod
+    def add_assistant_message(self, content: str | list[KernelContent], **kwargs: Any) -> None:
         """Add an assistant message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.ASSISTANT, content, **kwargs))
+        raise NotImplementedError
 
-    def add_tool_message(
-        self, content: str | None = None, metadata: dict[str, Any] | None = None, **kwargs: Any
-    ) -> None:
+    @add_assistant_message.register
+    def add_assistant_message_str(self, content: str, **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.ASSISTANT, content=content, **kwargs))
+
+    @add_assistant_message.register(list)
+    def add_assistant_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.ASSISTANT, items=content, **kwargs))
+
+    @singledispatchmethod
+    def add_tool_message(self, content: str | list[KernelContent], **kwargs: Any) -> None:
         """Add a tool message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.TOOL, content, **kwargs), metadata=metadata)
+        raise NotImplementedError
+
+    @add_tool_message.register
+    def add_tool_message_str(self, content: str, **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.TOOL, content=content, **kwargs))
+
+    @add_tool_message.register(list)
+    def add_tool_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        self.add_message(message=self._prepare_for_add(role=AuthorRole.TOOL, items=content, **kwargs))
 
     def add_message(
         self,
-        message: "ChatMessageContent" | dict[str, Any],
+        message: ChatMessageContent | dict[str, Any],
         encoding: str | None = None,
         metadata: dict[str, Any] | None = None,
     ) -> None:
         """Add a message to the history.
 
         This method accepts either a ChatMessageContent instance or a
         dictionary with the necessary information to construct a ChatMessageContent instance.
 
         Args:
             message (Union[ChatMessageContent, dict]): The message to add, either as
                 a pre-constructed ChatMessageContent instance or a dictionary specifying 'role' and 'content'.
             encoding (Optional[str]): The encoding of the message. Required if 'message' is a dict.
             metadata (Optional[dict[str, Any]]): Any metadata to attach to the message. Required if 'message' is a dict.
         """
-        from semantic_kernel.contents.chat_message_content import ChatMessageContent
-
         if isinstance(message, ChatMessageContent):
             self.messages.append(message)
             return
         if "role" not in message:
             raise ContentInitializationError(f"Dictionary must contain at least the role. Got: {message}")
         if encoding:
             message["encoding"] = encoding
         if metadata:
             message["metadata"] = metadata
-        if "type" not in message:
-            message["type"] = self.message_type
-        self.messages.append(ChatMessageContentBase.from_dict(message))
+        self.messages.append(ChatMessageContent(**message))
 
-    def _prepare_for_add(self, role: ChatRole, content: str | None = None, **kwargs: Any) -> dict[str, str]:
+    def _prepare_for_add(
+        self, role: AuthorRole, content: str | None = None, items: list[KernelContent] | None = None, **kwargs: Any
+    ) -> dict[str, str]:
         """Prepare a message to be added to the history."""
         kwargs["role"] = role
-        kwargs["content"] = content
+        if content:
+            kwargs["content"] = content
+        if items:
+            kwargs["items"] = items
         return kwargs
 
-    def remove_message(self, message: "ChatMessageContent") -> bool:
+    def remove_message(self, message: ChatMessageContent) -> bool:
         """Remove a message from the history.
 
         Args:
             message (ChatMessageContent): The message to remove.
 
         Returns:
             bool: True if the message was removed, False if the message was not found.
@@ -160,111 +187,104 @@
         except ValueError:
             return False
 
     def __len__(self) -> int:
         """Return the number of messages in the history."""
         return len(self.messages)
 
-    def __getitem__(self, index: int) -> "ChatMessageContent":
+    def __getitem__(self, index: int) -> ChatMessageContent:
         """Get a message from the history using the [] operator.
 
         Args:
             index (int): The index of the message to get.
 
         Returns:
             ChatMessageContent: The message at the specified index.
         """
         return self.messages[index]
 
-    def __contains__(self, item: "ChatMessageContent") -> bool:
+    def __contains__(self, item: ChatMessageContent) -> bool:
         """Check if a message is in the history.
 
         Args:
             item (ChatMessageContent): The message to check for.
 
         Returns:
             bool: True if the message is in the history, False otherwise.
         """
         return item in self.messages
 
     def __str__(self) -> str:
         """Return a string representation of the history."""
-        chat_history_xml = Element(ROOT_KEY_HISTORY)
+        chat_history_xml = Element(CHAT_HISTORY_TAG)
         for message in self.messages:
-            chat_history_xml.append(message.to_element(root_key=ROOT_KEY_MESSAGE))
+            chat_history_xml.append(message.to_element())
         return tostring(chat_history_xml, encoding="unicode", short_empty_elements=True)
 
-    def __iter__(self) -> Iterator["ChatMessageContent"]:
+    def __iter__(self) -> Generator[ChatMessageContent, None, None]:  # type: ignore
         """Return an iterator over the messages in the history."""
-        return iter(self.messages)
+        yield from self.messages
 
     def __eq__(self, other: Any) -> bool:
         """Check if two ChatHistory instances are equal."""
         if not isinstance(other, ChatHistory):
             return False
 
         return self.messages == other.messages
 
     @classmethod
-    def from_rendered_prompt(cls, rendered_prompt: str, message_type: str = CHAT_MESSAGE_CONTENT) -> "ChatHistory":
+    def from_rendered_prompt(cls, rendered_prompt: str) -> "ChatHistory":
         """
         Create a ChatHistory instance from a rendered prompt.
 
         Args:
             rendered_prompt (str): The rendered prompt to convert to a ChatHistory instance.
 
         Returns:
             ChatHistory: The ChatHistory instance created from the rendered prompt.
         """
-        messages: List[ChatMessageContent] = []
+        prompt_tag = "prompt"
+        messages: list["ChatMessageContent"] = []
         prompt = rendered_prompt.strip()
         try:
-            xml_prompt = XML(text=f"<prompt>{prompt}</prompt>")
+            xml_prompt = XML(text=f"<{prompt_tag}>{prompt}</{prompt_tag}>")
         except ParseError:
             logger.info(f"Could not parse prompt {prompt} as xml, treating as text")
-            return cls(
-                messages=[ChatMessageContentBase.from_fields(role=ChatRole.USER, content=prompt, type=message_type)]
-            )
+            return cls(messages=[ChatMessageContent(role=AuthorRole.USER, content=prompt)])
         if xml_prompt.text and xml_prompt.text.strip():
-            messages.append(
-                ChatMessageContentBase.from_fields(
-                    role=ChatRole.SYSTEM, content=xml_prompt.text.strip(), type=message_type
-                )
-            )
+            messages.append(ChatMessageContent(role=AuthorRole.SYSTEM, content=xml_prompt.text.strip()))
         for item in xml_prompt:
-            if item.tag == ROOT_KEY_MESSAGE:
-                messages.append(ChatMessageContentBase.from_element(item))
-            elif item.tag == ROOT_KEY_HISTORY:
+            if item.tag == CHAT_MESSAGE_CONTENT_TAG:
+                messages.append(ChatMessageContent.from_element(item))
+            elif item.tag == CHAT_HISTORY_TAG:
                 for message in item:
-                    messages.append(ChatMessageContentBase.from_element(message))
+                    messages.append(ChatMessageContent.from_element(message))
             if item.tail and item.tail.strip():
-                messages.append(
-                    ChatMessageContentBase.from_fields(role=ChatRole.USER, content=item.tail.strip(), type=message_type)
-                )
-        if len(messages) == 1 and messages[0].role == ChatRole.SYSTEM:
-            messages[0].role = ChatRole.USER
-        return cls(messages=messages, message_type=message_type)
+                messages.append(ChatMessageContent(role=AuthorRole.USER, content=item.tail.strip()))
+        if len(messages) == 1 and messages[0].role == AuthorRole.SYSTEM:
+            messages[0].role = AuthorRole.USER
+        return cls(messages=messages)
 
     def serialize(self) -> str:
         """
         Serializes the ChatHistory instance to a JSON string.
 
         Returns:
             str: A JSON string representation of the ChatHistory instance.
 
         Raises:
             ValueError: If the ChatHistory instance cannot be serialized to JSON.
         """
         try:
-            return self.model_dump_json(indent=4, exclude_none=True)
-        except Exception as e:
+            return self.model_dump_json(indent=2, exclude_none=True)
+        except Exception as e:  # pragma: no cover
             raise ContentSerializationError(f"Unable to serialize ChatHistory to JSON: {e}") from e
 
     @classmethod
-    def restore_chat_history(cls, chat_history_json: str) -> "ChatHistory":
+    def restore_chat_history(cls, chat_history_json: str) -> ChatHistory:
         """
         Restores a ChatHistory instance from a JSON string.
 
         Args:
             chat_history_json (str): The JSON string to deserialize
                 into a ChatHistory instance.
 
@@ -288,20 +308,20 @@
             file_path (str): The path to the file where the serialized data will be stored.
         """
         json_str = self.serialize()
         with open(file_path, "w") as file:
             file.write(json_str)
 
     @classmethod
-    def load_chat_history_from_file(cls, file_path: str) -> "ChatHistory":
+    def load_chat_history_from_file(cls, file_path: str) -> ChatHistory:
         """
         Loads the ChatHistory from a file.
 
         Args:
             file_path (str): The path to the file from which to load the ChatHistory.
 
         Returns:
             ChatHistory: The deserialized ChatHistory instance.
         """
-        with open(file_path, "r") as file:
+        with open(file_path) as file:
             json_str = file.read()
         return cls.restore_chat_history(json_str)
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-0.9.7b1/semantic_kernel/contents/kernel_content.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional
+from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class KernelContent(KernelBaseModel, ABC):
     """Base class for all kernel contents."""
 
-    inner_content: Optional[Any] = None
-    ai_model_id: Optional[str] = None
-    metadata: Optional[Dict[str, Any]] = Field(default_factory=dict)
+    inner_content: Any | None = None
+    ai_model_id: str | None = None
+    metadata: dict[str, Any] = Field(default_factory=dict)
 
     @abstractmethod
     def __str__(self) -> str:
         pass
+
+    @abstractmethod
+    def to_element(self) -> Any:
+        pass
+
+    @classmethod
+    @abstractmethod
+    def from_element(cls, element: Any) -> "KernelContent":
+        pass
+
+    @abstractmethod
+    def to_dict(self) -> dict[str, Any]:
+        pass
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_text_content.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
-from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
+from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import ContentAdditionException
 
 
-class StreamingChatMessageContent(StreamingContentMixin, ChatMessageContent):
-    """This is the base class for streaming chat message response content.
+class StreamingTextContent(StreamingContentMixin, TextContent):
+    """This is the base class for streaming text response content.
 
-    All Chat Completion Services should return a instance of this class as streaming response,
-    where each part of the response as it is streamed is converted to a instance of this class,
-    the end-user will have to either do something directly or gather them and combine them into a
-    new instance. A service can implement their own subclass of this class and return instances of that.
+    All Text Completion Services should return a instance of this class as streaming response.
+    Or they can implement their own subclass of this class and return an instance.
 
     Args:
         choice_index: int - The index of the choice that generated this response.
         inner_content: Optional[Any] - The inner content of the response,
             this should hold all the information from the response so even
             when not creating a subclass a developer can leverage the full thing.
         ai_model_id: Optional[str] - The id of the AI model that generated this response.
         metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-        role: Optional[ChatRole] - The role of the chat message, defaults to ASSISTANT.
-        content: Optional[str] - The text of the response.
+        text: Optional[str] - The text of the response.
         encoding: Optional[str] - The encoding of the text.
 
     Methods:
-        __str__: Returns the content of the response.
+        __str__: Returns the text of the response.
         __bytes__: Returns the content of the response encoded in the encoding.
-        __add__: Combines two StreamingChatMessageContent instances.
+        __add__: Combines two StreamingTextContent instances.
     """
 
     def __bytes__(self) -> bytes:
-        return self.content.encode(self.encoding if self.encoding else "utf-8") if self.content else b""
+        return self.text.encode(self.encoding if self.encoding else "utf-8") if self.text else b""
 
-    def __add__(self, other: "StreamingChatMessageContent") -> "StreamingChatMessageContent":
-        """When combining two StreamingChatMessageContent instances, the content fields are combined.
+    def __add__(self, other: "TextContent") -> "StreamingTextContent":
+        """When combining two StreamingTextContent instances, the text fields are combined.
 
-        The inner_content of the first one is used, ai_model_id and encoding should be the same,
-        if role is set, they should be the same.
+        The inner_content of the first one is used, choice_index, ai_model_id and encoding should be the same.
         """
-        if self.choice_index != other.choice_index:
-            raise ContentAdditionException("Cannot add StreamingChatMessageContent with different choice_index")
+        if isinstance(other, StreamingTextContent) and self.choice_index != other.choice_index:
+            raise ContentAdditionException("Cannot add StreamingTextContent with different choice_index")
         if self.ai_model_id != other.ai_model_id:
-            raise ContentAdditionException("Cannot add StreamingChatMessageContent from different ai_model_id")
+            raise ContentAdditionException("Cannot add StreamingTextContent from different ai_model_id")
         if self.encoding != other.encoding:
-            raise ContentAdditionException("Cannot add StreamingChatMessageContent with different encoding")
-        if self.role and other.role and self.role != other.role:
-            raise ContentAdditionException("Cannot add StreamingChatMessageContent with different role")
-        return StreamingChatMessageContent(
+            raise ContentAdditionException("Cannot add StreamingTextContent with different encoding")
+        return StreamingTextContent(
             choice_index=self.choice_index,
             inner_content=self.inner_content,
             ai_model_id=self.ai_model_id,
             metadata=self.metadata,
-            role=self.role,
-            content=(self.content or "") + (other.content or ""),
+            text=(self.text or "") + (other.text or ""),
             encoding=self.encoding,
-            finish_reason=self.finish_reason or other.finish_reason,
         )
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
+
 import sys
 from abc import ABC, abstractmethod
+from typing import Any
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-from typing import Any
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class StreamingContentMixin(KernelBaseModel, ABC):
     """Mixin class for all streaming kernel contents."""
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-0.9.7b1/semantic_kernel/contents/text_content.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
-from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
-from semantic_kernel.contents.text_content import TextContent
-from semantic_kernel.exceptions import ContentAdditionException
+from xml.etree.ElementTree import Element
 
+from semantic_kernel.contents.const import TEXT_CONTENT_TAG
+from semantic_kernel.contents.kernel_content import KernelContent
 
-class StreamingTextContent(StreamingContentMixin, TextContent):
-    """This is the base class for streaming text response content.
 
-    All Text Completion Services should return a instance of this class as streaming response.
+class TextContent(KernelContent):
+    """This is the base class for text response content.
+
+    All Text Completion Services should return a instance of this class as response.
     Or they can implement their own subclass of this class and return an instance.
 
     Args:
-        choice_index: int - The index of the choice that generated this response.
-        inner_content: Optional[Any] - The inner content of the response,
+        inner_content: Any - The inner content of the response,
             this should hold all the information from the response so even
             when not creating a subclass a developer can leverage the full thing.
-        ai_model_id: Optional[str] - The id of the AI model that generated this response.
-        metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-        text: Optional[str] - The text of the response.
-        encoding: Optional[str] - The encoding of the text.
+        ai_model_id: str | None - The id of the AI model that generated this response.
+        metadata: dict[str, Any] - Any metadata that should be attached to the response.
+        text: str | None - The text of the response.
+        encoding: str | None - The encoding of the text.
 
     Methods:
         __str__: Returns the text of the response.
-        __bytes__: Returns the content of the response encoded in the encoding.
-        __add__: Combines two StreamingTextContent instances.
     """
 
-    def __bytes__(self) -> bytes:
-        return self.text.encode(self.encoding if self.encoding else "utf-8") if self.text else b""
+    text: str
+    encoding: str | None = None
 
-    def __add__(self, other: "StreamingTextContent") -> "StreamingTextContent":
-        """When combining two StreamingTextContent instances, the text fields are combined.
+    def __str__(self) -> str:
+        return self.text
 
-        The inner_content of the first one is used, choice_index, ai_model_id and encoding should be the same.
-        """
-        if self.choice_index != other.choice_index:
-            raise ContentAdditionException("Cannot add StreamingTextContent with different choice_index")
-        if self.ai_model_id != other.ai_model_id:
-            raise ContentAdditionException("Cannot add StreamingTextContent from different ai_model_id")
-        if self.encoding != other.encoding:
-            raise ContentAdditionException("Cannot add StreamingTextContent with different encoding")
-        return StreamingTextContent(
-            choice_index=self.choice_index,
-            inner_content=self.inner_content,
-            ai_model_id=self.ai_model_id,
-            metadata=self.metadata,
-            text=(self.text or "") + (other.text or ""),
-            encoding=self.encoding,
-        )
+    def to_element(self) -> Element:
+        """Convert the instance to an Element."""
+        element = Element(TEXT_CONTENT_TAG)
+        element.text = self.text
+        if self.encoding:
+            element.set("encoding", self.encoding)
+        return element
+
+    @classmethod
+    def from_element(cls, element: Element) -> "TextContent":
+        """Create an instance from an Element."""
+        if element.tag != TEXT_CONTENT_TAG:
+            raise ValueError(f"Element tag is not {TEXT_CONTENT_TAG}")
+
+        return TextContent(text=element.text or "", encoding=element.get("encoding", None))
+
+    def to_dict(self) -> dict[str, str]:
+        """Convert the instance to a dictionary."""
+        return {"type": "text", "text": self.text}
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class HttpPlugin(KernelBaseModel):
     """
     A plugin that provides HTTP functionality.
 
     Usage:
-        kernel.import_plugin_from_object(HttpPlugin(), "http")
+        kernel.add_plugin(HttpPlugin(), "http")
 
     Examples:
 
         {{http.getAsync $url}}
         {{http.postAsync $url}}
         {{http.putAsync $url}}
         {{http.deleteAsync $url}}
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class MathPlugin:
     """
     Description: MathPlugin provides a set of functions to make Math calculations.
 
     Usage:
-        kernel.import_plugin_from_object(MathPlugin(), plugin_name="math")
+        kernel.add_plugin(MathPlugin(), plugin_name="math")
 
     Examples:
         {{math.Add}} => Returns the sum of input and amount (provided in the KernelArguments)
         {{math.Subtract}} => Returns the difference of input and amount (provided in the KernelArguments)
     """
 
     @kernel_function(name="Add")
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 # Copyright (c) Microsoft. All rights reserved.
 import json
 import logging
 import sys
-from typing import ClassVar, Optional
+from typing import Any, Dict, Final
+
+from pydantic import Field
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
+
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 
 logger: logging.Logger = logging.getLogger(__name__)
 
+DEFAULT_COLLECTION: Final[str] = "generic"
+COLLECTION_PARAM: Final[str] = "collection"
+DEFAULT_RELEVANCE: Final[float] = 0.75
+RELEVANCE_PARAM: Final[str] = "relevance"
+DEFAULT_LIMIT: Final[int] = 1
 
-class TextMemoryPlugin(KernelBaseModel):
-    DEFAULT_COLLECTION: ClassVar[str] = "generic"
-    COLLECTION_PARAM: ClassVar[str] = "collection"
-    DEFAULT_RELEVANCE: ClassVar[float] = 0.75
-    RELEVANCE_PARAM: ClassVar[str] = "relevance"
-    DEFAULT_LIMIT: ClassVar[int] = 1
 
+class TextMemoryPlugin(KernelBaseModel):
     memory: SemanticTextMemoryBase
+    embeddings_kwargs: Dict[str, Any] = Field(default_factory=dict)
 
-    def __init__(self, memory: SemanticTextMemoryBase) -> None:
+    def __init__(self, memory: SemanticTextMemoryBase, embeddings_kwargs: Dict[str, Any] = {}) -> None:
         """
         Initialize a new instance of the TextMemoryPlugin
 
         Args:
             memory (SemanticTextMemoryBase) - the underlying Semantic Text Memory to use
+            embeddings_kwargs (Optional[Dict[str, Any]]) - the keyword arguments to pass to the embedding generator
         """
-        super().__init__(memory=memory)
+        super().__init__(memory=memory, embeddings_kwargs=embeddings_kwargs)
 
     @kernel_function(
         description="Recall a fact from the long term memory",
         name="recall",
     )
     async def recall(
         self,
         ask: Annotated[str, "The information to retrieve"],
-        collection: Annotated[Optional[str], "The collection to search for information."] = DEFAULT_COLLECTION,
+        collection: Annotated[str, "The collection to search for information."] = DEFAULT_COLLECTION,
         relevance: Annotated[
-            Optional[float], "The relevance score, from 0.0 to 1.0; 1.0 means perfect match"
+            float, "The relevance score, from 0.0 to 1.0; 1.0 means perfect match"
         ] = DEFAULT_RELEVANCE,
-        limit: Annotated[Optional[int], "The maximum number of relevant memories to recall."] = DEFAULT_LIMIT,
+        limit: Annotated[int, "The maximum number of relevant memories to recall."] = DEFAULT_LIMIT,
     ) -> str:
         """
         Recall a fact from the long term memory.
 
         Example:
             {{memory.recall $ask}} => "Paris"
 
@@ -77,21 +82,23 @@
         description="Save information to semantic memory",
         name="save",
     )
     async def save(
         self,
         text: Annotated[str, "The information to save."],
         key: Annotated[str, "The unique key to associate with the information."],
-        collection: Annotated[Optional[str], "The collection to save the information."] = DEFAULT_COLLECTION,
+        collection: Annotated[str, "The collection to save the information."] = DEFAULT_COLLECTION,
     ) -> None:
         """
         Save a fact to the long term memory.
 
         Args:
             text -- The text to save to the memory
             kernel -- The kernel instance, that has a memory store
             collection -- The collection to save the information
             key -- The unique key to associate with the information
 
         """
 
-        await self.memory.save_information(collection, text=text, id=key)
+        await self.memory.save_information(
+            collection=collection, text=text, id=key, embeddings_kwargs=self.embeddings_kwargs
+        )
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class TextPlugin(KernelBaseModel):
     """
     TextPlugin provides a set of functions to manipulate strings.
 
     Usage:
-        kernel.import_plugin_from_object(TextPlugin(), plugin_name="text")
+        kernel.add_plugin(TextPlugin(), plugin_name="text")
 
     Examples:
         KernelArguments["input"] = "  hello world  "
         {{text.trim $input}} => "hello world"
 
         KernelArguments["input"] = "  hello world  "
         {{text.trimStart $input} => "hello world  "
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class TimePlugin(KernelBaseModel):
     """
     Description: TimePlugin provides a set of functions
                  to get the current time and date.
 
     Usage:
-        kernel.import_plugin_from_object(TimePlugin(), plugin_name="time")
+        kernel.add_plugin(TimePlugin(), plugin_name="time")
 
     Examples:
         {{time.date}}            => Sunday, 12 January, 2031
         {{time.today}}           => Sunday, 12 January, 2031
         {{time.iso_date}}        => 2031-01-12
         {{time.now}}             => Sunday, January 12, 2031 9:15 PM
         {{time.utcNow}}          => Sunday, January 13, 2031 5:15 AM
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class WaitPlugin(KernelBaseModel):
     """
     WaitPlugin provides a set of functions to wait for a certain amount of time.
 
     Usage:
-        kernel.import_plugin_from_object(WaitPlugin(), plugin_name="wait")
+        kernel.add_plugin(WaitPlugin(), plugin_name="wait")
 
     Examples:
         {{wait.wait 5}} => Wait for 5 seconds
     """
 
     @kernel_function(description="Wait for a certain number of seconds.")
     async def wait(
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class WebSearchEnginePlugin:
     """
     Description: A plugin that provides web search engine functionality
 
     Usage:
         connector = BingConnector(bing_search_api_key)
-        kernel.import_plugin_from_object(WebSearchEnginePlugin(connector), plugin_name="WebSearch")
+        kernel.add_plugin(WebSearchEnginePlugin(connector), plugin_name="WebSearch")
 
     Examples:
         {{WebSearch.search "What is semantic kernel?"}}
         =>  Returns the first `num_results` number of results for the given search query
             and ignores the first `offset` number of results.
     """
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/events/function_invoked_event_args.py` & `semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoked_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/events/function_invoking_event_args.py` & `semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoking_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/events/kernel_events_args.py` & `semantic_kernel-0.9.7b1/semantic_kernel/events/kernel_events_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/function_result.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/function_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
 import logging
-from typing import Any, Mapping, Optional
+from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.contents.kernel_content import KernelContent
 from semantic_kernel.exceptions import FunctionResultError
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
@@ -27,15 +28,15 @@
         get_inner_content: Get the inner content of the function result
             when that is a KernelContent or subclass of the first item of the value if it is a list.
 
     """
 
     function: KernelFunctionMetadata
     value: Any
-    metadata: Mapping[str, Any] = Field(default_factory=dict)
+    metadata: dict[str, Any] = Field(default_factory=dict)
 
     def __str__(self) -> str:
         """Get the string representation of the result."""
         if self.value:
             try:
                 if isinstance(self.value, list):
                     return str(self.value[0])
@@ -45,15 +46,15 @@
                     return str(list(self.value.values())[-1])
                 return str(self.value)
             except Exception as e:
                 raise FunctionResultError(f"Failed to convert value to string: {e}") from e
         else:
             return ""
 
-    def get_inner_content(self, index: int = 0) -> Optional[Any]:
+    def get_inner_content(self, index: int = 0) -> Any | None:
         """Get the inner content of the function result.
 
         Arguments:
             index (int): The index of the inner content if the inner content is a list, default 0.
         """
         if isinstance(self.value, list):
             if isinstance(self.value[index], KernelContent):
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             settings (PromptExecutionSettings | List[PromptExecutionSettings] | None) --
                 The settings for the execution.
                 If a list is given, make sure all items in the list have a unique service_id
                 as that is used as the key for the dict.
             **kwargs (dict[str, Any]) -- The arguments for the function invocation, works similar to a regular dict.
         """
         super().__init__(**kwargs)
-        settings_dict = {}
+        settings_dict = None
         if settings:
+            settings_dict = {}
             if isinstance(settings, list):
-                settings_dict = {s.service_id: s for s in settings}
+                settings_dict = {s.service_id or "default": s for s in settings}
             else:
-                settings_dict = {settings.service_id: settings}
+                settings_dict = {settings.service_id or "default": settings}
         self.execution_settings: dict[str, "PromptExecutionSettings"] | None = settings_dict
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
+from collections.abc import AsyncGenerator
 from copy import copy, deepcopy
-from typing import TYPE_CHECKING, Any, AsyncIterable, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable
 
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import (
@@ -65,23 +66,23 @@
     metadata: KernelFunctionMetadata
 
     @classmethod
     def from_prompt(
         cls,
         function_name: str,
         plugin_name: str,
-        description: Optional[str] = None,
-        prompt: Optional[str] = None,
+        description: str | None = None,
+        prompt: str | None = None,
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
-        prompt_template: Optional["PromptTemplateBase"] = None,
-        prompt_template_config: Optional["PromptTemplateConfig"] = None,
-        prompt_execution_settings: Optional[
-            Union["PromptExecutionSettings", List["PromptExecutionSettings"], Dict[str, "PromptExecutionSettings"]]
-        ] = None,
-    ) -> "KernelFunctionFromPrompt":
+        prompt_template: PromptTemplateBase | None = None,
+        prompt_template_config: PromptTemplateConfig | None = None,
+        prompt_execution_settings: (
+            PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None
+        ) = None,
+    ) -> KernelFunctionFromPrompt:
         """
         Create a new instance of the KernelFunctionFromPrompt class.
         """
         from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
 
         return KernelFunctionFromPrompt(
             function_name=function_name,
@@ -94,17 +95,17 @@
             prompt_execution_settings=prompt_execution_settings,
         )
 
     @classmethod
     def from_method(
         cls,
         method: Callable[..., Any],
-        plugin_name: Optional[str] = None,
-        stream_method: Optional[Callable[..., Any]] = None,
-    ) -> "KernelFunctionFromMethod":
+        plugin_name: str | None = None,
+        stream_method: Callable[..., Any] | None = None,
+    ) -> KernelFunctionFromMethod:
         """
         Create a new instance of the KernelFunctionFromMethod class.
         """
         from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 
         return KernelFunctionFromMethod(
             plugin_name=plugin_name,
@@ -121,35 +122,35 @@
         return self.metadata.plugin_name or ""
 
     @property
     def fully_qualified_name(self) -> str:
         return self.metadata.fully_qualified_name
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         return self.metadata.description
 
     @property
     def is_prompt(self) -> bool:
         return self.metadata.is_prompt
 
     @property
-    def parameters(self) -> List[KernelParameterMetadata]:
+    def parameters(self) -> list[KernelParameterMetadata]:
         return self.metadata.parameters
 
     @property
-    def return_parameter(self) -> Optional[KernelParameterMetadata]:
+    def return_parameter(self) -> KernelParameterMetadata | None:
         return self.metadata.return_parameter
 
     async def __call__(
         self,
-        kernel: "Kernel",
-        arguments: Optional[KernelArguments] = None,
+        kernel: Kernel,
+        arguments: KernelArguments | None = None,
         **kwargs: Any,
-    ) -> "FunctionResult":
+    ) -> FunctionResult:
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (Optional[KernelArguments]): The Kernel arguments.
                 Optional, defaults to None.
             kwargs (Dict[str, Any]): Additional keyword arguments that will be
@@ -158,25 +159,25 @@
             FunctionResult: The result of the function
         """
         return await self.invoke(kernel, arguments, **kwargs)
 
     @abstractmethod
     async def _invoke_internal(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         arguments: KernelArguments,
-    ) -> "FunctionResult":
+    ) -> FunctionResult:
         pass
 
     async def invoke(
         self,
-        kernel: "Kernel",
-        arguments: Optional[KernelArguments] = None,
+        kernel: Kernel,
+        arguments: KernelArguments | None = None,
         **kwargs: Any,
-    ) -> "FunctionResult":
+    ) -> FunctionResult:
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
             kwargs (Any): Additional keyword arguments that will be
                 added to the KernelArguments.
@@ -191,27 +192,32 @@
         except Exception as exc:
             logger.error(f"Error occurred while invoking function {self.name}: {exc}")
             return FunctionResult(
                 function=self.metadata, value=None, metadata={"exception": exc, "arguments": arguments}
             )
 
     @abstractmethod
-    async def _invoke_internal_stream(
+    def _invoke_internal_stream(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[FunctionResult, List[Union["StreamingContentMixin", Any]]]]:
-        pass
+    ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]:
+        """Internal invoke method of the the function with the given arguments.
+
+        The abstract method is defined without async because otherwise the typing fails.
+        A implementation of this function should be async.
+        """
+        ...
 
     async def invoke_stream(
         self,
-        kernel: "Kernel",
-        arguments: Optional[KernelArguments] = None,
+        kernel: Kernel,
+        arguments: KernelArguments | None = None,
         **kwargs: Any,
-    ) -> AsyncIterable[Union[FunctionResult, List[Union["StreamingContentMixin", Any]]]]:
+    ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]:
         """
         Invoke a stream async function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
             kwargs (Any): Additional keyword arguments that will be
@@ -226,15 +232,15 @@
         try:
             async for partial_result in self._invoke_internal_stream(kernel, arguments):
                 yield partial_result
         except Exception as e:
             logger.error(f"Error occurred while invoking function {self.name}: {e}")
             yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e, "arguments": arguments})
 
-    def function_copy(self, plugin_name: str | None = None) -> "KernelFunction":
+    def function_copy(self, plugin_name: str | None = None) -> KernelFunction:
         """Copy the function, can also override the plugin_name.
 
         Args:
             plugin_name (str): The new plugin name.
 
         Returns:
             KernelFunction: The copied function.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from typing import Any, Callable
 
 NoneType = type(None)
 logger = logging.getLogger(__name__)
 
 
 def kernel_function(
-    func: Callable[..., Any] | None = None,
+    func: Callable[..., object] | None = None,
     name: str | None = None,
     description: str | None = None,
-) -> Callable[..., Any]:
+) -> Callable[..., object]:
     """
     Decorator for kernel functions.
 
     This decorator is used to mark a function as a kernel function. It also provides metadata for the function.
     The name and description can be left empty, and then the function name and docstring will be used.
 
     The parameters are parsed from the function signature, use typing.Annotated to provide a description for the
@@ -39,38 +39,38 @@
     Args:
         name (Optional[str]) -- The name of the function, if not supplied, the function name will be used.
         description (Optional[str]) -- The description of the function,
             if not supplied, the function docstring will be used, can be None.
 
     """
 
-    @wraps(func)
-    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
-        func.__kernel_function__ = True
-        func.__kernel_function_description__ = description or func.__doc__
-        func.__kernel_function_name__ = name or func.__name__
-        func.__kernel_function_streaming__ = isasyncgenfunction(func) or isgeneratorfunction(func)
-        logger.debug(f"Parsing decorator for function: {func.__kernel_function_name__}")
+    @wraps(wrapped=func)  # type: ignore
+    def decorator(func: Callable[..., object]) -> Callable[..., object]:
+        func.__kernel_function__ = True  # type: ignore
+        func.__kernel_function_description__ = description or func.__doc__  # type: ignore
+        func.__kernel_function_name__ = name or func.__name__  # type: ignore
+        func.__kernel_function_streaming__ = isasyncgenfunction(func) or isgeneratorfunction(func)  # type: ignore
+        logger.debug(f"Parsing decorator for function: {func.__kernel_function_name__}")  # type: ignore
 
         func_sig = signature(func)
         logger.debug(f"{func_sig=}")
-        func.__kernel_function_parameters__ = [
+        func.__kernel_function_parameters__ = [  # type: ignore
             _parse_parameter(param) for param in func_sig.parameters.values() if param.name != "self"
         ]
         return_param_dict = {}
         if func_sig.return_annotation != Signature.empty:
             return_param_dict = _parse_annotation(func_sig.return_annotation)
-        func.__kernel_function_return_type__ = return_param_dict.get("type_", "None")
-        func.__kernel_function_return_description__ = return_param_dict.get("description", "")
-        func.__kernel_function_return_required__ = return_param_dict.get("is_required", False)
+        func.__kernel_function_return_type__ = return_param_dict.get("type_", "None")  # type: ignore
+        func.__kernel_function_return_description__ = return_param_dict.get("description", "")  # type: ignore
+        func.__kernel_function_return_required__ = return_param_dict.get("is_required", False)  # type: ignore
         return func
 
     if func:
         return decorator(func)
-    return decorator
+    return decorator  # type: ignore
 
 
 def _parse_parameter(param: Parameter) -> dict[str, Any]:
     logger.debug(f"Parsing param: {param}")
     ret = {}
     if param != Parameter.empty:
         ret = _parse_annotation(param.annotation)
@@ -84,27 +84,27 @@
     logger.debug(f"Parsing annotation: {annotation}")
     if annotation == Signature.empty:
         return {"type_": "Any", "is_required": True}
     if isinstance(annotation, str):
         return {"type_": annotation, "is_required": True}
     logger.debug(f"{annotation=}")
     ret = _parse_internal_annotation(annotation, True)
-    if hasattr(annotation, "__metadata__") and annotation.__metadata__:
-        ret["description"] = annotation.__metadata__[0]
+    if hasattr(annotation, "__metadata__") and annotation.__metadata__:  # type: ignore
+        ret["description"] = annotation.__metadata__[0]  # type: ignore
     return ret
 
 
 def _parse_internal_annotation(annotation: Parameter, required: bool) -> dict[str, Any]:
     logger.debug(f"Internal {annotation=}")
     if hasattr(annotation, "__forward_arg__"):
-        return {"type_": annotation.__forward_arg__, "is_required": required}
+        return {"type_": annotation.__forward_arg__, "is_required": required}  # type: ignore
     if getattr(annotation, "__name__", None) == "Optional":
         required = False
     if hasattr(annotation, "__args__"):
-        results = [_parse_internal_annotation(arg, required) for arg in annotation.__args__]
+        results = [_parse_internal_annotation(arg, required) for arg in annotation.__args__]  # type: ignore
         type_objects = [
             result["type_object"]
             for result in results
             if "type_object" in result and result["type_object"] is not NoneType
         ]
         str_results = [result["type_"] for result in results]
         if "NoneType" in str_results:
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
 import logging
 from inspect import isasyncgen, isasyncgenfunction, isawaitable, iscoroutinefunction, isgenerator, isgeneratorfunction
-from typing import TYPE_CHECKING, Any, AsyncIterable, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable
 
 from pydantic import ValidationError
 
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
@@ -23,21 +24,21 @@
 
 class KernelFunctionFromMethod(KernelFunction):
     """Semantic Kernel Function from a method."""
 
     # some attributes are now properties, still listed here for documentation purposes
 
     method: Callable[..., Any]
-    stream_method: Optional[Callable[..., Any]] = None
+    stream_method: Callable[..., Any] | None = None
 
     def __init__(
         self,
         method: Callable[..., Any],
-        plugin_name: Optional[str] = None,
-        stream_method: Optional[Callable[..., Any]] = None,
+        plugin_name: str | None = None,
+        stream_method: Callable[..., Any] | None = None,
     ) -> None:
         """
         Initializes a new instance of the KernelFunctionFromMethod class
 
         Args:
             method (Callable[..., Any]): The method to be called
             plugin_name (Optional[str]): The name of the plugin
@@ -72,29 +73,29 @@
                 is_asynchronous=isasyncgenfunction(method) or iscoroutinefunction(method),
                 plugin_name=plugin_name,
             )
         except ValidationError as exc:
             # reraise the exception to clarify it comes from KernelFunction init
             raise FunctionInitializationError("Failed to create KernelFunctionMetadata") from exc
 
-        args: Dict[str, Any] = {
+        args: dict[str, Any] = {
             "metadata": metadata,
             "method": method,
             "stream_method": (
                 stream_method
                 if stream_method is not None
                 else method if isasyncgenfunction(method) or isgeneratorfunction(method) else None
             ),
         }
 
         super().__init__(**args)
 
     async def _invoke_internal(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         arguments: KernelArguments,
     ) -> FunctionResult:
         """Invoke the function with the given arguments."""
         function_arguments = self.gather_function_parameters(kernel, arguments)
         result = self.method(**function_arguments)
         if isasyncgen(result):
             result = [x async for x in result]
@@ -108,46 +109,46 @@
             function=self.metadata,
             value=result,
             metadata={"arguments": arguments, "used_arguments": function_arguments},
         )
 
     async def _invoke_internal_stream(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[List[StreamingContentMixin], Any]]:
+    ) -> AsyncGenerator[list[StreamingContentMixin] | Any, Any]:
         if self.stream_method is None:
             raise NotImplementedError("Stream method not implemented")
         function_arguments = self.gather_function_parameters(kernel, arguments)
         if isasyncgenfunction(self.stream_method):
             async for partial_result in self.stream_method(**function_arguments):
                 yield partial_result
         elif isgeneratorfunction(self.stream_method):
             for partial_result in self.stream_method(**function_arguments):
                 yield partial_result
 
-    def gather_function_parameters(self, kernel: "Kernel", arguments: "KernelArguments") -> Dict[str, Any]:
+    def gather_function_parameters(self, kernel: Kernel, arguments: KernelArguments) -> dict[str, Any]:
         """Gathers the function parameters from the arguments."""
-        function_arguments: Dict[str, Any] = {}
+        function_arguments: dict[str, Any] = {}
         for param in self.parameters:
             if param.name == "kernel":
                 function_arguments[param.name] = kernel
                 continue
             if param.name == "service":
                 function_arguments[param.name] = kernel.select_ai_service(self, arguments)[0]
                 continue
             if param.name == "execution_settings":
                 function_arguments[param.name] = kernel.select_ai_service(self, arguments)[1]
                 continue
             if param.name == "arguments":
                 function_arguments[param.name] = arguments
                 continue
             if param.name in arguments:
-                value = arguments[param.name]
-                if param.type_.find(",") == -1 and param.type_object:
+                value: Any = arguments[param.name]
+                if param.type_ and "," not in param.type_ and param.type_object:
                     if hasattr(param.type_object, "model_validate"):
                         try:
                             value = param.type_object.model_validate(value)
                         except Exception as exc:
                             raise FunctionExecutionException(
                                 f"Parameter {param.name} is expected to be parsed to {param.type_} but is not."
                             ) from exc
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 import os
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, AsyncGenerator
 
 import yaml
 from pydantic import Field, ValidationError, model_validator
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
-    OpenAIChatPromptExecutionSettings,
-)
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
+from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
+from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import TEMPLATE_FORMAT_MAP, KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
@@ -35,37 +34,37 @@
 
 PROMPT_FILE_NAME = "skprompt.txt"
 CONFIG_FILE_NAME = "config.json"
 PROMPT_RETURN_PARAM = KernelParameterMetadata(
     name="return",
     description="The completion result",
     default_value=None,
-    type="FunctionResult",
+    type="FunctionResult",  # type: ignore
     is_required=True,
 )
 
 
 class KernelFunctionFromPrompt(KernelFunction):
     """Semantic Kernel Function from a prompt."""
 
     prompt_template: PromptTemplateBase
-    prompt_execution_settings: Dict[str, PromptExecutionSettings] = Field(default_factory=dict)
+    prompt_execution_settings: dict[str, PromptExecutionSettings] = Field(default_factory=dict)
 
     def __init__(
         self,
         function_name: str,
-        plugin_name: Optional[str] = None,
-        description: Optional[str] = None,
-        prompt: Optional[str] = None,
+        plugin_name: str | None = None,
+        description: str | None = None,
+        prompt: str | None = None,
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
-        prompt_template: Optional[PromptTemplateBase] = None,
-        prompt_template_config: Optional[PromptTemplateConfig] = None,
-        prompt_execution_settings: Optional[
-            Union[PromptExecutionSettings, List[PromptExecutionSettings], Dict[str, PromptExecutionSettings]]
-        ] = None,
+        prompt_template: PromptTemplateBase | None = None,
+        prompt_template_config: PromptTemplateConfig | None = None,
+        prompt_execution_settings: None | (
+            PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings]
+        ) = None,
     ) -> None:
         """
         Initializes a new instance of the KernelFunctionFromPrompt class
 
         Args:
             function_name (str): The name of the function
             plugin_name (str): The name of the plugin
@@ -91,38 +90,40 @@
                 # prompt must be there if prompt_template and prompt_template_config is not supplied
                 prompt_template_config = PromptTemplateConfig(
                     name=function_name,
                     description=description,
                     template=prompt,
                     template_format=template_format,
                 )
-            prompt_template = TEMPLATE_FORMAT_MAP[template_format](prompt_template_config=prompt_template_config)
+            prompt_template = TEMPLATE_FORMAT_MAP[template_format](prompt_template_config=prompt_template_config)  # type: ignore
 
         try:
             metadata = KernelFunctionMetadata(
                 name=function_name,
                 plugin_name=plugin_name,
                 description=description,
                 parameters=prompt_template.prompt_template_config.get_kernel_parameter_metadata(),
                 is_prompt=True,
                 is_asynchronous=True,
                 return_parameter=PROMPT_RETURN_PARAM,
             )
         except ValidationError as exc:
             raise FunctionInitializationError("Failed to create KernelFunctionMetadata") from exc
         super().__init__(
-            metadata=metadata, prompt_template=prompt_template, prompt_execution_settings=prompt_execution_settings
+            metadata=metadata,
+            prompt_template=prompt_template,
+            prompt_execution_settings=prompt_execution_settings,
         )
 
     @model_validator(mode="before")
     @classmethod
     def rewrite_execution_settings(
         cls,
-        data: Dict[str, Any],
-    ) -> Dict[str, PromptExecutionSettings]:
+        data: dict[str, Any],
+    ) -> dict[str, PromptExecutionSettings]:
         """Rewrite execution settings to a dictionary.
 
         If the prompt_execution_settings is not a dictionary, it is converted to a dictionary.
         If it is not supplied, but prompt_template is, the prompt_template's execution settings are used.
         """
         prompt_execution_settings = data.get("prompt_execution_settings")
         prompt_template = data.get("prompt_template")
@@ -138,17 +139,17 @@
             }
         if isinstance(prompt_execution_settings, list):
             data["prompt_execution_settings"] = {s.service_id or "default": s for s in prompt_execution_settings}
         return data
 
     async def _invoke_internal(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         arguments: KernelArguments,
-    ) -> "FunctionResult":
+    ) -> FunctionResult:
         """Invokes the function with the given arguments."""
         arguments = self.add_default_values(arguments)
         service, execution_settings = kernel.select_ai_service(self, arguments)
         prompt = await self.prompt_template.render(kernel, arguments)
 
         if isinstance(service, ChatCompletionClientBase):
             return await self._handle_complete_chat(
@@ -167,67 +168,65 @@
                 arguments=arguments,
             )
 
         raise ValueError(f"Service `{type(service).__name__}` is not a valid AI service")
 
     async def _handle_complete_chat(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         service: ChatCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
         arguments: KernelArguments,
     ) -> FunctionResult:
         """Handles the chat service call."""
-        chat_history = ChatHistory.from_rendered_prompt(prompt, service.get_chat_message_content_type())
+        chat_history = ChatHistory.from_rendered_prompt(prompt)
 
         # pass the kernel in for auto function calling
-        kwargs = {}
-        if isinstance(execution_settings, OpenAIChatPromptExecutionSettings) and isinstance(
-            service, ChatCompletionClientBase
-        ):
+        kwargs: dict[str, Any] = {}
+        if hasattr(execution_settings, "auto_invoke_kernel_functions"):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
         try:
             completions = await service.complete_chat(
                 chat_history=chat_history,
                 settings=execution_settings,
                 **kwargs,
             )
             if not completions:
                 raise FunctionExecutionException(f"No completions returned while invoking function {self.name}")
 
-            return self._create_function_result(completions, chat_history, arguments)
+            return self._create_function_result(completions=completions, chat_history=chat_history, arguments=arguments)
         except Exception as exc:
             raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
 
     async def _handle_text_complete(
         self,
         service: TextCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
         arguments: KernelArguments,
     ) -> FunctionResult:
         """Handles the text service call."""
         try:
             completions = await service.complete(prompt, execution_settings)
-            return self._create_function_result(completions, None, arguments, prompt=prompt)
+            return self._create_function_result(completions=completions, arguments=arguments, prompt=prompt)
         except Exception as exc:
             raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
 
     def _create_function_result(
         self,
-        completions: Union[List[ChatMessageContent], List[TextContent]],
-        chat_history: ChatHistory,
+        completions: list[ChatMessageContent] | list[TextContent],
         arguments: KernelArguments,
-        prompt: str = None,
+        chat_history: ChatHistory | None = None,
+        prompt: str | None = None,
     ) -> FunctionResult:
         """Creates a function result with the given completions."""
-        metadata = {
+        metadata: dict[str, Any] = {
             "arguments": arguments,
             "metadata": [completion.metadata for completion in completions],
         }
         if chat_history:
             metadata["messages"] = chat_history
         if prompt:
             metadata["prompt"] = prompt
@@ -235,65 +234,61 @@
             function=self.metadata,
             value=completions,
             metadata=metadata,
         )
 
     async def _invoke_internal_stream(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[FunctionResult, List[StreamingContentMixin]]]:
+    ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin], Any]:
         """Invokes the function stream with the given arguments."""
         arguments = self.add_default_values(arguments)
         service, execution_settings = kernel.select_ai_service(self, arguments)
         prompt = await self.prompt_template.render(kernel, arguments)
 
         if isinstance(service, ChatCompletionClientBase):
             async for content in self._handle_complete_chat_stream(
                 kernel=kernel,
                 service=service,
                 execution_settings=execution_settings,
                 prompt=prompt,
                 arguments=arguments,
             ):
-                yield content
+                yield content  # type: ignore
             return
 
         if isinstance(service, TextCompletionClientBase):
-            async for content in self._handle_complete_text_stream(
+            async for content in self._handle_complete_text_stream(  # type: ignore
                 service=service,
                 execution_settings=execution_settings,
                 prompt=prompt,
             ):
-                yield content
+                yield content  # type: ignore
             return
 
         raise FunctionExecutionException(f"Service `{type(service)}` is not a valid AI service")  # pragma: no cover
 
     async def _handle_complete_chat_stream(
         self,
-        kernel: "Kernel",
+        kernel: Kernel,
         service: ChatCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[FunctionResult, List[StreamingContentMixin]]]:
+    ) -> AsyncGenerator[FunctionResult | list[StreamingChatMessageContent], Any]:
         """Handles the chat service call."""
 
         # pass the kernel in for auto function calling
-        kwargs = {}
-        if isinstance(execution_settings, OpenAIChatPromptExecutionSettings) and isinstance(
-            service, ChatCompletionClientBase
-        ):
+        kwargs: dict[str, Any] = {}
+        if hasattr(execution_settings, "auto_invoke_kernel_functions"):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
-        chat_history = ChatHistory.from_rendered_prompt(
-            prompt,
-        )
+        chat_history = ChatHistory.from_rendered_prompt(prompt)
         try:
             async for partial_content in service.complete_chat_stream(
                 chat_history=chat_history,
                 settings=execution_settings,
                 **kwargs,
             ):
                 yield partial_content
@@ -304,33 +299,33 @@
             yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e})
 
     async def _handle_complete_text_stream(
         self,
         service: TextCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
-    ) -> AsyncIterable[Union[FunctionResult, List[StreamingContentMixin]]]:
+    ) -> AsyncGenerator[FunctionResult | list[StreamingTextContent], Any]:
         """Handles the text service call."""
         try:
             async for partial_content in service.complete_stream(prompt=prompt, settings=execution_settings):
                 yield partial_content
             return
         except Exception as e:
             logger.error(f"Error occurred while invoking function {self.name}: {e}")
             yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e})
 
-    def add_default_values(self, arguments: "KernelArguments") -> KernelArguments:
+    def add_default_values(self, arguments: KernelArguments) -> KernelArguments:
         """Gathers the function parameters from the arguments."""
         for parameter in self.prompt_template.prompt_template_config.input_variables:
             if parameter.name not in arguments and parameter.default not in {None, "", False, 0}:
                 arguments[parameter.name] = parameter.default
         return arguments
 
     @classmethod
-    def from_yaml(cls, yaml_str: str, plugin_name: str | None = None) -> "KernelFunctionFromPrompt":
+    def from_yaml(cls, yaml_str: str, plugin_name: str | None = None) -> KernelFunctionFromPrompt:
         """Creates a new instance of the KernelFunctionFromPrompt class from a YAML string."""
         try:
             data = yaml.safe_load(yaml_str)
         except yaml.YAMLError as exc:  # pragma: no cover
             raise FunctionInitializationError(f"Invalid YAML content: {yaml_str}, error: {exc}") from exc
 
         if not isinstance(data, dict):
@@ -347,15 +342,15 @@
             plugin_name=plugin_name,
             description=prompt_template_config.description,
             prompt_template_config=prompt_template_config,
             template_format=prompt_template_config.template_format,
         )
 
     @classmethod
-    def from_directory(cls, path: str, plugin_name: str | None = None) -> "KernelFunctionFromPrompt":
+    def from_directory(cls, path: str, plugin_name: str | None = None) -> KernelFunctionFromPrompt:
         """Creates a new instance of the KernelFunctionFromPrompt class from a directory.
 
         The directory needs to contain:
         - A prompt file named `skprompt.txt`
         - A config file named `config.json`
 
         Returns:
@@ -379,19 +374,19 @@
             raise FunctionInitializationError(
                 f"{PROMPT_FILE_NAME} files are required to create a function from a directory, "
                 f"path: {str(path)}, config file is there."
             )
 
         function_name = os.path.basename(path)
 
-        with open(config_path, "r") as config_file:
+        with open(config_path) as config_file:
             prompt_template_config = PromptTemplateConfig.from_json(config_file.read())
         prompt_template_config.name = function_name
 
-        with open(prompt_path, "r") as prompt_file:
+        with open(prompt_path) as prompt_file:
             prompt_template_config.template = prompt_file.read()
 
         prompt_template = TEMPLATE_FORMAT_MAP[prompt_template_config.template_format](  # type: ignore
             prompt_template_config=prompt_template_config
         )
         return cls(
             function_name=function_name,
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 
 import importlib
 import inspect
 import json
 import logging
 import os
 import sys
-from collections.abc import Callable, Iterable
+from collections.abc import Generator
+from functools import singledispatchmethod
 from glob import glob
 from types import MethodType
 from typing import TYPE_CHECKING, Any, ItemsView
 
-from semantic_kernel.connectors.openapi_plugin.openapi_manager import create_functions_from_openapi
-from semantic_kernel.exceptions.function_exceptions import FunctionInitializationError
-
 if sys.version_info >= (3, 9):
     from typing import Annotated  # pragma: no cover
 else:
     from typing_extensions import Annotated  # pragma: no cover
 
 import httpx
 from pydantic import Field, StringConstraints
 
 from semantic_kernel.connectors.openai_plugin.openai_authentication_config import OpenAIAuthenticationConfig
 from semantic_kernel.connectors.openai_plugin.openai_function_execution_parameters import (
     OpenAIFunctionExecutionParameters,
 )
 from semantic_kernel.connectors.openai_plugin.openai_utils import OpenAIUtils
+from semantic_kernel.connectors.openapi_plugin.openapi_manager import create_functions_from_openapi
 from semantic_kernel.connectors.utils.document_loader import DocumentLoader
 from semantic_kernel.exceptions import PluginInitializationError
+from semantic_kernel.exceptions.function_exceptions import FunctionInitializationError
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
 from semantic_kernel.functions.types import KERNEL_FUNCTION_TYPE
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.utils.validation import PLUGIN_NAME_REGEX
 
@@ -133,18 +133,18 @@
             name=name,
             description=description,
             functions=self._validate_functions(functions=functions, plugin_name=name),
         )
 
     # region Dict-like methods
 
-    def __setitem__(self, key: str, value: KernelFunction) -> None:
+    def __setitem__(self, key: str, value: KERNEL_FUNCTION_TYPE) -> None:
         self.functions[key] = KernelPlugin._parse_or_copy(value, self.name)
 
-    def set(self, key: str, value: KernelFunction) -> None:
+    def set(self, key: str, value: KERNEL_FUNCTION_TYPE) -> None:
         """Set a function in the plugin.
 
         Args:
             key (str): The name of the function.
             value (KernelFunction): The function to set.
 
         """
@@ -163,67 +163,73 @@
             *args: The functions to update the plugin with, can be a dict, list or KernelPlugin.
             **kwargs: The kernel functions to update the plugin with.
 
         """
         if len(args) > 1:
             raise TypeError("update expected at most 1 arguments, got %d" % len(args))
         if args:
-            other = args[0]
-            if isinstance(other, KernelPlugin):
-                other = other.functions
-            if not isinstance(other, (dict, list)):
-                raise TypeError(f"Expected dict, KernelPlugin or list as arg, got {type(other)}")
-            if isinstance(other, dict):
-                for key in other:
-                    self[key] = other[key]
+            if isinstance(args[0], KernelPlugin):
+                self.add(args[0].functions)
             else:
-                for item in other:
-                    if isinstance(item, (KernelFunction, Callable)):
-                        item = KernelPlugin._parse_or_copy(item, self.name)
-                        self[item.name] = item
-                    elif isinstance(item, KernelPlugin):
-                        for key in item.functions:
-                            self[key] = item.functions[key]
-        if kwargs:
-            for key in kwargs:
-                self[key] = kwargs[key]
+                self.add(args[0])
+        self.add(kwargs)
+
+    @singledispatchmethod
+    def add(self, functions: Any) -> None:
+        raise TypeError(f"Unknown type being added, type was {type(functions)}")
+
+    @add.register(list)
+    def add_list(self, functions: list[KERNEL_FUNCTION_TYPE | KernelPlugin]) -> None:
+        """Add a list of functions to the plugin."""
+        for function in functions:
+            if isinstance(function, KernelPlugin):
+                self.add(function.functions)
+                continue
+            function = KernelPlugin._parse_or_copy(function, self.name)
+            self[function.name] = function
+
+    @add.register(dict)
+    def add_dict(self, functions: dict[str, KERNEL_FUNCTION_TYPE]) -> None:
+        """Add a dictionary of functions to the plugin."""
+        for name, function in functions.items():
+            self[name] = function
 
     def setdefault(self, key: str, value: KernelFunction | None = None):
         if key not in self.functions:
             if value is None:
                 raise ValueError("Value must be provided for new key.")
             self[key] = value
         return self[key]
 
-    def __iter__(self) -> Iterable[KernelFunction]:
-        for function in self.functions.values():
-            yield function
+    def __iter__(self) -> Generator[KernelFunction, None, None]:  # type: ignore
+        """Iterate over the functions in the plugin."""
+        yield from self.functions.values()
 
     def __contains__(self, key: str) -> bool:
         return key in self.functions
 
     # endregion
     # region Properties
 
-    def get_functions_metadata(self) -> list["KernelFunctionMetadata"]:
+    def get_functions_metadata(self) -> list[KernelFunctionMetadata]:
         """
         Get the metadata for the functions in the plugin.
 
         Returns:
             A list of KernelFunctionMetadata instances.
         """
         return [func.metadata for func in self]
 
     # endregion
     # region Class Methods
 
     @classmethod
     def from_object(
         cls, plugin_name: str, plugin_instance: Any | dict[str, Any], description: str | None = None
-    ) -> "KernelPlugin":
+    ) -> KernelPlugin:
         """
         Creates a plugin that wraps the specified target object and imports it into the kernel's plugin collection
 
         Args:
             plugin_instance (Any | dict[str, Any]): The plugin instance. This can be a custom class or a
                 dictionary of classes that contains methods with the kernel_function decorator for one or
                 several methods. See `TextMemoryPlugin` as an example.
@@ -250,15 +256,15 @@
     @classmethod
     def from_directory(
         cls,
         plugin_name: str,
         parent_directory: str,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
-    ) -> "KernelPlugin":
+    ) -> KernelPlugin:
         """Create a plugin from a specified directory.
 
         This method does not recurse into subdirectories beyond one level deep from the specified plugin directory.
         For YAML files, function names are extracted from the content of the YAML files themselves (the name property).
         For directories, the function name is assumed to be the name of the directory. Each KernelFunction object is
         initialized with data parsed from the associated files and added to a list of functions that are then assigned
         to the created KernelPlugin object.
@@ -311,15 +317,15 @@
                 if os.path.basename(object).startswith("__"):
                     continue
                 try:
                     functions.append(KernelFunctionFromPrompt.from_directory(path=object))
                 except FunctionInitializationError:
                     logger.warning(f"Failed to create function from directory: {object}")
             elif object.endswith(".yaml") or object.endswith(".yml"):
-                with open(object, "r") as file:
+                with open(object) as file:
                     try:
                         functions.append(KernelFunctionFromPrompt.from_yaml(file.read()))
                     except FunctionInitializationError:
                         logger.warning(f"Failed to create function from YAML file: {object}")
             elif object.endswith(".py"):
                 try:
                     functions.extend(
@@ -332,24 +338,24 @@
                     )
                 except PluginInitializationError:
                     logger.warning(f"Failed to create function from Python file: {object}")
             else:
                 logger.warning(f"Unknown file found: {object}")
         if not functions:
             raise PluginInitializationError(f"No functions found in folder: {parent_directory}/{plugin_name}")
-        return cls(name=plugin_name, description=description, functions=functions)
+        return cls(name=plugin_name, description=description, functions=functions)  # type: ignore
 
     @classmethod
     def from_openapi(
         cls,
         plugin_name: str,
         openapi_document_path: str,
-        execution_settings: "OpenAPIFunctionExecutionParameters | None" = None,
+        execution_settings: OpenAPIFunctionExecutionParameters | None = None,
         description: str | None = None,
-    ) -> "KernelPlugin":
+    ) -> KernelPlugin:
         """Create a plugin from an OpenAPI document.
 
         Args:
             plugin_name (str): The name of the plugin
             plugin_url (str | None): The URL of the plugin
             plugin_str (str | None): The JSON string of the plugin
             execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
@@ -361,33 +367,33 @@
         Raises:
             PluginInitializationError: if the plugin URL or plugin JSON/YAML is not provided
         """
 
         if not openapi_document_path:
             raise PluginInitializationError("OpenAPI document path is required.")
 
-        return cls(
+        return cls(  # type: ignore
             name=plugin_name,
             description=description,
-            functions=create_functions_from_openapi(
+            functions=create_functions_from_openapi(  # type: ignore
                 plugin_name=plugin_name,
                 openapi_document_path=openapi_document_path,
                 execution_settings=execution_settings,
             ),
         )
 
     @classmethod
     async def from_openai(
         cls,
         plugin_name: str,
         plugin_url: str | None = None,
         plugin_str: str | None = None,
         execution_parameters: OpenAIFunctionExecutionParameters | None = None,
         description: str | None = None,
-    ) -> "KernelPlugin":
+    ) -> KernelPlugin:
         """Create a plugin from the Open AI manifest.
 
         Args:
             plugin_name (str): The name of the plugin
             plugin_url (str | None): The URL of the plugin
             plugin_str (str | None): The JSON string of the plugin
             execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
@@ -429,33 +435,36 @@
                 return await initial_auth_callback(plugin_name, openai_auth_config, **kwargs)  # pragma: no cover
 
             execution_parameters.auth_callback = custom_auth_callback
 
         return cls(
             name=plugin_name,
             description=description,
-            functions=create_functions_from_openapi(
+            functions=create_functions_from_openapi(  # type: ignore
                 plugin_name=plugin_name,
                 openapi_document_path=openapi_spec_url,
                 execution_settings=execution_parameters,
             ),
         )
 
     @classmethod
     def from_python_file(
         cls,
         plugin_name: str,
         py_file: str,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
-    ) -> "KernelPlugin":
+    ) -> KernelPlugin:
         module_name = os.path.basename(py_file).replace(".py", "")
         spec = importlib.util.spec_from_file_location(module_name, py_file)
+        if not spec:
+            raise PluginInitializationError(f"Could not load spec from file {py_file}")
         module = importlib.util.module_from_spec(spec)
-        assert spec.loader
+        if not module or not spec.loader:
+            raise PluginInitializationError(f"No module found in file {py_file}")
         spec.loader.exec_module(module)
 
         for name, cls_instance in inspect.getmembers(module, inspect.isclass):
             if cls_instance.__module__ != module_name:
                 continue
             instance = getattr(module, name)(**class_init_arguments.get(name, {}) if class_init_arguments else {})
             return cls.from_object(plugin_name=plugin_name, description=description, plugin_instance=instance)
@@ -486,21 +495,21 @@
             }
         if isinstance(functions, KernelPlugin):
             return {
                 name: function.function_copy(plugin_name=plugin_name) for name, function in functions.functions.items()
             }
         if isinstance(functions, KernelFunction):
             return {functions.name: KernelPlugin._parse_or_copy(function=functions, plugin_name=plugin_name)}
-        if isinstance(functions, Callable):
+        if callable(functions):
             function = KernelPlugin._parse_or_copy(function=functions, plugin_name=plugin_name)
             return {function.name: function}
         if isinstance(functions, list):
             functions_dict: dict[str, KernelFunction] = {}
-            for function in functions:
-                if isinstance(function, (KernelFunction, Callable)):
+            for function in functions:  # type: ignore
+                if isinstance(function, KernelFunction) or callable(function):
                     function = KernelPlugin._parse_or_copy(function=function, plugin_name=plugin_name)
                     functions_dict[function.name] = function
                 elif isinstance(function, KernelPlugin):  # type: ignore
                     functions_dict.update(
                         {
                             name: KernelPlugin._parse_or_copy(function=function, plugin_name=plugin_name)
                             for name, function in function.functions.items()
@@ -512,12 +521,12 @@
         raise ValueError(f"Invalid type for supplied functions: {functions} (type: {type(functions)})")
 
     @staticmethod
     def _parse_or_copy(function: KERNEL_FUNCTION_TYPE, plugin_name: str) -> KernelFunction:
         """Handle the function and return a KernelFunction instance."""
         if isinstance(function, KernelFunction):
             return function.function_copy(plugin_name=plugin_name)
-        if isinstance(function, Callable):
+        if callable(function):
             return KernelFunctionFromMethod(method=function, plugin_name=plugin_name)
         raise ValueError(f"Invalid type for function: {function} (type: {type(function)})")
 
     # endregion
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-0.9.7b1/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
-from typing import Any, Optional
+from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
@@ -16,8 +17,8 @@
         rendered_prompt (str): The rendered prompt.
         ai_service (Any): The AI service that rendered the prompt.
         prompt_template (PromptTemplateConfig): The prompt template used to render the prompt.
     """
 
     rendered_prompt: str
     ai_service: Any
-    execution_settings: Optional[PromptExecutionSettings] = Field(default_factory=PromptExecutionSettings)
+    execution_settings: PromptExecutionSettings | None = Field(default_factory=PromptExecutionSettings)
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/kernel.py` & `semantic_kernel-0.9.7b1/semantic_kernel/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from copy import copy
-from typing import TYPE_CHECKING, Any, AsyncIterable, Callable, Literal, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, Callable, Literal, Type, TypeVar, Union
 
 from pydantic import Field, field_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.events import FunctionInvokedEventArgs, FunctionInvokingEventArgs
 from semantic_kernel.exceptions import (
@@ -146,15 +146,15 @@
         self,
         function: "KernelFunction" | None = None,
         arguments: KernelArguments | None = None,
         function_name: str | None = None,
         plugin_name: str | None = None,
         return_function_results: bool | None = False,
         **kwargs: Any,
-    ) -> AsyncIterable[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult]]:
+    ) -> AsyncGenerator[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult], Any]:
         """Execute one or more stream functions.
 
         This will execute the functions in the order they are provided, if a list of functions is provided.
         When multiple functions are provided only the last one is streamed, the rest is executed as a pipeline.
 
         Arguments:
             functions (KernelFunction): The function or functions to execute,
@@ -342,14 +342,80 @@
             function_name=function_name,
             plugin_name=plugin_name,
             prompt=prompt,
             template_format=template_format,
         )
         return await self.invoke(function=function, arguments=arguments)
 
+    async def invoke_prompt_stream(
+        self,
+        function_name: str,
+        plugin_name: str,
+        prompt: str,
+        arguments: KernelArguments | None = None,
+        template_format: Literal[
+            "semantic-kernel",
+            "handlebars",
+            "jinja2",
+        ] = KERNEL_TEMPLATE_FORMAT_NAME,
+        return_function_results: bool | None = False,
+        **kwargs: Any,
+    ) -> AsyncIterable[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult]]:
+        """
+        Invoke a function from the provided prompt and stream the results
+
+        Args:
+            function_name (str): The name of the function
+            plugin_name (str): The name of the plugin
+            prompt (str): The prompt to use
+            arguments (KernelArguments | None): The arguments to pass to the function(s), optional
+            template_format (str | None): The format of the prompt template
+            kwargs (dict[str, Any]): arguments that can be used instead of supplying KernelArguments
+
+        Returns:
+            AsyncIterable[StreamingContentMixin]: The content of the stream of the last function provided.
+        """
+        if not arguments:
+            arguments = KernelArguments(**kwargs)
+        if not prompt:
+            raise TemplateSyntaxError("The prompt is either null or empty.")
+
+        from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
+
+        function = KernelFunctionFromPrompt(
+            function_name=function_name,
+            plugin_name=plugin_name,
+            prompt=prompt,
+            template_format=template_format,
+        )
+
+        function_result: list[list["StreamingContentMixin"] | Any] = []
+
+        async for stream_message in self.invoke_stream(function=function, arguments=arguments):
+            if isinstance(stream_message, FunctionResult) and (
+                exception := stream_message.metadata.get("exception", None)
+            ):
+                raise KernelInvokeException(
+                    f"Error occurred while invoking function: '{function.fully_qualified_name}'"
+                ) from exception
+            function_result.append(stream_message)
+            yield stream_message
+
+        if return_function_results:
+            output_function_result: list["StreamingContentMixin"] = []
+            for result in function_result:
+                for choice in result:
+                    if not isinstance(choice, StreamingContentMixin):
+                        continue
+                    if len(output_function_result) <= choice.choice_index:
+                        output_function_result.append(copy(choice))
+                    else:
+                        output_function_result[choice.choice_index] += choice
+            yield FunctionResult(function=function.metadata, value=output_function_result)
+
     # endregion
     # region Function Invoking/Invoked Events
 
     def on_function_invoked(
         self,
         kernel_function_metadata: KernelFunctionMetadata,
         arguments: KernelArguments,
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/kernel_pydantic.py` & `semantic_kernel-0.9.7b1/semantic_kernel/kernel_pydantic.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import PrivateAttr
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
@@ -34,14 +34,15 @@
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
         description: Optional[str] = None,
         additional_metadata: Optional[str] = None,
+        embeddings_kwargs: Optional[Dict[str, Any]] = {},
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the information to.
             text {str} -- The text to save.
             id {str} -- The id of the information.
@@ -50,15 +51,15 @@
         Returns:
             None -- None.
         """
         # TODO: not the best place to create collection, but will address this behavior together with .NET SK
         if not await self._storage.does_collection_exist(collection_name=collection):
             await self._storage.create_collection(collection_name=collection)
 
-        embedding = (await self._embeddings_generator.generate_embeddings([text]))[0]
+        embedding = (await self._embeddings_generator.generate_embeddings([text], **embeddings_kwargs))[0]
         data = MemoryRecord.local_record(
             id=id,
             text=text,
             description=description,
             additional_metadata=additional_metadata,
             embedding=embedding,
         )
@@ -69,14 +70,15 @@
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: Optional[str] = None,
         additional_metadata: Optional[str] = None,
+        embeddings_kwargs: Optional[Dict[str, Any]] = {},
     ) -> None:
         """Save a reference to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the reference to.
             text {str} -- The text to save.
             external_id {str} -- The external id of the reference.
@@ -86,15 +88,15 @@
         Returns:
             None -- None.
         """
         # TODO: not the best place to create collection, but will address this behavior together with .NET SK
         if not await self._storage.does_collection_exist(collection_name=collection):
             await self._storage.create_collection(collection_name=collection)
 
-        embedding = (await self._embeddings_generator.generate_embeddings([text]))[0]
+        embedding = (await self._embeddings_generator.generate_embeddings([text], **embeddings_kwargs))[0]
         data = MemoryRecord.reference_record(
             external_id=external_id,
             source_name=external_source_name,
             description=description,
             additional_metadata=additional_metadata,
             embedding=embedding,
         )
@@ -121,28 +123,29 @@
     async def search(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
+        embeddings_kwargs: Optional[Dict[str, Any]] = {},
     ) -> List[MemoryQueryResult]:
         """Search the memory (calls the memory store's get_nearest_matches method).
 
         Arguments:
             collection {str} -- The collection to search in.
             query {str} -- The query to search for.
             limit {int} -- The maximum number of results to return. (default: {1})
             min_relevance_score {float} -- The minimum relevance score to return. (default: {0.0})
             with_embeddings {bool} -- Whether to return the embeddings of the results. (default: {False})
 
         Returns:
             List[MemoryQueryResult] -- The list of MemoryQueryResult found.
         """
-        query_embedding = (await self._embeddings_generator.generate_embeddings([query]))[0]
+        query_embedding = (await self._embeddings_generator.generate_embeddings([query], **embeddings_kwargs))[0]
         results = await self._storage.get_nearest_matches(
             collection_name=collection,
             embedding=query_embedding,
             limit=limit,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embeddings,
         )
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import abstractmethod
-from typing import List, Optional, TypeVar
+from typing import Any, Dict, List, Optional, TypeVar
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 
 SemanticTextMemoryT = TypeVar("SemanticTextMemoryT", bound="SemanticTextMemoryBase")
 
 
@@ -14,14 +14,15 @@
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
         description: Optional[str] = None,
         additional_metadata: Optional[str] = None,
+        embeddings_kwargs: Optional[Dict[str, Any]] = None,
         # TODO: ctoken?
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the information to.
             text {str} -- The text to save.
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.9.7b1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/action_planner/action_planner.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/action_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/basic_planner.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.azure_chat_completion import AzureChatCompletion
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion import OpenAIChatCompletion
 from semantic_kernel.connectors.ai.open_ai.utils import get_function_calling_object, get_tool_call_object
 from semantic_kernel.contents.chat_history import ChatHistory
+from semantic_kernel.contents.function_call_content import FunctionCallContent
 from semantic_kernel.exceptions.planner_exceptions import PlannerInvalidConfigurationError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner_options import (
     FunctionCallingStepwisePlannerOptions,
@@ -155,21 +156,25 @@
                 chat_history=chat_history_for_steps,
                 settings=prompt_execution_settings,
                 kernel=cloned_kernel,
             )
             chat_result = chat_result[0]
             chat_history_for_steps.add_message(chat_result)
 
-            if not chat_result.tool_calls:
+            if not any(isinstance(item, FunctionCallContent) for item in chat_result.items):
                 chat_history_for_steps.add_user_message("That function call is invalid. Try something else!")
                 continue
 
             # Try to get the final answer out
-            if chat_result.tool_calls[0].function.name == USER_INTERACTION_SEND_FINAL_ANSWER:
-                args = chat_result.tool_calls[0].function.parse_arguments()
+            if (
+                chat_result.items[0]
+                and isinstance(chat_result.items[0], FunctionCallContent)
+                and chat_result.items[0].name == USER_INTERACTION_SEND_FINAL_ANSWER
+            ):
+                args = chat_result.items[0].parse_arguments()
                 answer = args["answer"]
                 return FunctionCallingStepwisePlannerResult(
                     final_answer=answer,
                     chat_history=chat_history_for_steps,
                     iterations=i + 1,
                 )
 
@@ -205,15 +210,15 @@
         arguments.update(additional_arguments)
         kernel_prompt_template = KernelPromptTemplate(
             prompt_template_config=PromptTemplateConfig(
                 template=self.step_prompt,
             )
         )
         prompt = await kernel_prompt_template.render(kernel, arguments)
-        chat_history = ChatHistory.from_rendered_prompt(prompt, service.get_chat_message_content_type())
+        chat_history = ChatHistory.from_rendered_prompt(prompt)
         return chat_history
 
     def _create_config_from_yaml(self, kernel: Kernel) -> "KernelFunction":
         """A temporary method to create a function from the yaml file.
         The yaml.safe_load will be replaced with the proper kernel
         method later."""
         data = yaml.safe_load(self.generate_plan_yaml)
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/plan.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py` & `semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/const.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import Literal, get_args
 
 KERNEL_TEMPLATE_FORMAT_NAME_TYPE = Literal["semantic-kernel"]
-KERNEL_TEMPLATE_FORMAT_NAME = get_args(KERNEL_TEMPLATE_FORMAT_NAME_TYPE)[0]
+KERNEL_TEMPLATE_FORMAT_NAME: KERNEL_TEMPLATE_FORMAT_NAME_TYPE = get_args(KERNEL_TEMPLATE_FORMAT_NAME_TYPE)[0]
 HANDLEBARS_TEMPLATE_FORMAT_NAME_TYPE = Literal["handlebars"]
-HANDLEBARS_TEMPLATE_FORMAT_NAME = get_args(HANDLEBARS_TEMPLATE_FORMAT_NAME_TYPE)[0]
+HANDLEBARS_TEMPLATE_FORMAT_NAME: HANDLEBARS_TEMPLATE_FORMAT_NAME_TYPE = get_args(HANDLEBARS_TEMPLATE_FORMAT_NAME_TYPE)[
+    0
+]
 JINJA2_TEMPLATE_FORMAT_NAME_TYPE = Literal["jinja2"]
-JINJA2_TEMPLATE_FORMAT_NAME = get_args(JINJA2_TEMPLATE_FORMAT_NAME_TYPE)[0]
+JINJA2_TEMPLATE_FORMAT_NAME: JINJA2_TEMPLATE_FORMAT_NAME_TYPE = get_args(JINJA2_TEMPLATE_FORMAT_NAME_TYPE)[0]
 
 TEMPLATE_FORMAT_TYPES = Literal[
     KERNEL_TEMPLATE_FORMAT_NAME_TYPE, HANDLEBARS_TEMPLATE_FORMAT_NAME_TYPE, JINJA2_TEMPLATE_FORMAT_NAME_TYPE
 ]
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 
 import json
 import logging
 import re
 from enum import Enum
 from typing import Callable, Dict
 
-from semantic_kernel.contents.chat_history import ROOT_KEY_MESSAGE, ChatHistory
-from semantic_kernel.contents.chat_message_content import ChatMessageContent
-
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _messages(this, options, *args, **kwargs):
+    from semantic_kernel.contents.chat_history import ChatHistory
+
     if not isinstance(this.context["chat_history"], ChatHistory):
         return ""
     return str(this.context["chat_history"])
 
 
 def _message_to_prompt(this, *args, **kwargs):
+    from semantic_kernel.contents.chat_message_content import ChatMessageContent
+
     if isinstance(this.context, ChatMessageContent):
-        return str(this.context.to_prompt(ROOT_KEY_MESSAGE))
+        return str(this.context.to_prompt())
     return str(this.context)
 
 
 def _message(this, options, *args, **kwargs):
+    from semantic_kernel.contents.const import CHAT_MESSAGE_CONTENT_TAG
+
     # everything in kwargs, goes to <ROOT_KEY_MESSAGE kwargs_key="kwargs_value">
     # everything in options, goes in between <ROOT_KEY_MESSAGE>options</ROOT_KEY_MESSAGE>
-    start = f"<{ROOT_KEY_MESSAGE}"
+    start = f"<{CHAT_MESSAGE_CONTENT_TAG}"
     for key, value in kwargs.items():
         if isinstance(value, Enum):
             value = value.value
         if value is not None:
             start += f' {key}="{value}"'
     start += ">"
-    end = f"</{ROOT_KEY_MESSAGE}>"
+    end = f"</{CHAT_MESSAGE_CONTENT_TAG}>"
     try:
         content = options["fn"](this)
     except Exception:
         content = ""
     return f"{start}{content}{end}"
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import re
 from enum import Enum
 from typing import Callable, Dict
 
-from semantic_kernel.contents.chat_history import ROOT_KEY_MESSAGE, ChatHistory
-from semantic_kernel.contents.chat_message_content import ChatMessageContent
-
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _messages(chat_history):
+    from semantic_kernel.contents.chat_history import ChatHistory
+
     if not isinstance(chat_history, ChatHistory):
         return ""
     return str(chat_history)
 
 
 def _message_to_prompt(context):
+    from semantic_kernel.contents.chat_message_content import ChatMessageContent
+
     if isinstance(context, ChatMessageContent):
-        return str(context.to_prompt(ROOT_KEY_MESSAGE))
+        return str(context.to_prompt())
     return str(context)
 
 
 def _message(item):
-    start = f"<{ROOT_KEY_MESSAGE}"
+    from semantic_kernel.contents.const import CHAT_MESSAGE_CONTENT_TAG
+
+    start = f"<{CHAT_MESSAGE_CONTENT_TAG}"
     role = item.role
     content = item.content
     if isinstance(role, Enum):
         role = role.value
     start += f' role="{role}"'
     start += ">"
-    end = f"</{ROOT_KEY_MESSAGE}>"
+    end = f"</{CHAT_MESSAGE_CONTENT_TAG}>"
     return f"{start}{content}{end}"
 
 
 # Wrap the _get function to safely handle calls without arguments
 def _safe_get_wrapper(context=None, name=None, default=""):
     if context is None or name is None:
         return default
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.9.7b1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_selector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.9.7b1/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.9.7b1/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/utils/naming.py` & `semantic_kernel-0.9.7b1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/utils/null_logger.py` & `semantic_kernel-0.9.7b1/semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/utils/settings.py` & `semantic_kernel-0.9.7b1/semantic_kernel/utils/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Dict, Optional, Tuple, Union
+from __future__ import annotations
+
+from typing import Optional, Tuple, Union
 
 from dotenv import dotenv_values
 
 
 def openai_settings_from_dot_env() -> Tuple[str, Optional[str]]:
     """
     Reads the OpenAI API key and organization ID from the .env file.
@@ -58,20 +60,20 @@
     if include_api_version:
         return deployment or "", api_key, endpoint, api_version or ""
     return deployment or "", api_key, endpoint
 
 
 def azure_openai_settings_from_dot_env_as_dict(
     include_deployment: bool = True, include_api_version: bool = False
-) -> Dict[str, str]:
+) -> dict[str, str]:
     """
     Reads the Azure OpenAI API key and endpoint from the .env file.
 
     Returns:
-        Dict[str, str]: The deployment name (or empty), Azure OpenAI API key,
+        dict[str, str]: The deployment name (or empty), Azure OpenAI API key,
         endpoint and api version (or empty)
     """
     (
         deployment_name,
         api_key,
         endpoint,
         api_version,
@@ -283,20 +285,20 @@
         return api_key, url
     else:
         index_name = config.get("AZURE_AISEARCH_INDEX_NAME", None)
         assert index_name is not None, "Azure AI Search index name not found in .env file"
         return api_key, url, index_name
 
 
-def azure_aisearch_settings_from_dot_env_as_dict() -> Dict[str, str]:
+def azure_aisearch_settings_from_dot_env_as_dict() -> dict[str, str]:
     """
     Reads the Azure AI Search environment variables including index name from the .env file.
 
     Returns:
-        Dict[str, str]: the Azure AI search environment variables
+        dict[str, str]: the Azure AI search environment variables
     """
     api_key, url, index_name = azure_aisearch_settings_from_dot_env(include_index_name=True)
     return {"authentication": {"type": "api_key", "key": api_key}, "endpoint": url, "index_name": index_name}
 
 
 def azure_key_vault_settings_from_dot_env(
     include_client_id: bool = True, include_client_secret: bool = True
@@ -319,16 +321,46 @@
         assert client_secret is not None, "Azure Key Vault client secret not found in .env file"
 
     if include_client_id and include_client_secret:
         return endpoint, client_id, client_secret
     return endpoint, client_id
 
 
-def azure_key_vault_settings_from_dot_env_as_dict() -> Dict[str, str]:
+def azure_key_vault_settings_from_dot_env_as_dict() -> dict[str, str]:
     """
     Reads the Azure Key Vault environment variables for the .env file.
 
     Returns:
-        Dict[str, str]: Azure Key Vault environment variables
+        dict[str, str]: Azure Key Vault environment variables
     """
     endpoint, client_id, client_secret = azure_key_vault_settings_from_dot_env()
     return {"endpoint": endpoint, "client_id": client_id, "client_secret": client_secret}
+
+
+def booking_sample_settings_from_dot_env() -> Tuple[str, str, str]:
+    """
+    Reads the Booking Sample environment variables for the .env file.
+
+    Returns:
+        Tuple[str, str]: Booking Sample environment variables
+    """
+    config = dotenv_values(".env")
+    client_id = config.get("BOOKING_SAMPLE_CLIENT_ID", None)
+    tenant_id = config.get("BOOKING_SAMPLE_TENANT_ID", None)
+    client_secret = config.get("BOOKING_SAMPLE_CLIENT_SECRET", None)
+
+    assert client_id, "Booking Sample Client ID not found in .env file"
+    assert tenant_id, "Booking Sample Tenant ID not found in .env file"
+    assert client_secret, "Booking Sample Client Secret not found in .env file"
+
+    return client_id, tenant_id, client_secret
+
+
+def booking_sample_settings_from_dot_env_as_dict() -> dict[str, str]:
+    """
+    Reads the Booking Sample environment variables for the .env file.
+
+    Returns:
+        dict[str, str]: Booking Sample environment variables
+    """
+    client_id, tenant_id, client_secret = booking_sample_settings_from_dot_env()
+    return {"client_id": client_id, "tenant_id": tenant_id, "client_secret": client_secret}
```

### Comparing `semantic_kernel-0.9.6b1/semantic_kernel/utils/validation.py` & `semantic_kernel-0.9.7b1/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.6b1/PKG-INFO` & `semantic_kernel-0.9.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.9.6b1
+Version: 0.9.7b1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
-Requires-Python: >=3.8,<3.13
+Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: chromadb
 Provides-Extra: google
```

