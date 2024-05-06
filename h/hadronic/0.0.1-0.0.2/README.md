# Comparing `tmp/hadronic-0.0.1.tar.gz` & `tmp/hadronic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadronic-0.0.1.tar", last modified: Mon May  6 10:23:23 2024, max compression
+gzip compressed data, was "hadronic-0.0.2.tar", last modified: Mon May  6 11:22:12 2024, max compression
```

## Comparing `hadronic-0.0.1.tar` & `hadronic-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.852814 hadronic-0.0.1/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      178 2024-05-06 10:23:23.852814 hadronic-0.0.1/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-06 10:23:23.852814 hadronic-0.0.1/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)      490 2024-05-06 09:56:27.000000 hadronic-0.0.1/setup.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.848814 hadronic-0.0.1/src/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.849814 hadronic-0.0.1/src/hadronic/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      140 2024-05-06 09:39:44.000000 hadronic-0.0.1/src/hadronic/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.850814 hadronic-0.0.1/src/hadronic/core/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-06 07:52:53.000000 hadronic-0.0.1/src/hadronic/core/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2240 2024-05-06 10:04:35.000000 hadronic-0.0.1/src/hadronic/core/cli.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1426 2024-05-06 09:20:52.000000 hadronic-0.0.1/src/hadronic/core/config.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.850814 hadronic-0.0.1/src/hadronic/hadron/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-06 09:38:25.000000 hadronic-0.0.1/src/hadronic/hadron/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)    16157 2024-05-06 09:55:08.000000 hadronic-0.0.1/src/hadronic/hadron/hadron.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1297 2024-05-06 09:46:05.000000 hadronic-0.0.1/src/hadronic/hadron/tests.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.851814 hadronic-0.0.1/src/hadronic/hadron/workspace/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-06 09:55:17.000000 hadronic-0.0.1/src/hadronic/hadron/workspace/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)       25 2024-05-06 09:05:54.000000 hadronic-0.0.1/src/hadronic/hadron/workspace/config.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      154 2024-05-06 09:42:27.000000 hadronic-0.0.1/src/hadronic/hadron/workspace/fibonacci.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 10:23:23.851814 hadronic-0.0.1/src/hadronic.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      178 2024-05-06 10:23:23.000000 hadronic-0.0.1/src/hadronic.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      550 2024-05-06 10:23:23.000000 hadronic-0.0.1/src/hadronic.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-06 10:23:23.000000 hadronic-0.0.1/src/hadronic.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       50 2024-05-06 10:23:23.000000 hadronic-0.0.1/src/hadronic.egg-info/entry_points.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       12 2024-05-06 10:23:23.000000 hadronic-0.0.1/src/hadronic.egg-info/requires.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        9 2024-05-06 10:23:23.000000 hadronic-0.0.1/src/hadronic.egg-info/top_level.txt
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.292247 hadronic-0.0.2/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      178 2024-05-06 11:22:12.291247 hadronic-0.0.2/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-06 11:22:12.292247 hadronic-0.0.2/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      490 2024-05-06 11:21:52.000000 hadronic-0.0.2/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.288247 hadronic-0.0.2/src/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.288247 hadronic-0.0.2/src/hadronic/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      140 2024-05-06 09:39:44.000000 hadronic-0.0.2/src/hadronic/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.290247 hadronic-0.0.2/src/hadronic/core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-06 07:52:53.000000 hadronic-0.0.2/src/hadronic/core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2240 2024-05-06 10:04:35.000000 hadronic-0.0.2/src/hadronic/core/cli.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1426 2024-05-06 09:20:52.000000 hadronic-0.0.2/src/hadronic/core/config.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.290247 hadronic-0.0.2/src/hadronic/hadron/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-06 09:38:25.000000 hadronic-0.0.2/src/hadronic/hadron/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)    16739 2024-05-06 11:21:28.000000 hadronic-0.0.2/src/hadronic/hadron/hadron.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1297 2024-05-06 09:46:05.000000 hadronic-0.0.2/src/hadronic/hadron/tests.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.291247 hadronic-0.0.2/src/hadronic/hadron/workspace/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-06 09:55:17.000000 hadronic-0.0.2/src/hadronic/hadron/workspace/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       25 2024-05-06 09:05:54.000000 hadronic-0.0.2/src/hadronic/hadron/workspace/config.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      154 2024-05-06 09:42:27.000000 hadronic-0.0.2/src/hadronic/hadron/workspace/fibonacci.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:22:12.291247 hadronic-0.0.2/src/hadronic.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      178 2024-05-06 11:22:12.000000 hadronic-0.0.2/src/hadronic.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      550 2024-05-06 11:22:12.000000 hadronic-0.0.2/src/hadronic.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-06 11:22:12.000000 hadronic-0.0.2/src/hadronic.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       50 2024-05-06 11:22:12.000000 hadronic-0.0.2/src/hadronic.egg-info/entry_points.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       12 2024-05-06 11:22:12.000000 hadronic-0.0.2/src/hadronic.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        9 2024-05-06 11:22:12.000000 hadronic-0.0.2/src/hadronic.egg-info/top_level.txt
```

### Comparing `hadronic-0.0.1/src/hadronic/core/cli.py` & `hadronic-0.0.2/src/hadronic/core/cli.py`

 * *Files identical despite different names*

### Comparing `hadronic-0.0.1/src/hadronic/core/config.py` & `hadronic-0.0.2/src/hadronic/core/config.py`

 * *Files identical despite different names*

### Comparing `hadronic-0.0.1/src/hadronic/hadron/hadron.py` & `hadronic-0.0.2/src/hadronic/hadron/hadron.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 
     def __init__(self, workspace_dir: Optional[str] = None, verbose: Optional[bool] = True):
         """
         Initializes the Hadron 'Client' object. Leaving the workspace_dir empty
         will default to the quarks built in 'hadronic.workspace' directory.
 
         Example:
-        ```python
-        hadron = Hadron()
-        hadron = Hadron(workspace_dir="path/to/workspace")
-        ```
+            ```python
+            hadron = Hadron()
+            hadron = Hadron(workspace_dir="path/to/workspace")
+            ```
 
         Parameters:
-        workspace_dir (Optional[str]): The path to the workspace directory.
-        verbose (Optional[bool]): Whether to display verbose logging output. Defaults to True.
+            workspace_dir (Optional[str]): The path to the workspace directory.
+            verbose (Optional[bool]): Whether to display verbose logging output. Defaults to True.
         """
         self.config = config
         self.config.VERBOSE = verbose
         logger.info(f"Verbose outputs can be toggled with 'hadron.config.VERBOSE'") if self.config.VERBOSE else None
 
         try:
             self.workspace_path = self._validate_workspace(dir=workspace_dir)
