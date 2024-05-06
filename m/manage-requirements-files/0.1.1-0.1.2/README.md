# Comparing `tmp/manage_requirements_files-0.1.1.tar.gz` & `tmp/manage_requirements_files-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manage_requirements_files-0.1.1.tar", last modified: Sun May  5 13:42:54 2024, max compression
+gzip compressed data, was "manage_requirements_files-0.1.2.tar", last modified: Mon May  6 21:22:52 2024, max compression
```

## Comparing `manage_requirements_files-0.1.1.tar` & `manage_requirements_files-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     1070 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.1/LICENSE
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3270 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/PKG-INFO
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2722 2024-05-05 13:35:43.000000 manage_requirements_files-0.1.1/README.md
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/manage_requirements_files/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.1/manage_requirements_files/__init__.py
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2033 2024-05-05 13:10:13.000000 manage_requirements_files-0.1.1/manage_requirements_files/cli.py
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3270 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/PKG-INFO
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      381 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/SOURCES.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        1 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/dependency_links.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       76 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/entry_points.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       32 2024-05-05 13:42:54.000000 manage_requirements_files-0.1.1/manage_requirements_files.egg-info/top_level.txt
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       38 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/setup.cfg
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      829 2024-05-05 13:34:38.000000 manage_requirements_files-0.1.1/setup.py
-drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 13:42:54.183116 manage_requirements_files-0.1.1/tests/
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 10:51:15.000000 manage_requirements_files-0.1.1/tests/__init__.py
--rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     7338 2024-05-05 13:24:19.000000 manage_requirements_files-0.1.1/tests/test_cli.py
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     1070 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.2/LICENSE
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3255 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/PKG-INFO
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2707 2024-05-06 21:08:20.000000 manage_requirements_files-0.1.2/README.md
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.486938 manage_requirements_files-0.1.2/manage_requirements_files/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-05 10:03:57.000000 manage_requirements_files-0.1.2/manage_requirements_files/__init__.py
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     2055 2024-05-06 21:08:30.000000 manage_requirements_files-0.1.2/manage_requirements_files/cli.py
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     3255 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/PKG-INFO
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      381 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        1 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       76 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/entry_points.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       32 2024-05-06 21:22:52.000000 manage_requirements_files-0.1.2/manage_requirements_files.egg-info/top_level.txt
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)       38 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/setup.cfg
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)      829 2024-05-06 21:22:04.000000 manage_requirements_files-0.1.2/setup.py
+drwxrwxr-x   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:22:52.490938 manage_requirements_files-0.1.2/tests/
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)        0 2024-05-06 21:08:30.000000 manage_requirements_files-0.1.2/tests/__init__.py
+-rw-rw-r--   0 guilhermegouw  (1000) guilhermegouw  (1000)     7293 2024-05-06 21:08:30.000000 manage_requirements_files-0.1.2/tests/test_cli.py
```

### Comparing `manage_requirements_files-0.1.1/LICENSE` & `manage_requirements_files-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `manage_requirements_files-0.1.1/PKG-INFO` & `manage_requirements_files-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: manage_requirements_files
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility to manage project dependencies for development and production.
 Home-page: https://github.com/guilhermegouw/manage-requirements-files
 Author: Guilherme Gouw
 Author-email: guilherme.gouw@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Manage Requirements Files Version: 0.1.1
+# Manage Requirements Files
 
 `manage-requirements-files` is a Python CLI tool designed to help developers efficiently manage their project dependencies. It automates the updating of `requirements.txt` and `requirements-dev.txt` by appending new dependencies from the activated Python environment.
 
 ## Features
 
 - Detects newly installed packages not listed in `requirements.txt` or `requirements-dev.txt`.
 - Appends new dependencies to the appropriate requirements file without duplicating entries.
```

### Comparing `manage_requirements_files-0.1.1/README.md` & `manage_requirements_files-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Manage Requirements Files Version: 0.1.1
+# Manage Requirements Files
 
 `manage-requirements-files` is a Python CLI tool designed to help developers efficiently manage their project dependencies. It automates the updating of `requirements.txt` and `requirements-dev.txt` by appending new dependencies from the activated Python environment.
 
 ## Features
 
 - Detects newly installed packages not listed in `requirements.txt` or `requirements-dev.txt`.
 - Appends new dependencies to the appropriate requirements file without duplicating entries.
