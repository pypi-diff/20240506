# Comparing `tmp/rastervision_pipeline-0.30.0.tar.gz` & `tmp/rastervision_pipeline-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_pipeline-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
+gzip compressed data, was "rastervision_pipeline-0.30.1.tar", last modified: Mon May  6 21:02:13 2024, max compression
```

## Comparing `rastervision_pipeline-0.30.0.tar` & `rastervision_pipeline-0.30.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      577 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1657 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8465 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/cli.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    13496 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      360 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4721 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/file_system.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4452 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/http_file_system.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4777 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/local_file_system.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11469 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/utils.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1850 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1794 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9604 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/registry.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      274 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      927 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/inprocess_runner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4145 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/local_runner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1580 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/runner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11204 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/rv_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1643 2024-04-06 20:13:30.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/utils.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      351 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/verbosity.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/version.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      951 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      833 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/config1.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      440 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/config2.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2764 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2252 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline2.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      894 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      523 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/config3.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      779 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/deluxe_message_maker.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      577 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1536 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       65 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       56 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      108 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1878 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      577 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision/pipeline/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1657 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9085 2024-05-03 19:36:07.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/cli.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    13294 2024-05-03 19:36:14.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      360 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4721 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/file_system.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4452 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/http_file_system.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4777 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/local_file_system.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11578 2024-05-03 19:36:24.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1850 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/pipeline.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1937 2024-05-03 19:36:14.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/pipeline_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9604 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/registry.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision/pipeline/runner/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      274 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/runner/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      927 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/runner/inprocess_runner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4145 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/runner/local_runner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1580 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/runner/runner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11204 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/rv_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1643 2024-04-06 20:13:30.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      351 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/verbosity.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2024-05-06 20:16:58.000000 rastervision_pipeline-0.30.1/rastervision/pipeline/version.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      951 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      833 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/config1.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      440 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/config2.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2764 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/sample_pipeline.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2252 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/sample_pipeline2.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      894 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      523 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/config3.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      779 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/deluxe_message_maker.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      577 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1536 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       65 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       56 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:13.000000 rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      108 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:13.243119 rastervision_pipeline-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1878 2024-05-06 20:16:58.000000 rastervision_pipeline-0.30.1/setup.py
```

### Comparing `rastervision_pipeline-0.30.0/PKG-INFO` & `rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rastervision_pipeline
-Version: 0.30.0
+Name: rastervision-pipeline
+Version: 0.30.1
 Summary: The main rastervision package for configuring, defining, and running pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/__init__.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/cli.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import TYPE_CHECKING
 import sys
 import os
 import logging
-import importlib
-import importlib.util
-from typing import List, Dict, Optional, Tuple
 
 import click
 
 from rastervision.pipeline import (registry_ as registry, rv_config_ as
                                    rv_config)
 from rastervision.pipeline.file_system import (file_to_json, get_tmp_dir)
-from rastervision.pipeline.config import build_config, save_pipeline_config
+from rastervision.pipeline.config import (build_config, Config,
+                                          save_pipeline_config)
 from rastervision.pipeline.pipeline_config import PipelineConfig
 
+if TYPE_CHECKING:
+    from rastervision.pipeline.runner import Runner
+
 log = logging.getLogger(__name__)
 
 
 def print_error(msg):
     """Print error message to console in red."""
     click.echo(click.style(msg, fg='red'), err=True)
 
@@ -36,91 +38,107 @@
             v = True
         elif v.lower() == 'false':
             v = False
         new_args[k] = v
     return new_args
 
 
-def get_configs(cfg_module_path: str, runner: str,
-                args: Dict[str, any]) -> List[PipelineConfig]:
+def get_configs(cfg_module_path: str,
+                runner: str | None = None,
+                args: dict[str, any] | None = None) -> list[PipelineConfig]:
     """Get PipelineConfigs from a module.
 
     Calls a get_config(s) function with some arguments from the CLI
     to get a list of PipelineConfigs.
 
     Args:
         cfg_module_path: the module with `get_configs` function that returns
             PipelineConfigs. This can either be a Python module path or a local path to
             a .py file.
         runner: name of the runner
         args: CLI args to pass to the get_config(s) function that comes from
             the --args option
     """
