# Comparing `tmp/celi_framework-0.1.0.tar.gz` & `tmp/celi_framework-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celi_framework-0.1.0.tar", max compression
+gzip compressed data, was "celi_framework-0.2.0.tar", max compression
```

## Comparing `celi_framework-0.1.0.tar` & `celi_framework-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,63 @@
--rw-r--r--   0        0        0     1084 2024-04-22 10:44:04.665814 celi_framework-0.1.0/LICENSE
--rw-r--r--   0        0        0    12984 2024-04-22 10:44:04.665814 celi_framework-0.1.0/README.md
--rw-r--r--   0        0        0    10399 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/job_description.py
--rw-r--r--   0        0        0    23124 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/monitor.py
--rw-r--r--   0        0        0    11301 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/mt_factory.py
--rw-r--r--   0        0        0    14719 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/post_monitor.py
--rw-r--r--   0        0        0    59120 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/processor.py
--rw-r--r--   0        0        0     3060 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/runner.py
--rw-r--r--   0        0        0    23630 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/core/templates.py
--rw-r--r--   0        0        0    13793 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/examples/reporting_template/job_description.py
--rw-r--r--   0        0        0    10317 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/examples/reporting_template/tools.py
--rw-r--r--   0        0        0     6133 2024-04-22 10:44:04.665814 celi_framework-0.1.0/celi_framework/examples/wikipedia/Index_cache.py
--rw-r--r--   0        0        0     7694 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
--rw-r--r--   0        0        0     5552 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/eval/run_eval.py
--rw-r--r--   0        0        0      530 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/eval/test_sets.json
--rw-r--r--   0        0        0      851 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/eval/test_sets_large.json
--rw-r--r--   0        0        0      161 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/example_config.json
--rw-r--r--   0        0        0    13876 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/index.py
--rw-r--r--   0        0        0    13330 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/job_description.py
--rw-r--r--   0        0        0     7111 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/loader.py
--rw-r--r--   0        0        0    14758 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/tools.py
--rw-r--r--   0        0        0      549 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/examples/wikipedia/wikipedia_utils.py
--rw-r--r--   0        0        0    12668 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/embeddor.py
--rw-r--r--   0        0        0     7936 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/mapper.py
--rw-r--r--   0        0        0     1354 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/mechanic.py
--rw-r--r--   0        0        0        0 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/__init__.py
--rw-r--r--   0        0        0    23634 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/pre-processor.py
--rw-r--r--   0        0        0       94 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
--rw-r--r--   0        0        0     8832 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
--rw-r--r--   0        0        0     2056 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
--rw-r--r--   0        0        0    10669 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
--rw-r--r--   0        0        0     7835 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
--rw-r--r--   0        0        0     5471 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/task_builder/factory.py
--rw-r--r--   0        0        0     4242 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/task_builder/llm_helper_funcs.py
--rw-r--r--   0        0        0     4352 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/task_builder/llms.py
--rw-r--r--   0        0        0     5939 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/task_builder/template.py
--rw-r--r--   0        0        0     9914 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/utils/ada.py
--rw-r--r--   0        0        0    19041 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/utils/mapper_utils.py
--rw-r--r--   0        0        0    13615 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
--rw-r--r--   0        0        0     5118 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
--rw-r--r--   0        0        0     5458 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/utils/postprocessor_utils.py
--rw-r--r--   0        0        0     9091 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/experimental/utils/synthetic_data.py
--rw-r--r--   0        0        0     1350 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/logging_config.json
--rw-r--r--   0        0        0     2171 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/logging_setup.py
--rw-r--r--   0        0        0     6954 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/main.py
--rw-r--r--   0        0        0        0 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/__init__.py
--rw-r--r--   0        0        0    10889 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/codex.py
--rw-r--r--   0        0        0      461 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/exceptions.py
--rw-r--r--   0        0        0    22485 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/llmcore_utils.py
--rw-r--r--   0        0        0    10021 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/llms.py
--rw-r--r--   0        0        0       77 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/log.py
--rw-r--r--   0        0        0    10717 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/sql_utils.py
--rw-r--r--   0        0        0    10871 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/token_counters.py
--rw-r--r--   0        0        0    28482 2024-04-22 10:44:04.669814 celi_framework-0.1.0/celi_framework/utils/utils.py
--rw-r--r--   0        0        0     1757 2024-04-22 10:44:33.782019 celi_framework-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14419 1970-01-01 00:00:00.000000 celi_framework-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-06 14:31:21.781694 celi_framework-0.2.0/LICENSE
+-rw-r--r--   0        0        0    12984 2024-05-06 14:31:21.781694 celi_framework-0.2.0/README.md
+-rw-r--r--   0        0        0    11983 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/job_description.py
+-rw-r--r--   0        0        0    23124 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/monitor.py
+-rw-r--r--   0        0        0    11341 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/mt_factory.py
+-rw-r--r--   0        0        0    14719 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/post_monitor.py
+-rw-r--r--   0        0        0    17145 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/processor.py
+-rw-r--r--   0        0        0     2859 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/runner.py
+-rw-r--r--   0        0        0    23630 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/templates.py
+-rw-r--r--   0        0        0      371 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/README.md
+-rw-r--r--   0        0        0      815 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/eval.py
+-rw-r--r--   0        0        0    46321 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/example_output.json
+-rw-r--r--   0        0        0     4074 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/job_description.py
+-rwxr-xr-x   0        0        0   196170 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/test.csv
+-rw-r--r--   0        0        0     2629 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/test_tools.py
+-rw-r--r--   0        0        0     3577 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/tools.py
+-rw-r--r--   0        0        0    13793 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/reporting_template/job_description.py
+-rw-r--r--   0        0        0    10352 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/reporting_template/tools.py
+-rw-r--r--   0        0        0     6133 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/wikipedia/Index_cache.py
+-rw-r--r--   0        0        0     7694 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
+-rw-r--r--   0        0        0     4282 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/run_eval.py
+-rw-r--r--   0        0        0      530 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets.json
+-rw-r--r--   0        0        0      851 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets_large.json
+-rw-r--r--   0        0        0      161 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/example_config.json
+-rw-r--r--   0        0        0    13876 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/index.py
+-rw-r--r--   0        0        0    10858 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/job_description.py
+-rw-r--r--   0        0        0     7133 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/loader.py
+-rw-r--r--   0        0        0    14762 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/tools.py
+-rw-r--r--   0        0        0      549 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/wikipedia_utils.py
+-rw-r--r--   0        0        0    12668 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/embeddor.py
+-rw-r--r--   0        0        0     7936 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/mapper.py
+-rw-r--r--   0        0        0     1354 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/mechanic.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/__init__.py
+-rw-r--r--   0        0        0    23634 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/pre-processor.py
+-rw-r--r--   0        0        0       94 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
+-rw-r--r--   0        0        0     8832 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
+-rw-r--r--   0        0        0     2056 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
+-rw-r--r--   0        0        0    10669 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
+-rw-r--r--   0        0        0     7835 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
+-rw-r--r--   0        0        0     5471 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/factory.py
+-rw-r--r--   0        0        0     4242 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/llm_helper_funcs.py
+-rw-r--r--   0        0        0     4352 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/llms.py
+-rw-r--r--   0        0        0     5939 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/template.py
+-rw-r--r--   0        0        0     9914 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/ada.py
+-rw-r--r--   0        0        0    19041 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/mapper_utils.py
+-rw-r--r--   0        0        0    13615 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
+-rw-r--r--   0        0        0     5118 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
+-rw-r--r--   0        0        0     5458 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/postprocessor_utils.py
+-rw-r--r--   0        0        0     9091 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/synthetic_data.py
+-rw-r--r--   0        0        0     1449 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/logging_config.json
+-rw-r--r--   0        0        0     2171 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/logging_setup.py
+-rw-r--r--   0        0        0     6787 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/__init__.py
+-rw-r--r--   0        0        0    11028 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/codex.py
+-rw-r--r--   0        0        0      461 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/exceptions.py
+-rw-r--r--   0        0        0    22723 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/llmcore_utils.py
+-rw-r--r--   0        0        0    10021 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/llms.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/log.py
+-rw-r--r--   0        0        0    10717 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/sql_utils.py
+-rw-r--r--   0        0        0    10871 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/token_counters.py
+-rw-r--r--   0        0        0    28482 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/utils.py
+-rw-r--r--   0        0        0     1806 2024-05-06 14:34:13.148816 celi_framework-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14509 1970-01-01 00:00:00.000000 celi_framework-0.2.0/PKG-INFO
```

### Comparing `celi_framework-0.1.0/LICENSE` & `celi_framework-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/README.md` & `celi_framework-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/core/job_description.py` & `celi_framework-0.2.0/celi_framework/core/job_description.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from __future__ import annotations
+
+import datetime
+import json
+import logging
+import os
 from abc import ABC, abstractmethod
 import inspect
 from typing import Any, Callable, Dict, List, Optional, Type
 
 from celi_framework.utils.llms import ToolDescription
 
 from pydantic import BaseModel, field_serializer