```

### Comparing `manage_requirements_files-0.1.1/manage_requirements_files/cli.py` & `manage_requirements_files-0.1.2/manage_requirements_files/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 import argparse
 import subprocess
 import sys
 
 
 def main():
     parser = argparse.ArgumentParser(
```

### Comparing `manage_requirements_files-0.1.1/manage_requirements_files.egg-info/PKG-INFO` & `manage_requirements_files-0.1.2/manage_requirements_files.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: manage-requirements-files
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility to manage project dependencies for development and production.
 Home-page: https://github.com/guilhermegouw/manage-requirements-files
 Author: Guilherme Gouw
 Author-email: guilherme.gouw@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Manage Requirements Files Version: 0.1.1
+# Manage Requirements Files
 
 `manage-requirements-files` is a Python CLI tool designed to help developers efficiently manage their project dependencies. It automates the updating of `requirements.txt` and `requirements-dev.txt` by appending new dependencies from the activated Python environment.
 
 ## Features
 
 - Detects newly installed packages not listed in `requirements.txt` or `requirements-dev.txt`.
 - Appends new dependencies to the appropriate requirements file without duplicating entries.
```

### Comparing `manage_requirements_files-0.1.1/setup.py` & `manage_requirements_files-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="manage_requirements_files",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "manage-dependencies=manage_requirements_files.cli:main",
         ],
     },
     author="Guilherme Gouw",
```

### Comparing `manage_requirements_files-0.1.1/tests/test_cli.py` & `manage_requirements_files-0.1.2/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,16 @@
         ],
     )
     def test_file_creation_on_not_found(self, mock_file):
         # Test handling of FileNotFoundError and file creation if not present
         expected_output = set()
         result = read_requirements("requirements.txt")
         self.assertEqual(result, expected_output)
-        self.assertEqual(
-            mock_file.call_args_list[0], call("requirements.txt", "r")
-        )
-        self.assertEqual(
-            mock_file.call_args_list[1], call("requirements.txt", "a")
-        )
+        self.assertEqual(mock_file.call_args_list[0], call("requirements.txt", "r"))
+        self.assertEqual(mock_file.call_args_list[1], call("requirements.txt", "a"))
 
 
 class TestWriteRequirements(unittest.TestCase):
     @patch("builtins.open", new_callable=mock_open)
     def test_write_to_existing_file(self, mock_file):
         # Test appending new lines to an existing file
         new_lines = ["django>=3.2", "requests>=2.25"]
@@ -118,17 +114,15 @@
     ):
         mock_pip_freeze.return_value = {"django>=3.2", "requests>=2.25"}
         mock_read_requirements.side_effect = [
             {"django>=3.2"},  # Existing dependencies in target_file
             {"flask>=1.1"},  # Existing dependencies in other_file
         ]
 
-        update_requirements(
-            "target_requirements.txt", "other_requirements.txt"
-        )
+        update_requirements("target_requirements.txt", "other_requirements.txt")
 
         mock_write_requirements.assert_called_once_with(
             "target_requirements.txt", {"requests>=2.25"}
         )
         mock_print.assert_called_once_with(
             "Updated target_requirements.txt with new dependencies: "
             + "{'requests>=2.25'}"
@@ -147,46 +141,47 @@
     ):
         mock_pip_freeze.return_value = {"django>=3.2"}
         mock_read_requirements.side_effect = [
             {"django>=3.2"},  # Existing dependencies in target_file
             {"flask>=1.1"},  # Existing dependencies in other_file
         ]
 
-        update_requirements(
-            "target_requirements.txt", "other_requirements.txt"
-        )
+        update_requirements("target_requirements.txt", "other_requirements.txt")
 
         mock_write_requirements.assert_not_called()
         mock_print.assert_called_once_with(
             "No new dependencies to add to target_requirements.txt."
         )
 
 
 class TestMainFunction(unittest.TestCase):
-    @patch('manage_requirements_files.cli.update_requirements')
-    @patch('argparse.ArgumentParser.parse_args')
+    @patch("manage_requirements_files.cli.update_requirements")
+    @patch("argparse.ArgumentParser.parse_args")
     def test_main_prod_mode(self, mock_parse_args, mock_update_requirements):
         # Setup mock to simulate command line arguments
-        mock_parse_args.return_value = MagicMock(mode='prod')
+        mock_parse_args.return_value = MagicMock(mode="prod")
 
         # Call main to test behavior
         main()
 
         # Check if update_requirements was called correctly
-        mock_update_requirements.assert_called_once_with("requirements.txt", "requirements-dev.txt")
+        mock_update_requirements.assert_called_once_with(
+            "requirements.txt", "requirements-dev.txt"
+        )
 
-    @patch('manage_requirements_files.cli.update_requirements')
-    @patch('argparse.ArgumentParser.parse_args')
+    @patch("manage_requirements_files.cli.update_requirements")
+    @patch("argparse.ArgumentParser.parse_args")
     def test_main_dev_mode(self, mock_parse_args, mock_update_requirements):
         # Setup mock to simulate command line arguments
-        mock_parse_args.return_value = MagicMock(mode='dev')
+        mock_parse_args.return_value = MagicMock(mode="dev")
 
         # Call main to test behavior
         main()
 
         # Check if update_requirements was called correctly
-        mock_update_requirements.assert_called_once_with("requirements-dev.txt", "requirements.txt")
-
+        mock_update_requirements.assert_called_once_with(
+            "requirements-dev.txt", "requirements.txt"
+        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

