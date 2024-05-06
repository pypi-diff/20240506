# Comparing `tmp/alex_sudoku-0.2.0.tar.gz` & `tmp/alex_sudoku-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_sudoku-0.2.0.tar", max compression
+gzip compressed data, was "alex_sudoku-0.2.1.tar", max compression
```

## Comparing `alex_sudoku-0.2.0.tar` & `alex_sudoku-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1090 2024-05-06 13:23:52.237100 alex_sudoku-0.2.0/LICENSE
--rw-r--r--   0        0        0     2791 2024-05-06 13:42:37.180334 alex_sudoku-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      928 2024-05-06 13:23:52.245131 alex_sudoku-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 13:23:52.210406 alex_sudoku-0.2.0/source/alex_sudoku/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 13:23:52.188410 alex_sudoku-0.2.0/source/alex_sudoku/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-06 13:33:10.729856 alex_sudoku-0.2.0/source/alex_sudoku/config/constants.py
--rw-r--r--   0        0        0     1443 2024-05-06 13:33:10.730857 alex_sudoku-0.2.0/source/alex_sudoku/config/paths.py
--rw-r--r--   0        0        0        0 2024-05-06 13:23:52.197427 alex_sudoku-0.2.0/source/alex_sudoku/interface/__init__.py
--rw-r--r--   0        0        0      471 2024-05-06 13:33:44.653205 alex_sudoku-0.2.0/source/alex_sudoku/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-05-06 13:23:52.203406 alex_sudoku-0.2.0/source/alex_sudoku/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-06 13:33:10.732855 alex_sudoku-0.2.0/source/alex_sudoku/logs/setup_logging.py
--rw-r--r--   0        0        0      538 2024-05-06 13:33:10.733858 alex_sudoku-0.2.0/source/alex_sudoku/main.py
--rw-r--r--   0        0        0        0 2024-05-06 13:23:52.216099 alex_sudoku-0.2.0/source/alex_sudoku/py.typed
--rw-r--r--   0        0        0        5 2024-05-06 13:23:52.218098 alex_sudoku-0.2.0/source/alex_sudoku/VERSION
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 alex_sudoku-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-06 13:23:52.237100 alex_sudoku-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2791 2024-05-06 14:07:27.967964 alex_sudoku-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      928 2024-05-06 13:23:52.245131 alex_sudoku-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 13:23:52.210406 alex_sudoku-0.2.1/source/alex_sudoku/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:23:52.188410 alex_sudoku-0.2.1/source/alex_sudoku/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-06 13:33:10.729856 alex_sudoku-0.2.1/source/alex_sudoku/config/constants.py
+-rw-r--r--   0        0        0     1443 2024-05-06 13:33:10.730857 alex_sudoku-0.2.1/source/alex_sudoku/config/paths.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:23:52.197427 alex_sudoku-0.2.1/source/alex_sudoku/interface/__init__.py
+-rw-r--r--   0        0        0      461 2024-05-06 14:06:43.219769 alex_sudoku-0.2.1/source/alex_sudoku/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:23:52.203406 alex_sudoku-0.2.1/source/alex_sudoku/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-06 13:33:10.732855 alex_sudoku-0.2.1/source/alex_sudoku/logs/setup_logging.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:05:31.969419 alex_sudoku-0.2.1/source/alex_sudoku/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:23:52.216099 alex_sudoku-0.2.1/source/alex_sudoku/py.typed
+-rw-r--r--   0        0        0        5 2024-05-06 13:23:52.218098 alex_sudoku-0.2.1/source/alex_sudoku/VERSION
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 alex_sudoku-0.2.1/PKG-INFO
```

### Comparing `alex_sudoku-0.2.0/LICENSE` & `alex_sudoku-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alex_sudoku-0.2.0/pyproject.toml` & `alex_sudoku-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "alex_sudoku"
-version = "0.2.0"
+version = "0.2.1"
 description = "A sudoku game"
 authors = ["A. Rushworth <rushworthalex7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alex_sudoku", from = "source"}]
 homepage = "https://github.com/HolyUsername/alex_sudoku"
 repository = "https://github.com/HolyUsername/alex_sudoku"
```

### Comparing `alex_sudoku-0.2.0/README.md` & `alex_sudoku-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alex_sudoku-0.2.0/source/alex_sudoku/config/constants.py` & `alex_sudoku-0.2.1/source/alex_sudoku/config/constants.py`

 * *Files identical despite different names*

### Comparing `alex_sudoku-0.2.0/source/alex_sudoku/config/paths.py` & `alex_sudoku-0.2.1/source/alex_sudoku/config/paths.py`

 * *Files identical despite different names*

### Comparing `alex_sudoku-0.2.0/source/alex_sudoku/logs/setup_logging.py` & `alex_sudoku-0.2.1/source/alex_sudoku/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `alex_sudoku-0.2.0/source/alex_sudoku/main.py` & `alex_sudoku-0.2.1/source/alex_sudoku/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """main.py: Called when the package is run as a script."""
 
+from .interface.command_line import command_line_interface
 from .logs.setup_logging import setup_logging
 
 main_logger = setup_logging()
 
 
 def main() -> None:
     """
@@ -11,14 +12,15 @@
 
     Notes
     -----
     This function is the entry point for the application.
     """
     try:
         main_logger.info("Application started.")
+        command_line_interface()
     except KeyboardInterrupt:
         print("\n")
         main_logger.info("Exiting application due to user interrupt...")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `alex_sudoku-0.2.0/PKG-INFO` & `alex_sudoku-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex_sudoku
-Version: 0.2.0
+Version: 0.2.1
 Summary: A sudoku game
 Home-page: https://github.com/HolyUsername/alex_sudoku
 License: MIT
 Author: A. Rushworth
 Author-email: rushworthalex7@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