-from celi_framework.utils.utils import encode_class_type
+from celi_framework.utils.utils import encode_class_type, read_json_from_file, write_string_to_file
+
+logger = logging.getLogger(__name__)
 
 
 class Task(BaseModel):
     task_name: str
     details: Dict[str, str | List[str] | Dict[str, Any]]
 
     def with_references_resolved(self, task_numbering: Dict[str, str]) -> Task:
@@ -56,17 +63,24 @@
             # Non-string, non-list, non-dict items are returned unchanged
             return item
 
 
 class ToolImplementations(ABC):
     """Each public function in the class becomes a tool that the LLM can use.
 
-    There is one required function, `def get_schema(self) -> Dict[str, str]`.  This function returns a dictionary describing the document sections.  The processor will work through the sections, completing the defined tasks for each section.  Each dictionary can have any string values, but it is intended to be a section number followed by a section name.
-
-    In addition to the `get_schema` function, the ToolImplementations class can have whatever other functions it needs to enable celi_framework.  Each function should be documented with type hints and a doc string.  The top section of the docstring will be included as the description of the overall function.  If the function takes arguments, there should be a section called "Args:" that contains a list of the arguments to the function and descriptions of each.  An example docstring is given below:
+    There is one required function, `def get_schema(self) -> Dict[str, str]`.  This function returns a dictionary
+    describing the document sections.  The processor will work through the sections, completing the defined tasks for
+    each section.  Each dictionary can have any string values, but it is intended to be a section number followed by
+    a section name.
+
+    In addition to the `get_schema` function, the ToolImplementations class can have whatever other functions it needs
+    to enable celi_framework.  Each function should be documented with type hints and a doc string.  The top section of
+    the docstring will be included as the description of the overall function.  If the function takes arguments, there
+    should be a section called "Args:" that contains a list of the arguments to the function and descriptions of each.
+    An example docstring is given below:
 
         '''
         Extracts text from specified sections of documents.
         It handles different document types and logs any errors or warnings encountered.
         Returns concatenated text from the specified sections of the documents.
         If there is no content for the section, <empty section> will be returned.
 
@@ -76,18 +90,54 @@
             sections_dict_str (str): A JSON string mapping document names to their respective section numbers.  The json string will have the documents and sections in a dictionary.  The sections values should correspond to an entry in the table of contents for the specified document.
 
         '''
     """
 
     @abstractmethod
     def get_schema(self) -> Dict[str, str]:
-        "This function returns a dictionary describing the document sections.  The processor will work through the sections, completing the defined tasks for each section.  Each dictionary can have any string values, but it is intended to be a section number followed by a section name."
+        """This function returns a dictionary describing the document sections.  The processor will work through the
+        sections, completing the defined tasks for each section.  Each dictionary can have any string values,
+        but it is intended to be a section number followed by a section name."""
         pass
 
 
