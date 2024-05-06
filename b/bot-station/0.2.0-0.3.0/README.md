# Comparing `tmp/bot_station-0.2.0.tar.gz` & `tmp/bot_station-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station-0.2.0.tar", last modified: Sat May  4 20:17:32 2024, max compression
+gzip compressed data, was "bot_station-0.3.0.tar", last modified: Mon May  6 05:52:57 2024, max compression
```

## Comparing `bot_station-0.2.0.tar` & `bot_station-0.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.912894 bot_station-0.2.0/
--rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-04 19:54:11.000000 bot_station-0.2.0/LICENSE
--rw-r--r--   0 mmarashan (1826057312) 593637566      697 2024-05-04 20:17:32.912692 bot_station-0.2.0/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566       17 2024-05-04 19:54:11.000000 bot_station-0.2.0/README.md
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.904586 bot_station-0.2.0/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.905424 bot_station-0.2.0/bot_station/api/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.905619 bot_station-0.2.0/bot_station/api/rest/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     6728 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/api.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.906830 bot_station-0.2.0/bot_station/api/rest/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_call_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      437 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_creation_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_creation_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_train_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/bot_train_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/api/rest/model/web_app_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.906964 bot_station-0.2.0/bot_station/data/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.907056 bot_station-0.2.0/bot_station/data/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/base/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.907381 bot_station-0.2.0/bot_station/data/base/database/
--rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/base/database/UUID.py
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/base/database/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/base/database/base_db_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.907836 bot_station-0.2.0/bot_station/data/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      992 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/bot_factory_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     7893 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/bot_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/chat_message_storage_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.908080 bot_station-0.2.0/bot_station/data/bot/mapper/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/mapper/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      887 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/mapper/document_mapper.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.908327 bot_station-0.2.0/bot_station/data/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      238 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot/model/yandex_cloud_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.908859 bot_station-0.2.0/bot_station/data/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     3035 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot_station/bot_registry_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.909238 bot_station-0.2.0/bot_station/data/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      750 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/data/bot_station/model/bot_info_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.909591 bot_station-0.2.0/bot_station/di/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/di/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1268 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/di/bot_station_module.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.909762 bot_station-0.2.0/bot_station/domain/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.910107 bot_station-0.2.0/bot_station/domain/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/base/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      544 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/base/const.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/base/utils.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.910559 bot_station-0.2.0/bot_station/domain/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      673 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/bot.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      267 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/bot_factory.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/chat_message_storage.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.911315 bot_station-0.2.0/bot_station/domain/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      143 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/model/document.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      350 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/model/lm_bot_meta_info.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/model/lm_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/model/lm_chat_message.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot/model/lm_train_data.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.911643 bot_station-0.2.0/bot_station/domain/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      692 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot_station/bot_registry.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2509 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot_station/bot_station.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.911856 bot_station-0.2.0/bot_station/domain/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      240 2024-05-04 19:54:11.000000 bot_station-0.2.0/bot_station/domain/bot_station/model/bot_creation_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.912449 bot_station-0.2.0/bot_station.egg-info/
--rw-r--r--   0 mmarashan (1826057312) 593637566      697 2024-05-04 20:17:32.000000 bot_station-0.2.0/bot_station.egg-info/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566     2363 2024-05-04 20:17:32.000000 bot_station-0.2.0/bot_station.egg-info/SOURCES.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-04 20:17:32.000000 bot_station-0.2.0/bot_station.egg-info/dependency_links.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-04 20:17:32.000000 bot_station-0.2.0/bot_station.egg-info/requires.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-04 20:17:32.000000 bot_station-0.2.0/bot_station.egg-info/top_level.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-04 20:17:32.912938 bot_station-0.2.0/setup.cfg
--rw-r--r--   0 mmarashan (1826057312) 593637566      768 2024-05-04 19:54:11.000000 bot_station-0.2.0/setup.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-04 20:17:32.912234 bot_station-0.2.0/tests/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-04 19:54:11.000000 bot_station-0.2.0/tests/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     3334 2024-05-04 19:54:11.000000 bot_station-0.2.0/tests/bot_station_api_test.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1051 2024-05-04 19:54:11.000000 bot_station-0.2.0/tests/test_bot_factory.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723927 bot_station-0.3.0/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     1070 2024-05-05 19:58:38.000000 bot_station-0.3.0/LICENSE
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      707 2024-05-06 05:52:57.723743 bot_station-0.3.0/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       17 2024-05-05 19:58:38.000000 bot_station-0.3.0/README.md
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.716646 bot_station-0.3.0/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.717454 bot_station-0.3.0/bot_station/api/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.717665 bot_station-0.3.0/bot_station/api/rest/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     6751 2024-05-06 05:45:03.000000 bot_station-0.3.0/bot_station/api/rest/api.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.718894 bot_station-0.3.0/bot_station/api/rest/model/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      257 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_call_dto.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      331 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      486 2024-05-06 05:44:47.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_creation_dto.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      126 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_creation_result.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      433 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_dto.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      391 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_train_dto.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       90 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_train_result.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      204 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/web_app_config.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719017 bot_station-0.3.0/bot_station/data/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719120 bot_station-0.3.0/bot_station/data/base/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719452 bot_station-0.3.0/bot_station/data/base/database/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      975 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/database/UUID.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/database/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      428 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/database/base_db_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719888 bot_station-0.3.0/bot_station/data/bot/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      992 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/bot_factory_impl.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     7893 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/bot_impl.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     2169 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/chat_message_storage_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720086 bot_station-0.3.0/bot_station/data/bot/mapper/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/mapper/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      887 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/mapper/document_mapper.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720280 bot_station-0.3.0/bot_station/data/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      238 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/model/yandex_cloud_config.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720499 bot_station-0.3.0/bot_station/data/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      508 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     3061 2024-05-06 05:42:48.000000 bot_station-0.3.0/bot_station/data/bot_station/bot_registry_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720707 bot_station-0.3.0/bot_station/data/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      853 2024-05-06 05:42:37.000000 bot_station-0.3.0/bot_station/data/bot_station/model/bot_info_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720922 bot_station-0.3.0/bot_station/di/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/di/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     1268 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/di/bot_station_module.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.721036 bot_station-0.3.0/bot_station/domain/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.721355 bot_station-0.3.0/bot_station/domain/base/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/base/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      544 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/base/const.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      391 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/base/utils.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.721764 bot_station-0.3.0/bot_station/domain/bot/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      673 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/bot.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      267 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/bot_factory.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      798 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/chat_message_storage.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.722417 bot_station-0.3.0/bot_station/domain/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      143 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/document.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      350 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_bot_meta_info.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      254 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      361 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_chat_message.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      379 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_train_data.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.722738 bot_station-0.3.0/bot_station/domain/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      692 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/bot_registry.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     2509 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/bot_station.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723031 bot_station-0.3.0/bot_station/domain/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      279 2024-05-06 05:37:14.000000 bot_station-0.3.0/bot_station/domain/bot_station/model/bot_creation_config.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723534 bot_station-0.3.0/bot_station.egg-info/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      707 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     2363 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/SOURCES.txt
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        1 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/dependency_links.txt
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      190 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/requires.txt
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       18 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/top_level.txt
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       38 2024-05-06 05:52:57.723964 bot_station-0.3.0/setup.cfg
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      778 2024-05-06 05:51:27.000000 bot_station-0.3.0/setup.py
+drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723368 bot_station-0.3.0/tests/
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/tests/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     3334 2024-05-05 19:58:38.000000 bot_station-0.3.0/tests/bot_station_api_test.py
+-rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     1051 2024-05-05 19:58:38.000000 bot_station-0.3.0/tests/test_bot_factory.py
```

### Comparing `bot_station-0.2.0/LICENSE` & `bot_station-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/PKG-INFO` & `bot_station-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.2.0
-Summary: Bot Station SDK
+Version: 0.3.0
+Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bot_station-0.2.0/bot_station/api/rest/api.py` & `bot_station-0.3.0/bot_station/api/rest/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     @staticmethod
     def launch():
         run_server()
 
     @staticmethod
     async def create(dto: BotCreationDto) -> str:
         config = BotCreationConfig(
+            id=dto.id,
             name=dto.name,
             description=dto.description,
             prompt_intro=dto.prompt_intro,
             add_external_context_to_prompt=dto.add_external_context_to_prompt,
             add_messages_history_to_prompt=dto.add_messages_history_to_prompt,
             temperature=dto.temperature,
         )