+    if cfg_module_path.endswith('.json'):
+        cfgs_json = file_to_json(cfg_module_path)
+        if not isinstance(cfgs_json, list):
+            cfgs_json = [cfgs_json]
+        cfgs = [Config.deserialize(json) for json in cfgs_json]
+    else:
+        cfgs = get_configs_from_module(cfg_module_path, runner, args)
+
+    for cfg in cfgs:
+        if not issubclass(type(cfg), PipelineConfig):
+            raise TypeError('All objects returned by get_configs in '
+                            f'{cfg_module_path} must be PipelineConfigs.')
+    return cfgs
+
+
+def get_configs_from_module(cfg_module_path: str, runner: str,
+                            args: dict[str, any]) -> list[PipelineConfig]:
+    import importlib
+    import importlib.util
+
     if cfg_module_path.endswith('.py'):
         # From https://stackoverflow.com/questions/67631/how-to-import-a-module-given-the-full-path  # noqa
         spec = importlib.util.spec_from_file_location('rastervision.pipeline',
                                                       cfg_module_path)
         cfg_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(cfg_module)
     else:
         cfg_module = importlib.import_module(cfg_module_path)
 
     _get_config = getattr(cfg_module, 'get_config', None)
-    _get_configs = _get_config
-    if _get_config is None:
-        _get_configs = getattr(cfg_module, 'get_configs', None)
+    _get_configs = getattr(cfg_module, 'get_configs', _get_config)
     if _get_configs is None:
-        raise Exception('There must be a get_config or get_configs function '
-                        f'in {cfg_module_path}.')
+        raise ImportError('There must be a get_config() or get_configs() '
+                          f'function in {cfg_module_path}.')
+
     cfgs = _get_configs(runner, **args)
     if not isinstance(cfgs, list):
         cfgs = [cfgs]
-
-    for cfg in cfgs:
-        if not issubclass(type(cfg), PipelineConfig):
-            raise Exception('All objects returned by get_configs in '
-                            f'{cfg_module_path} must be PipelineConfigs.')
     return cfgs
 
 
 @click.group()
 @click.pass_context
 @click.option(
     '--profile', '-p', help='Sets the configuration profile name to use.')
 @click.option(
     '-v', '--verbose', help='Increment the verbosity level.', count=True)
 @click.option('--tmpdir', help='Root of temporary directories to use.')
-def main(ctx: click.Context, profile: Optional[str], verbose: int,
-         tmpdir: str):
+def main(ctx: click.Context, profile: str | None, verbose: int, tmpdir: str):
     """The main click command.
 
     Sets the profile, verbosity, and tmp_dir in RVConfig.
     """
     # Make sure current directory is on PYTHON_PATH
     # so that we can run against modules in current dir.
     sys.path.append(os.curdir)
     rv_config.set_verbosity(verbosity=verbose + 1)
     rv_config.set_tmp_dir_root(tmp_dir_root=tmpdir)
     rv_config.set_everett_config(profile=profile)
 
 
-def _run_pipeline(cfg,
-                  runner,
-                  tmp_dir,
-                  splits=1,
-                  commands=None,
+def _run_pipeline(cfg: PipelineConfig,
+                  runner: 'Runner',
+                  tmp_dir: str,
+                  splits: int = 1,
+                  commands: list[str] | None = None,
                   pipeline_run_name: str = 'raster-vision'):
     cfg.update()
     cfg.recursive_validate_config()
-    # This is to run the validation again to check any fields that may have changed
-    # after the Config was constructed, possibly by the update method.
+
+    # This is to run the validation again to check any fields that may have
+    # changed after the Config was constructed, possibly by the update method.
     build_config(cfg.dict())
     cfg_json_uri = cfg.get_config_uri()
     save_pipeline_config(cfg, cfg_json_uri)
     pipeline = cfg.build(tmp_dir)
+
     if not commands:
         commands = pipeline.commands
 
     click.secho(f'Stages to run: {commands}', fg='white', bold=True)
 
     runner.run(
         cfg_json_uri,
@@ -146,16 +164,16 @@
     '-s',
     default=1,
     help='Number of splits to run in parallel for splittable commands')
 @click.option(
     '--pipeline-run-name',
     default='raster-vision',
     help='The name for this run of the pipeline.')
-def run(runner: str, cfg_module: str, commands: List[str],
-        arg: List[Tuple[str, str]], splits: int, pipeline_run_name: str):
+def run(runner: str, cfg_module: str, commands: list[str],
+        arg: list[tuple[str, str]], splits: int, pipeline_run_name: str):
     """Run COMMANDS within pipelines in CFG_MODULE using RUNNER.
 
     RUNNER: name of the Runner to use
 
     CFG_MODULE: the module with `get_configs` function that returns PipelineConfigs.
     This can either be a Python module path or a local path to a .py file.
 
@@ -174,17 +192,17 @@
     for cfg in cfgs:
         _run_pipeline(cfg, runner, tmp_dir, splits, commands,
                       pipeline_run_name)
 
 
 def _run_command(cfg_json_uri: str,
                  command: str,
-                 split_ind: Optional[int] = None,
-                 num_splits: Optional[int] = None,
-                 runner: Optional[str] = None):
+                 split_ind: int | None = None,
+                 num_splits: int | None = None,
+                 runner: str | None = None):
     """Run a single command using a serialized PipelineConfig.
 
     Args:
         cfg_json_uri: URI of a JSON file with a serialized PipelineConfig
         command: name of command to run
         split_ind: the index that a split command should assume
         num_splits: the total number of splits to use
@@ -225,16 +243,16 @@
     '--split-ind', type=int, help='The process index of a split command')
 @click.option(
     '--num-splits',
     type=int,
     help='The number of processes to use for running splittable commands')
 @click.option(
     '--runner', type=str, help='Name of runner to use', default='inprocess')