+class BaseDocToolImplementations(ToolImplementations, ABC):
+    """ A base class for ToolImplementations that draft documents.  Adds a standard `update_draft_doc` tool.
+    """
+
+    def __init__(self, drafts_dir: str = "target/celi_output/drafts"):
+        os.makedirs(drafts_dir, exist_ok=True)
+        self.draft_doc = (
+            f"{drafts_dir}/{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.json"
+        )
+        logger.info(f"Writing output to {self.draft_doc}")
+
+    def save_draft_section(self, doc_section: str, draft: str):
+        """Saves a draft of the current section.
+
+        This must be called with the final output before calling pop_context and moving on to the next section.
+
+        Args:
+            doc_section: The section name to save
+            draft: The draft text
+        """
+        logger.info(
+            f"Completed section {doc_section}.  Draft output is:\n{draft}",
+            extra={"color": "orange"},
+        )
+
+        logger.info(f"Adding section {doc_section} to {self.draft_doc}")
+        try:
+            current = read_json_from_file(self.draft_doc)
+        except FileNotFoundError:
+            current = {}
+        current[doc_section] = draft
+        write_string_to_file(json.dumps(current, indent=2), self.draft_doc)
+
+
 class JobDescription(BaseModel):
     """
     Specifies a configuration for MasterTemplateFactory
 
     This configuration file is a critical component of the automated document drafting framework, designed to work in tandem with the `MasterTemplateFactory` class. It outlines a series of structured tasks and instructions that guide the drafting process for various types of documents, emphasizing step-by-step clarity and comprehensive coverage of necessary content.
 
     Key Components:
@@ -136,21 +186,23 @@
     parts = docstring.split("Args:")
     description = parts[0].strip()
     args = "" if len(parts) == 1 else parts[1].strip()
 
     # Extracting parameters and their annotations, skipping 'self'
     sig = inspect.signature(method)
     parameters = {}
+    #logger.debug(f"Inspecting {method}: {sig}")
     for param_name, param in sig.parameters.items():
         if param_name == "self":  # Skip 'self' parameter
             continue
+        #logger.debug(f"Param {param}")
 
         if param.annotation == param.empty:
             param_type_dict = {"type": "string"}
-        elif param.annotation.__name__ == "str":
+        elif param.annotation == "str" or param.annotation.__name__ == "str":
             param_type_dict = {"type": "string"}
         elif param.annotation.__name__ == "List":
             param_type_dict = {"type": "array", "items": {"type": "string"}}
         else:
             param_type_dict = {"type": param.annotation.__name__}
 
         param_description = "No description provided."  # Default description
```

### Comparing `celi_framework-0.1.0/celi_framework/core/monitor.py` & `celi_framework-0.2.0/celi_framework/core/monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/core/mt_factory.py` & `celi_framework-0.2.0/celi_framework/core/mt_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Classes:
     MasterTemplateFactory: A versatile class that generates structured instructions and tasks, adaptable
     to various drafting and analytical needs.
 
 This module represents a flexible tool for automating and enhancing the document creation process,
 capable of catering to a broad spectrum of document types and requirements.
 """
+from typing import Dict
 
 from celi_framework.core.job_description import JobDescription, Task
 from celi_framework.utils.utils import generate_hash_id
 
 
 class MasterTemplateFactory:
     """
@@ -50,15 +51,15 @@
         create_system_message(): Synthesizes the setup instructions, task details, and general comments into a unified system message for users or systems.
 
     The MasterTemplateFactory is designed to bridge the gap between conceptual document planning and practical execution,
     offering a systematic approach to document creation and analysis that enhances productivity, consistency, and quality
     across a wide array of applications.
     """
 
