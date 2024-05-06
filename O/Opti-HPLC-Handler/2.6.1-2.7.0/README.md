# Comparing `tmp/Opti_HPLC_Handler-2.6.1.tar.gz` & `tmp/opti_hplc_handler-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Opti_HPLC_Handler-2.6.1.tar", last modified: Fri Mar 22 09:37:42 2024, max compression
+gzip compressed data, was "opti_hplc_handler-2.7.0.tar", last modified: Mon May  6 06:49:57 2024, max compression
```

## Comparing `Opti_HPLC_Handler-2.6.1.tar` & `opti_hplc_handler-2.7.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:37:42.985272 Opti_HPLC_Handler-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-03-22 09:37:42.985272 Opti_HPLC_Handler-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-22 09:37:27.000000 Opti_HPLC_Handler-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 09:37:42.985272 Opti_HPLC_Handler-2.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:37:42.981272 Opti_HPLC_Handler-2.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:37:42.981272 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-22 09:37:27.000000 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_api_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17108 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_instrument_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    15791 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_module_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:37:42.985272 Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-03-22 09:37:42.000000 Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-22 09:37:42.000000 Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 09:37:42.000000 Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-22 09:37:42.000000 Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-22 09:37:42.000000 Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:37:42.985272 Opti_HPLC_Handler-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/tests/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/tests/test_instrument_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    51416 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/tests/test_module_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    23590 2024-03-22 09:37:19.000000 Opti_HPLC_Handler-2.6.1/tests/test_proxy_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.678278 opti_hplc_handler-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-06 06:49:57.678278 opti_hplc_handler-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 06:49:43.000000 opti_hplc_handler-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:49:57.678278 opti_hplc_handler-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.670278 opti_hplc_handler-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 06:49:43.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_api_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_instrument_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_module_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/validate_gradient_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/validate_method_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_instrument_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50054 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_module_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23590 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_proxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_utils.py
```

### Comparing `Opti_HPLC_Handler-2.6.1/LICENSE` & `opti_hplc_handler-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-2.6.1/PKG-INFO` & `opti_hplc_handler-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Opti_HPLC_Handler
-Version: 2.6.1
+Version: 2.7.0
 Summary: Simplified proxy API for interacting with the Waters Empower Web API.
 Author-email: Søren Furbo <srfu@novonordisk.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, novonordisk-research
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.6.1 Summary:
+Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.7.0 Summary:
 Simplified proxy API for interacting with the Waters Empower Web API. Author-
 email: SÃ¸ren Furbo
 novonordisk.com> License: BSD 3-Clause License Copyright (c) 2023, novonordisk-
 research Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
```

### Comparing `Opti_HPLC_Handler-2.6.1/README.md` & `opti_hplc_handler-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-2.6.1/pyproject.toml` & `opti_hplc_handler-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Opti_HPLC_Handler"
-version = "2.6.1"
+version = "2.7.0"
 description = "Simplified proxy API for interacting with the Waters Empower Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   { name="Søren Furbo", email="srfu@novonordisk.com" },
 ]
@@ -90,15 +90,15 @@
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
 
 [tool.bumpver]
-current_version = "2.6.1"
+current_version = "2.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/data_types.py` & `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/data_types.py`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_api_core.py` & `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_api_core.py`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_handler.py` & `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Generic, Iterable, List, Mapping, Optional, TypeVar
 
-from .data_types import HplcResult, HPLCSetup
 from .empower_api_core import EmpowerConnection
 from .empower_instrument_method import EmpowerInstrumentMethod
+from .utils.data_types import HplcResult, HPLCSetup
 
 Result = TypeVar("Result")
 
 Setup = TypeVar("Setup")
 
 logger = logging.getLogger(__name__)
```

### Comparing `Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_instrument_method.py` & `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_instrument_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
+import re
 from typing import List, Optional, Union
 
