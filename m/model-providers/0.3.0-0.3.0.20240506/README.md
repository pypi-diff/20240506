# Comparing `tmp/model_providers-0.3.0.tar.gz` & `tmp/model_providers-0.3.0.20240506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_providers-0.3.0.tar", max compression
+gzip compressed data, was "model_providers-0.3.0.20240506.tar", max compression
```

## Comparing `model_providers-0.3.0.tar` & `model_providers-0.3.0.20240506.tar`

### file list

```diff
@@ -1,457 +1,443 @@
--rw-r--r--   0        0        0     3116 2024-04-15 10:42:33.446241 model_providers-0.3.0/model_providers/__init__.py
--rw-r--r--   0        0        0     1330 2024-04-23 02:42:28.146930 model_providers-0.3.0/model_providers/__main__.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.212454 model_providers-0.3.0/model_providers/bootstrap_web/entities/__init__.py
--rw-r--r--   0        0        0     5340 2024-04-23 02:42:28.174367 model_providers-0.3.0/model_providers/bootstrap_web/entities/model_provider_entities.py
--rw-r--r--   0        0        0      318 2024-04-15 07:06:42.233652 model_providers-0.3.0/model_providers/bootstrap_web/message_convert/__init__.py
--rw-r--r--   0        0        0     9580 2024-04-15 07:06:42.233652 model_providers-0.3.0/model_providers/bootstrap_web/message_convert/core.py
--rw-r--r--   0        0        0    11025 2024-04-23 02:42:28.190582 model_providers-0.3.0/model_providers/bootstrap_web/openai_bootstrap_web.py
--rw-r--r--   0        0        0      251 2024-04-15 07:06:42.257190 model_providers-0.3.0/model_providers/core/bootstrap/__init__.py
--rw-r--r--   0        0        0     1679 2024-04-15 07:06:42.263361 model_providers-0.3.0/model_providers/core/bootstrap/base.py
--rw-r--r--   0        0        0     1256 2024-04-15 07:06:42.264364 model_providers-0.3.0/model_providers/core/bootstrap/bootstrap_register.py
--rw-r--r--   0        0        0     5260 2024-04-23 02:42:28.216148 model_providers-0.3.0/model_providers/core/bootstrap/openai_protocol.py
--rw-r--r--   0        0        0     5877 2024-04-23 02:42:28.237263 model_providers-0.3.0/model_providers/core/bootstrap/providers_wapper.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.280027 model_providers-0.3.0/model_providers/core/entities/__init__.py
--rw-r--r--   0        0        0      166 2024-04-15 07:06:42.280027 model_providers-0.3.0/model_providers/core/entities/agent_entities.py
--rw-r--r--   0        0        0     7484 2024-04-23 02:42:28.258651 model_providers-0.3.0/model_providers/core/entities/application_entities.py
--rw-r--r--   0        0        0     5777 2024-04-23 02:42:28.279127 model_providers-0.3.0/model_providers/core/entities/message_entities.py
--rw-r--r--   0        0        0     1895 2024-04-23 02:42:28.295180 model_providers-0.3.0/model_providers/core/entities/model_entities.py
--rw-r--r--   0        0        0    11780 2024-04-23 02:42:28.317488 model_providers-0.3.0/model_providers/core/entities/provider_configuration.py
--rw-r--r--   0        0        0     2361 2024-04-23 02:42:28.343443 model_providers-0.3.0/model_providers/core/entities/provider_entities.py
--rw-r--r--   0        0        0     2727 2024-04-23 02:42:28.360534 model_providers-0.3.0/model_providers/core/entities/queue_entities.py
--rw-r--r--   0        0        0    10489 2024-04-23 02:42:28.375130 model_providers-0.3.0/model_providers/core/model_manager.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.328344 model_providers-0.3.0/model_providers/core/model_runtime/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.344010 model_providers-0.3.0/model_providers/core/model_runtime/callbacks/__init__.py
--rw-r--r--   0        0        0     4617 2024-04-23 02:42:28.433240 model_providers-0.3.0/model_providers/core/model_runtime/callbacks/base_callback.py
--rw-r--r--   0        0        0     6100 2024-04-23 02:42:28.460277 model_providers-0.3.0/model_providers/core/model_runtime/callbacks/logging_callback.py
--rw-r--r--   0        0        0   379070 2024-04-15 07:06:42.391497 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/images/index/image-20231210143654461.png
--rw-r--r--   0        0        0   115258 2024-04-15 07:06:42.391497 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/images/index/image-20231210144229650.png
--rw-r--r--   0        0        0   111420 2024-04-15 07:06:42.409146 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/images/index/image-20231210144814617.png
--rw-r--r--   0        0        0    71354 2024-04-15 07:06:42.409146 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/images/index/image-20231210151548521.png
--rw-r--r--   0        0        0    76990 2024-04-15 07:06:42.428164 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/images/index/image-20231210151628992.png
--rw-r--r--   0        0        0   554357 2024-04-15 07:06:42.440186 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/images/index/image-20231210165243632.png
--rw-r--r--   0        0        0    21453 2024-04-23 02:42:28.510100 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/interfaces.md
--rw-r--r--   0        0        0    12030 2024-04-23 02:42:28.529913 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/provider_scale_out.md
--rw-r--r--   0        0        0     9330 2024-04-15 07:06:42.455953 model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/schema.md
--rw-r--r--   0        0        0    10579 2024-04-23 02:42:28.562040 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/customizable_model_scale_out.md
--rw-r--r--   0        0        0   235102 2024-04-15 07:06:42.502606 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-1.png
--rw-r--r--   0        0        0   210087 2024-04-15 07:06:42.523688 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-2.png
--rw-r--r--   0        0        0   394062 2024-04-15 07:06:42.541362 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-20231210143654461.png
--rw-r--r--   0        0        0   115258 2024-04-15 07:06:42.549871 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-20231210144229650.png
--rw-r--r--   0        0        0   111420 2024-04-15 07:06:42.557097 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-20231210144814617.png
--rw-r--r--   0        0        0    71354 2024-04-15 07:06:42.567171 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-20231210151548521.png
--rw-r--r--   0        0        0    76990 2024-04-15 07:06:42.567171 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-20231210151628992.png
--rw-r--r--   0        0        0   554357 2024-04-15 07:06:42.581678 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-20231210165243632.png
--rw-r--r--   0        0        0    44778 2024-04-15 07:06:42.597934 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image-3.png
--rw-r--r--   0        0        0   267979 2024-04-15 07:06:42.602543 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/images/index/image.png
--rw-r--r--   0        0        0    21493 2024-04-23 02:42:28.588487 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/interfaces.md
--rw-r--r--   0        0        0     6890 2024-04-23 02:42:28.620487 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/predefined_model_scale_out.md
--rw-r--r--   0        0        0     8195 2024-04-15 07:06:42.630711 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/provider_scale_out.md
--rw-r--r--   0        0        0     8437 2024-04-15 07:06:42.630711 model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/schema.md
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.650331 model_providers-0.3.0/model_providers/core/model_runtime/entities/__init__.py
--rw-r--r--   0        0        0      323 2024-04-15 07:06:42.658889 model_providers-0.3.0/model_providers/core/model_runtime/entities/common_entities.py
--rw-r--r--   0        0        0     3673 2024-04-23 02:42:28.657669 model_providers-0.3.0/model_providers/core/model_runtime/entities/defaults.py
--rw-r--r--   0        0        0     2541 2024-04-23 02:42:28.693949 model_providers-0.3.0/model_providers/core/model_runtime/entities/llm_entities.py
--rw-r--r--   0        0        0     3473 2024-04-23 02:42:28.716981 model_providers-0.3.0/model_providers/core/model_runtime/entities/message_entities.py
--rw-r--r--   0        0        0     5479 2024-04-23 02:42:28.777721 model_providers-0.3.0/model_providers/core/model_runtime/entities/model_entities.py
--rw-r--r--   0        0        0     3624 2024-04-23 02:42:28.810476 model_providers-0.3.0/model_providers/core/model_runtime/entities/provider_entities.py
--rw-r--r--   0        0        0      322 2024-04-23 02:42:28.862220 model_providers-0.3.0/model_providers/core/model_runtime/entities/rerank_entities.py
--rw-r--r--   0        0        0      580 2024-04-23 02:42:28.930006 model_providers-0.3.0/model_providers/core/model_runtime/entities/text_embedding_entities.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.712407 model_providers-0.3.0/model_providers/core/model_runtime/errors/__init__.py
--rw-r--r--   0        0        0     1113 2024-04-15 07:06:42.712407 model_providers-0.3.0/model_providers/core/model_runtime/errors/invoke.py
--rw-r--r--   0        0        0      113 2024-04-15 07:06:42.729200 model_providers-0.3.0/model_providers/core/model_runtime/errors/validate.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.744215 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/__init__.py
--rw-r--r--   0        0        0    13961 2024-04-23 02:42:29.045772 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/ai_model.py
--rw-r--r--   0        0        0   218880 2024-04-15 07:06:42.759847 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/audio.mp3
--rw-r--r--   0        0        0    34387 2024-04-23 02:42:29.100627 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/large_language_model.py
--rw-r--r--   0        0        0     4980 2024-04-23 02:42:29.147324 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/model_provider.py
--rw-r--r--   0        0        0     1402 2024-04-15 07:06:42.775472 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/moderation_model.py
--rw-r--r--   0        0        0     2019 2024-04-23 02:42:29.171811 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/rerank_model.py
--rw-r--r--   0        0        0     1686 2024-04-15 07:06:42.791540 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/speech2text_model.py
--rw-r--r--   0        0        0     1597 2024-04-23 02:42:29.210641 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/text2img_model.py
--rw-r--r--   0        0        0     3077 2024-04-23 02:42:29.243336 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/text_embedding_model.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.815455 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/__init__.py
--rw-r--r--   0        0        0   456318 2024-04-15 07:06:42.828973 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/merges.txt
--rw-r--r--   0        0        0      438 2024-04-15 07:06:42.841002 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/special_tokens_map.json
--rw-r--r--   0        0        0      727 2024-04-15 07:06:42.843515 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/tokenizer_config.json
--rw-r--r--   0        0        0   999186 2024-04-15 07:06:42.860367 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/vocab.json
--rw-r--r--   0        0        0     1022 2024-04-15 07:06:42.863374 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2_tokenzier.py
--rw-r--r--   0        0        0     6864 2024-04-15 07:06:42.863374 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tts_model.py
--rw-r--r--   0        0        0      165 2024-04-15 07:06:42.863374 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__init__.py
--rw-r--r--   0        0        0      277 2024-04-15 07:06:42.874889 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/_position.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.887421 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/__init__.py
--rw-r--r--   0        0        0     5400 2024-04-15 07:06:42.890933 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/_assets/icon_l_en.svg
--rw-r--r--   0        0        0      410 2024-04-15 07:06:42.890933 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1202 2024-04-15 07:06:42.906566 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/anthropic.py
--rw-r--r--   0        0        0      981 2024-04-15 07:06:42.914667 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/anthropic.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.922688 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/__init__.py
--rw-r--r--   0        0        0      116 2024-04-15 07:06:42.929196 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/_position.yaml
--rw-r--r--   0        0        0      775 2024-04-15 07:06:42.938702 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.1.yaml
--rw-r--r--   0        0        0      788 2024-04-15 07:06:42.941558 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.yaml
--rw-r--r--   0        0        0      801 2024-04-15 07:06:42.941558 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-haiku-20240307.yaml
--rw-r--r--   0        0        0      801 2024-04-15 07:06:42.954569 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-opus-20240229.yaml
--rw-r--r--   0        0        0      804 2024-04-15 07:06:42.954569 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-sonnet-20240229.yaml
--rw-r--r--   0        0        0      766 2024-04-15 07:06:42.967293 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.2.yaml
--rw-r--r--   0        0        0      789 2024-04-15 07:06:42.970299 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.yaml
--rw-r--r--   0        0        0    21749 2024-04-23 02:42:29.292904 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:42.996249 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/__init__.py
--rw-r--r--   0        0        0     5007 2024-04-15 07:06:43.003243 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_assets/icon_l_en.png
--rw-r--r--   0        0        0      439 2024-04-15 07:06:43.003243 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1657 2024-04-23 02:42:29.325618 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_common.py
--rw-r--r--   0        0        0    29393 2024-04-15 07:06:43.022763 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_constant.py
--rw-r--r--   0        0        0      291 2024-04-15 07:06:43.022763 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/azure_openai.py
--rw-r--r--   0        0        0     4223 2024-04-15 07:06:43.029280 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/azure_openai.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.034287 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/llm/__init__.py
--rw-r--r--   0        0        0    29753 2024-04-23 02:42:29.356342 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.050214 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/speech2text/__init__.py
--rw-r--r--   0        0        0     3183 2024-04-15 07:06:43.066479 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/speech2text/speech2text.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.075626 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/text_embedding/__init__.py
--rw-r--r--   0        0        0     7870 2024-04-23 02:42:29.386812 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.091343 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/tts/__init__.py
--rw-r--r--   0        0        0     8820 2024-04-15 07:06:43.097355 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/tts/tts.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.097355 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/__init__.py
--rw-r--r--   0        0        0     4140 2024-04-15 07:06:43.117750 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_l_en.svg
--rw-r--r--   0        0        0      748 2024-04-15 07:06:43.117750 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1197 2024-04-15 07:06:43.130180 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/baichuan.py
--rw-r--r--   0        0        0      857 2024-04-15 07:06:43.130180 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/baichuan.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.145046 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/__init__.py
--rw-r--r--   0        0        0     1109 2024-04-15 07:06:43.145046 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-53b.yaml
--rw-r--r--   0        0        0     1127 2024-04-15 07:06:43.161470 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo-192k.yaml
--rw-r--r--   0        0        0     1117 2024-04-15 07:06:43.166691 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo.yaml
--rw-r--r--   0        0        0      870 2024-04-15 07:06:43.168699 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_tokenizer.py
--rw-r--r--   0        0        0     8828 2024-04-23 02:42:29.453435 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_turbo.py
--rw-r--r--   0        0        0      303 2024-04-15 07:06:43.177602 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_turbo_errors.py
--rw-r--r--   0        0        0     9597 2024-04-23 02:42:29.495408 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.193504 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/__init__.py
--rw-r--r--   0        0        0      113 2024-04-15 07:06:43.209320 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/baichuan-text-embedding.yaml
--rw-r--r--   0        0        0     7345 2024-04-23 02:42:29.560917 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.225576 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/__init__.py
--rw-r--r--   0        0        0    12612 2024-04-15 07:06:43.240588 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     3301 2024-04-15 07:06:43.240588 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1201 2024-04-15 07:06:43.240588 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/bedrock.py
--rw-r--r--   0        0        0     1918 2024-04-15 07:06:43.256221 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/bedrock.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.256221 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/__init__.py
--rw-r--r--   0        0        0      267 2024-04-15 07:06:43.275088 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/_position.yaml
--rw-r--r--   0        0        0      839 2024-04-15 07:06:43.275088 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-mid-v1.yaml
--rw-r--r--   0        0        0      843 2024-04-15 07:06:43.291831 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-ultra-v1.yaml
--rw-r--r--   0        0        0      473 2024-04-15 07:06:43.291831 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/amazon.titan-text-express-v1.yaml
--rw-r--r--   0        0        0      467 2024-04-15 07:06:43.291831 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/amazon.titan-text-lite-v1.yaml
--rw-r--r--   0        0        0      750 2024-04-15 07:06:43.308093 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-instant-v1.yaml
--rw-r--r--   0        0        0      734 2024-04-15 07:06:43.308093 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v1.yaml
--rw-r--r--   0        0        0      738 2024-04-15 07:06:43.322599 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.1.yaml
--rw-r--r--   0        0        0      734 2024-04-15 07:06:43.329610 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.yaml
--rw-r--r--   0        0        0      753 2024-04-15 07:06:43.329610 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-light-text-v14.yaml
--rw-r--r--   0        0        0      710 2024-04-15 07:06:43.339567 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-text-v14.yaml
--rw-r--r--   0        0        0    20697 2024-04-23 02:42:29.606192 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/llm.py
--rw-r--r--   0        0        0      434 2024-04-15 07:06:43.355207 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/meta.llama2-13b-chat-v1.yaml
--rw-r--r--   0        0        0      434 2024-04-15 07:06:43.355207 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/meta.llama2-70b-chat-v1.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.450235 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/__init__.py
--rw-r--r--   0        0        0     5500 2024-04-15 07:06:43.462064 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     1355 2024-04-15 07:06:43.466074 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1206 2024-04-15 07:06:43.466074 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/cohere.py
--rw-r--r--   0        0        0     1638 2024-04-15 07:06:43.481707 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/cohere.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.490934 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/__init__.py
--rw-r--r--   0        0        0      156 2024-04-15 07:06:43.497443 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/_position.yaml
--rw-r--r--   0        0        0     1762 2024-04-15 07:06:43.497443 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-chat.yaml
--rw-r--r--   0        0        0     1780 2024-04-15 07:06:43.497443 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-chat.yaml
--rw-r--r--   0        0        0     1804 2024-04-15 07:06:43.513079 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly-chat.yaml
--rw-r--r--   0        0        0      946 2024-04-15 07:06:43.517452 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly.yaml
--rw-r--r--   0        0        0      922 2024-04-15 07:06:43.517452 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light.yaml
--rw-r--r--   0        0        0     1786 2024-04-15 07:06:43.530086 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly-chat.yaml
--rw-r--r--   0        0        0      928 2024-04-15 07:06:43.530086 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly.yaml
--rw-r--r--   0        0        0      904 2024-04-15 07:06:43.530086 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command.yaml
--rw-r--r--   0        0        0    22098 2024-04-23 02:42:29.655320 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.544763 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/rerank/__init__.py
--rw-r--r--   0        0        0       85 2024-04-15 07:06:43.560937 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank-english-v2.0.yaml
--rw-r--r--   0        0        0       90 2024-04-15 07:06:43.570887 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank-multilingual-v2.0.yaml
--rw-r--r--   0        0        0     4003 2024-04-23 02:42:29.682325 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.576393 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/__init__.py
--rw-r--r--   0        0        0      180 2024-04-15 07:06:43.595037 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/_position.yaml
--rw-r--r--   0        0        0      174 2024-04-15 07:06:43.595037 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-light-v2.0.yaml
--rw-r--r--   0        0        0      173 2024-04-15 07:06:43.595037 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-light-v3.0.yaml
--rw-r--r--   0        0        0      168 2024-04-15 07:06:43.608045 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-v2.0.yaml
--rw-r--r--   0        0        0      168 2024-04-15 07:06:43.608045 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-v3.0.yaml
--rw-r--r--   0        0        0      178 2024-04-15 07:06:43.615673 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-multilingual-light-v3.0.yaml
--rw-r--r--   0        0        0      172 2024-04-15 07:06:43.623700 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-multilingual-v2.0.yaml
--rw-r--r--   0        0        0      173 2024-04-15 07:06:43.629710 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-multilingual-v3.0.yaml
--rw-r--r--   0        0        0     7533 2024-04-23 02:42:29.718393 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.639227 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/__init__.py
--rw-r--r--   0        0        0     3710 2024-04-15 07:06:43.644734 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/_assets/icon_l_en.svg
--rw-r--r--   0        0        0      689 2024-04-15 07:06:43.658699 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1185 2024-04-15 07:06:43.658699 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/google.py
--rw-r--r--   0        0        0      692 2024-04-15 07:06:43.674328 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/google.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.685039 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/__init__.py
--rw-r--r--   0        0        0      720 2024-04-15 07:06:43.690047 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro-vision.yaml
--rw-r--r--   0        0        0      773 2024-04-15 07:06:43.690047 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro.yaml
--rw-r--r--   0        0        0    17195 2024-04-23 02:42:29.750670 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.710129 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/__init__.py
--rw-r--r--   0        0        0     5889 2024-04-15 07:06:43.721637 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/_assets/icon_l_en.svg
--rw-r--r--   0        0        0      828 2024-04-15 07:06:43.731022 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1136 2024-04-15 07:06:43.736032 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/groq.py
--rw-r--r--   0        0        0      850 2024-04-15 07:06:43.738374 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/groq.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.738374 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/llm/__init__.py
--rw-r--r--   0        0        0      456 2024-04-15 07:06:43.757887 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/llm/llama2-70b-4096.yaml
--rw-r--r--   0        0        0     1352 2024-04-23 02:42:29.784592 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/llm/llm.py
--rw-r--r--   0        0        0      483 2024-04-15 07:06:43.769394 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/llm/mixtral-8x7b-instruct-v0.1.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.774708 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/__init__.py
--rw-r--r--   0        0        0    20353 2024-04-15 07:06:43.785225 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     9298 2024-04-15 07:06:43.785225 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_s_en.svg
--rw-r--r--   0        0        0      419 2024-04-23 02:42:29.815088 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/_common.py
--rw-r--r--   0        0        0      294 2024-04-15 07:06:43.802773 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/huggingface_hub.py
--rw-r--r--   0        0        0     2850 2024-04-15 07:06:43.802773 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/huggingface_hub.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.821951 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/llm/__init__.py
--rw-r--r--   0        0        0    13140 2024-04-23 02:42:29.847287 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.832429 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/text_embedding/__init__.py
--rw-r--r--   0        0        0     8640 2024-04-23 02:42:29.882551 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.856768 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/__init__.py
--rw-r--r--   0        0        0     1681 2024-04-15 07:06:43.867190 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/_assets/icon_l_en.svg
--rw-r--r--   0        0        0      566 2024-04-15 07:06:43.879735 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1309 2024-04-15 07:06:43.883251 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/jina.py
--rw-r--r--   0        0        0      668 2024-04-15 07:06:43.883251 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/jina.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.899751 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/rerank/__init__.py
--rw-r--r--   0        0        0       90 2024-04-15 07:06:43.899751 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/rerank/jina-reranker-v1-base-en.yaml
--rw-r--r--   0        0        0     4048 2024-04-23 02:42:29.919366 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/rerank/rerank.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.915702 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/__init__.py
--rw-r--r--   0        0        0      177 2024-04-15 07:06:43.915702 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-base-de.yaml
--rw-r--r--   0        0        0      177 2024-04-15 07:06:43.931537 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-base-en.yaml
--rw-r--r--   0        0        0      177 2024-04-15 07:06:43.935044 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-base-zh.yaml
--rw-r--r--   0        0        0      178 2024-04-15 07:06:43.935044 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-small-en.yaml
--rw-r--r--   0        0        0      950 2024-04-15 07:06:43.946052 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina_tokenizer.py
--rw-r--r--   0        0        0     5928 2024-04-23 02:42:29.951569 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/text_embedding.py
--rw-r--r--   0        0        0   711577 2024-04-15 07:06:43.961547 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/tokenizer/tokenizer.json
--rw-r--r--   0        0        0      373 2024-04-15 07:06:43.977216 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/tokenizer/tokenizer_config.json
--rw-r--r--   0        0        0        0 2024-04-15 07:06:43.993796 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/__init__.py
--rw-r--r--   0        0        0    77919 2024-04-15 07:06:43.993796 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/_assets/icon_l_en.svg
--rw-r--r--   0        0        0    74478 2024-04-15 07:06:44.014527 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/_assets/icon_s_en.svg
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.024550 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/llm/__init__.py
--rw-r--r--   0        0        0    25761 2024-04-23 02:42:29.989163 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/llm/llm.py
--rw-r--r--   0        0        0      287 2024-04-15 07:06:44.035246 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/localai.py
--rw-r--r--   0        0        0     1678 2024-04-15 07:06:44.040873 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/localai.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.040873 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/text_embedding/__init__.py
--rw-r--r--   0        0        0     7053 2024-04-23 02:42:30.031329 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.063633 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/__init__.py
--rw-r--r--   0        0        0     5767 2024-04-15 07:06:44.073813 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_l_en.png
--rw-r--r--   0        0        0     2007 2024-04-15 07:06:44.073813 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_s_en.png
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.091234 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/__init__.py
--rw-r--r--   0        0        0      564 2024-04-15 07:06:44.104101 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab5-chat.yaml
--rw-r--r--   0        0        0      851 2024-04-15 07:06:44.104101 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5-chat.yaml
--rw-r--r--   0        0        0      655 2024-04-15 07:06:44.110606 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5s-chat.yaml
--rw-r--r--   0        0        0      681 2024-04-15 07:06:44.119615 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab6-chat.yaml
--rw-r--r--   0        0        0     6398 2024-04-23 02:42:30.073704 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion.py
--rw-r--r--   0        0        0     8378 2024-04-23 02:42:30.101475 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion_pro.py
--rw-r--r--   0        0        0      308 2024-04-15 07:06:44.130528 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/errors.py
--rw-r--r--   0        0        0    12273 2024-04-23 02:42:30.136415 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/llm.py
--rw-r--r--   0        0        0      960 2024-04-23 02:42:30.164044 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/types.py
--rw-r--r--   0        0        0     1227 2024-04-15 07:06:44.151646 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/minimax.py
--rw-r--r--   0        0        0      894 2024-04-15 07:06:44.151646 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/minimax.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.169780 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/text_embedding/__init__.py
--rw-r--r--   0        0        0      156 2024-04-15 07:06:44.172787 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/text_embedding/embo-01.yaml
--rw-r--r--   0        0        0     6482 2024-04-23 02:42:30.196771 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.183298 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/__init__.py
--rw-r--r--   0        0        0     7064 2024-04-15 07:06:44.198468 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_l_en.png
--rw-r--r--   0        0        0     7418 2024-04-15 07:06:44.198468 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_s_en.png
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.214837 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/__init__.py
--rw-r--r--   0        0        0      108 2024-04-15 07:06:44.224065 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/_position.yaml
--rw-r--r--   0        0        0     1538 2024-04-23 02:42:30.228804 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/llm.py
--rw-r--r--   0        0        0     1179 2024-04-15 07:06:44.231090 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-large-latest.yaml
--rw-r--r--   0        0        0     1184 2024-04-15 07:06:44.231090 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-medium-latest.yaml
--rw-r--r--   0        0        0     1179 2024-04-15 07:06:44.246101 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-small-latest.yaml
--rw-r--r--   0        0        0     1167 2024-04-15 07:06:44.248607 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mistral-7b.yaml
--rw-r--r--   0        0        0     1172 2024-04-15 07:06:44.248607 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mixtral-8x7b.yaml
--rw-r--r--   0        0        0     1141 2024-04-15 07:06:44.248607 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/mistralai.py
--rw-r--r--   0        0        0      816 2024-04-15 07:06:44.262763 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/mistralai.yaml
--rw-r--r--   0        0        0    11866 2024-04-23 02:42:30.253223 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/model_provider_factory.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.280015 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/__init__.py
--rw-r--r--   0        0        0    13654 2024-04-15 07:06:44.281013 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_l_en.png
--rw-r--r--   0        0        0     7419 2024-04-15 07:06:44.296866 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_s_en.png
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.296866 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/__init__.py
--rw-r--r--   0        0        0       54 2024-04-15 07:06:44.313342 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/_position.yaml
--rw-r--r--   0        0        0     1513 2024-04-23 02:42:30.286210 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/llm.py
--rw-r--r--   0        0        0      461 2024-04-15 07:06:44.322080 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/moonshot-v1-128k.yaml
--rw-r--r--   0        0        0      458 2024-04-15 07:06:44.329253 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/moonshot-v1-32k.yaml
--rw-r--r--   0        0        0      452 2024-04-15 07:06:44.330765 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/moonshot-v1-8k.yaml
--rw-r--r--   0        0        0     1139 2024-04-15 07:06:44.330765 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/moonshot.py
--rw-r--r--   0        0        0      869 2024-04-15 07:06:44.341769 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/moonshot.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.344780 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/__init__.py
--rw-r--r--   0        0        0    12066 2024-04-15 07:06:44.361118 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     7922 2024-04-15 07:06:44.369530 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_s_en.svg
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.376536 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/llm/__init__.py
--rw-r--r--   0        0        0    27882 2024-04-23 02:42:30.323743 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/llm/llm.py
--rw-r--r--   0        0        0      501 2024-04-15 07:06:44.376536 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/ollama.py
--rw-r--r--   0        0        0     2426 2024-04-15 07:06:44.393176 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/ollama.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.393176 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/text_embedding/__init__.py
--rw-r--r--   0        0        0     7866 2024-04-23 02:42:30.356703 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.424774 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/__init__.py
--rw-r--r--   0        0        0     4773 2024-04-15 07:06:44.430779 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     7038 2024-04-15 07:06:44.444124 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     2149 2024-04-23 02:42:30.394244 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/_common.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.457158 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/__init__.py
--rw-r--r--   0        0        0      275 2024-04-15 07:06:44.464347 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/_position.yaml
--rw-r--r--   0        0        0      932 2024-04-15 07:06:44.469854 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0125.yaml
--rw-r--r--   0        0        0      692 2024-04-15 07:06:44.472874 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0613.yaml
--rw-r--r--   0        0        0      930 2024-04-15 07:06:44.472874 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-1106.yaml
--rw-r--r--   0        0        0      705 2024-04-15 07:06:44.487885 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k-0613.yaml
--rw-r--r--   0        0        0      690 2024-04-15 07:06:44.494173 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k.yaml
--rw-r--r--   0        0        0      655 2024-04-15 07:06:44.494173 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-instruct.yaml
--rw-r--r--   0        0        0      914 2024-04-15 07:06:44.504642 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo.yaml
--rw-r--r--   0        0        0     1631 2024-04-15 07:06:44.504642 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-0125-preview.yaml
--rw-r--r--   0        0        0     1631 2024-04-15 07:06:44.504642 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-1106-preview.yaml
--rw-r--r--   0        0        0     1604 2024-04-15 07:06:44.521083 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-32k.yaml
--rw-r--r--   0        0        0     1634 2024-04-15 07:06:44.521083 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-turbo-preview.yaml
--rw-r--r--   0        0        0     1589 2024-04-15 07:06:44.531094 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-vision-preview.yaml
--rw-r--r--   0        0        0     1590 2024-04-15 07:06:44.535603 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4.yaml
--rw-r--r--   0        0        0    42510 2024-04-23 02:42:30.424780 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/llm.py
--rw-r--r--   0        0        0      593 2024-04-15 07:06:44.552401 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/text-davinci-003.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.552401 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/moderation/__init__.py
--rw-r--r--   0        0        0     4301 2024-04-23 02:42:30.456083 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/moderation/moderation.py
--rw-r--r--   0        0        0      121 2024-04-15 07:06:44.578251 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/moderation/text-moderation-stable.yaml
--rw-r--r--   0        0        0     1274 2024-04-15 07:06:44.588609 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/openai.py
--rw-r--r--   0        0        0     2268 2024-04-15 07:06:44.595364 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/openai.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.611961 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/speech2text/__init__.py
--rw-r--r--   0        0        0     2100 2024-04-15 07:06:44.616157 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/speech2text/speech2text.py
--rw-r--r--   0        0        0      152 2024-04-15 07:06:44.616157 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/speech2text/whisper-1.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.630936 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/text_embedding/__init__.py
--rw-r--r--   0        0        0      173 2024-04-15 07:06:44.630936 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/text_embedding/text-embedding-3-large.yaml
--rw-r--r--   0        0        0      173 2024-04-15 07:06:44.646927 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/text_embedding/text-embedding-3-small.yaml
--rw-r--r--   0        0        0      172 2024-04-15 07:06:44.657161 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/text_embedding/text-embedding-ada-002.yaml
--rw-r--r--   0        0        0     7509 2024-04-23 02:42:30.490183 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.662673 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/__init__.py
--rw-r--r--   0        0        0     1007 2024-04-15 07:06:44.680178 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/tts-1-hd.yaml
--rw-r--r--   0        0        0      993 2024-04-15 07:06:44.682186 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/tts-1.yaml
--rw-r--r--   0        0        0     7747 2024-04-15 07:06:44.682186 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/tts.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.697847 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-23 02:42:30.523032 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/_common.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.715676 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/llm/__init__.py
--rw-r--r--   0        0        0    31259 2024-04-23 02:42:30.557398 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/llm/llm.py
--rw-r--r--   0        0        0      289 2024-04-15 07:06:44.717686 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/openai_api_compatible.py
--rw-r--r--   0        0        0     2881 2024-04-15 07:06:44.731238 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/openai_api_compatible.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.741748 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/text_embedding/__init__.py
--rw-r--r--   0        0        0     8038 2024-04-23 02:42:30.588254 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.746085 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/__init__.py
--rw-r--r--   0        0        0    11337 2024-04-15 07:06:44.766414 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     7299 2024-04-15 07:06:44.766414 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_s_en.svg
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.786690 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/llm/__init__.py
--rw-r--r--   0        0        0    10841 2024-04-23 02:42:30.624216 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/llm/llm.py
--rw-r--r--   0        0        0     7362 2024-04-23 02:42:30.653270 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/llm/openllm_generate.py
--rw-r--r--   0        0        0      308 2024-04-15 07:06:44.801200 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/llm/openllm_generate_errors.py
--rw-r--r--   0        0        0      287 2024-04-15 07:06:44.808707 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/openllm.py
--rw-r--r--   0        0        0      896 2024-04-15 07:06:44.810632 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/openllm.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.814138 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/text_embedding/__init__.py
--rw-r--r--   0        0        0     5542 2024-04-23 02:42:30.678010 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.836425 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-15 07:06:44.841057 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/_assets/icon_l_en.svg
--rw-r--r--   0        0        0      384 2024-04-15 07:06:44.856565 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/_assets/icon_s_en.svg
--rw-r--r--   0        0        0      403 2024-04-23 02:42:30.711492 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/_common.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.872802 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/llm/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-23 02:42:30.732906 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/llm/llm.py
--rw-r--r--   0        0        0      289 2024-04-15 07:06:44.885186 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/replicate.py
--rw-r--r--   0        0        0      973 2024-04-15 07:06:44.885186 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/replicate.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.891695 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/text_embedding/__init__.py
--rw-r--r--   0        0        0     5906 2024-04-23 02:42:30.766537 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/text_embedding/text_embedding.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.910283 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/__init__.py
--rw-r--r--   0        0        0     5942 2024-04-15 07:06:44.931489 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     3889 2024-04-15 07:06:44.939008 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_zh.svg
--rw-r--r--   0        0        0     2005 2024-04-15 07:06:44.939008 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/_assets/icon_s_en.svg
--rw-r--r--   0        0        0        0 2024-04-15 07:06:44.956912 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/__init__.py
--rw-r--r--   0        0        0     5990 2024-04-15 07:06:44.960416 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/_client.py
--rw-r--r--   0        0        0       44 2024-04-15 07:06:44.960416 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/_position.yaml
--rw-r--r--   0        0        0    10372 2024-04-23 02:42:30.796100 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/llm.py
--rw-r--r--   0        0        0     1079 2024-04-15 07:06:44.970423 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-1.5.yaml
--rw-r--r--   0        0        0     1095 2024-04-15 07:06:44.970423 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-2.yaml
--rw-r--r--   0        0        0     1080 2024-04-15 07:06:44.987113 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.5.yaml
--rw-r--r--   0        0        0     1078 2024-04-15 07:06:44.997139 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.yaml
--rw-r--r--   0        0        0      592 2024-04-15 07:06:45.001649 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/spark.py
--rw-r--r--   0        0        0     1087 2024-04-15 07:06:45.001649 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/spark.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.001649 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/__init__.py
--rw-r--r--   0        0        0     7942 2024-04-15 07:06:45.027131 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai.svg
--rw-r--r--   0        0        0     1536 2024-04-15 07:06:45.034099 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai_square.svg
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.034099 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/llm/__init__.py
--rw-r--r--   0        0        0     2924 2024-04-23 02:42:30.838398 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/llm/llm.py
--rw-r--r--   0        0        0      290 2024-04-15 07:06:45.050884 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/togetherai.py
--rw-r--r--   0        0        0     1828 2024-04-15 07:06:45.050884 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/togetherai.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.069345 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/__init__.py
--rw-r--r--   0        0        0     4741 2024-04-15 07:06:45.080864 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_en.png
--rw-r--r--   0        0        0     7052 2024-04-15 07:06:45.080864 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_zh.png
--rw-r--r--   0        0        0     2835 2024-04-15 07:06:45.080864 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_s_en.png
--rw-r--r--   0        0        0      768 2024-04-23 02:42:30.892175 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_common.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.097509 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-23 02:42:30.924162 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/_client.py
--rw-r--r--   0        0        0    16022 2024-04-23 02:42:30.944473 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/llm.py
--rw-r--r--   0        0        0     4739 2024-04-15 07:06:45.122794 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-1201.yaml
--rw-r--r--   0        0        0     4755 2024-04-15 07:06:45.129254 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-longcontext.yaml
--rw-r--r--   0        0        0     4729 2024-04-15 07:06:45.131260 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max.yaml
--rw-r--r--   0        0        0     4793 2024-04-15 07:06:45.131260 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-plus.yaml
--rw-r--r--   0        0        0     4815 2024-04-15 07:06:45.144268 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-turbo.yaml
--rw-r--r--   0        0        0     1185 2024-04-15 07:06:45.151160 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tongyi.py
--rw-r--r--   0        0        0      698 2024-04-15 07:06:45.151160 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tongyi.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.161041 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tts/__init__.py
--rw-r--r--   0        0        0     4708 2024-04-15 07:06:45.161041 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tts/tts-1.yaml
--rw-r--r--   0        0        0     7663 2024-04-23 02:42:30.976495 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tts/tts.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.177856 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/__init__.py
--rw-r--r--   0        0        0     6615 2024-04-15 07:06:45.196204 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_en.png
--rw-r--r--   0        0        0     7967 2024-04-15 07:06:45.202210 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_zh.png
--rw-r--r--   0        0        0     3350 2024-04-15 07:06:45.209225 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_s_en.png
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.219729 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/__init__.py
--rw-r--r--   0        0        0      846 2024-04-15 07:06:45.226000 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-4.yaml
--rw-r--r--   0        0        0      849 2024-04-15 07:06:45.231506 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-8k.yaml
--rw-r--r--   0        0        0      603 2024-04-15 07:06:45.231506 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-turbo.yaml
--rw-r--r--   0        0        0      842 2024-04-15 07:06:45.241682 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot.yaml
--rw-r--r--   0        0        0    14218 2024-04-23 02:42:31.004006 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie_bot.py
--rw-r--r--   0        0        0      303 2024-04-15 07:06:45.247693 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie_bot_errors.py
--rw-r--r--   0        0        0    13386 2024-04-23 02:42:31.034479 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/llm.py
--rw-r--r--   0        0        0     1183 2024-04-15 07:06:45.256701 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/wenxin.py
--rw-r--r--   0        0        0      910 2024-04-15 07:06:45.256701 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/wenxin.yaml
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.273193 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/__init__.py
--rw-r--r--   0        0        0    12240 2024-04-15 07:06:45.290366 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_l_en.svg
--rw-r--r--   0        0        0     1888 2024-04-15 07:06:45.293520 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_s_en.svg
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.307697 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/llm/__init__.py
--rw-r--r--   0        0        0       14 2024-04-15 07:06:45.307697 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/llm/_position.yaml
--rw-r--r--   0        0        0      908 2024-04-15 07:06:45.314917 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/llm/chatglm3-6b.yaml
--rw-r--r--   0        0        0    30900 2024-04-23 02:42:31.068142 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.331601 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/rerank/__init__.py
--rw-r--r--   0        0        0     5467 2024-04-23 02:42:31.099559 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/rerank/rerank.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.341613 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/text_embedding/__init__.py
--rw-r--r--   0        0        0     7210 2024-04-23 02:42:31.125120 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/text_embedding/text_embedding.py
--rw-r--r--   0        0        0      292 2024-04-15 07:06:45.359259 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/xinference.py
--rw-r--r--   0        0        0     1172 2024-04-15 07:06:45.363264 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/xinference.yaml
--rw-r--r--   0        0        0     4499 2024-04-23 02:42:31.148769 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/xinference_helper.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.371476 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/__init__.py
--rw-r--r--   0        0        0    12982 2024-04-15 07:06:45.387993 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_en.svg
--rw-r--r--   0        0        0    13013 2024-04-15 07:06:45.387993 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_zh.svg
--rw-r--r--   0        0        0    10263 2024-04-15 07:06:45.402692 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_s_en.svg
--rw-r--r--   0        0        0     1607 2024-04-23 02:42:31.171047 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_common.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.417988 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/__init__.py
--rw-r--r--   0        0        0     2039 2024-04-15 07:06:45.417988 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite.yaml
--rw-r--r--   0        0        0     2047 2024-04-15 07:06:45.431495 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite_32k.yaml
--rw-r--r--   0        0        0     2037 2024-04-15 07:06:45.434765 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_pro.yaml
--rw-r--r--   0        0        0     2037 2024-04-15 07:06:45.439629 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_std.yaml
--rw-r--r--   0        0        0     3229 2024-04-15 07:06:45.449640 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_turbo.yaml
--rw-r--r--   0        0        0     2666 2024-04-15 07:06:45.449640 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_3_turbo.yaml
--rw-r--r--   0        0        0     2654 2024-04-15 07:06:45.466393 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4.yaml
--rw-r--r--   0        0        0     2608 2024-04-15 07:06:45.473211 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4v.yaml
--rw-r--r--   0        0        0    21498 2024-04-23 02:42:31.207261 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/llm.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.482135 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/__init__.py
--rw-r--r--   0        0        0     4595 2024-04-23 02:42:31.234252 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/text_embedding.py
--rw-r--r--   0        0        0       87 2024-04-15 07:06:45.500139 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/text_embedding.yaml
--rw-r--r--   0        0        0     1138 2024-04-15 07:06:45.500139 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.py
--rw-r--r--   0        0        0      919 2024-04-23 02:42:31.249311 model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.yaml
--rw-r--r--   0        0        0     3877 2024-04-15 07:06:42.327338 model_providers-0.3.0/model_providers/core/model_runtime/README.md
--rw-r--r--   0        0        0     5367 2024-04-23 02:42:28.397537 model_providers-0.3.0/model_providers/core/model_runtime/README_CN.md
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.801450 model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/__init__.py
--rw-r--r--   0        0        0     4583 2024-04-23 02:42:31.273907 model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/common_validator.py
--rw-r--r--   0        0        0     1227 2024-04-15 07:06:45.824329 model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/model_credential_schema_validator.py
--rw-r--r--   0        0        0      957 2024-04-15 07:06:45.824329 model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/provider_credential_schema_validator.py
--rw-r--r--   0        0        0        0 2024-04-15 07:06:45.832346 model_providers-0.3.0/model_providers/core/model_runtime/utils/__init__.py
--rw-r--r--   0        0        0      612 2024-04-15 07:06:45.832346 model_providers-0.3.0/model_providers/core/model_runtime/utils/_compat.py
--rw-r--r--   0        0        0     7476 2024-04-23 02:42:31.281425 model_providers-0.3.0/model_providers/core/model_runtime/utils/encoders.py
--rw-r--r--   0        0        0      211 2024-04-15 07:06:45.850488 model_providers-0.3.0/model_providers/core/model_runtime/utils/helper.py
--rw-r--r--   0        0        0    10981 2024-04-23 02:42:31.307605 model_providers-0.3.0/model_providers/core/provider_manager.py
--rw-r--r--   0        0        0      569 2024-04-15 07:06:45.850488 model_providers-0.3.0/model_providers/core/utils/generic.py
--rw-r--r--   0        0        0      239 2024-04-15 07:06:45.863999 model_providers-0.3.0/model_providers/core/utils/json_dumps.py
--rw-r--r--   0        0        0     2389 2024-04-23 02:42:31.329154 model_providers-0.3.0/model_providers/core/utils/position_helper.py
--rw-r--r--   0        0        0     2620 2024-04-15 07:06:45.875592 model_providers-0.3.0/model_providers/core/utils/utils.py
--rw-r--r--   0        0        0     1037 2024-04-15 07:06:45.881167 model_providers-0.3.0/model_providers/errors/error.py
--rw-r--r--   0        0        0      824 2024-04-15 07:06:45.881167 model_providers-0.3.0/model_providers/extensions/ext_redis.py
--rw-r--r--   0        0        0     5122 2024-04-15 07:06:45.881167 model_providers-0.3.0/model_providers/extensions/ext_storage.py
--rw-r--r--   0        0        0     5007 2024-04-23 07:18:06.592616 model_providers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2430 2024-04-23 02:42:28.115200 model_providers-0.3.0/README.md
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 model_providers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2430 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/README.md
+-rw-r--r--   0        0        0     3116 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/__init__.py
+-rw-r--r--   0        0        0     1330 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/bootstrap_web/entities/__init__.py
+-rw-r--r--   0        0        0     5340 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/bootstrap_web/entities/model_provider_entities.py
+-rw-r--r--   0        0        0      318 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/bootstrap_web/message_convert/__init__.py
+-rw-r--r--   0        0        0     9580 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/bootstrap_web/message_convert/core.py
+-rw-r--r--   0        0        0    11025 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/bootstrap_web/openai_bootstrap_web.py
+-rw-r--r--   0        0        0      251 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/bootstrap/__init__.py
+-rw-r--r--   0        0        0     1679 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/bootstrap/base.py
+-rw-r--r--   0        0        0     1256 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/bootstrap/bootstrap_register.py
+-rw-r--r--   0        0        0     5260 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/bootstrap/openai_protocol.py
+-rw-r--r--   0        0        0     5877 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/bootstrap/providers_wapper.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/entities/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/entities/agent_entities.py
+-rw-r--r--   0        0        0     7484 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/entities/application_entities.py
+-rw-r--r--   0        0        0     5777 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/entities/message_entities.py
+-rw-r--r--   0        0        0     1895 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/entities/model_entities.py
+-rw-r--r--   0        0        0    11780 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/entities/provider_configuration.py
+-rw-r--r--   0        0        0     2361 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/entities/provider_entities.py
+-rw-r--r--   0        0        0     2727 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/entities/queue_entities.py
+-rw-r--r--   0        0        0    10489 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/model_manager.py
+-rw-r--r--   0        0        0     4831 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/model_runtime/README.md
+-rw-r--r--   0        0        0     3980 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/model_runtime/README_CN.md
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/model_runtime/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.358383 model_providers-0.3.0.20240506/model_providers/core/model_runtime/callbacks/__init__.py
+-rw-r--r--   0        0        0     4617 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/model_runtime/callbacks/base_callback.py
+-rw-r--r--   0        0        0     6100 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/model_runtime/callbacks/logging_callback.py
+-rw-r--r--   0        0        0    28170 2024-05-05 14:19:31.011622 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/images/index/img.png
+-rw-r--r--   0        0        0    21453 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/interfaces.md
+-rw-r--r--   0        0        0    12244 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/provider_scale_out.md
+-rw-r--r--   0        0        0     9330 2024-05-05 13:09:55.361716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/schema.md
+-rw-r--r--   0        0        0    10307 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/customizable_model_scale_out.md
+-rw-r--r--   0        0        0    28170 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/images/index/img.png
+-rw-r--r--   0        0        0    21493 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/interfaces.md
+-rw-r--r--   0        0        0     6789 2024-05-05 14:20:18.511073 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/predefined_model_scale_out.md
+-rw-r--r--   0        0        0     8333 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/provider_scale_out.md
+-rw-r--r--   0        0        0     8437 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/schema.md
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/common_entities.py
+-rw-r--r--   0        0        0     3673 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/defaults.py
+-rw-r--r--   0        0        0     2541 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/llm_entities.py
+-rw-r--r--   0        0        0     3473 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/message_entities.py
+-rw-r--r--   0        0        0     5479 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/model_entities.py
+-rw-r--r--   0        0        0     3624 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/provider_entities.py
+-rw-r--r--   0        0        0      322 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/rerank_entities.py
+-rw-r--r--   0        0        0      580 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/text_embedding_entities.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/errors/__init__.py
+-rw-r--r--   0        0        0     1113 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/errors/invoke.py
+-rw-r--r--   0        0        0      113 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/errors/validate.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/__init__.py
+-rw-r--r--   0        0        0    13961 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/ai_model.py
+-rw-r--r--   0        0        0   218880 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/audio.mp3
+-rw-r--r--   0        0        0    34387 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/large_language_model.py
+-rw-r--r--   0        0        0     4980 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/model_provider.py
+-rw-r--r--   0        0        0     1402 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/moderation_model.py
+-rw-r--r--   0        0        0     2019 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/rerank_model.py
+-rw-r--r--   0        0        0     1686 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/speech2text_model.py
+-rw-r--r--   0        0        0     1597 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/text2img_model.py
+-rw-r--r--   0        0        0     3077 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/text_embedding_model.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.371716 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/__init__.py
+-rw-r--r--   0        0        0   456318 2024-05-05 13:09:55.375049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/merges.txt
+-rw-r--r--   0        0        0      438 2024-05-05 13:09:55.375049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/special_tokens_map.json
+-rw-r--r--   0        0        0      727 2024-05-05 13:09:55.375049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/tokenizer_config.json
+-rw-r--r--   0        0        0   999186 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/vocab.json
+-rw-r--r--   0        0        0     1022 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2_tokenzier.py
+-rw-r--r--   0        0        0     6864 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tts_model.py
+-rw-r--r--   0        0        0      165 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/_position.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/__init__.py
+-rw-r--r--   0        0        0     5400 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0      410 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1202 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/anthropic.py
+-rw-r--r--   0        0        0      981 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/anthropic.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/_position.yaml
+-rw-r--r--   0        0        0      775 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.1.yaml
+-rw-r--r--   0        0        0      788 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.yaml
+-rw-r--r--   0        0        0      801 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-haiku-20240307.yaml
+-rw-r--r--   0        0        0      801 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-opus-20240229.yaml
+-rw-r--r--   0        0        0      804 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-sonnet-20240229.yaml
+-rw-r--r--   0        0        0      766 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.2.yaml
+-rw-r--r--   0        0        0      789 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.yaml
+-rw-r--r--   0        0        0    21749 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/__init__.py
+-rw-r--r--   0        0        0     5007 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_assets/icon_l_en.png
+-rw-r--r--   0        0        0      439 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1657 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_common.py
+-rw-r--r--   0        0        0    29393 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_constant.py
+-rw-r--r--   0        0        0      291 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/azure_openai.py
+-rw-r--r--   0        0        0     4223 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/azure_openai.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/llm/__init__.py
+-rw-r--r--   0        0        0    29753 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/speech2text/__init__.py
+-rw-r--r--   0        0        0     3183 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/speech2text/speech2text.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/text_embedding/__init__.py
+-rw-r--r--   0        0        0     7870 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/tts/__init__.py
+-rw-r--r--   0        0        0     8820 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/tts/tts.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/__init__.py
+-rw-r--r--   0        0        0     4140 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0      748 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1197 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/baichuan.py
+-rw-r--r--   0        0        0      857 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/baichuan.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/__init__.py
+-rw-r--r--   0        0        0     1109 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-53b.yaml
+-rw-r--r--   0        0        0     1127 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo-192k.yaml
+-rw-r--r--   0        0        0     1117 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo.yaml
+-rw-r--r--   0        0        0      870 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_tokenizer.py
+-rw-r--r--   0        0        0     8828 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_turbo.py
+-rw-r--r--   0        0        0      303 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_turbo_errors.py
+-rw-r--r--   0        0        0     9597 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/baichuan-text-embedding.yaml
+-rw-r--r--   0        0        0     7345 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/__init__.py
+-rw-r--r--   0        0        0    12612 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     3301 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1201 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/bedrock.py
+-rw-r--r--   0        0        0     1918 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/bedrock.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/_position.yaml
+-rw-r--r--   0        0        0      839 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-mid-v1.yaml
+-rw-r--r--   0        0        0      843 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-ultra-v1.yaml
+-rw-r--r--   0        0        0      473 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/amazon.titan-text-express-v1.yaml
+-rw-r--r--   0        0        0      467 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/amazon.titan-text-lite-v1.yaml
+-rw-r--r--   0        0        0      750 2024-05-05 13:09:55.378382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-instant-v1.yaml
+-rw-r--r--   0        0        0      734 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v1.yaml
+-rw-r--r--   0        0        0      738 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.1.yaml
+-rw-r--r--   0        0        0      734 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.yaml
+-rw-r--r--   0        0        0      753 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-light-text-v14.yaml
+-rw-r--r--   0        0        0      710 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-text-v14.yaml
+-rw-r--r--   0        0        0    20697 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/llm.py
+-rw-r--r--   0        0        0      434 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/meta.llama2-13b-chat-v1.yaml
+-rw-r--r--   0        0        0      434 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/meta.llama2-70b-chat-v1.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/__init__.py
+-rw-r--r--   0        0        0     5500 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     1355 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1206 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/cohere.py
+-rw-r--r--   0        0        0     1638 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/cohere.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/_position.yaml
+-rw-r--r--   0        0        0     1762 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-chat.yaml
+-rw-r--r--   0        0        0     1780 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-chat.yaml
+-rw-r--r--   0        0        0     1804 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly-chat.yaml
+-rw-r--r--   0        0        0      946 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly.yaml
+-rw-r--r--   0        0        0      922 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light.yaml
+-rw-r--r--   0        0        0     1786 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly-chat.yaml
+-rw-r--r--   0        0        0      928 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly.yaml
+-rw-r--r--   0        0        0      904 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command.yaml
+-rw-r--r--   0        0        0    22098 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/rerank/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank-english-v2.0.yaml
+-rw-r--r--   0        0        0       90 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank-multilingual-v2.0.yaml
+-rw-r--r--   0        0        0     4003 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/__init__.py
+-rw-r--r--   0        0        0      180 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/_position.yaml
+-rw-r--r--   0        0        0      174 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-light-v2.0.yaml
+-rw-r--r--   0        0        0      173 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-light-v3.0.yaml
+-rw-r--r--   0        0        0      168 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-v2.0.yaml
+-rw-r--r--   0        0        0      168 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-english-v3.0.yaml
+-rw-r--r--   0        0        0      178 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-multilingual-light-v3.0.yaml
+-rw-r--r--   0        0        0      172 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-multilingual-v2.0.yaml
+-rw-r--r--   0        0        0      173 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/embed-multilingual-v3.0.yaml
+-rw-r--r--   0        0        0     7533 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/__init__.py
+-rw-r--r--   0        0        0     3710 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0      689 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1185 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/google.py
+-rw-r--r--   0        0        0      692 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/google.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro-vision.yaml
+-rw-r--r--   0        0        0      773 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro.yaml
+-rw-r--r--   0        0        0    17195 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/__init__.py
+-rw-r--r--   0        0        0     5889 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0      828 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1136 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/groq.py
+-rw-r--r--   0        0        0      850 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/groq.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/llm/__init__.py
+-rw-r--r--   0        0        0      456 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/llm/llama2-70b-4096.yaml
+-rw-r--r--   0        0        0     1352 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/llm/llm.py
+-rw-r--r--   0        0        0      483 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/llm/mixtral-8x7b-instruct-v0.1.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/__init__.py
+-rw-r--r--   0        0        0    20353 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     9298 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0      419 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/_common.py
+-rw-r--r--   0        0        0      294 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/huggingface_hub.py
+-rw-r--r--   0        0        0     2850 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/huggingface_hub.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/llm/__init__.py
+-rw-r--r--   0        0        0    13140 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/text_embedding/__init__.py
+-rw-r--r--   0        0        0     8640 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0      566 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1309 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/jina.py
+-rw-r--r--   0        0        0      668 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/jina.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/rerank/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/rerank/jina-reranker-v1-base-en.yaml
+-rw-r--r--   0        0        0     4048 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/rerank/rerank.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-base-de.yaml
+-rw-r--r--   0        0        0      177 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-base-en.yaml
+-rw-r--r--   0        0        0      177 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-base-zh.yaml
+-rw-r--r--   0        0        0      178 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina-embeddings-v2-small-en.yaml
+-rw-r--r--   0        0        0      950 2024-05-05 13:09:55.381715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina_tokenizer.py
+-rw-r--r--   0        0        0     5928 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0   711577 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/tokenizer/tokenizer.json
+-rw-r--r--   0        0        0      373 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/tokenizer/tokenizer_config.json
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/__init__.py
+-rw-r--r--   0        0        0    77919 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0    74478 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/llm/__init__.py
+-rw-r--r--   0        0        0    25761 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/llm/llm.py
+-rw-r--r--   0        0        0      287 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/localai.py
+-rw-r--r--   0        0        0     1678 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/localai.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/text_embedding/__init__.py
+-rw-r--r--   0        0        0     7053 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/__init__.py
+-rw-r--r--   0        0        0     5767 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_l_en.png
+-rw-r--r--   0        0        0     2007 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_s_en.png
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab5-chat.yaml
+-rw-r--r--   0        0        0      851 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5-chat.yaml
+-rw-r--r--   0        0        0      655 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5s-chat.yaml
+-rw-r--r--   0        0        0      681 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab6-chat.yaml
+-rw-r--r--   0        0        0     6398 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion.py
+-rw-r--r--   0        0        0     8378 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion_pro.py
+-rw-r--r--   0        0        0      308 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/errors.py
+-rw-r--r--   0        0        0    12273 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/llm.py
+-rw-r--r--   0        0        0      960 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/types.py
+-rw-r--r--   0        0        0     1227 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/minimax.py
+-rw-r--r--   0        0        0      894 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/minimax.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/text_embedding/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-05 13:09:55.385049 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/text_embedding/embo-01.yaml
+-rw-r--r--   0        0        0     6482 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/__init__.py
+-rw-r--r--   0        0        0     7064 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_l_en.png
+-rw-r--r--   0        0        0     7418 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_s_en.png
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/_position.yaml
+-rw-r--r--   0        0        0     1538 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/llm.py
+-rw-r--r--   0        0        0     1179 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-large-latest.yaml
+-rw-r--r--   0        0        0     1184 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-medium-latest.yaml
+-rw-r--r--   0        0        0     1179 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-small-latest.yaml
+-rw-r--r--   0        0        0     1167 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mistral-7b.yaml
+-rw-r--r--   0        0        0     1172 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mixtral-8x7b.yaml
+-rw-r--r--   0        0        0     1141 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/mistralai.py
+-rw-r--r--   0        0        0      816 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/mistralai.yaml
+-rw-r--r--   0        0        0    11866 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/model_provider_factory.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/__init__.py
+-rw-r--r--   0        0        0    13654 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_l_en.png
+-rw-r--r--   0        0        0     7419 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_s_en.png
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/_position.yaml
+-rw-r--r--   0        0        0     1513 2024-05-05 14:19:31.014955 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/llm.py
+-rw-r--r--   0        0        0      461 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/moonshot-v1-128k.yaml
+-rw-r--r--   0        0        0      458 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/moonshot-v1-32k.yaml
+-rw-r--r--   0        0        0      452 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/moonshot-v1-8k.yaml
+-rw-r--r--   0        0        0     1139 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/moonshot.py
+-rw-r--r--   0        0        0      869 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/moonshot.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/__init__.py
+-rw-r--r--   0        0        0    12066 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     7922 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/llm/__init__.py
+-rw-r--r--   0        0        0    27882 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/llm/llm.py
+-rw-r--r--   0        0        0      501 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/ollama.py
+-rw-r--r--   0        0        0     2430 2024-05-06 13:54:50.024800 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/ollama.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/text_embedding/__init__.py
+-rw-r--r--   0        0        0     7866 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/__init__.py
+-rw-r--r--   0        0        0     4773 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     7038 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     2149 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/_common.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/__init__.py
+-rw-r--r--   0        0        0      275 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/_position.yaml
+-rw-r--r--   0        0        0      932 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0125.yaml
+-rw-r--r--   0        0        0      692 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0613.yaml
+-rw-r--r--   0        0        0      930 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-1106.yaml
+-rw-r--r--   0        0        0      705 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k-0613.yaml
+-rw-r--r--   0        0        0      690 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k.yaml
+-rw-r--r--   0        0        0      655 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-instruct.yaml
+-rw-r--r--   0        0        0      914 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo.yaml
+-rw-r--r--   0        0        0     1631 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-0125-preview.yaml
+-rw-r--r--   0        0        0     1631 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-1106-preview.yaml
+-rw-r--r--   0        0        0     1604 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-32k.yaml
+-rw-r--r--   0        0        0     1634 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-turbo-preview.yaml
+-rw-r--r--   0        0        0     1589 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-vision-preview.yaml
+-rw-r--r--   0        0        0     1590 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4.yaml
+-rw-r--r--   0        0        0    42510 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/llm.py
+-rw-r--r--   0        0        0      593 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/text-davinci-003.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/moderation/__init__.py
+-rw-r--r--   0        0        0     4301 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/moderation/moderation.py
+-rw-r--r--   0        0        0      121 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/moderation/text-moderation-stable.yaml
+-rw-r--r--   0        0        0     1274 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/openai.py
+-rw-r--r--   0        0        0     2268 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/openai.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/speech2text/__init__.py
+-rw-r--r--   0        0        0     2100 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/speech2text/speech2text.py
+-rw-r--r--   0        0        0      152 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/speech2text/whisper-1.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/text_embedding/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/text_embedding/text-embedding-3-large.yaml
+-rw-r--r--   0        0        0      173 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/text_embedding/text-embedding-3-small.yaml
+-rw-r--r--   0        0        0      172 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/text_embedding/text-embedding-ada-002.yaml
+-rw-r--r--   0        0        0     7509 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/tts-1-hd.yaml
+-rw-r--r--   0        0        0      993 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/tts-1.yaml
+-rw-r--r--   0        0        0     7747 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/tts.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/__init__.py
+-rw-r--r--   0        0        0     1626 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/_common.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/llm/__init__.py
+-rw-r--r--   0        0        0    31259 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/llm/llm.py
+-rw-r--r--   0        0        0      289 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/openai_api_compatible.py
+-rw-r--r--   0        0        0     2881 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/openai_api_compatible.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/text_embedding/__init__.py
+-rw-r--r--   0        0        0     8038 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/__init__.py
+-rw-r--r--   0        0        0    11337 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     7299 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.388382 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/llm/__init__.py
+-rw-r--r--   0        0        0    10841 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/llm/llm.py
+-rw-r--r--   0        0        0     7362 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/llm/openllm_generate.py
+-rw-r--r--   0        0        0      308 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/llm/openllm_generate_errors.py
+-rw-r--r--   0        0        0      287 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/openllm.py
+-rw-r--r--   0        0        0      896 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/openllm.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/text_embedding/__init__.py
+-rw-r--r--   0        0        0     5542 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0      384 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0      403 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/_common.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/llm/__init__.py
+-rw-r--r--   0        0        0    12185 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/llm/llm.py
+-rw-r--r--   0        0        0      289 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/replicate.py
+-rw-r--r--   0        0        0      973 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/replicate.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/text_embedding/__init__.py
+-rw-r--r--   0        0        0     5906 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/__init__.py
+-rw-r--r--   0        0        0     5942 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     3889 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_zh.svg
+-rw-r--r--   0        0        0     2005 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/__init__.py
+-rw-r--r--   0        0        0     5990 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/_client.py
+-rw-r--r--   0        0        0       44 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/_position.yaml
+-rw-r--r--   0        0        0    10372 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/llm.py
+-rw-r--r--   0        0        0     1079 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-1.5.yaml
+-rw-r--r--   0        0        0     1095 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-2.yaml
+-rw-r--r--   0        0        0     1080 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.5.yaml
+-rw-r--r--   0        0        0     1078 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.yaml
+-rw-r--r--   0        0        0      592 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/spark.py
+-rw-r--r--   0        0        0     1087 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/spark.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/__init__.py
+-rw-r--r--   0        0        0     7942 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai.svg
+-rw-r--r--   0        0        0     1536 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai_square.svg
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/llm/__init__.py
+-rw-r--r--   0        0        0     2924 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/llm/llm.py
+-rw-r--r--   0        0        0      290 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/togetherai.py
+-rw-r--r--   0        0        0     1828 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/togetherai.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/__init__.py
+-rw-r--r--   0        0        0     4741 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_en.png
+-rw-r--r--   0        0        0     7052 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_zh.png
+-rw-r--r--   0        0        0     2835 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_s_en.png
+-rw-r--r--   0        0        0      768 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_common.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/__init__.py
+-rw-r--r--   0        0        0     2782 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/_client.py
+-rw-r--r--   0        0        0    16022 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/llm.py
+-rw-r--r--   0        0        0     4739 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-1201.yaml
+-rw-r--r--   0        0        0     4755 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-longcontext.yaml
+-rw-r--r--   0        0        0     4729 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max.yaml
+-rw-r--r--   0        0        0     4793 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-plus.yaml
+-rw-r--r--   0        0        0     4815 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-turbo.yaml
+-rw-r--r--   0        0        0     1185 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tongyi.py
+-rw-r--r--   0        0        0      698 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tongyi.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tts/__init__.py
+-rw-r--r--   0        0        0     4708 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tts/tts-1.yaml
+-rw-r--r--   0        0        0     7663 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tts/tts.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/__init__.py
+-rw-r--r--   0        0        0     6615 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_en.png
+-rw-r--r--   0        0        0     7967 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_zh.png
+-rw-r--r--   0        0        0     3350 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_s_en.png
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/__init__.py
+-rw-r--r--   0        0        0      846 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-4.yaml
+-rw-r--r--   0        0        0      849 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-8k.yaml
+-rw-r--r--   0        0        0      603 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-turbo.yaml
+-rw-r--r--   0        0        0      842 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot.yaml
+-rw-r--r--   0        0        0    14218 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie_bot.py
+-rw-r--r--   0        0        0      303 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie_bot_errors.py
+-rw-r--r--   0        0        0    13386 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/llm.py
+-rw-r--r--   0        0        0     1183 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/wenxin.py
+-rw-r--r--   0        0        0      910 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/wenxin.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/__init__.py
+-rw-r--r--   0        0        0    12240 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0     1888 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/llm/__init__.py
+-rw-r--r--   0        0        0       14 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/llm/_position.yaml
+-rw-r--r--   0        0        0      908 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/llm/chatglm3-6b.yaml
+-rw-r--r--   0        0        0    30924 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/rerank/__init__.py
+-rw-r--r--   0        0        0     5467 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/rerank/rerank.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/text_embedding/__init__.py
+-rw-r--r--   0        0        0     7210 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0      292 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/xinference.py
+-rw-r--r--   0        0        0     1172 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/xinference.yaml
+-rw-r--r--   0        0        0     4499 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/xinference_helper.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/__init__.py
+-rw-r--r--   0        0        0    12982 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_en.svg
+-rw-r--r--   0        0        0    13013 2024-05-05 13:09:55.391715 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_zh.svg
+-rw-r--r--   0        0        0    10263 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_s_en.svg
+-rw-r--r--   0        0        0     1607 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_common.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/__init__.py
+-rw-r--r--   0        0        0     2039 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite.yaml
+-rw-r--r--   0        0        0     2047 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite_32k.yaml
+-rw-r--r--   0        0        0     2037 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_pro.yaml
+-rw-r--r--   0        0        0     2037 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_std.yaml
+-rw-r--r--   0        0        0     3229 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_turbo.yaml
+-rw-r--r--   0        0        0     2666 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_3_turbo.yaml
+-rw-r--r--   0        0        0     2654 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4.yaml
+-rw-r--r--   0        0        0     2608 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4v.yaml
+-rw-r--r--   0        0        0    21498 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/llm.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/__init__.py
+-rw-r--r--   0        0        0     4595 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/text_embedding.py
+-rw-r--r--   0        0        0       87 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/text_embedding.yaml
+-rw-r--r--   0        0        0     1138 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.py
+-rw-r--r--   0        0        0      919 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/__init__.py
+-rw-r--r--   0        0        0     4583 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/common_validator.py
+-rw-r--r--   0        0        0     1227 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/model_credential_schema_validator.py
+-rw-r--r--   0        0        0      957 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/provider_credential_schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/utils/__init__.py
+-rw-r--r--   0        0        0      612 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/utils/_compat.py
+-rw-r--r--   0        0        0     7476 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/model_runtime/utils/encoders.py
+-rw-r--r--   0        0        0      211 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/model_runtime/utils/helper.py
+-rw-r--r--   0        0        0    10981 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/provider_manager.py
+-rw-r--r--   0        0        0      569 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/utils/generic.py
+-rw-r--r--   0        0        0      239 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/utils/json_dumps.py
+-rw-r--r--   0        0        0     2389 2024-05-05 14:19:31.018289 model_providers-0.3.0.20240506/model_providers/core/utils/position_helper.py
+-rw-r--r--   0        0        0     2620 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/core/utils/utils.py
+-rw-r--r--   0        0        0     1037 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/errors/error.py
+-rw-r--r--   0        0        0      824 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/extensions/ext_redis.py
+-rw-r--r--   0        0        0     5122 2024-05-05 13:09:55.395048 model_providers-0.3.0.20240506/model_providers/extensions/ext_storage.py
+-rw-r--r--   0        0        0     5082 2024-05-06 13:56:17.762777 model_providers-0.3.0.20240506/pyproject.toml
+-rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 model_providers-0.3.0.20240506/PKG-INFO
```

### Comparing `model_providers-0.3.0/model_providers/__init__.py` & `model_providers-0.3.0.20240506/model_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/__main__.py` & `model_providers-0.3.0.20240506/model_providers/__main__.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/bootstrap_web/entities/model_provider_entities.py` & `model_providers-0.3.0.20240506/model_providers/bootstrap_web/entities/model_provider_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/bootstrap_web/message_convert/core.py` & `model_providers-0.3.0.20240506/model_providers/bootstrap_web/message_convert/core.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/bootstrap_web/openai_bootstrap_web.py` & `model_providers-0.3.0.20240506/model_providers/bootstrap_web/openai_bootstrap_web.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/bootstrap/base.py` & `model_providers-0.3.0.20240506/model_providers/core/bootstrap/base.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/bootstrap/bootstrap_register.py` & `model_providers-0.3.0.20240506/model_providers/core/bootstrap/bootstrap_register.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/bootstrap/openai_protocol.py` & `model_providers-0.3.0.20240506/model_providers/core/bootstrap/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/bootstrap/providers_wapper.py` & `model_providers-0.3.0.20240506/model_providers/core/bootstrap/providers_wapper.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/entities/application_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/entities/application_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/entities/message_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/entities/message_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/entities/model_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/entities/model_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/entities/provider_configuration.py` & `model_providers-0.3.0.20240506/model_providers/core/entities/provider_configuration.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/entities/provider_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/entities/provider_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/entities/queue_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/entities/queue_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_manager.py` & `model_providers-0.3.0.20240506/model_providers/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/callbacks/base_callback.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/callbacks/logging_callback.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/callbacks/logging_callback.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/interfaces.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/interfaces.md`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/provider_scale_out.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/provider_scale_out.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 ## Adding a New Provider
 
+> If you have completed the following steps, you can configure the corresponding supplier in the `model_providers.yaml` file.
+
 Providers support three types of model configuration methods:
 
 - `predefined-model` Predefined model
 
   This indicates that users only need to configure the unified provider credentials to use the predefined models under the provider.
 
 - `customizable-model` Customizable model
 
   Users need to add credential configurations for each model.
 
-- `fetch-from-remote` Fetch from remote
+- `fetch-from-remote` Fetch from a remote source (Dify has not implemented this, and we do not intend to implement it either).
 
   This is consistent with the `predefined-model` configuration method. Only unified provider credentials need to be configured, and models are obtained from the provider through credential information.
 
 These three configuration methods **can coexist**, meaning a provider can support `predefined-model` + `customizable-model` or `predefined-model` + `fetch-from-remote`, etc. In other words, configuring the unified provider credentials allows the use of predefined and remotely fetched models, and if new models are added, they can be used in addition to the custom models.
 
 ## Getting Started
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/en_US/schema.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/en_US/schema.md`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/customizable_model_scale_out.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/customizable_model_scale_out.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 
 ### 介绍
 
 供应商集成完成后，接下来为供应商下模型的接入，为了帮助理解整个接入过程，我们以`Xinference`为例，逐步完成一个完整的供应商接入。
 
 需要注意的是，对于自定义模型，每一个模型的接入都需要填写一个完整的供应商凭据。
 