-    def __init__(self, job_desc: JobDescription, schema):
+    def __init__(self, job_desc: JobDescription, schema: Dict[str, str]):
         """
         Initializes the MasterTemplateFactory with the provided configuration and schema, setting up the necessary
         attributes for generating structured document instructions. This method prepares the factory to create
         actionable, step-by-step guides tailored to specific document creation or analysis needs across various domains.
 
         Args:
             config (dict): A dictionary containing configuration details that guide the instruction generation process.
```

### Comparing `celi_framework-0.1.0/celi_framework/core/post_monitor.py` & `celi_framework-0.2.0/celi_framework/core/post_monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/core/runner.py` & `celi_framework-0.2.0/celi_framework/core/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from __future__ import annotations
 from dataclasses import asdict, dataclass
 from queue import Queue
 import threading
-from typing import Type
+from typing import Type, Optional
 from llm_core.parsers import BaseParser
 from celi_framework.core.job_description import JobDescription, ToolImplementations
 from celi_framework.core.monitor import MonitoringAgent
 from celi_framework.core.mt_factory import MasterTemplateFactory
 from celi_framework.core.processor import ProcessRunner
 from celi_framework.utils.codex import MongoDBUtilitySingleton
 from celi_framework.utils.llmcore_utils import ParserFactory, new_parser_factory
 from celi_framework.utils.log import app_logger
 
 
 @dataclass
 class Directories:
     output_dir: str
-    drafts_dir: str
     evaluations_dir: str
 
     @staticmethod
     def create(output_dir: str) -> Directories:
         return Directories(
             output_dir=output_dir,
-            drafts_dir=f"{output_dir}/drafts",
             evaluations_dir=f"{output_dir}/evaluations",
         )
 
 
 @dataclass
 class MongoDBConfig:
     db_url: str
     db_name: str
     external_db: bool
 
 
 @dataclass
 class CELIConfig:
-    mongo_config: MongoDBConfig
+    mongo_config: Optional[MongoDBConfig]
     directories: Directories
     job_description: JobDescription
     tool_implementations: ToolImplementations
     parser_cls: Type[BaseParser]
     parser_model_name: str
     llm_cache: bool
     use_monitor: bool
@@ -63,18 +61,15 @@
         cache=celi_config.llm_cache,
         codex=codex,
     )
 
     process_runner = ProcessRunner(
         master_template=mt,
         codex=codex,
-        parser_factory=parser_factory,
         tool_implementations=celi_config.tool_implementations,
-        drafts_dir=celi_config.directories.drafts_dir,
-        update_queue=update_queue,
         llm_cache=celi_config.llm_cache,
     )
 
     # Start ProcessRunner in its own thread
     process_runner_thread = threading.Thread(target=process_runner.run, daemon=True)
     process_runner_thread.start()
     threads = [process_runner_thread]
@@ -93,8 +88,8 @@
         )
         monitoring_agent_thread.start()
         threads.append(monitoring_agent_thread)
 
     # Wait for threads to finish
     [_.join() for _ in threads]
     app_logger.info("Threads completed. Exiting.")
-    return process_runner.draft_doc
+    return
```

### Comparing `celi_framework-0.1.0/celi_framework/core/templates.py` & `celi_framework-0.2.0/celi_framework/core/templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/reporting_template/job_description.py` & `celi_framework-0.2.0/celi_framework/examples/reporting_template/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/reporting_template/tools.py` & `celi_framework-0.2.0/celi_framework/examples/reporting_template/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import json
 import os
 from typing import Dict
 
 from attr import dataclass
 from celi_framework.core.job_description import (
     ToolImplementations,
-    generate_tool_descriptions,
+    generate_tool_descriptions, BaseDocToolImplementations,
 )
 from celi_framework.core.templates import (
     make_draft_setting_output_prompt,
     make_table_setting_output_prompt,
 )
 from celi_framework.utils.llms import quick_ask
 from celi_framework.utils.token_counters import get_master_counter_instance
@@ -34,15 +34,15 @@
 
 @dataclass
 class Document:
     toc: Dict[str, str]
     content: Dict[str, str]
 
 
-class ReportingToolImplementations(ToolImplementations):
+class ReportingToolImplementations(BaseDocToolImplementations):
     doc_dir: str
 
     def __init__(self, doc_dir: str):
         super().__init__()
         self.doc_dir = doc_dir
 
         def dir(s):
```

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/Index_cache.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/Index_cache.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/eval/run_eval.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/run_eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-from celi_framework.logging_setup import setup_logging
-
-setup_logging()
-
-import json
-import argparse
 import copy
+import json
 import logging
-import logging.config
 import os
-
 from functools import lru_cache
 from pathlib import Path
 from typing import List
 
 import pandas as pd
 from dotenv import load_dotenv
 from evaluate import load
@@ -20,66 +13,25 @@
 from celi_framework.core.runner import CELIConfig, Directories, MongoDBConfig, run_celi
 from celi_framework.examples.wikipedia.job_description import job_description
 from celi_framework.examples.wikipedia.loader import (
     format_content,
     load_content_from_wikipedia_url,
 )
 from celi_framework.examples.wikipedia.tools import WikipediaToolImplementations
-from celi_framework.main import instantiate_with_argparse_args
-from celi_framework.utils.utils import get_obj_by_name, read_json_from_file, str2bool
+from celi_framework.logging_setup import setup_logging
+from celi_framework.main import instantiate_with_argparse_args, setup_standard_args
+from celi_framework.utils.utils import get_obj_by_name, read_json_from_file
 
 logger = logging.getLogger(__name__)
 
 
 def get_config():
     load_dotenv()
 
-    parser = argparse.ArgumentParser(description="Run the document generator.")
-
-    def bool_opt(opt: str, env_var: str, help: str):
-        parser.add_argument(
-            opt,
-            action="store_true",
-            default=str2bool(os.getenv(env_var, "False")),
-            help=help,
-        )
-
-    parser.add_argument(
-        "--output-dir",
-        type=str,
-        default=os.getenv("OUTPUT_DIR"),
-        help="Output directory path",
-    )
-    parser.add_argument(
-        "--db-url",
-        type=str,
-        default=os.getenv("DB_URL", "mongodb://localhost:27017/"),
-        help="Mongo DB URL",
-    )
-    parser.add_argument(
-        "--db-name", type=str, default="celi", help="Mongo database name"
-    )
-    bool_opt(
-        "--external-db", "EXTERNAL_DB", "Set to True if using an existing mongo server."
-    )
-    parser.add_argument(
-        "--parser-model-class",
-        type=str,
-        default=os.getenv("PARSER_MODEL_CLASS", "llm_core.parsers.LLaMACPPParser"),
-    )
-    parser.add_argument(
-        "--parser-model-name",
-        type=str,
-        default=os.getenv("PARSER_MODEL_NAME", "mixtral-8x7b-v0.1.Q5_K_M.gguf"),
-    )
-    bool_opt("--no-cache", "NO_CACHE", "Set to True to turn off LLM caching")
-    bool_opt(
-        "--no-monitor", "NO_MONITOR", "Set to True to turn off the monitoring thread"
-    )
-
+    parser = setup_standard_args()
     args = parser.parse_args()
 
     directories = Directories.create(args.output_dir)
     mongo_config = instantiate_with_argparse_args(args, MongoDBConfig)
 
     llm_cache = not args.no_cache
     use_monitor = not args.no_monitor
@@ -115,15 +67,16 @@
         logger.info(f"Skipping test {result_file_name} as it already exists")
         return read_json_from_file(eval_path)
     else:
         config = copy.deepcopy(config)
         config.tool_implementations = WikipediaToolImplementations(
             example, target, ignore_updates=True
         )
-        draft_doc_path = run_celi(config)
+        run_celi(config)
+        draft_doc_path = config.tool_implementations.draft_doc
         draft_doc_sections = read_json_from_file(draft_doc_path)
         draft_doc = "\n".join(f"{k}\n{v}" for k, v in draft_doc_sections.items())
         result = evaluate(draft_doc, target)
         result_out = {
             "example": page_name(example),
             "target": page_name(target),
             **result,
@@ -149,31 +102,33 @@
 def evaluate(generated_doc: str, target_url: str):
     bertscore = load_eval_model()
     target_dict, _ = load_content_from_wikipedia_url(
         target_url, include_references=False
     )
     ground_truth_doc = format_content(target_dict)
 
-    results = bertscore.compute(
+    eval_results = bertscore.compute(
         predictions=[generated_doc],
         references=[ground_truth_doc],
         model_type="distilbert-base-uncased",
     )
-    return results
+    return eval_results
 
 
 @lru_cache()
 def load_eval_model():
     return load("bertscore")
 
 
 if __name__ == "__main__":
-    config = get_config()
+    setup_logging()
+
+    celi_config = get_config()
 
     test_sets = read_json_from_file(Path(__file__).parent / "test_sets.json")
-    result = [
+    results = [
         _
         for test_set_name, test_set in test_sets.items()
-        for _ in run_test_set(config, test_set_name, test_set)
+        for _ in run_test_set(celi_config, test_set_name, test_set)
     ]
-    ret = pd.DataFrame.from_records(result)
+    ret = pd.DataFrame.from_records(results)
     print(ret)
```

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/eval/test_sets.json` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/eval/test_sets_large.json` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets_large.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/index.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/index.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/job_description.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/job_description.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,29 +45,35 @@
     ),
     Task(
         task_name="Ask additional questions",
         details={
             "description": """Determine if any additional information is required to draft the section and call the ask_question_about_target function to gather that information.
             Feel free to ask as many questions as you need and keep working on this task until you have the information you need.  This is especially important if
             the initial references turn out not to be useful.
