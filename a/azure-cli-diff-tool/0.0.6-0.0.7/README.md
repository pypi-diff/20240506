# Comparing `tmp/azure-cli-diff-tool-0.0.6.tar.gz` & `tmp/azure_cli_diff_tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-cli-diff-tool-0.0.6.tar", last modified: Mon Mar 25 06:57:14 2024, max compression
+gzip compressed data, was "azure_cli_diff_tool-0.0.7.tar", last modified: Mon May  6 09:02:17 2024, max compression
```

## Comparing `azure-cli-diff-tool-0.0.6.tar` & `azure_cli_diff_tool-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-25 06:57:14.540374 azure-cli-diff-tool-0.0.6/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3868 2024-03-25 06:57:14.540374 azure-cli-diff-tool-0.0.6/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3050 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/README.rst
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-25 06:57:14.536373 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6501 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4574 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/_const.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-25 06:57:14.540374 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/data/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      164 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/data/blob_config.ini
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      540 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/data/meta_change_whitelist.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18429 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/meta_change.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23660 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/meta_change_detect.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10696 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/utils.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-25 06:57:14.540374 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3868 2024-03-25 06:57:14.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      538 2024-03-25 06:57:14.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-25 06:57:14.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2024-03-25 06:57:14.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-25 06:57:14.000000 azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-25 06:57:14.540374 azure-cli-diff-tool-0.0.6/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1405 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-25 06:57:14.540374 azure-cli-diff-tool-0.0.6/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      317 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/tests/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9026 2024-03-25 06:57:01.000000 azure-cli-diff-tool-0.0.6/tests/test_break_change.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 09:02:17.884428 azure_cli_diff_tool-0.0.7/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3934 2024-05-06 09:02:17.884428 azure_cli_diff_tool-0.0.7/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3050 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/README.rst
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 09:02:17.880428 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6501 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4574 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/_const.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 09:02:17.880428 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/data/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      164 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/data/blob_config.ini
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      540 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/data/meta_change_whitelist.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18429 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/meta_change.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23522 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/meta_change_detect.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10696 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 09:02:17.884428 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3934 2024-05-06 09:02:17.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      538 2024-05-06 09:02:17.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-06 09:02:17.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2024-05-06 09:02:17.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-05-06 09:02:17.000000 azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-06 09:02:17.884428 azure_cli_diff_tool-0.0.7/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1405 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 09:02:17.884428 azure_cli_diff_tool-0.0.7/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      317 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/tests/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9813 2024-05-06 09:01:16.000000 azure_cli_diff_tool-0.0.7/tests/test_break_change.py
```

### Comparing `azure-cli-diff-tool-0.0.6/PKG-INFO` & `azure_cli_diff_tool-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-cli-diff-tool
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for cli metadata management
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Requires-Dist: deepdiff
 Requires-Dist: requests
 
@@ -94,14 +94,18 @@
     THE SOFTWARE IS PROVIDED *AS IS*, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.::
 
 
 .. :changelog:
 
 Release History
 ===============
+0.0.7
+++++++
+* Remove unnecessary debug logs for meta comparison
+
 0.0.6
 ++++++
 * Add diff support for deprecate_info in subgroup, cmd, parameters and options
 
 0.0.5
 ++++++
 * Add `DiffLevel` to meta comparison
```

### Comparing `azure-cli-diff-tool-0.0.6/README.rst` & `azure_cli_diff_tool-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/__init__.py` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 from deepdiff import DeepDiff
 from .meta_change_detect import MetaChangeDetect
 from .utils import get_blob_config, load_blob_config_file, get_target_version_modules, get_target_version_module, \
     extract_module_name_from_meta_file, export_meta_changes_to_csv, export_meta_changes_to_json, \
     export_meta_changes_to_dict, expand_deprecate_obj
 
-__VERSION__ = '0.0.6'
+__VERSION__ = '0.0.7'
 
 logger = logging.getLogger(__name__)
 
 
 class DiffExportFormat(Enum):
     DICT = "dict"
     TEXT = "text"
```

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/_const.py` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/_const.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/data/meta_change_whitelist.txt` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/data/meta_change_whitelist.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/meta_change.py` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/meta_change.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/meta_change_detect.py` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/meta_change_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,17 +382,14 @@
         for obj in self.diff_objs:
             if obj.filter_key and obj.is_break and "\t".join(obj.filter_key) in self.meta_change_whitelist:
                 continue
             new_diff_objs.append(obj)
         self.diff_objs = new_diff_objs
 
     def check_deep_diffs(self):
