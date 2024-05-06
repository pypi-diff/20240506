# Comparing `tmp/holytools-0.9.3.tar.gz` & `tmp/holytools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holytools-0.9.3.tar", last modified: Mon Apr 29 12:31:23 2024, max compression
+gzip compressed data, was "holytools-0.9.4.tar", last modified: Mon May  6 19:05:36 2024, max compression
```

## Comparing `holytools-0.9.3.tar` & `holytools-0.9.4.tar`

### file list

```diff
@@ -1,121 +1,124 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2024-04-26 10:13:20.000000 holytools-0.9.3/LICENSE.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2818 2024-04-29 12:31:23.945153 holytools-0.9.3/PKG-INFO
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.933152 holytools-0.9.3/holytools/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.933152 holytools-0.9.3/holytools/abstract/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      704 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/enum.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/abstract/serialization/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      139 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      805 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/dillable.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4388 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/jsondataclass.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      903 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/serializable.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/abstract/tree/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       32 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/tree/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3393 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/tree/node.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/configs/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       51 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/configs/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1846 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/configs/abstr.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2617 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/configs/impl.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/crypto/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       42 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/crypto/encrypt/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       41 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2117 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/aes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/algo.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2041 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/rsa.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/crypto/hash/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/hash/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      828 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/hash/salt.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      643 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/hash/sha.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/devtools/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/devtools/inspection/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       93 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/inspection/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/inspection/module_inspect.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1354 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/inspection/type_inspect.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/devtools/test/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       62 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2065 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/cases.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/configurable_unit.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4783 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/results.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4066 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/unit.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/events/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      169 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1373 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/countdown.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      682 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/input_waiter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3133 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/task_scheduler.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/timer.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/file/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       57 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/file/mock/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1557 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/file_mock.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1024 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.bin
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   171225 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.csv
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   102796 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.jpg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13264 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.pdf
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2670 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.png
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   775192 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.wav
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/file/types/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      190 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1252 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/binary.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2152 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/file.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4855 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/image.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      950 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/plaintext.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/fsys/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      116 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5213 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/fsys_node.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1821 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/location_manager.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2516 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/resource.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1715 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/save_manager.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/display/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2151 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/display.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3953 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/grid_draw.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3162 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/types.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/input/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       84 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/input/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/input/keyboard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2137 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/input/mouse.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/memory/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3265 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/drives.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      827 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/ram.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2260 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/usage.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/microphone/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/microphone/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/microphone/recorder.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/logging/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      149 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/customlogger.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1825 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/interface.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/log_settings.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/network/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       87 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5058 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/adapter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      969 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/endpoint.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2221 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/ip.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/userIO/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       61 2024-04-29 12:23:52.000000 holytools-0.9.3/holytools/userIO/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4140 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/userIO/cli.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2319 2024-04-29 12:29:15.000000 holytools-0.9.3/holytools/userIO/progr.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/web/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1293 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/link_soup.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2145 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/search_engine.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3690 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/site_visitor.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2818 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2947 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      166 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       10 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-29 12:31:01.000000 holytools-0.9.3/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2072 2024-04-26 10:13:20.000000 holytools-0.9.3/readme.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      166 2024-04-29 12:28:15.000000 holytools-0.9.3/requirements.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-29 12:31:23.945153 holytools-0.9.3/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.834800 holytools-0.9.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2024-04-26 10:13:20.000000 holytools-0.9.4/LICENSE.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2842 2024-05-06 19:05:36.834800 holytools-0.9.4/PKG-INFO
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.810800 holytools-0.9.4/holytools/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.814800 holytools-0.9.4/holytools/abstract/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/abstract/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      704 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/abstract/enum.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.814800 holytools-0.9.4/holytools/abstract/serialization/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      139 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/abstract/serialization/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      817 2024-05-04 18:20:59.000000 holytools-0.9.4/holytools/abstract/serialization/dillable.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4388 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/abstract/serialization/jsondataclass.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1748 2024-05-02 18:36:44.000000 holytools-0.9.4/holytools/abstract/serialization/serializable.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.814800 holytools-0.9.4/holytools/abstract/tree/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       32 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/abstract/tree/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3422 2024-05-03 20:53:17.000000 holytools-0.9.4/holytools/abstract/tree/node.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.814800 holytools-0.9.4/holytools/configs/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       58 2024-05-01 17:40:32.000000 holytools-0.9.4/holytools/configs/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2873 2024-05-01 17:49:08.000000 holytools-0.9.4/holytools/configs/base.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2692 2024-05-01 17:46:56.000000 holytools-0.9.4/holytools/configs/configs.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.814800 holytools-0.9.4/holytools/crypto/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       42 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.818800 holytools-0.9.4/holytools/crypto/encrypt/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       41 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/encrypt/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2117 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/encrypt/aes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/encrypt/algo.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2041 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/encrypt/rsa.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.818800 holytools-0.9.4/holytools/crypto/hash/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/hash/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      828 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/hash/salt.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      643 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/crypto/hash/sha.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.818800 holytools-0.9.4/holytools/devtools/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       70 2024-05-04 18:27:23.000000 holytools-0.9.4/holytools/devtools/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.818800 holytools-0.9.4/holytools/devtools/inspection/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       93 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/inspection/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/inspection/module_inspect.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1354 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/inspection/type_inspect.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.818800 holytools-0.9.4/holytools/devtools/profiling/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       34 2024-05-04 18:27:23.000000 holytools-0.9.4/holytools/devtools/profiling/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1730 2024-05-04 23:36:03.000000 holytools-0.9.4/holytools/devtools/profiling/profilable.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.818800 holytools-0.9.4/holytools/devtools/test/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       62 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/test/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2065 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/test/cases.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/test/configurable_unit.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4783 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/devtools/test/results.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4066 2024-05-05 16:12:24.000000 holytools-0.9.4/holytools/devtools/test/unit.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.822800 holytools-0.9.4/holytools/events/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      169 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/events/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1373 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/events/countdown.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      682 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/events/input_waiter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3133 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/events/task_scheduler.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      810 2024-05-02 18:08:36.000000 holytools-0.9.4/holytools/events/timer.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.822800 holytools-0.9.4/holytools/file/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       57 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.822800 holytools-0.9.4/holytools/file/mock/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1557 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/file_mock.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1024 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.bin
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   171225 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.csv
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   102796 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.jpg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13264 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.pdf
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2670 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.png
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   775192 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/mock/mock.wav
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/file/types/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      190 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/types/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1252 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/types/binary.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2152 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/types/file.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4855 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/file/types/image.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1095 2024-05-01 12:17:53.000000 holytools-0.9.4/holytools/file/types/plaintext.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/fsys/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      116 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/fsys/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5213 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/fsys/fsys_node.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1821 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/fsys/location_manager.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2516 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/fsys/resource.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1642 2024-05-01 18:00:27.000000 holytools-0.9.4/holytools/fsys/save_manager.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/hardware/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/hardware/display/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/display/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2151 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/display/display.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3953 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/display/grid_draw.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3162 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/display/types.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/hardware/input/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       84 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/input/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/input/keyboard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2137 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/input/mouse.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/hardware/memory/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/memory/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3265 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/memory/drives.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      827 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/memory/ram.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2260 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/memory/usage.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/hardware/microphone/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/microphone/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/hardware/microphone/recorder.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.830800 holytools-0.9.4/holytools/logging/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      149 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/logging/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/logging/customlogger.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1825 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/logging/interface.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/logging/log_settings.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.834800 holytools-0.9.4/holytools/network/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       87 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/network/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5058 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/network/adapter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      969 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/network/endpoint.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2221 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/network/ip.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.834800 holytools-0.9.4/holytools/userIO/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       61 2024-04-29 12:23:52.000000 holytools-0.9.4/holytools/userIO/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4140 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/userIO/cli.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2278 2024-05-03 23:50:41.000000 holytools-0.9.4/holytools/userIO/progr.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.834800 holytools-0.9.4/holytools/web/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/web/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1293 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/web/link_soup.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2145 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/web/search_engine.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3690 2024-04-26 10:13:20.000000 holytools-0.9.4/holytools/web/site_visitor.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-06 19:05:36.834800 holytools-0.9.4/holytools.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2842 2024-05-06 19:05:36.000000 holytools-0.9.4/holytools.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3033 2024-05-06 19:05:36.000000 holytools-0.9.4/holytools.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-06 19:05:36.000000 holytools-0.9.4/holytools.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      175 2024-05-06 19:05:36.000000 holytools-0.9.4/holytools.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       10 2024-05-06 19:05:36.000000 holytools-0.9.4/holytools.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-05-06 19:04:29.000000 holytools-0.9.4/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2072 2024-04-26 10:13:20.000000 holytools-0.9.4/readme.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      175 2024-05-04 18:24:56.000000 holytools-0.9.4/requirements.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-06 19:05:36.834800 holytools-0.9.4/setup.cfg
```

### Comparing `holytools-0.9.3/LICENSE.txt` & `holytools-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/PKG-INFO` & `holytools-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holytools
-Version: 0.9.3
+Version: 0.9.4
 Summary: Collection of general python utilities for future projects
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Project-URL: repository, https://github.com/Somerandomguy10111/holytools
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: func_timeout
@@ -19,14 +19,15 @@
 Requires-Dist: orjson
 Requires-Dist: mss
 Requires-Dist: screeninfo
 Requires-Dist: pynput
 Requires-Dist: pillow
 Requires-Dist: configobj
 Requires-Dist: progressbar2