+            If you ask questions, make sure they are specific and include the names of what you are asking about.  For 
+            example, ask "What are major events in Henry Thoreau's life" instead of "What are major events in the author's life?"
             If you don't have any questions, just move on to the next section.""",
             "example_call": '{"prompt": "What is unusual about when this band formed?"}',
         },
     ),
     Task(
         task_name="Define subsections for this section",
         details={
             "description": """Define what subsections should be present within this individual section.  Use the table of contents from the example document and your knowledge of the target page to structure the subsections.  Keeep in mind over differentiation of this section from other sections in the document.  It is totally fine to not have subsections, especially if the example document does not have them.
             Also, remember that the subsections should be relevant for the target document.  The detailed structure of subsections used in the example may not be relevant for our target document.""",
         },
     ),
     Task(
         task_name="Draft New Document Section",
         details={
-            "description": "Draft a new section analogous to the revised example section, ensuring alignment with its structure, format, and scope (from {{TaskRef:Understand Differentiation}} output).  Use the section structure you defined in {{TaskRef:Define subsections for this section}}. However, the details should be related to the target and not the example document.",
+            "description": "Draft a new section analogous to the revised example section, ensuring alignment with its "
+                           "structure, format, and scope (from {{TaskRef:Understand Differentiation}} output).  Use "
+                           "the section structure you defined in {{TaskRef:Define subsections for this section}}. "
+                           "However, the details should be related to the target and not the example document."
+                           "Call the save_draft_section tool to save the draft.",
             "guidelines": [
                 "Clearly identify the section number and section heading/title at the top of the content.",
                 "The new section should have its unique scope and purpose, distinct from the example section.",
                 "Avoid duplicating content or including redundant information.",
                 "Aim for the new section to mirror the example section in length and detail, but using content related to the target.",
                 "Follow the instructions set out by {{TaskRef:Understand Differentiation}} output.",
                 "Maintain consistency in documentation methodology, using the revised example as a template.",
@@ -75,63 +81,24 @@
             ],
             "specific_instructions": [
                 "Do not copy text verbatim. Include only text within the scope of the current section, as highlighted in the output of {{TaskRef:Understand Differentiation}}.",
                 "Include cross-references to other sections as seen in the example if applicable.",
             ],
         },
     ),
-    # Task(
-    #     task_name="Final Section Review",
-    #     details={
-    #         "description": "Review the final text for this section and provide a PASS/FAIL decision based on the success criteria.",
-    #         "prerequisite_tasks": ["Draft New Document Section"],
-    #         "instructions": [
-    #             "Evaluate the success of the new section draft",
-    #             "Document the review outcome",
-    #             "Print the final review output.",
-    #         ],
-    #         "success_flag_criteria": {
-    #             "FAIL": [
-    #                 "The section includes information beyond what's relevant as indicated by {{TaskRef:Understand Differentiation}}.",
-    #                 "Any mention of specific drugs or combination therapies not relevant to the new study context.",
-    #                 "Information in the new section is redundant with the sections analyzed in {{TaskRef:Understand Differentiation}}.",
-    #                 "The draft does not reflect the structure, format, or detail level of the revised example section (output of {{TaskRef:Handle Treatment Details}}).",
-    #                 "Missing or incorrectly referenced tables or figures from the new reference materials.",
-    #                 "Significant deviation from the new reference materials, suggesting misalignment with the study's current focus.",
-    #                 "Inconsistent use of verb tenses where required.",
-    #             ],
-    #             "PASS": [
-    #                 "The section appropriately includes information within the scope defined by {{TaskRef:Understand Differentiation}}.",
-    #                 "The draft logically follows what the section heading describes.",
-    #                 "The draft focuses exclusively on the new study context.",
-    #                 "The draft meets criteria for completeness, accuracy, and is aligned with the revised example and the new reference materials.",
-    #             ],
-    #         },
-    #         "additional_instructions": "Offer feedback on the process of differentiating from other sections, the use of source materials, and the rationale for selected source mappings.",
-    #         "output_format": {
-    #             "Section Review": "[SECTION NUMBER] - [SECTION HEADING]",
-    #             "Draft Review": "[content here]",
-    #             "Comments": "[comments here]",
-    #             "Success Flag": "[FAIL/PASS]",
-    #             "Source Mapping Review": "[REVIEW OF UTILIZED SOURCES]",
-    #             "Tables": "[LIST OF REFERENCED TABLES]",
-    #             "Figures": "[LIST OF REFERENCED FIGURES]",
-    #             "Cross-References": "[REFERENCES TO OTHER DOCUMENT SECTIONS (FROM EXAMPLE DOCUMENT)]",
-    #             "Scope of Section Review": "[REFLECTION ON FOLLOWING THE SCOPE GUIDELINES SET OUT IN {{TaskRef:Understand Differentiation}} OUTPUT]",
-    #         },
-    #     },
-    # ),
     Task(
         task_name="Prepare for Next Document Section",
         details={
-            "description": "SIgnal that you have completed the draft by calling the pop_context function and prepare to start drafting the next section of the document.",
+            "description": "Signal that you have completed the draft by calling the pop_context function and prepare "
+                           "to start drafting the next section of the document.",
             "function_call": "Use the pop_context function with the argument value = current section identifier.",
             "example_call": "{{'current_section_identifier': ['1.2']}}",
             "instructions": [
-                "Announce completion: 'Proceed to the next section of the document, [current section identifier] has been completed.'"
+                "Announce completion: 'Proceed to the next section of the document, [current section identifier] has "
+                "been completed.'"
             ],
         },
     ),
 ]
 
 general_comments = """
 ============
```

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/loader.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from celi_framework.examples.wikipedia.wikipedia_utils import get_cached_session
 
 
 __all__ = [
     "ContentHierarchyNode",
     "ContentReference",
     "load_content_from_wikipedia_url",
+    "format_content",
 ]
 
 
 @dataclass
 class ContentReference:
     """A numbered reference with an external link from a wikipedia article.