-from OptiHPLCHandler.data_types import EmpowerInstrumentMethodModel as DataModel
-from OptiHPLCHandler.empower_module_method import (
+from .empower_module_method import (
     ColumnManagerMethod,
     ColumnOvenMethod,
     EmpowerModuleMethod,
     SampleManagerMethod,
     SolventManagerMethod,
     module_method_factory,
 )
+from .utils.data_types import EmpowerInstrumentMethodModel as DataModel
 
 logger = logging.getLogger(__name__)
 
 
 class EmpowerInstrumentMethod:
     """
     A class to handle Empower instrument methods.
@@ -131,30 +132,39 @@
             )
         self.solvent_handler_method.gradient_table = gradient_table
 
     @property
     def valve_position(self):
         """
         The valve position for the solvent manager, if a solvent manager module method
-        is present.
+        is present. When setting, can be a list of valve positions (e.g. ["A1", "B2"]),
+        or a string containing one or more valve positions, (e.g. "A1, B2").
         """
         if self.solvent_handler_method is None:
             raise ValueError(
                 "Can't get valve position, "
                 "no solvent manager found in instrument method."
             )
         return self.solvent_handler_method.valve_position
 
     @valve_position.setter
-    def valve_position(self, valve_position: str):
+    def valve_position(self, valve_position: Union[str, List[str]]):
         if self.solvent_handler_method is None:
             raise ValueError(
                 "Can't set valve position, "
                 "no solvent manager found in instrument method."
             )
+        if isinstance(valve_position, str):
+            valve_position = [i[0] for i in re.finditer(r"[A-D]\d", valve_position)]
+            # Make a list of every instance of XY in the string, where X is A, B, C
+            # or D, and Y is a digit (0-9). These are presumed to be valve positions.
+            if len(valve_position) == 0:
+                raise ValueError(
+                    f"Found nothing that could be a valve position in {valve_position}"
+                )
         self.solvent_handler_method.valve_position = valve_position
 
     def __str__(self):
         return (
             f"{type(self).__name__} with "
             f"{len(self.module_method_list)} module methods of types "
             + (", ".join([type(method).__name__ for method in self.module_method_list]))
```

### Comparing `Opti_HPLC_Handler-2.6.1/src/OptiHPLCHandler/empower_module_method.py` & `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_module_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import re
 import warnings
 from typing import Dict, List, Mapping, Tuple, Union
 from xml.etree import ElementTree as ET
 
-from OptiHPLCHandler.data_types import EmpowerModuleMethodModel as DataModel
+from .utils.data_types import EmpowerModuleMethodModel as DataModel
 
 logger = logging.getLogger(__name__)
 
 
 class EmpowerModuleMethod:
     """
     Generic module method class that can be used for any Empower module method.
@@ -208,37 +208,30 @@
     valve_tag_suffix: str
     solvent_lines: List[str]
 
     @property
     def valve_position(self) -> List[str]:
         """
         The current valve position for each solvent line. When setting, the value can be
-        a string or a list of strings. If a string is given, it should be of the form
-        `XY`, where `X` is the solvent line (A, B, C, D) and `Y` is the position (0-6).
-        If a list is given, each string should be of that form.
-        """
-        valve_position_tags = [
-            self.valve_tag_prefix + solvent + self.valve_tag_suffix
-            for solvent in self.solvent_lines
-        ]
-        valve_positions = [
-            solvent + self[tag]
-            for solvent, tag in zip(self.solvent_lines, valve_position_tags)
+        a list of strings. Each string should should be of the form `XY`, where `X`
+        is the solvent line (A, B, C, D) and `Y` is the position (0-6).
+        """
+        valve_position_list = [
+            line + self[self.valve_tag_prefix + line + self.valve_tag_suffix]
+            for line in self.solvent_lines
         ]
         # Consider removing the ones that have position 0,
         # to make QSM methods easier to read.
-        return valve_positions
+        return valve_position_list
 
     def __str__(self):
         return f"{type(self).__name__} with valve positions {self.valve_position}"
 
     @valve_position.setter
-    def valve_position(self, value: Union[str, List[str]]) -> None:
-        if isinstance(value, str):
-            value = [value]
+    def valve_position(self, value: List[str]) -> None:
         for position in value:
             if position[0] not in self.solvent_lines:
                 raise ValueError(
                     f"Invalid valve position {position}, "
                     f"must start with one of {self.solvent_lines}"
                 )
             self[
@@ -301,17 +294,17 @@
                     f"got {new_gradient_table[0]['Time']}."
                 )
         new_gradient_table[0]["Curve"] = "Initial"
         xml = ET.Element("GradientTable")
         for row in new_gradient_table:
             row_xml = ET.SubElement(xml, "GradientRow")
             curve = row.get("Curve", "6")
+            # "6" is linear, which covers 90% of the use cases
             ET.SubElement(row_xml, "Time").text = self._round(row["Time"])
             ET.SubElement(row_xml, "Flow").text = self._round(row["Flow"])
-            # "6" is linear, which covers 90% of the use cases
             for line in self.solvent_lines:
                 line_name = f"Composition{line}"
                 ET.SubElement(row_xml, line_name).text = self._round(row[line_name])
             ET.SubElement(row_xml, "Curve").text = str(curve)
             # Consider validating curve (1-11)
         gradient_xml = ET.tostring(xml, encoding="unicode")
         gradient_xml = gradient_xml.replace("<GradientTable>", "").replace(
```

### Comparing `Opti_HPLC_Handler-2.6.1/src/Opti_HPLC_Handler.egg-info/PKG-INFO` & `opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Opti_HPLC_Handler
-Version: 2.6.1
+Version: 2.7.0
 Summary: Simplified proxy API for interacting with the Waters Empower Web API.
 Author-email: Søren Furbo <srfu@novonordisk.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, novonordisk-research
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.6.1 Summary:
+Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.7.0 Summary:
 Simplified proxy API for interacting with the Waters Empower Web API. Author-
 email: SÃ¸ren Furbo
 novonordisk.com> License: BSD 3-Clause License Copyright (c) 2023, novonordisk-
 research Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
```

### Comparing `Opti_HPLC_Handler-2.6.1/tests/test_core_api.py` & `opti_hplc_handler-2.7.0/tests/test_core_api.py`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-2.6.1/tests/test_instrument_method.py` & `opti_hplc_handler-2.7.0/tests/test_instrument_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,112 +205,137 @@
         assert method.module_method_list[1].column_temperature == "50.03"
 
 
 class TestSolventManager(unittest.TestCase):
     def setUp(self) -> None:
         self.example = get_example_file_dict()
         self.bsm_example = self.example["response-BSM-PDA-Acq.json"]
+        self.method = EmpowerInstrumentMethod(self.bsm_example)
 
     def test_init(self):
-        method = EmpowerInstrumentMethod(self.bsm_example)
-        assert method.solvent_handler_method is not None
-        assert isinstance(method.solvent_handler_method, SolventManagerMethod)
+        assert self.method.solvent_handler_method is not None
+        assert isinstance(self.method.solvent_handler_method, SolventManagerMethod)
 
     def test_init_none(self):
         method_definition = self.bsm_example["results"][0]
         method_definition["modules"] = [method_definition["modules"][0]]
         method = EmpowerInstrumentMethod(method_definition)
         assert method.solvent_handler_method is None
 
     def test_init_multiple(self):
         method_definition = self.bsm_example["results"][0]
         method_definition["modules"].append(method_definition["modules"][1])
         with self.assertRaises(ValueError):
             EmpowerInstrumentMethod(method_definition)
 
     def test_get_gradient_table(self):
-        method = EmpowerInstrumentMethod(self.bsm_example)
-        gradient_table = method.gradient_table
+        gradient_table = self.method.gradient_table
         assert isinstance(gradient_table, list)
         assert isinstance(gradient_table[0], dict)
 
     def test_get_gradient_table_none(self):
         method_definition = self.bsm_example["results"][0]
         method_definition["modules"] = [method_definition["modules"][0]]
         method = EmpowerInstrumentMethod(method_definition)
         with self.assertRaises(ValueError):
             method.gradient_table
 
     def test_set_gradient_table(self):
-        method = EmpowerInstrumentMethod(self.bsm_example)
-        gradient_table = method.gradient_table
+        gradient_table = self.method.gradient_table
         assert gradient_table[0]["Flow"] != "0.1"
         assert (
-            "<Flow>0.1</Flow>" not in method.current_method["modules"][1]["nativeXml"]
+            "<Flow>0.1</Flow>"
+            not in self.method.current_method["modules"][1]["nativeXml"]
         )
         gradient_table[0]["Flow"] = "0.1"
-        method.gradient_table = gradient_table
-        assert method.gradient_table[0]["Flow"] == "0.1"
-        assert "<Flow>0.1</Flow>" in method.current_method["modules"][1]["nativeXml"]
+        self.method.gradient_table = gradient_table
+        assert self.method.gradient_table[0]["Flow"] == "0.1"
+        assert (
+            "<Flow>0.1</Flow>" in self.method.current_method["modules"][1]["nativeXml"]
+        )
 
     def test_set_gradient_table_none(self):
         method_definition = self.bsm_example["results"][0]
         method_definition["modules"] = [method_definition["modules"][0]]
         method = EmpowerInstrumentMethod(method_definition)
         with self.assertRaises(ValueError):
             method.gradient_table = [{"Flow": "0.1"}]
 
 
 class TestValvePosition(unittest.TestCase):
     def setUp(self) -> None:
         self.example = get_example_file_dict()
         self.bsm_example = self.example["response-BSM-PDA-Acq.json"]
+        self.method = EmpowerInstrumentMethod(self.bsm_example)
 
     def test_get(self):
-        method = EmpowerInstrumentMethod(self.bsm_example)
-        assert method.valve_position == ["A1", "B1"]
+        assert self.method.valve_position == ["A1", "B1"]
 
     def test_get_none(self):
         method_definition = self.bsm_example["results"][0]
         method_definition["modules"] = [method_definition["modules"][0]]
         method = EmpowerInstrumentMethod(method_definition)
         with self.assertRaises(ValueError):
             method.valve_position
 
-    def test_set(self):
-        method = EmpowerInstrumentMethod(self.bsm_example)
-        method.valve_position = "A2"
-        assert method.valve_position == ["A2", "B1"]
+    def test_set_list_one(self):
+        self.method.valve_position = ["A2"]
+        assert self.method.valve_position == ["A2", "B1"]
         assert (
             "<FlowSourceA>2</FlowSourceA>"
-            in method.current_method["modules"][1]["nativeXml"]
+            in self.method.current_method["modules"][1]["nativeXml"]
         )
         assert (
             "<FlowSourceB>1</FlowSourceB>"
-            in method.current_method["modules"][1]["nativeXml"]
+            in self.method.current_method["modules"][1]["nativeXml"]
         )
-        method.valve_position = ["A7", "B5"]
-        assert method.valve_position == ["A7", "B5"]
+
+    def test_set_list_multiple(self):
+        self.method.valve_position = ["A7", "B5"]
+        assert self.method.valve_position == ["A7", "B5"]
         assert (
             "<FlowSourceA>7</FlowSourceA>"
-            in method.current_method["modules"][1]["nativeXml"]
+            in self.method.current_method["modules"][1]["nativeXml"]
         )
         assert (
             "<FlowSourceB>5</FlowSourceB>"
-            in method.current_method["modules"][1]["nativeXml"]
+            in self.method.current_method["modules"][1]["nativeXml"]
+        )
+
+    def test_set_str_single(self):
+        self.method.valve_position = "A2"
+        assert self.method.valve_position == ["A2", "B1"]
+        assert (
+            "<FlowSourceA>2</FlowSourceA>"
+            in self.method.current_method["modules"][1]["nativeXml"]
+        )
+        assert (
+            "<FlowSourceB>1</FlowSourceB>"
+            in self.method.current_method["modules"][1]["nativeXml"]
+        )
+
+    def test_set_str_multiple(self):
+        self.method.valve_position = "A2, B3"
+        assert self.method.valve_position == ["A2", "B3"]
+        assert (
+            "<FlowSourceA>2</FlowSourceA>"
+            in self.method.current_method["modules"][1]["nativeXml"]
+        )
+        assert (
+            "<FlowSourceB>3</FlowSourceB>"
+            in self.method.current_method["modules"][1]["nativeXml"]
         )
 
     def test_set_none(self):
         method_definition = self.bsm_example["results"][0]
         method_definition["modules"] = [method_definition["modules"][0]]
         method = EmpowerInstrumentMethod(method_definition)
         with self.assertRaises(ValueError):
             method.valve_position = "A2"
         with self.assertRaises(ValueError):
             method.valve_position = ["A2", "B1"]
 
     def test_method_name(self):
-        method = EmpowerInstrumentMethod(self.bsm_example)
-        assert method.method_name == "AcquityBSMPDA"
-        method.method_name = "new_name"
-        assert method.method_name == "new_name"
-        assert method.current_method["methodName"] == "new_name"
+        assert self.method.method_name == "AcquityBSMPDA"
+        self.method.method_name = "new_name"
+        assert self.method.method_name == "new_name"
+        assert self.method.current_method["methodName"] == "new_name"
```

### Comparing `Opti_HPLC_Handler-2.6.1/tests/test_module_method.py` & `opti_hplc_handler-2.7.0/tests/test_module_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,36 +387,14 @@
             "<SolventSelectionValveCPosition>0</SolventSelectionValveCPosition>"
             in module_method.current_method["nativeXml"]
         )
         assert (
             "<SolventSelectionValveDPosition>2</SolventSelectionValveDPosition>"
             in module_method.current_method["nativeXml"]
         )
-        module_method.valve_position = "D1"
-        assert module_method.valve_position == ["A0", "B0", "C0", "D1"]
-        assert "A0" in str(module_method)
-        assert "B0" in str(module_method)
-        assert "C0" in str(module_method)
-        assert "D1" in str(module_method)
-        assert (
-            "<SolventSelectionValveAPosition>0</SolventSelectionValveAPosition>"
-            in module_method.current_method["nativeXml"]
-        )
-        assert (
-            "<SolventSelectionValveBPosition>0</SolventSelectionValveBPosition>"
-            in module_method.current_method["nativeXml"]
-        )
-        assert (
-            "<SolventSelectionValveCPosition>0</SolventSelectionValveCPosition>"
-            in module_method.current_method["nativeXml"]
-        )
-        assert (
-            "<SolventSelectionValveDPosition>1</SolventSelectionValveDPosition>"
-            in module_method.current_method["nativeXml"]
-        )
 
     def test_gradient_table(self):
         module_method = QSMMethod(self.minimal_definition)
         assert len(module_method.gradient_table) == 1
         assert module_method.gradient_table[0]["Time"] == "Initial"
         assert module_method.gradient_table[0]["Flow"] == "1.5"
         assert module_method.gradient_table[0]["CompositionA"] == "25.0"
@@ -885,24 +863,14 @@
         assert "B2" in str(module_method)
         assert (
             "<FlowSourceA>2</FlowSourceA>" in module_method.current_method["nativeXml"]
         )
         assert (
             "<FlowSourceB>2</FlowSourceB>" in module_method.current_method["nativeXml"]
         )
-        module_method.valve_position = "A1"
-        assert module_method.valve_position == ["A1", "B2"]
-        assert "A1" in str(module_method)
-        assert "B2" in str(module_method)
-        assert (
-            "<FlowSourceA>1</FlowSourceA>" in module_method.current_method["nativeXml"]
-        )
-        assert (
-            "<FlowSourceB>2</FlowSourceB>" in module_method.current_method["nativeXml"]
-        )
 
     def test_gradient_table(self):
         module_method = BSMMethod(self.minimal_definition)
         assert len(module_method.gradient_table) == 1
         assert module_method.gradient_table[0]["Time"] == "Initial"
         assert module_method.gradient_table[0]["Flow"] == "0.600"
         assert module_method.gradient_table[0]["CompositionA"] == "100.0"
```

### Comparing `Opti_HPLC_Handler-2.6.1/tests/test_proxy_api.py` & `opti_hplc_handler-2.7.0/tests/test_proxy_api.py`

 * *Files identical despite different names*