-而不同于预定义模型，自定义供应商接入时永远会拥有如下两个参数，不需要在供应商yaml中定义。
-
-![Alt text](images/index/image-3.png)
-
 
 在前文中，我们已经知道了供应商无需实现`validate_provider_credential`，Runtime会自行根据用户在此选择的模型类型和模型名称调用对应的模型层的`validate_credentials`来进行验证。
 
 ### 编写供应商yaml
 
 我们首先要确定，接入的这个供应商支持哪些类型的模型。
 
@@ -290,8 +286,8 @@
       The value is the error type thrown by the model,
       which needs to be converted into a unified error type for the caller.
   
       :return: Invoke error mapping
       """
   ```
 
-接口方法说明见：[Interfaces](./interfaces.md)，具体实现可参考：[llm.py](https://github.com/langgenius/dify-runtime/blob/main/lib/model_providers/anthropic/llm/llm.py)。
+接口方法说明见：[Interfaces](./interfaces.md)，具体实现可参考代码
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/interfaces.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/interfaces.md`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/predefined_model_scale_out.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/predefined_model_scale_out.md`

 * *Files 3% similar despite different names*

```diff
@@ -165,8 +165,8 @@
       The value is the error type thrown by the model,
       which needs to be converted into a unified error type for the caller.
   
       :return: Invoke error mapping
       """
   ```
 
-接口方法说明见：[Interfaces](./interfaces.md)，具体实现可参考：[llm.py](https://github.com/langgenius/dify-runtime/blob/main/lib/model_providers/anthropic/llm/llm.py)。
+接口方法说明见：[Interfaces](./interfaces.md)，具体实现可参考代码
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/provider_scale_out.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/provider_scale_out.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 ## 增加新供应商
 
+> 如果你完成了下面步骤，即可在`model_providers.yaml`中配置对应供应商
+
 供应商支持三种模型配置方式：
 
 - `predefined-model  ` 预定义模型
 
   表示用户只需要配置统一的供应商凭据即可使用供应商下的预定义模型。
   
 - `customizable-model` 自定义模型
 
   用户需要新增每个模型的凭据配置，如Xinference，它同时支持 LLM 和 Text Embedding，但是每个模型都有唯一的**model_uid**，如果想要将两者同时接入，就需要为每个模型配置一个**model_uid**。
 
-- `fetch-from-remote` 从远程获取
+- `fetch-from-remote` 从远程获取（Dify没有实现，我们也不会实现）
 
   与 `predefined-model` 配置方式一致，只需要配置统一的供应商凭据即可，模型通过凭据信息从供应商获取。
 
   如OpenAI，我们可以基于gpt-turbo-3.5来Fine Tune多个模型，而他们都位于同一个**api_key**下，当配置为 `fetch-from-remote` 时，开发者只需要配置统一的**api_key**即可让DifyRuntime获取到开发者所有的微调模型并接入Dify。
 
 这三种配置方式**支持共存**，即存在供应商支持 `predefined-model` + `customizable-model` 或 `predefined-model` + `fetch-from-remote` 等，也就是配置了供应商统一凭据可以使用预定义模型和从远程获取的模型，若新增了模型，则可以在此基础上额外使用自定义的模型。
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/docs/zh_Hans/schema.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/docs/zh_Hans/schema.md`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/entities/defaults.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/defaults.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/entities/llm_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/llm_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/entities/message_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/message_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/entities/model_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/model_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/entities/provider_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/provider_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/entities/text_embedding_entities.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/entities/text_embedding_entities.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/errors/invoke.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/errors/invoke.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/ai_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/ai_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/audio.mp3` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/audio.mp3`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/large_language_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/large_language_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/model_provider.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/model_provider.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/moderation_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/moderation_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/rerank_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/rerank_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/speech2text_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/speech2text_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/text2img_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/text2img_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/text_embedding_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/text_embedding_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/merges.txt` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/merges.txt`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/tokenizer_config.json` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/vocab.json` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2/vocab.json`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2_tokenzier.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tokenizers/gpt2_tokenzier.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/__base/tts_model.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/__base/tts_model.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/anthropic.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/anthropic.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/anthropic.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-2.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-haiku-20240307.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-haiku-20240307.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-opus-20240229.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-opus-20240229.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-sonnet-20240229.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-3-sonnet-20240229.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.2.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.2.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/claude-instant-1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/anthropic/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/anthropic/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_assets/icon_l_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_assets/icon_l_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_common.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_common.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/_constant.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/_constant.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/azure_openai.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/azure_openai.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/speech2text/speech2text.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/speech2text/speech2text.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/azure_openai/tts/tts.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/azure_openai/tts/tts.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/baichuan.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/baichuan.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/baichuan.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/baichuan.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-53b.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-53b.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo-192k.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo-192k.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan2-turbo.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_tokenizer.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_tokenizer.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_turbo.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/baichuan_turbo.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/baichuan/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/bedrock.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/bedrock.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/bedrock.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-mid-v1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-mid-v1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-ultra-v1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/ai21.j2-ultra-v1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-instant-v1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-instant-v1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/anthropic.claude-v2.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-light-text-v14.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-light-text-v14.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-text-v14.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/cohere.command-text-v14.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/bedrock/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/bedrock/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/cohere.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/cohere.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/cohere.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light-nightly.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-light.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-light.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command-nightly.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/command.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/command.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/rerank/rerank.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/cohere/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/cohere/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/google.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/google.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/google.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/google.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro-vision.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro-vision.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/gemini-pro.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/google/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/google/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/groq.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/groq.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/groq.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/groq.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/groq/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/groq/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/huggingface_hub.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/huggingface_hub.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/huggingface_hub/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/huggingface_hub/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/jina.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/jina.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/jina.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/jina.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/rerank/rerank.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/rerank/rerank.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina_tokenizer.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/jina_tokenizer.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/jina/text_embedding/tokenizer/tokenizer.json` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/jina/text_embedding/tokenizer/tokenizer.json`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/localai.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/localai.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/localai/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/localai/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_l_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_l_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_s_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/_assets/icon_s_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab5-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab5-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5s-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab5.5s-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/abab6-chat.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/abab6-chat.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion_pro.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/chat_completion_pro.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/llm/types.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/llm/types.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/minimax.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/minimax.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/minimax.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/minimax.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/minimax/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/minimax/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_l_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_l_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_s_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/_assets/icon_s_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-large-latest.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-large-latest.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-medium-latest.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-medium-latest.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-small-latest.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/mistral-small-latest.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mistral-7b.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mistral-7b.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mixtral-8x7b.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/llm/open-mixtral-8x7b.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/mistralai.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/mistralai.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/mistralai/mistralai.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/mistralai/mistralai.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/model_provider_factory.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/model_provider_factory.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_l_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_l_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_s_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/_assets/icon_s_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/moonshot.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/moonshot.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/moonshot/moonshot.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/moonshot/moonshot.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/ollama.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/ollama.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -86,13 +86,13 @@
           value: llm
       default: 'false'
       type: radio
       required: false
       options:
         - value: 'true'
           label:
-            en_US: Yes
+            en_US: "Yes"
             zh_Hans: 是
         - value: 'false'
           label:
-            en_US: No
+            en_US: "No"
             zh_Hans: 否
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/ollama/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/ollama/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/_common.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/_common.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0125.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0125.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0613.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-0613.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-1106.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-1106.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k-0613.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k-0613.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-16k.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-instruct.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo-instruct.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-3.5-turbo.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-0125-preview.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-0125-preview.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-1106-preview.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-1106-preview.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-32k.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-32k.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-turbo-preview.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-turbo-preview.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-vision-preview.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4-vision-preview.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/gpt-4.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/llm/text-davinci-003.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/llm/text-davinci-003.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/moderation/moderation.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/moderation/moderation.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/openai.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/openai.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/openai.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/openai.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/speech2text/speech2text.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/speech2text/speech2text.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/tts-1-hd.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/tts-1-hd.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/tts-1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/tts-1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai/tts/tts.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai/tts/tts.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/_common.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/_common.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/openai_api_compatible.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/openai_api_compatible.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openai_api_compatible/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openai_api_compatible/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/llm/openllm_generate.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/llm/openllm_generate.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/openllm.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/openllm.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/openllm/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/openllm/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/replicate.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/replicate.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/replicate/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/replicate/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_zh.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/_assets/icon_l_zh.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/_client.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/_client.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-1.5.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-1.5.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-2.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-2.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.5.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.5.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/llm/spark-3.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/spark.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/spark.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/spark/spark.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/spark/spark.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai_square.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/_assets/togetherai_square.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/togetherai/togetherai.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/togetherai/togetherai.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_zh.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_l_zh.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_s_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_assets/icon_s_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/_common.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/_common.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/_client.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/_client.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-1201.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-1201.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-longcontext.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max-longcontext.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-max.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-plus.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-plus.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-turbo.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/llm/qwen-turbo.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tongyi.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tongyi.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tongyi.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tongyi.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tts/tts-1.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tts/tts-1.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/tongyi/tts/tts.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/tongyi/tts/tts.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_zh.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_l_zh.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_s_en.png` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/_assets/icon_s_en.png`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-4.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-4.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-8k.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-8k.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-turbo.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot-turbo.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie-bot.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie_bot.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/ernie_bot.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/wenxin.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/wenxin.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/wenxin/wenxin.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/wenxin/wenxin.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/llm/chatglm3-6b.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/llm/chatglm3-6b.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/llm/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Generator, Iterator
-from typing import Dict, List, Union, cast
+from typing import Dict, List, Union, cast, Type
 
 from openai import (
     APIConnectionError,
     APITimeoutError,
     AuthenticationError,
     ConflictError,
     InternalServerError,
@@ -522,15 +522,16 @@
             raise NotImplementedError(
                 f"xinference model handle type {type(xinference_model)} is not supported"
             )
 
     def _extract_response_tool_calls(
         self,
         response_tool_calls: Union[
-            List[ChatCompletionMessageToolCall, ChoiceDeltaToolCall]
+            List[ChatCompletionMessageToolCall],
+            List[ChoiceDeltaToolCall]
         ],
     ) -> List[AssistantPromptMessage.ToolCall]:
         """
         Extract tool calls from response
 
         :param response_tool_calls: response tool calls
         :return: list of tool calls
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/rerank/rerank.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/rerank/rerank.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/xinference.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/xinference.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/xinference/xinference_helper.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/xinference/xinference_helper.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_zh.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_l_zh.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_s_en.svg` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_assets/icon_s_en.svg`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/_common.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/_common.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite_32k.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_lite_32k.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_pro.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_pro.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_std.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_std.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_turbo.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/chatglm_turbo.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_3_turbo.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_3_turbo.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4v.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/glm_4v.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/llm/llm.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/llm/llm.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/text_embedding.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/text_embedding/text_embedding.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.yaml` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/model_providers/zhipuai/zhipuai.yaml`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/README.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 # Model Runtime
 
-This module provides the interface for invoking and authenticating various models, and offers Dify a unified information and credentials form rule for model providers.
+This module is the loading module that unifies Dify's supplier information and credential form. The project has an OpenAI service forwarding capability at the upper layer, which can support the conversion of supplier services to OpenAI EndPoint calls.
 
-- On one hand, it decouples models from upstream and downstream processes, facilitating horizontal expansion for developers,
-- On the other hand, it allows for direct display of providers and models in the frontend interface by simply defining them in the backend, eliminating the need to modify frontend logic.
+On the basis of the original, this module has added `VIewProfileConfig`, `RESTFulProfileServer`, `OpenAIPluginsClient`, and has rewritten the logic for loading supplier configuration, focusing only on the supplier's configuration. The model configuration and calling logic are implemented in this module, providing a separation of model calls for `Chatchat`. The benefits of doing so are:
+- It changes the decoupling method between the model and the upstream and downstream callers.
+- During development, one does not need to pay attention to the specific implementation of the service provider module, but can simply make calls through the OpenAI EndPoint provided by Model Runtime.
+
+> Please note! Because the model configuration storage module has been removed, the ability to operate suppliers and models on the front-end page has been deleted accordingly. Now, it is only possible to configure suppliers and models through a backend yaml file.
+> Only a supplier configuration details interface is provided, and in the future, we will consider providing a model configuration details interface through other means.
 
 ## Features
 
 - Supports capability invocation for 5 types of models
 
   - `LLM` - LLM text completion, dialogue, pre-computed tokens capability
   - `Text Embedding Model` - Text Embedding, pre-computed tokens capability
   - `Rerank Model` - Segment Rerank capability
   - `Speech-to-text Model` - Speech to text capability
   - `Text-to-speech Model` - Text to speech capability
   - `Moderation` - Moderation capability
 
 - Model provider display
 
-  ![image-20231210143654461](./docs/en_US/images/index/image-20231210143654461.png)
-
   Displays a list of all supported providers, including provider names, icons, supported model types list, predefined model list, configuration method, and credentials form rules, etc. For detailed rule design, see: [Schema](./schema.md).
 
-- Selectable model list display
-
-  ![image-20231210144229650](./docs/en_US/images/index/image-20231210144229650.png)
-
-  After configuring provider/model credentials, the dropdown (application orchestration interface/default model) allows viewing of the available LLM list. Greyed out items represent predefined model lists from providers without configured credentials, facilitating user review of supported models.
-
-  In addition, this list also returns configurable parameter information and rules for LLM, as shown below:
-
-  ![image-20231210144814617](./docs/en_US/images/index/image-20231210144814617.png)	
-
-  These parameters are all defined in the backend, allowing different settings for various parameters supported by different models, as detailed in: [Schema](./docs/en_US/schema.md#ParameterRule).
-
 - Provider/model credential authentication
-
-  ![image-20231210151548521](./docs/en_US/images/index/image-20231210151548521.png)
-
-  ![image-20231210151628992](./docs/en_US/images/index/image-20231210151628992.png)
-
-  The provider list returns configuration information for the credentials form, which can be authenticated through Runtime's interface. The first image above is a provider credential DEMO, and the second is a model credential DEMO.
+  The provider list returns configuration information for the credentials form, which can be authenticated through Runtime's interface. 
 
 ## Structure
 
-![](./docs/en_US/images/index/image-20231210165243632.png)
+![](./docs/en_US/images/index/img.png)
 
 Model Runtime is divided into three layers:
 
-- The outermost layer is the factory method
+- The outermost layer is the OpenAI EndPoint publishing layer
 
-  It provides methods for obtaining all providers, all model lists, getting provider instances, and authenticating provider/model credentials.
+  It provides asynchronous loading configuration `VIewProfileConfig`
+  Supplier service publishing `RESTFulProfileServer`
 
 - The second layer is the provider layer
 
   It provides the current provider's model list, model instance obtaining, provider credential authentication, and provider configuration rule information, **allowing horizontal expansion** to support different providers.
+  For supplier/model credentials, there are two situations:
+  - For centralized suppliers like OpenAI, you need to define authentication credentials like **api_key**.
+  - For locally deployed suppliers like [**Xinference**](https://github.com/xorbitsai/inference), you need to define address credentials like **server_url**. Sometimes you also need to define model type credentials like **model_uid**.
 
 - The bottom layer is the model layer
 
-  It offers direct invocation of various model types, predefined model configuration information, getting predefined/remote model lists, model credential authentication methods. Different models provide additional special methods, like LLM's pre-computed tokens method, cost information obtaining method, etc., **allowing horizontal expansion** for different models under the same provider (within supported model types).
+  It provides direct calls for various model types, predefined model configuration information, obtaining predefined/remote model lists, model credential authentication methods, and different models provide special methods, such as LLM providing pre-computed tokens methods, obtaining cost information methods, etc., **which can be scaled horizontally** for different models under the same supplier (under the supported model types).
+  
+  Here we need to distinguish between model parameters and model credentials first.
 
+  - Model parameters (**defined in this layer**): These are parameters that often need to be changed and adjusted at any time, such as LLM's **max_tokens**, **temperature**, etc. These parameters are adjusted by users on the front-end page, so it is necessary to define the rules of parameters on the backend to facilitate the display and adjustment on the front-end page. In DifyRuntime, their parameter names are generally **model_parameters: Dict[str, any]**.
 
+  - Model credentials (**defined in the supplier layer**): These are parameters that do not often change and generally do not change after configuration, such as **api_key**, **server_url**, etc. In DifyRuntime, their parameter names are generally **credentials: Dict[str, any]**. The credentials of the Provider layer will be directly passed to this layer, and there is no need to define them separately.
 
-## Next Steps
+ 
 
-- Add new provider configuration: [Link](./docs/en_US/provider_scale_out.md)
-- Add new models for existing providers: [Link](./docs/en_US/provider_scale_out.md#AddModel)
-- View YAML configuration rules: [Link](./docs/en_US/schema.md)
-- Implement interface methods: [Link](./docs/en_US/interfaces.md)
+### If you want to implement a custom service provider model capability
+- [Go here 👈🏻](./docs/en_US/interfaces.md)
+- [Details about custom models](./docs/en_US/provider_scale_out.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/README_CN.md` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/README_CN.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,68 @@
+
 # Model Runtime
 