```

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/tools.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-from dataclasses import asdict, dataclass
 import json
 import logging
-from platform import node
 import re
+from dataclasses import asdict, dataclass
 from typing import Any, Dict, List, Optional
-from llama_index.core import VectorStoreIndex
+
 from llama_index.core.base.response.schema import Response
 from llama_index.core.schema import MetadataMode, QueryBundle, NodeWithScore, TextNode
 from llama_index.vector_stores.chroma.base import ChromaVectorStore
-from numpy import isin
 
-from celi_framework.core.job_description import ToolImplementations
-from celi_framework.core.templates import (
-    make_draft_setting_output_prompt,
-    make_table_setting_output_prompt,
-)
+from celi_framework.core.job_description import BaseDocToolImplementations
 from celi_framework.examples.wikipedia.index import get_wikipedia_index
 from celi_framework.utils.codex import MongoDBUtilitySingleton
-from celi_framework.utils.llms import quick_ask
-from celi_framework.utils.token_counters import get_master_counter_instance
 from celi_framework.utils.utils import format_toc, get_section_context_as_text
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class RecreatedNode:
@@ -33,19 +25,27 @@
     text: str
 
     def get_content(self):
         return self.text
 
 
 @dataclass
-class WikipediaToolImplementations(ToolImplementations):
+class WikipediaToolImplementations(BaseDocToolImplementations):
+    """If ignore_updates is set, then a cached version of that URL will be used, even if it is out of date.
+    Otherwise, a cache will only be used if it hasn't expired and the content hasn't changed."""
     example_url: str
     target_url: str
     ignore_updates: bool = False
-    """If ignore_updates is set, then a cached version of that URL will be used, even if it is out of date.  Otherwise, a cache will only be used if it hasn't expired and the content hasn't changed."""
+
+    def __init__(self, example_url: str, target_url: str, ignore_updates: bool, drafts_dir: str = "target/celi_output/drafts"):
+        super().__init__(drafts_dir=drafts_dir)
+        self.example_url = example_url
+        self.target_url = target_url
+        self.ignore_updates = ignore_updates
+        self.__post_init__()
 
     def __post_init__(self):
         self.example_page = self._page_title(self.example_url)
         self.target_page = self._page_title(self.target_url)
         self.example_index = get_wikipedia_index(
             self.example_url, ignore_updates=self.ignore_updates
         )
```

