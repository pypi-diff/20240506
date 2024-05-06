# Comparing `tmp/pytest_cmake-0.5.1.tar.gz` & `tmp/pytest_cmake-0.5.2.tar.gz`

## Comparing `pytest_cmake-0.5.1.tar` & `pytest_cmake-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/build_backend.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/build_config.py
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/cmake/FindPytest.cmake
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/cmake/PytestAddTests.cmake
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/setup.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/LICENSE
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/README.md
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 pytest_cmake-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/build_backend.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/build_config.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/cmake/FindPytest.cmake
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/cmake/PytestAddTests.cmake
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/setup.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/README.md
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/PKG-INFO
```

### Comparing `pytest_cmake-0.5.1/build_config.py` & `pytest_cmake-0.5.2/build_config.py`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.1/cmake/FindPytest.cmake` & `pytest_cmake-0.5.2/cmake/FindPytest.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -95,14 +95,16 @@
         list(JOIN libpath "${_env_sep}" libpath)
         list(JOIN pythonpath "${_env_sep}" pythonpath)
 
         if (NOT _WORKING_DIRECTORY)
             set(_WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})
         endif()
 
+        get_filename_component(_WORKING_DIRECTORY "${_WORKING_DIRECTORY}" REALPATH)
+
         # Override option by environment variable if available.
         if (DEFINED ENV{BUNDLE_PYTHON_TESTS})
             set(_BUNDLE_TESTS $ENV{BUNDLE_PYTHON_TESTS})
         endif()
 
         set(_tests_file "${CMAKE_CURRENT_BINARY_DIR}/${NAME}_tests.cmake")
```

### Comparing `pytest_cmake-0.5.1/cmake/PytestAddTests.cmake` & `pytest_cmake-0.5.2/cmake/PytestAddTests.cmake`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.1/setup.py` & `pytest_cmake-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         subprocess.call(["cmake", "-P", str(script_path), "-VV"])
         return install.run(self)
 
 
 setup(
     name="pytest-cmake",
-    version="0.5.1",
+    version="0.5.2",
     data_files=[
         (
             "share/Pytest/cmake",
             [
                 "build/PytestConfig.cmake",
                 "build/PytestConfigVersion.cmake",
                 "cmake/FindPytest.cmake",
```

### Comparing `pytest_cmake-0.5.1/.gitignore` & `pytest_cmake-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.1/LICENSE` & `pytest_cmake-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.1/README.md` & `pytest_cmake-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.1/pyproject.toml` & `pytest_cmake-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "cmake >= 3.20, < 3.30"
 ]
 build-backend = "build_backend"
 backend-path = ["."]
 
 [project]
 name = "pytest-cmake"
-version = "0.5.1"
+version = "0.5.2"
 description = "Provide CMake module for Pytest"
 readme = "README.md"
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4"
 license = {file = "LICENSE"}
 keywords = ["cmake", "pytest", "development"]
 authors = [
     {name = "Jeremy Retailleau", email = "jeremy.retailleau@gmail.com" }
```

### Comparing `pytest_cmake-0.5.1/PKG-INFO` & `pytest_cmake-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-cmake
-Version: 0.5.1
+Version: 0.5.2
 Summary: Provide CMake module for Pytest
 Author-email: Jeremy Retailleau <jeremy.retailleau@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jeremy Retailleau
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