```

### Comparing `bot_station-0.2.0/bot_station/data/base/database/UUID.py` & `bot_station-0.3.0/bot_station/data/base/database/UUID.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/data/bot/bot_factory_impl.py` & `bot_station-0.3.0/bot_station/data/bot/bot_factory_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/data/bot/bot_impl.py` & `bot_station-0.3.0/bot_station/data/bot/bot_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/data/bot/chat_message_storage_impl.py` & `bot_station-0.3.0/bot_station/data/bot/chat_message_storage_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/data/bot/mapper/document_mapper.py` & `bot_station-0.3.0/bot_station/data/bot/mapper/document_mapper.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/data/bot_station/bot_registry_impl.py` & `bot_station-0.3.0/bot_station/data/bot_station/bot_registry_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class BotRegistryImpl(BotRegistry):
     __engine = create_engine(db_path, echo=True)
     __storage = {}
 
     async def create(self, config: BotCreationConfig) -> LMBotMetaInfo:
         session = Session(self.__engine)
         dto = BotInfoDto(
+            id=config.id,
             name=config.name,
             description=config.description,
             prompt_intro=config.prompt_intro,
             add_external_context_to_prompt=config.add_external_context_to_prompt,
             add_messages_history_to_prompt=config.add_messages_history_to_prompt,
             temperature=config.temperature,
         )