### Comparing `celi_framework-0.1.0/celi_framework/examples/wikipedia/wikipedia_utils.py` & `celi_framework-0.2.0/celi_framework/examples/wikipedia/wikipedia_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/embeddor.py` & `celi_framework-0.2.0/celi_framework/experimental/embeddor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/mapper.py` & `celi_framework-0.2.0/celi_framework/experimental/mapper.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/mechanic.py` & `celi_framework-0.2.0/celi_framework/experimental/mechanic.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/preprocessing/pre-processor.py` & `celi_framework-0.2.0/celi_framework/experimental/preprocessing/pre-processor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py` & `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py` & `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py` & `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py` & `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/task_builder/factory.py` & `celi_framework-0.2.0/celi_framework/experimental/task_builder/factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/task_builder/llm_helper_funcs.py` & `celi_framework-0.2.0/celi_framework/experimental/task_builder/llm_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/task_builder/llms.py` & `celi_framework-0.2.0/celi_framework/experimental/task_builder/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/task_builder/template.py` & `celi_framework-0.2.0/celi_framework/experimental/task_builder/template.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/utils/ada.py` & `celi_framework-0.2.0/celi_framework/experimental/utils/ada.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/utils/mapper_utils.py` & `celi_framework-0.2.0/celi_framework/experimental/utils/mapper_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py` & `celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py` & `celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/utils/postprocessor_utils.py` & `celi_framework-0.2.0/celi_framework/experimental/utils/postprocessor_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/experimental/utils/synthetic_data.py` & `celi_framework-0.2.0/celi_framework/experimental/utils/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/logging_config.json` & `celi_framework-0.2.0/celi_framework/logging_config.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8273809523809524%*

 * *Differences: {"'disable_existing_loggers'": 'False',*

 * * "'loggers'": "{'pymongo': OrderedDict([('level', 'INFO')])}"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "disable_existing_loggers": false,
     "formatters": {
         "simple": {
             "format": "%(asctime)s %(name)s %(levelname)s - %(message)s"
         }
     },
     "handlers": {
         "console": {
@@ -42,14 +43,17 @@
         },
         "openai": {
             "level": "INFO"
         },
         "opensearch": {
             "level": "INFO"
         },
+        "pymongo": {
+            "level": "INFO"
+        },
         "requests_cache": {
             "level": "INFO"
         },
         "urllib3": {
             "level": "INFO"
         }
     },
```

### Comparing `celi_framework-0.1.0/celi_framework/logging_setup.py` & `celi_framework-0.2.0/celi_framework/logging_setup.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/main.py` & `celi_framework-0.2.0/celi_framework/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,88 @@
 """
-This Python script establishes a multi-threaded environment for document processing and monitoring within a given system. It is designed to efficiently manage and monitor the processing of documents by utilizing a combination of custom classes, threading, and resource management techniques. The script integrates several components, including:
+This Python script establishes a multithreaded environment for document processing and monitoring within a given system. It is designed to efficiently manage and monitor the processing of documents by utilizing a combination of custom classes, threading, and resource management techniques. The script integrates several components, including:
 
 - `ProcessRunner`: A class responsible for managing the processing pipeline of documents. It uses MongoDB for storage and retrieval of documents and employs a queue for managing updates.
 - `MonitoringAgent`: A class tasked with monitoring the progress and status of document processing, ensuring that system performance is maintained and any issues are promptly addressed.
 - `MongoDBUtilitySingleton`: A singleton class that provides a centralized connection to MongoDB, ensuring efficient data handling and retrieval.
 - `Queue`: A thread-safe queue used for communication between the process runner and monitoring agent, facilitating efficient data exchange and task management.
 
 Key features include:
 - Threading: Utilizes Python's `threading` module to run document processing and monitoring tasks concurrently, improving system throughput and responsiveness.
 - Memory Profiling: Employs the `memory_profiler` module to monitor and optimize memory usage, ensuring the application runs efficiently even under heavy load.
 - Environment Configuration: Leverages `dotenv` for managing environment variables, allowing for flexible configuration of critical paths and parameters without hardcoding.
 
 The script is structured to initiate and manage parallel threads dedicated to document processing and system monitoring, demonstrating an effective pattern for building scalable and responsive Python applications. By separating concerns into distinct threads and utilizing a shared queue for communication, it achieves a high degree of concurrency and efficiency in processing tasks.
 """
 
-if __name__ == "__main__":
-    # This has to be run before any loggers are created.
-    from celi_framework.logging_setup import setup_logging
-
-    setup_logging()
-
 import argparse
-from dataclasses import asdict
 import inspect
-import logging
 import logging.config
 import os
 from typing import Type
 
 from dotenv import load_dotenv
 
 from celi_framework.core.runner import CELIConfig, Directories, MongoDBConfig, run_celi
-from celi_framework.utils.codex import MongoDBUtilitySingleton
-from celi_framework.utils.llmcore_utils import new_parser_factory
+from celi_framework.logging_setup import setup_logging
 from celi_framework.utils.utils import get_obj_by_name, read_json_from_file, str2bool
 
 logger = logging.getLogger(__name__)
 
 
 def get_config():
     load_dotenv("./.env")
-    logger.info(f"Tool config env. var is {os.getenv('TOOL_CONFIG_JSON', '<not set>')}")
 
+    parser = setup_standard_args()
+
+    args = parser.parse_args()
+
+    directories = Directories.create(args.output_dir)
+    mongo_config = None if args.no_db else instantiate_with_argparse_args(args, MongoDBConfig)
+
+    job_description = get_obj_by_name(args.job_description)
+
+    # If the tool_config_json file doesn't exist, try to find it relative to the root of the installed package.
+    # This allows examples packaged with celi to work correctly.
+    if args.tool_config_json:
+        if os.path.exists(args.tool_config_json):
+            tool_config_json = args.tool_config_json
+        else:
+            # Find the root of the installed package
+            root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+            tool_config_json = os.path.join(root_dir, args.tool_config_json)
+            if not os.path.exists(tool_config_json):
+                raise FileNotFoundError(
+                    f"Could not find {args.tool_config_json} or {tool_config_json}"
+                )
+        tool_config = read_json_from_file(tool_config_json)
+    else:
+        tool_config = {}
+
+    tool_implementations = job_description.tool_implementations_class(**tool_config)
+
+    llm_cache = not args.no_cache
+    use_monitor = not args.no_monitor
+
+    # Instantiate the class, passing parser_model as a parameter
+    parser_cls = get_obj_by_name(args.parser_model_class)
+
+    return CELIConfig(  # noqa: F821
+        mongo_config=mongo_config,
+        directories=directories,
+        job_description=job_description,
+        tool_implementations=tool_implementations,
+        parser_cls=parser_cls,
+        parser_model_name=args.parser_model_name,
+        llm_cache=llm_cache,
+        use_monitor=use_monitor,
+    )
+
+
+def setup_standard_args():
     parser = argparse.ArgumentParser(description="Run the document generator.")
 
     def bool_opt(opt: str, env_var: str, help: str):
         parser.add_argument(
             opt,
             action="store_true",
             default=str2bool(os.getenv(env_var, "False")),
@@ -54,15 +91,14 @@
 
     parser.add_argument(
         "--output-dir",
         type=str,
         default=os.getenv("OUTPUT_DIR"),
         help="Output directory path",
     )
-
     parser.add_argument(
         "--db-url",
         type=str,
         default=os.getenv("DB_URL", "mongodb://localhost:27017/"),
         help="Mongo DB URL",
     )
     parser.add_argument(
@@ -95,62 +131,21 @@
     )
     parser.add_argument(
         "--parser-model-name",
         type=str,
         default=os.getenv("PARSER_MODEL_NAME", "mixtral-8x7b-v0.1.Q5_K_M.gguf"),
     )
     bool_opt("--no-cache", "NO_CACHE", "Set to True to turn off LLM caching")
+    bool_opt("--no-db", "NO_DB", "Set to True to turn off database persistence")
     bool_opt(
         "--no-monitor",
         "NO_MONITOR",
         "Set to True to turn off the monitoring thread",
     )
-
-    args = parser.parse_args()
-
-    directories = Directories.create(args.output_dir)
-    mongo_config = instantiate_with_argparse_args(args, MongoDBConfig)
-
-    job_description = get_obj_by_name(args.job_description)
-
-    # If the tool_config_json file doesn't exist, try to find it relative to the root of the installed package.
-    # This allows examples packaged with celi to work correctly.
-    if args.tool_config_json:
-        if os.path.exists(args.tool_config_json):
-            tool_config_json = args.tool_config_json
-        else:
-            # Find the root of the installed package
-            root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-            tool_config_json = os.path.join(root_dir, args.tool_config_json)
-            if not os.path.exists(tool_config_json):
-                raise FileNotFoundError(
-                    f"Could not find {args.tool_config_json} or {tool_config_json}"
-                )
-        tool_config = read_json_from_file(tool_config_json)
-    else:
-        tool_config = {}
-
-    tool_implementations = job_description.tool_implementations_class(**tool_config)
-
-    llm_cache = not args.no_cache
-    use_monitor = not args.no_monitor
-
-    # Instantiate the class, passing parser_model as a parameter
-    parser_cls = get_obj_by_name(args.parser_model_class)
-
-    return CELIConfig(  # noqa: F821
-        mongo_config=mongo_config,
-        directories=directories,
-        job_description=job_description,
-        tool_implementations=tool_implementations,
-        parser_cls=parser_cls,
-        parser_model_name=args.parser_model_name,
-        llm_cache=llm_cache,
-        use_monitor=use_monitor,
-    )
+    return parser
 
 
 def instantiate_with_argparse_args(args: argparse.Namespace, cls: Type):
     """Instantiates the given class, passing any args that match class members as keyword args."""
     init_signature = inspect.signature(cls.__init__)
     arg_names = [
         param_name
@@ -159,10 +154,13 @@
     ]
     # cls.__annotations__
     cls_args = {k: v for k, v in vars(args).items() if k in arg_names}
     return cls(**cls_args)
 
 
 if __name__ == "__main__":
+    setup_logging()
     logger.debug("Starting CELI")
     config = get_config()
     run_celi(config)
+
+
```

### Comparing `celi_framework-0.1.0/celi_framework/utils/codex.py` & `celi_framework-0.2.0/celi_framework/utils/codex.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 from datetime import datetime
 
 from celi_framework.utils.utils import generate_hash_id
 
 logger = logging.getLogger(__name__)
 
 
+class NoDBCodex:
+    _id: str = 'NullCodex'
+
+    def save_document_with_versioning(self, document, collection_name):
+        return None
+
+
 class MongoDBUtilitySingleton:
     _instance = None
     _lock = threading.Lock()
 
     def __new__(
         cls,
         id_prefix: str = "process",
```

### Comparing `celi_framework-0.1.0/celi_framework/utils/llmcore_utils.py` & `celi_framework-0.2.0/celi_framework/utils/llmcore_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,20 @@
 
 def parse(dataclass_parser: ParserFactory, target_cls: Type[T], msg: str) -> T:
     """
     Parses the given message into the specified target_cls, using the model defined by parser_factory.
     """
     try:
         with dataclass_parser(target_cls) as parser:
-            ret = parser.parse(msg)  # type: ignore
+            try:
+                ret = parser.parse(msg)  # type: ignore
+            except Exception:
+                app_logger.info(f"Parsing failed, retrying")
+                msg = "Make sure your response is valid JSON.\n"+ msg
+                ret = parser.parse(msg)  # type: ignore
             app_logger.info(f"Parsed {ret}")
             setattr(ret, "parser_model", parser.model_name)
             return ret
     except ValueError as e:
         if "Model path does not exist" in str(e):
             raise UnrecoverableException(
                 f"Model has not been cached.  Download with something like\nwget -P {MODELS_CACHE_DIR} https://huggingface.co/TheBloke/Mixtral-8x7B-v0.1-GGUF/resolve/main/mixtral-8x7b-v0.1.Q2_K.gguf\n",
```

### Comparing `celi_framework-0.1.0/celi_framework/utils/llms.py` & `celi_framework-0.2.0/celi_framework/utils/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/utils/sql_utils.py` & `celi_framework-0.2.0/celi_framework/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/utils/token_counters.py` & `celi_framework-0.2.0/celi_framework/utils/token_counters.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/celi_framework/utils/utils.py` & `celi_framework-0.2.0/celi_framework/utils/utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.1.0/pyproject.toml` & `celi_framework-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celi-framework"
-version = "0.1.0"
+version = "0.2.0"
 description = "Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment."
 authors = ["Jan-Samuel Wagner <jwab@genmab.com>","Dave DeCaprio <daved@alum.mit.edu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/x3n0cr4735/celi"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -24,14 +24,16 @@
 python-dotenv = ">=1.0.0"
 requests-cache = ">=1.2.0"
 llama-index = ">=0.10.23"
 llama-index-vector-stores-chroma = "^0.1.6"
 scikit-learn = "^1.4.2"
 pymupdf = "^1.24.1"
 python-docx = "^1.1.0"
+jupyter = "^1.0.0"
+timeout-decorator = "^0.5.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.4.4"
 pytest-asyncio = ">=0.23.3"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = ">=6.29.3"
@@ -45,12 +47,12 @@
 sphinx-autobuild = "^2021.3.14"
 protobuf = ">=4.21.6" # Added to address build issues with readthedocs.
 cffi = ">=1.10.0" # Added to address build issues with readthedocs. pyo3_runtime.PanicException: Python API call failed
 sphinx-autodoc-typehints = "^2.0.0"
 
 [tool.pytest.ini_options]
 log_level="DEBUG"
-log_cli=true
+#log_cli=true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `celi_framework-0.1.0/PKG-INFO` & `celi_framework-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celi-framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment.
 Home-page: https://github.com/x3n0cr4735/celi
 License: MIT
 Author: Jan-Samuel Wagner
 Author-email: jwab@genmab.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,23 +15,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Requires-Dist: bert-score (>=0.3.13)
 Requires-Dist: evaluate (>=0.4.1)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: llama-index (>=0.10.23)
 Requires-Dist: llama-index-vector-stores-chroma (>=0.1.6,<0.2.0)
 Requires-Dist: py-llm-core (>=2.8.2)
 Requires-Dist: pymongo (>=4.6.2)
 Requires-Dist: pymupdf (>=1.24.1,<2.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0)
 Requires-Dist: requests-cache (>=1.2.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: timeout-decorator (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/x3n0cr4735/celi
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/celi-framework.svg)](https://badge.fury.io/py/celi-framework)
 [![Tests](https://github.com/x3n0cr4735/celi/actions/workflows/tests.yml/badge.svg)](https://github.com/x3n0cr4735/celi/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/celi/badge/?version=latest)](https://celi.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