+Requires-Dist: tabulate
 
 ## Holytools
 A collection of general utilities in various very general areas that aim for simplicity in use. 
 Functionalities include:
 
 - object serialization -> holytools.abstract.serialization
 - fileIO and mock files -> holytools.file
```

### Comparing `holytools-0.9.3/holytools/abstract/enum.py` & `holytools-0.9.4/holytools/abstract/enum.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/abstract/serialization/dillable.py` & `holytools-0.9.4/holytools/abstract/serialization/dillable.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,8 +27,8 @@
             self.data = data
 
     original = Example(data="Sample data")
     test_dill_str = original.to_str()
     restored = Example.from_str(test_dill_str)
 
     print(f"Original: {original.data}")
-    print(f"Restored: {restored.data}")
+    print(f"Restored: {restored._execution_times}")
```

### Comparing `holytools-0.9.3/holytools/abstract/serialization/jsondataclass.py` & `holytools-0.9.4/holytools/abstract/serialization/jsondataclass.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/abstract/tree/node.py` & `holytools-0.9.4/holytools/abstract/tree/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         root_size = 0
         return Tree(get_subdict(node=self, depth=0))
 
     # -------------------------------------------
     # descendants
 
     def get_subnodes(self, *args, **kwargs) -> list[TreeNode]:
+        _, __ = args, kwargs
         subnodes = []
         for child in self.get_child_nodes():
             subnodes.append(child)
             subnodes += child.get_subnodes()
         return subnodes
 
     @abstractmethod
```

### Comparing `holytools-0.9.3/holytools/configs/impl.py` & `holytools-0.9.4/holytools/configs/configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import os.path
 from configobj import ConfigObj
 
 import subprocess
 from typing import Optional
 from holytools.logging import LogLevel
-from holytools.configs.abstr import Configs, DictType
+from holytools.configs.base import BaseConfigs, DictType
 
 # ---------------------------------------------------------
 
 
-class FileConfigs(Configs):
+class FileConfigs(BaseConfigs):
     def __init__(self, config_fpath : str = '~/.pyconfig'):
         self._config_fpath: str = as_absolute(path=config_fpath)
         config_dirpath = os.path.dirname(self._config_fpath)
         os.makedirs(config_dirpath, exist_ok=True)
         super().__init__()
 
     def _retrieve_map(self) -> ConfigObj:
         self.log(f'Initialized {self.__class__.__name__} with config file at \"{self._config_fpath}\"')
         return ConfigObj(self._config_fpath)
 
-    def update_config_resouce(self, key : str, value : str):
+    def update_config_resouce(self, key : str, value : str, section : Optional[str] = None):
         self._map.write()
 
 
-class PassConfigs(Configs):
+class PassConfigs(BaseConfigs):
     def __init__(self, pass_dirpath : str = '~/.password-store' ):
         self._pass_dirpath: str = as_absolute(path=pass_dirpath)
         os.environ['PASSWORD_STORE_DIR'] = pass_dirpath
         super().__init__()
 
-    def update_config_resouce(self, key : str, value : str):
+    def update_config_resouce(self, key : str, value : str, section : Optional[str] = None):
         insert_command = f"echo \"{value}\" | pass insert --echo {key}"
         self.try_run_cmd(cmd=insert_command)
 
     def _retrieve_map(self) -> DictType:
         keys = self.get_keys()
         config_map = {}
         for k in keys:
```

### Comparing `holytools-0.9.3/holytools/crypto/encrypt/aes.py` & `holytools-0.9.4/holytools/crypto/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/crypto/encrypt/rsa.py` & `holytools-0.9.4/holytools/crypto/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/crypto/hash/salt.py` & `holytools-0.9.4/holytools/crypto/hash/salt.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/crypto/hash/sha.py` & `holytools-0.9.4/holytools/crypto/hash/sha.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/devtools/inspection/module_inspect.py` & `holytools-0.9.4/holytools/devtools/inspection/module_inspect.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/devtools/inspection/type_inspect.py` & `holytools-0.9.4/holytools/devtools/inspection/type_inspect.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/devtools/test/cases.py` & `holytools-0.9.4/holytools/devtools/test/cases.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/devtools/test/results.py` & `holytools-0.9.4/holytools/devtools/test/results.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/devtools/test/unit.py` & `holytools-0.9.4/holytools/devtools/test/unit.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/events/countdown.py` & `holytools-0.9.4/holytools/events/countdown.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/events/input_waiter.py` & `holytools-0.9.4/holytools/events/input_waiter.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/events/task_scheduler.py` & `holytools-0.9.4/holytools/events/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/mock/file_mock.py` & `holytools-0.9.4/holytools/file/mock/file_mock.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/mock/mock.csv` & `holytools-0.9.4/holytools/file/mock/mock.csv`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/mock/mock.jpg` & `holytools-0.9.4/holytools/file/mock/mock.jpg`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/mock/mock.pdf` & `holytools-0.9.4/holytools/file/mock/mock.pdf`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/mock/mock.png` & `holytools-0.9.4/holytools/file/mock/mock.png`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/mock/mock.wav` & `holytools-0.9.4/holytools/file/mock/mock.wav`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/types/binary.py` & `holytools-0.9.4/holytools/file/types/binary.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/types/file.py` & `holytools-0.9.4/holytools/file/types/file.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/types/image.py` & `holytools-0.9.4/holytools/file/types/image.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/file/types/plaintext.py` & `holytools-0.9.4/holytools/file/types/plaintext.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,7 +20,13 @@
         content = self.read()
         print(content)
 
     @classmethod
     def get_non_plaintext_formats(cls) -> list[str]:
         return [".doc", ".docx", ".eml", ".epub", ".gif", ".jpg", ".jpeg", ".json", ".html", ".htm",
                     ".msg", ".odt", ".ogg", ".pdf", ".png", ".pptx", ".ps", ".rtf", ".xlsx", ".xls"]
+
+    @classmethod
+    def get_text(cls, fpath : str) -> str:
+        with open(fpath, 'r') as f:
+            text = f.read()
+        return text
```

### Comparing `holytools-0.9.3/holytools/fsys/fsys_node.py` & `holytools-0.9.4/holytools/fsys/fsys_node.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/fsys/location_manager.py` & `holytools-0.9.4/holytools/fsys/location_manager.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/fsys/resource.py` & `holytools-0.9.4/holytools/fsys/resource.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/fsys/save_manager.py` & `holytools-0.9.4/holytools/fsys/save_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,21 +32,20 @@
         parts = fpath.split('.')
         if len(parts) > 1:
             return parts[-1]
         else:
             return None
 
     @staticmethod
-    def get_free_path(save_dirpath : str, name : str, suffix : Optional[str] = None, start_zero_indexed : bool = False) -> str:
+    def get_free_path(save_dirpath: str, name: str, suffix: Optional[str] = None, start_index: int = 1) -> str:
         if suffix:
             if not suffix.startswith('.'):
                 suffix = f'.{suffix}'
 
-        start_index = 0 if start_zero_indexed else None
-        def get_path(index : int = start_index):
+        def get_path(index: int = start_index):
             conditional_suffix = '' if suffix is None else f'{suffix}'
             conditional_index = f'_{index}' if not index is None else ''
             return os.path.join(save_dirpath, f'{name}{conditional_index}{conditional_suffix}')
 
         fpath = get_path()
         current_index = 0
         while os.path.isfile(path=fpath) or os.path.isdir(fpath):
```

### Comparing `holytools-0.9.3/holytools/hardware/display/display.py` & `holytools-0.9.4/holytools/hardware/display/display.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/display/grid_draw.py` & `holytools-0.9.4/holytools/hardware/display/grid_draw.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/display/types.py` & `holytools-0.9.4/holytools/hardware/display/types.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/input/keyboard.py` & `holytools-0.9.4/holytools/hardware/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/input/mouse.py` & `holytools-0.9.4/holytools/hardware/input/mouse.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/memory/drives.py` & `holytools-0.9.4/holytools/hardware/memory/drives.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/memory/ram.py` & `holytools-0.9.4/holytools/hardware/memory/ram.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/memory/usage.py` & `holytools-0.9.4/holytools/hardware/memory/usage.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/hardware/microphone/recorder.py` & `holytools-0.9.4/holytools/hardware/microphone/recorder.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/logging/customlogger.py` & `holytools-0.9.4/holytools/logging/customlogger.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/logging/interface.py` & `holytools-0.9.4/holytools/logging/interface.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/logging/log_settings.py` & `holytools-0.9.4/holytools/logging/log_settings.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/network/adapter.py` & `holytools-0.9.4/holytools/network/adapter.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/network/endpoint.py` & `holytools-0.9.4/holytools/network/endpoint.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/network/ip.py` & `holytools-0.9.4/holytools/network/ip.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/userIO/cli.py` & `holytools-0.9.4/holytools/userIO/cli.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/userIO/progr.py` & `holytools-0.9.4/holytools/userIO/progr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from typing import Iterable
-
 import progressbar
 from progressbar import ProgressBar
 # ---------------------------------------------------------
 
 class TrackedInt:
     progressbar.streams.wrap_stderr()
     progressbar.streams.wrap_stdout()
 
     def __init__(self, start_value : int, max_value : int):
         self._value : int = start_value