-def run_command(cfg_json_uri: str, command: str, split_ind: Optional[int],
-                num_splits: Optional[int], runner: str):
+def run_command(cfg_json_uri: str, command: str, split_ind: int | None,
+                num_splits: int | None, runner: str):
     """Run a single COMMAND using a serialized PipelineConfig in CFG_JSON_URI."""
     _run_command(
         cfg_json_uri,
         command,
         split_ind=split_ind,
         num_splits=num_splits,
         runner=runner)
```

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/config.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,30 +111,31 @@
             for v in val:
                 if v not in valid_options:
                     raise ConfigError(f'{v} is not a valid option for {field}')
         else:
             if val not in valid_options:
                 raise ConfigError(f'{val} is not a valid option for {field}')
 
+    def dict(self, with_rv_metadata: bool = False, **kwargs) -> dict:
+        cfg_json = self.json(**kwargs)
+        cfg_dict = json.loads(cfg_json)
+        if with_rv_metadata:
+            cfg_dict['plugin_versions'] = registry.plugin_versions
+        return cfg_dict
+
     def to_file(self, uri: str, with_rv_metadata: bool = True) -> None:
         """Save a Config to a JSON file, optionally with RV metadata.
 
         Args:
             uri: URI to save to.
             with_rv_metadata: If True, inject Raster Vision metadata such as
                 ``plugin_versions``, so that the config can be upgraded when
                 loaded.
         """
-        cfg_json = self.json()
-        if with_rv_metadata:
-            # self.dict() --> json_to_file() would be simpler but runs into
-            # JSON serialization problems
-            cfg_dict = json.loads(cfg_json)
-            cfg_dict['plugin_versions'] = registry.plugin_versions
-            cfg_json = json.dumps(cfg_dict)
+        cfg_dict = self.dict(with_rv_metadata=with_rv_metadata)
         json_to_file(cfg_dict, uri)
 
     @classmethod
     def deserialize(cls, inp: 'str | dict | Config') -> 'Self':
         """Deserialize Config from a JSON file or dict, upgrading if possible.
 
         If ``inp`` is already a :class:`.Config`, it is returned as is.
@@ -153,25 +154,28 @@
     @classmethod
     def from_file(cls, uri: str) -> 'Self':
         """Deserialize Config from a JSON file, upgrading if possible.
 
         Args:
             uri: URI to load from.
         """
-        cfg_dict = load_config_dict(uri)
+        cfg_dict = file_to_json(uri)
         cfg = cls.from_dict(cfg_dict)
         return cfg
 
     @classmethod
     def from_dict(cls, cfg_dict: dict) -> 'Self':
         """Deserialize Config from a dict.
 
         Args:
             cfg_dict: Dict to deserialize.
         """
+        if 'plugin_versions' in cfg_dict:
+            cfg_dict: dict = upgrade_config(cfg_dict)
+            cfg_dict.pop('plugin_versions', None)
         cfg = build_config(cfg_dict)
         return cfg
 
     def __repr_args__(self):
         """Override to delete 'type_hint' field."""
         args = dict(super().__repr_args__())
         try:
@@ -188,23 +192,14 @@
     """
     cfg.rv_config = rv_config.get_config_dict(registry.rv_config_schema)
     cfg.plugin_versions = registry.plugin_versions
     cfg_json = cfg.json()
     str_to_file(cfg_json, output_uri)
 
 
-def load_config_dict(uri: str) -> dict:
-    """Load a serialized Config from a JSON file as a dict and upgrade it."""
-    cfg_dict = file_to_json(uri)
-    if 'plugin_versions' in cfg_dict:
-        cfg_dict = upgrade_config(cfg_dict)
-        cfg_dict.pop('plugin_versions', None)
-    return cfg_dict
-
-
 def build_config(x: Union[dict, List[Union[dict, Config]], Config]
                  ) -> Union[Config, List[Config]]:
     """Build a Config from various types of input.
 
     This is useful for deserializing from JSON. It implements polymorphic
     deserialization by using the `type_hint` in each dict to get the
     corresponding Config class from the registry.
@@ -212,17 +207,18 @@
     Args:
         x: some representation of Config(s)
 
     Returns:
         Config: the corresponding Config(s)
     """
     if isinstance(x, dict):
-        new_x = {}
-        for k, v in x.items():
-            new_x[k] = build_config(v)
+        new_x = {
+            k: build_config(v)
+            for k, v in x.items() if k not in ('plugin_versions', 'rv_config')
+        }
         type_hint = new_x.get('type_hint')
         if type_hint is not None:
             config_cls = registry.get_config(type_hint)
             new_x = config_cls(**new_x)
         return new_x
     elif isinstance(x, list):
         return [build_config(v) for v in x]
@@ -307,20 +303,19 @@
             non-current version
 
     Returns:
         The corresponding serialized PipelineConfig(s) that have been upgraded
         to the current version.
     """
     plugin_versions = config_dict.get('plugin_versions')
-    plugin_versions = upgrade_plugin_versions(plugin_versions)
     if plugin_versions is None:
-        raise ConfigError(
-            'Configuration is missing plugin_version field so is not backward '
-            'compatible.')
-    return _upgrade_config(config_dict, plugin_versions)
+        return config_dict
+    plugin_versions = upgrade_plugin_versions(plugin_versions)
+    out = _upgrade_config(config_dict, plugin_versions)
+    return out
 
 
 def get_plugin(config_cls: Type) -> str:
     """Infer the module path of the plugin where a Config class is defined.
 
     This only works correctly if the plugin is in a module under rastervision.
     """
```

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/file_system.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/http_file_system.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/http_file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/local_file_system.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/local_file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/utils.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/file_system/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,33 +215,36 @@
             uri
     """
     if not fs:
         fs = FileSystem.get_file_system(uri, 'r')
     return fs.file_exists(uri, include_dir)
 
 
-def list_paths(uri: str, ext: str = '',
-               fs: Optional[FileSystem] = None) -> List[str]:
+def list_paths(uri: str,
+               ext: str = '',
+               fs: Optional[FileSystem] = None,
+               **kwargs) -> List[str]:
     """List paths rooted at URI.
 
     Optionally only includes paths with a certain file extension.
 
     Args:
         uri: the URI of a directory
         ext: the optional file extension to filter by
         fs: if supplied, use fs instead of automatically chosen FileSystem for
             uri