```

### Comparing `bot_station-0.2.0/bot_station/data/bot_station/model/bot_info_dto.py` & `bot_station-0.3.0/bot_station/data/bot_station/model/bot_info_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import uuid
+
 from sqlalchemy import String, Float, Boolean
 from sqlalchemy.orm import Mapped, mapped_column
 
 from bot_station.data.base.database.base_db_dto import BaseDBDto
 
 
 class BotInfoDto(BaseDBDto):
     __tablename__ = "bot_meta_info"
 
+    id: Mapped[str] = mapped_column("id", String(), primary_key=True, default=uuid.uuid4)
     name: Mapped[str] = mapped_column(String())
     description: Mapped[str] = mapped_column(String())
     temperature: Mapped[float] = mapped_column(Float())
     prompt_intro: Mapped[str] = mapped_column(String())
     add_external_context_to_prompt: Mapped[bool] = mapped_column(Boolean())
     add_messages_history_to_prompt: Mapped[bool] = mapped_column(Boolean())
```

### Comparing `bot_station-0.2.0/bot_station/di/bot_station_module.py` & `bot_station-0.3.0/bot_station/di/bot_station_module.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/domain/base/const.py` & `bot_station-0.3.0/bot_station/domain/base/const.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/domain/bot/bot.py` & `bot_station-0.3.0/bot_station/domain/bot/bot.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/domain/bot/chat_message_storage.py` & `bot_station-0.3.0/bot_station/domain/bot/chat_message_storage.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/domain/bot_station/bot_registry.py` & `bot_station-0.3.0/bot_station/domain/bot_station/bot_registry.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station/domain/bot_station/bot_station.py` & `bot_station-0.3.0/bot_station/domain/bot_station/bot_station.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/bot_station.egg-info/PKG-INFO` & `bot_station-0.3.0/bot_station.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.2.0
-Summary: Bot Station SDK
+Version: 0.3.0
+Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bot_station-0.2.0/bot_station.egg-info/SOURCES.txt` & `bot_station-0.3.0/bot_station.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/tests/bot_station_api_test.py` & `bot_station-0.3.0/tests/bot_station_api_test.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.2.0/tests/test_bot_factory.py` & `bot_station-0.3.0/tests/test_bot_factory.py`

 * *Files identical despite different names*