-该模块提供了各模型的调用、鉴权接口，并为 Dify 提供了统一的模型供应商的信息和凭据表单规则。
+该模块是Dify 统一供应商信息和凭据表单的加载模块，此项目在上层做了openai服务转发能力，可以支持对供应商服务转换为 OpenAI EndPoint的调用
+
+该模块在原有的基础上，增加了`VIewProfileConfig`、`RESTFulProfileServer`、`OpenAIPluginsClient`重写了供应商配置加载逻辑，仅关注供应商的配置，
+模型的配置和调用逻辑在本模块实现， 为`Chatchat`提供了模型调用的分离，这样做的好处是：
+- 改变了模型和上下游调用方解耦方式
+- 在开发时，不需要关注服务商模块的具体实现，仅通过Model Runtime提供的OpenAI EndPoint调用即可
 
-- 一方面将模型和上下游解耦，方便开发者对模型横向扩展，
-- 另一方面提供了只需在后端定义供应商和模型，即可在前端页面直接展示，无需修改前端逻辑。
+> 请注意！因为删除了模型配置的存储模块，原本在前端页面操作供应商和模型的能力因此被删除，现在只能通过后端yaml文件配置供应商和模型，
+> 仅提供了供应商的配置详情接口，未来会考虑通过其他方式提供模型的配置详情接口
 
 ## 功能介绍
 
 - 支持 5 种模型类型的能力调用
 
   - `LLM` - LLM 文本补全、对话，预计算 tokens 能力
   - `Text Embedidng Model` - 文本 Embedding ，预计算 tokens 能力
   - `Rerank Model` - 分段 Rerank 能力
   - `Speech-to-text Model` - 语音转文本能力
   - `Text-to-speech Model` - 文本转语音能力
   - `Moderation` - Moderation 能力
 