+        **kwargs: extra kwargs to pass to fs.list_paths().
     """
     if uri is None:
         return None
 
     if not fs:
         fs = FileSystem.get_file_system(uri, 'r')
 
-    return fs.list_paths(uri, ext=ext)
+    return fs.list_paths(uri, ext=ext, **kwargs)
 
 
 def upload_or_copy(src_path: str,
                    dst_uri: str,
                    fs: Optional[FileSystem] = None) -> None:
     """Upload or copy a file.
```

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline_config.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/pipeline_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,7 +40,10 @@
         corresponding subclass of Pipeline.
 
         Args:
             tmp_dir: root of any temporary directory to pass to pipeline
         """
         from rastervision.pipeline.pipeline import Pipeline  # noqa
         return Pipeline(self, tmp_dir)
+
+    def dict(self, with_rv_metadata: bool = True, **kwargs) -> dict:
+        return super().dict(with_rv_metadata=with_rv_metadata, **kwargs)
```

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/registry.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/runner/inprocess_runner.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/runner/inprocess_runner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/runner/local_runner.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/runner/runner.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/runner/runner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/rv_config.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/rv_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline/utils.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/__init__.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/config1.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/config1.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/sample_pipeline.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline2.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin1/sample_pipeline2.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/__init__.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/config3.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/config3.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/deluxe_message_maker.py` & `rastervision_pipeline-0.30.1/rastervision/pipeline_example_plugin2/deluxe_message_maker.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/PKG-INFO` & `rastervision_pipeline-0.30.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rastervision-pipeline
-Version: 0.30.0
+Name: rastervision_pipeline
+Version: 0.30.1
 Summary: The main rastervision package for configuring, defining, and running pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/SOURCES.txt` & `rastervision_pipeline-0.30.1/rastervision_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.30.0/setup.py` & `rastervision_pipeline-0.30.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_pipeline'
-version = '0.30.0'
+version = '0.30.1'
 description = 'The main rastervision package for configuring, defining, and running pipelines'
 requirement_constraints = {
     'pydantic': '<2',
 }
 
 here = abspath(dirname(__file__))
```

