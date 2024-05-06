# Comparing `tmp/common-tools-ai-bnq-0.1.3.tar.gz` & `tmp/common-tools-ai-bnq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.1.3.tar", last modified: Mon Apr 29 05:59:23 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.1.4.tar", last modified: Mon May  6 09:19:18 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.1.3.tar` & `common-tools-ai-bnq-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:59:23.061529 common-tools-ai-bnq-0.1.3/
--rw-rw-rw-   0        0        0     2598 2024-04-29 05:59:23.060528 common-tools-ai-bnq-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2236 2024-04-24 02:51:54.000000 common-tools-ai-bnq-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 05:59:23.043530 common-tools-ai-bnq-0.1.3/bnq_py_core/
--rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1090 2024-04-26 04:02:02.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     4617 2024-04-29 05:56:47.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3274 2024-04-26 04:19:35.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:59:23.059536 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     2598 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 05:59:23.061529 common-tools-ai-bnq-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-04-29 05:59:08.000000 common-tools-ai-bnq-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:19:18.672875 common-tools-ai-bnq-0.1.4/
+-rw-rw-rw-   0        0        0     2598 2024-05-06 09:19:18.671874 common-tools-ai-bnq-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2024-04-24 02:51:54.000000 common-tools-ai-bnq-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:19:18.653149 common-tools-ai-bnq-0.1.4/bnq_py_core/
+-rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     4566 2024-05-06 09:18:58.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:19:18.670873 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     2598 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:19:18.672875 common-tools-ai-bnq-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-06 09:19:13.000000 common-tools-ai-bnq-0.1.4/setup.py
```

### Comparing `common-tools-ai-bnq-0.1.3/PKG-INFO` & `common-tools-ai-bnq-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.3
+Version: 0.1.4
 Summary: Common tools of AI module for BNQ
 Author: BNQ
 Description-Content-Type: text/markdown
 Requires-Dist: structlog==23.1.0
 Requires-Dist: concurrent-log-handler==0.9.22
 Requires-Dist: nacos-sdk-python==0.1.12
 Requires-Dist: PyYAML==6.0.1
```

### Comparing `common-tools-ai-bnq-0.1.3/README.md` & `common-tools-ai-bnq-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.3/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.1.4/bnq_py_core/cos_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,7 @@
         self.secret_id = secret_id
         self.secret_key = secret_key
         self.region = region
 
         config = CosConfig(Region=region, SecretId=secret_id, SecretKey=secret_key)
         self.client = CosS3Client(config)
 
-
```

### Comparing `common-tools-ai-bnq-0.1.3/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.1.4/bnq_py_core/logger_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
         Returns:
 
         """
         if self.log_record_path is None:
             # 获取根目录路径，并创建日志文件夹
             self.log_record_path = os.path.join(os.getcwd(), "logs")
-            # raise ValueError("log_dir is None")
 
         pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
         log_filename = os.path.join(self.log_record_path, self.__filename)
         logging.config.dictConfig({
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
```

### Comparing `common-tools-ai-bnq-0.1.3/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.1.4/bnq_py_core/nacos_connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         Returns:
 
         """
         if pre_conf is None:
             pre_conf = {}
         conf_resolve = {}
         conf = self.client.get_config(data_id, group)  # 获取配置
-        self.client.add_config_watcher(data_id, group)
         if conf is None:
             return pre_conf
         if self.conf_type == "json":
             conf_resolve = json.loads(conf)  # 转换为json
         elif self.conf_type == "yaml":
             conf_resolve = yaml.load(conf, Loader=yaml.FullLoader)
         else:
```

### Comparing `common-tools-ai-bnq-0.1.3/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.1.4/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.3/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.1.4/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.3
+Version: 0.1.4
 Summary: Common tools of AI module for BNQ
 Author: BNQ
 Description-Content-Type: text/markdown
 Requires-Dist: structlog==23.1.0
 Requires-Dist: concurrent-log-handler==0.9.22
 Requires-Dist: nacos-sdk-python==0.1.12
 Requires-Dist: PyYAML==6.0.1
```

### Comparing `common-tools-ai-bnq-0.1.3/setup.py` & `common-tools-ai-bnq-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
```