-        for diff_type, diff_key in self.deep_diff.items():
-            for it in diff_key:
-                    print(diff_type, ": ", it)
         self.check_dict_item_remove()
         self.check_dict_item_add()
         self.check_list_item_remove()
         self.check_list_item_add()
         self.check_value_change()
         self.check_cmds_parameter_diff()
         self.filter_diffs_by_whitelist()
```

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool/utils.py` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool/utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/PKG-INFO` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-cli-diff-tool
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for cli metadata management
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Requires-Dist: deepdiff
 Requires-Dist: requests
 
@@ -94,14 +94,18 @@
     THE SOFTWARE IS PROVIDED *AS IS*, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.::
 
 
 .. :changelog:
 
 Release History
 ===============
+0.0.7
+++++++
+* Remove unnecessary debug logs for meta comparison
+
 0.0.6
 ++++++
 * Add diff support for deprecate_info in subgroup, cmd, parameters and options
 
 0.0.5
 ++++++
 * Add `DiffLevel` to meta comparison
```

### Comparing `azure-cli-diff-tool-0.0.6/azure_cli_diff_tool.egg-info/SOURCES.txt` & `azure_cli_diff_tool-0.0.7/azure_cli_diff_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/setup.py` & `azure_cli_diff_tool-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.6/tests/test_break_change.py` & `azure_cli_diff_tool-0.0.7/tests/test_break_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -----------------------------------------------------------------------------
 # pylint: disable=line-too-long
 
 import unittest
 import os
 from azure_cli_diff_tool import meta_diff
 from azure_cli_diff_tool.utils import get_command_tree, extract_cmd_name, extract_cmd_property, extract_para_info, \
-    extract_subgroup_name, extract_subgroup_deprecate_property, expand_deprecate_obj
+    extract_subgroup_name, extract_subgroup_deprecate_property, expand_deprecate_obj, extract_subgroup_property
 
 
 class MyTestCase(unittest.TestCase):
 
     def test_parse_cmd_tree(self):
         cmd_name = "monitor log-profiles create"
         ret = get_command_tree(cmd_name)
@@ -49,14 +49,25 @@
         has_subgroup, subgroup_name = extract_subgroup_name(test_key)
         self.assertTrue(has_subgroup, "sub group parse failed from diff dict key")
         self.assertEqual(subgroup_name, "acr", "sub group name extract failed")
         has_subgroup_deprecate_prop, subgroup_deprecate_prop = extract_subgroup_deprecate_property(test_key, "deprecate_info")
         self.assertTrue(has_subgroup_deprecate_prop, "sub group deprecate info prop parse failed from diff dict key")
         self.assertEqual(subgroup_deprecate_prop, "hide", "sub group deprecate prop extract failed")
 
+    def test_diff_dict_key_for_subgroups_prop(self):
+        test_key = "root['sub_groups']['acr']['deprecate_info_hide']"
+        has_cmd, _ = extract_cmd_name(test_key)
+        self.assertFalse(has_cmd, "cmd parse error from diff dict key")
+        has_subgroup, subgroup_name = extract_subgroup_name(test_key)
+        self.assertTrue(has_subgroup, "sub group parse failed from diff dict key")
+        self.assertEqual(subgroup_name, "acr", "sub group name extract failed")
+        has_subgroup_prop, subgroup_prop = extract_subgroup_property(test_key, subgroup_name)
+        self.assertTrue(has_subgroup_prop, "sub group prop parse failed from diff dict key")
+        self.assertEqual(subgroup_prop, "deprecate_info_hide", "sub group prop extract failed")
+
     def test_diff_meta(self):
         if not os.path.exists("./jsons/az_monitor_meta_before.json") \
                 or not os.path.exists("./jsons/az_monitor_meta_after.json"):
             return
         result = meta_diff(base_meta_file="./jsons/az_monitor_meta_before.json",
                            diff_meta_file="./jsons/az_monitor_meta_after.json",
                            output_type="text")
```