-        self.iterator : Iterable = iter(range(start_value, max_value))
         self.progressbar = ProgressBar(min_value=start_value, max_value=max_value)
+        self.progressbar.update()
 
     def update(self, incr : int):
+        self._value += incr
+
         if self.progressbar.finished():
             return
 
-        new_value = self._value + incr
-        if new_value > self.progressbar.max_value:
+        if self._value >= self.progressbar.max_value:
             self.progressbar.finish()
             return
 
-        self._value += incr
         self.progressbar.update(value=self._value)
 
+    def get_value(self) -> int:
+        return self._value
+
     def __iadd__(self, other):
         if not isinstance(other, int):
             raise ValueError("Only integers can be added to a TrackedInt.")
         self.update(incr=other)
         return self
 
     def __add__(self, other):
```

### Comparing `holytools-0.9.3/holytools/web/link_soup.py` & `holytools-0.9.4/holytools/web/link_soup.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/web/search_engine.py` & `holytools-0.9.4/holytools/web/search_engine.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools/web/site_visitor.py` & `holytools-0.9.4/holytools/web/site_visitor.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.3/holytools.egg-info/PKG-INFO` & `holytools-0.9.4/holytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holytools
-Version: 0.9.3
+Version: 0.9.4
 Summary: Collection of general python utilities for future projects
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Project-URL: repository, https://github.com/Somerandomguy10111/holytools
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: func_timeout
@@ -19,14 +19,15 @@
 Requires-Dist: orjson
 Requires-Dist: mss
 Requires-Dist: screeninfo
 Requires-Dist: pynput
 Requires-Dist: pillow
 Requires-Dist: configobj
 Requires-Dist: progressbar2
+Requires-Dist: tabulate
 
 ## Holytools
 A collection of general utilities in various very general areas that aim for simplicity in use. 
 Functionalities include:
 
 - object serialization -> holytools.abstract.serialization
 - fileIO and mock files -> holytools.file
```

### Comparing `holytools-0.9.3/holytools.egg-info/SOURCES.txt` & `holytools-0.9.4/holytools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 holytools/abstract/serialization/__init__.py
 holytools/abstract/serialization/dillable.py
 holytools/abstract/serialization/jsondataclass.py
 holytools/abstract/serialization/serializable.py
 holytools/abstract/tree/__init__.py
 holytools/abstract/tree/node.py
 holytools/configs/__init__.py
-holytools/configs/abstr.py
-holytools/configs/impl.py
+holytools/configs/base.py
+holytools/configs/configs.py
 holytools/crypto/__init__.py
 holytools/crypto/encrypt/__init__.py
 holytools/crypto/encrypt/aes.py
 holytools/crypto/encrypt/algo.py
 holytools/crypto/encrypt/rsa.py
 holytools/crypto/hash/__init__.py
 holytools/crypto/hash/salt.py
 holytools/crypto/hash/sha.py
 holytools/devtools/__init__.py
 holytools/devtools/inspection/__init__.py
 holytools/devtools/inspection/module_inspect.py
 holytools/devtools/inspection/type_inspect.py
+holytools/devtools/profiling/__init__.py
+holytools/devtools/profiling/profilable.py
 holytools/devtools/test/__init__.py
 holytools/devtools/test/cases.py
 holytools/devtools/test/configurable_unit.py
 holytools/devtools/test/results.py
 holytools/devtools/test/unit.py
 holytools/events/__init__.py
 holytools/events/countdown.py
```

### Comparing `holytools-0.9.3/readme.md` & `holytools-0.9.4/readme.md`

 * *Files identical despite different names*