+### 删除Dify配置页面的情况下，保留了以下功能：
 - 模型供应商展示
+展示所有已支持的供应商列表，除了返回供应商名称、图标之外，还提供了支持的模型类型列表，预定义模型列表、配置方式以及配置凭据的表单规则等等，规则设计详见：[Schema](./docs/zh_Hans/schema.md)。
 
-  ![image-20231210143654461](./docs/zh_Hans/images/index/image-20231210143654461.png)
-
-​	展示所有已支持的供应商列表，除了返回供应商名称、图标之外，还提供了支持的模型类型列表，预定义模型列表、配置方式以及配置凭据的表单规则等等，规则设计详见：[Schema](./docs/zh_Hans/schema.md)。
-
-- 可选择的模型列表展示
-
-  ![image-20231210144229650](./docs/zh_Hans/images/index/image-20231210144229650.png)
-
-​	配置供应商/模型凭据后，可在此下拉（应用编排界面/默认模型）查看可用的 LLM 列表，其中灰色的为未配置凭据供应商的预定义模型列表，方便用户查看已支持的模型。
-
-​	除此之外，该列表还返回了 LLM 可配置的参数信息和规则，如下图：
-
-​	![image-20231210144814617](./docs/zh_Hans/images/index/image-20231210144814617.png)	
-
-​	这里的参数均为后端定义，相比之前只有 5 种固定参数，这里可为不同模型设置所支持的各种参数，详见：[Schema](./docs/zh_Hans/schema.md#ParameterRule)。
-
-- 供应商/模型凭据鉴权
-
-  ![image-20231210151548521](./docs/zh_Hans/images/index/image-20231210151548521.png)
-
-![image-20231210151628992](./docs/zh_Hans/images/index/image-20231210151628992.png)
-
-​	供应商列表返回了凭据表单的配置信息，可通过 Runtime 提供的接口对凭据进行鉴权，上图 1 为供应商凭据 DEMO，上图 2 为模型凭据 DEMO。
+- 供应商/模型凭据鉴权 
+ 供应商列表返回了凭据表单的配置信息，可通过 Runtime 提供的接口对凭据进行鉴权， 
 
 ## 结构
 
-![](./docs/zh_Hans/images/index/image-20231210165243632.png)
+![](./docs/zh_Hans/images/index/img.png)
 
 Model Runtime 分三层：
 
-- 最外层为工厂方法
+- 最外层为OpenAI EndPoint发布层
 
-  提供获取所有供应商、所有模型列表、获取供应商实例、供应商/模型凭据鉴权方法。
+  提供异步加载配置`VIewProfileConfig`
+  供应商服务发布`RESTFulProfileServer` 
 
 - 第二层为供应商层
 
   提供获取当前供应商模型列表、获取模型实例、供应商凭据鉴权、供应商配置规则信息，**可横向扩展**以支持不同的供应商。
 
   对于供应商/模型凭据，有两种情况
   - 如OpenAI这类中心化供应商，需要定义如**api_key**这类的鉴权凭据
-  - 如[**Xinference**](https://github.com/xorbitsai/inference)这类本地部署的供应商，需要定义如**server_url**这类的地址凭据，有时候还需要定义**model_uid**之类的模型类型凭据，就像下面这样，当在供应商层定义了这些凭据后，就可以在前端页面上直接展示，无需修改前端逻辑。
-  ![Alt text](docs/zh_Hans/images/index/image.png)
-
-  当配置好凭据后，就可以通过DifyRuntime的外部接口直接获取到对应供应商所需要的**Schema**（凭据表单规则），从而在可以在不修改前端逻辑的情况下，提供新的供应商/模型的支持。
-
+  - 如[**Xinference**](https://github.com/xorbitsai/inference)这类本地部署的供应商，需要定义如**server_url**这类的地址凭据，有时候还需要定义**model_uid**之类的模型类型凭据， 
+ 
 - 最底层为模型层
 
   提供各种模型类型的直接调用、预定义模型配置信息、获取预定义/远程模型列表、模型凭据鉴权方法，不同模型额外提供了特殊方法，如 LLM 提供预计算 tokens 方法、获取费用信息方法等，**可横向扩展**同供应商下不同的模型（支持的模型类型下）。
 
   在这里我们需要先区分模型参数与模型凭据。
 
   - 模型参数(**在本层定义**)：这是一类经常需要变动，随时调整的参数，如 LLM 的 **max_tokens**、**temperature** 等，这些参数是由用户在前端页面上进行调整的，因此需要在后端定义参数的规则，以便前端页面进行展示和调整。在DifyRuntime中，他们的参数名一般为**model_parameters: Dict[str, any]**。
 
   - 模型凭据(**在供应商层定义**)：这是一类不经常变动，一般在配置好后就不会再变动的参数，如 **api_key**、**server_url** 等。在DifyRuntime中，他们的参数名一般为**credentials: Dict[str, any]**，Provider层的credentials会直接被传递到这一层，不需要再单独定义。
 
-## 下一步
-
-### [增加新的供应商配置 👈🏻](./docs/zh_Hans/provider_scale_out.md)
-当添加后，这里将会出现一个新的供应商
-
-![Alt text](docs/zh_Hans/images/index/image-1.png)
-
-### [为已存在的供应商新增模型 👈🏻](./docs/zh_Hans/provider_scale_out.md#增加模型)
-当添加后，对应供应商的模型列表中将会出现一个新的预定义模型供用户选择，如GPT-3.5 GPT-4 ChatGLM3-6b等，而对于支持自定义模型的供应商，则不需要新增模型。
-
-![Alt text](docs/zh_Hans/images/index/image-2.png)
+ 
+ 
 
-### [接口的具体实现 👈🏻](./docs/zh_Hans/interfaces.md)
-你可以在这里找到你想要查看的接口的具体实现，以及接口的参数和返回值的具体含义。
+ 
+### 如果你想实现自定义的服务商模型能力
+- [移步这里 👈🏻](./docs/zh_Hans/interfaces.md)
+- [关于自定义模型的细节](./docs/zh_Hans/provider_scale_out.md)
+
```

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/common_validator.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/common_validator.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/model_credential_schema_validator.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/model_credential_schema_validator.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/schema_validators/provider_credential_schema_validator.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/schema_validators/provider_credential_schema_validator.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/utils/_compat.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/model_runtime/utils/encoders.py` & `model_providers-0.3.0.20240506/model_providers/core/model_runtime/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/provider_manager.py` & `model_providers-0.3.0.20240506/model_providers/core/provider_manager.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/utils/generic.py` & `model_providers-0.3.0.20240506/model_providers/core/utils/generic.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/utils/position_helper.py` & `model_providers-0.3.0.20240506/model_providers/core/utils/position_helper.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/core/utils/utils.py` & `model_providers-0.3.0.20240506/model_providers/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/errors/error.py` & `model_providers-0.3.0.20240506/model_providers/errors/error.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/extensions/ext_redis.py` & `model_providers-0.3.0.20240506/model_providers/extensions/ext_redis.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/model_providers/extensions/ext_storage.py` & `model_providers-0.3.0.20240506/model_providers/extensions/ext_storage.py`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/pyproject.toml` & `model_providers-0.3.0.20240506/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-providers"
-version = "0.3.0"
+version = "0.3.0.20240506"
 description = ""
 authors = ["glide-the <2533736852@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12,!=3.9.7"
 transformers = "4.31.0"
@@ -17,29 +17,33 @@
 # config manage
 omegaconf = "2.0.6"
 # modle_runtime
 openai = "1.13.3"
 tiktoken = "0.5.2"
 pydub = "0.25.1"
 boto3 = "1.28.17"
+
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
+pytest-cov = "^4.0.0"
+pytest-dotenv = "^0.5.2"
+duckdb-engine = "^0.9.2"
+pytest-watcher = "^0.2.6"
 freezegun = "^1.2.2"
-pytest-mock = "^3.10.0"
+responses = "^0.22.0"
+pytest-asyncio = "^0.23.2"
+lark = "^1.1.5"
+pandas = "^2.0.0"
+pytest-mock  = "^3.10.0"
+pytest-socket = "^0.6.0"
 syrupy = "^4.0.2"
-pytest-watcher = "^0.3.4"
-pytest-asyncio = "^0.21.1"
-grandalf = "^0.8"
-pytest-profiling = "^1.7.0"
-responses = "^0.25.0"
-langchain = "0.1.5"
-langchain-openai = "0.0.5"
+requests-mock = "^1.11.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
@@ -200,8 +204,8 @@
 ignore-words-list = 'momento,collison,ned,foor,reworkd,parth,whats,aapply,mysogyny,unsecure,damon,crate,aadd,symbl,precesses,accademia,nin'
 
 
 # https://python-poetry.org/docs/repositories/
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
-priority = "default" 
+priority = "default"
```

### Comparing `model_providers-0.3.0/README.md` & `model_providers-0.3.0.20240506/README.md`

 * *Files identical despite different names*

### Comparing `model_providers-0.3.0/PKG-INFO` & `model_providers-0.3.0.20240506/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-providers
-Version: 0.3.0
+Version: 0.3.0.20240506
 Summary: 
 Author: glide-the
 Author-email: 2533736852@qq.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.12.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