@@ -133,20 +133,25 @@
             file.write(content)
         logger.info(f"{file_name} created or updated in workspace.") if self.config.VERBOSE else None
 
     def generate_code(self, prompt: str, model: str = "ollama/llama3", api_key : Optional[str] = None) -> str:
         """
         Generates code using the specified model based on the given prompt.
 
+        Example:
+            ```python
+            code = hadron.generate_code("Create a function that returns the nth Fibonacci number.")
+            ```
+
         Parameters:
-        prompt (str): The prompt to generate code from.
-        model (str): The model to use for code generation. Defaults to "ollama/llama3".
+            prompt (str): The prompt to generate code from.
+            model (str): The model to use for code generation. Defaults to "ollama/llama3".
 
         Returns:
-        str: The generated code.
+            str: The generated code.
         """
         try:
             result = completion(
                 api_key = api_key,
                 model= model,
                 messages= [{"role": "system", "content": self.config.LLM_SYSTEM_PROMPT},{"role": "user", "content": prompt}]
             )
@@ -156,20 +161,20 @@
         return result.choices[0].message.content
 
     def _write_code_to_file(self, filename: str, code: str, skip_logic: bool = False) -> Optional[str]:
         """
         Writes the generated code to a file in the workspace.
 
         Parameters:
-        filename (str): The name of the file to write the code to.
-        code (str): The generated code to write to the file.
-        skip_logic (bool): Whether to skip the code block extraction logic. Defaults to False.
+            filename (str): The name of the file to write the code to.
+            code (str): The generated code to write to the file.
+            skip_logic (bool): Whether to skip the code block extraction logic. Defaults to False.
 
         Returns:
-        Optional[str]: The path to the written file, or None if no valid code block is found.
+            Optional[str]: The path to the written file, or None if no valid code block is found.
         """
         file_path = os.path.join(self.workspace_path, filename)
         if not skip_logic:
             code_match = re.search(r'```(?:python)?\s+(.*?)\s+```', code, re.DOTALL)
             if code_match:
                 code = code_match.group(1)
             else:
@@ -184,18 +189,18 @@
         return file_path
 
     def _try_run_script(self, file_path: str) -> bool:
         """
         Attempts to run the Python script at the specified file path using subprocess.
 
         Parameters:
-        file_path (str): The path to the Python script to run.
+            file_path (str): The path to the Python script to run.
 
         Returns:
-        bool: True if the script executed successfully, False otherwise.
+            bool: True if the script executed successfully, False otherwise.
         """
         try:
             result = subprocess.run(['python', file_path], text=True, capture_output=True, check=True)
             logger.info("Script executed successfully: " + result.stdout) if self.config.VERBOSE else None
             return True
         except subprocess.CalledProcessError as e:
             logger.error("Script execution failed: " + e.stderr) if self.config.VERBOSE else None
@@ -217,22 +222,27 @@
                         logger.info("Retrying script execution after installing missing modules...") if self.config.VERBOSE else None
                         return self._try_run_script(file_path)
                     else:
                         logger.warning("User chose not to install missing modules. Skipping script execution.") if self.config.VERBOSE else None
             
             return False
 
-    def create_quark(self, filename: str, prompt: str, max_retries: int = 5):
+    def create_quark(self, prompt: str, filename: str, max_retries: int = 5):
         """
         Creates a quark (Python script) based on the given prompt.
 
+        Example:
+            ```python
+            hadron.create_quark("fibonacci.py", "Create a function that returns the nth Fibonacci number.")
+            ```
+
         Parameters:
-        filename (str): The name of the file to save the generated quark.
-        prompt (str): The prompt to generate the quark from.
-        max_retries (int): The maximum number of retries to generate a valid quark. Defaults to 5.
+            filename (str): The name of the file to save the generated quark.
+            prompt (str): The prompt to generate the quark from.
+            max_retries (int): The maximum number of retries to generate a valid quark. Defaults to 5.
         """
         attempts = 0
         while attempts < max_retries:
             logger.info("Generating code...") if self.config.VERBOSE else None
             generated_content = self.generate_code(prompt)
             logger.info("Writing code to file...") if self.config.VERBOSE else None
 
@@ -292,14 +302,19 @@
             file.write(f"from .{function_name} import {function_name}\n")
         logger.info(f"Added import for function {function_name} to __init__.py") if self.config.VERBOSE else None
 
     def clean(self):
         """
         Removes all non-essential files from the workspace directory, preserving only
         the __init__.py, config.py, and fibonacci.py files.
+
+        Example:
+            ```python
+            hadron.clean()
+            ```
         """
         essential_files = {'__init__.py', 'config.py', 'fibonacci.py'}
         files_in_workspace = os.listdir(self.workspace_path)
 
         for file in files_in_workspace:
             file_path = os.path.join(self.workspace_path, file)
             if file == '__init__.py':
@@ -314,17 +329,22 @@
                 except Exception as e:
                     logger.error(f"Failed to remove {file}: {e}") if self.config.VERBOSE else None
 
     def build(self, output_path: str, package_name: Optional[str] = None):
         """
         Builds a Python package from the quarks created in the workspace.
 
+        Example:
+            ```python
+            hadron.build("path/to/output")
+            ```
+
         Parameters:
-        output_path (str): The path where the package directory will be generated.
-        package_name (Optional[str]): The name of the package. If not provided, it will be derived from the output path.
+            output_path (str): The path where the package directory will be generated.
+            package_name (Optional[str]): The name of the package. If not provided, it will be derived from the output path.
         """
         if not package_name:
             package_name = os.path.basename(output_path)
 
         # Create the package directory structure
         package_dir = os.path.join(output_path, package_name)
         os.makedirs(package_dir, exist_ok=True)
```

### Comparing `hadronic-0.0.1/src/hadronic/hadron/tests.py` & `hadronic-0.0.2/src/hadronic/hadron/tests.py`

 * *Files identical despite different names*

### Comparing `hadronic-0.0.1/src/hadronic.egg-info/SOURCES.txt` & `hadronic-0.0.2/src/hadronic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

