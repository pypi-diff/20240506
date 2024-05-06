# Comparing `tmp/imy-0.2.8.tar.gz` & `tmp/imy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.8.tar", max compression
+gzip compressed data, was "imy-0.3.0.tar", max compression
```

## Comparing `imy-0.2.8.tar` & `imy-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.8/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.2.8/imy/__init__.py
--rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.2.8/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-04-22 13:27:52.000000 imy-0.2.8/imy/async_utils.py
--rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.2.8/imy/config.py
--rw-r--r--   0        0        0       71 2024-04-22 13:27:52.000000 imy-0.2.8/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     6498 2024-04-28 15:53:31.243915 imy-0.2.8/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    17144 2024-04-28 17:12:51.285582 imy-0.2.8/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.2.8/imy/inject.py
--rw-r--r--   0        0        0    13613 2024-04-22 13:27:52.000000 imy-0.2.8/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.2.8/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-28 17:12:41.805567 imy-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.0/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.0/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.0/imy/assets.py
+-rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.0/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.0/imy/config.py
+-rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.0/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     6498 2024-04-28 15:53:31.243915 imy-0.3.0/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    17433 2024-05-06 15:16:53.871680 imy-0.3.0/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.0/imy/inject.py
+-rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.0/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.0/imy/package_metadata.py
+-rw-r--r--   0        0        0      753 2024-05-06 18:22:57.896321 imy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.0/PKG-INFO
```

### Comparing `imy-0.2.8/LICENSE` & `imy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.8/imy/assets.py` & `imy-0.3.0/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.8/imy/async_utils.py` & `imy-0.3.0/imy/async_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     *,
     limit: int | None = None,
 ) -> list[IN]:
     """
     Collects the values from an asynchronous iterable into a list.
 
     If `limit` is set, the result will contain at most the first `limit` values.
+
+    ## Parameters
+
+    `values`: The asynchronous iterable to collect values from.
+
+    `limit`: The maximum number of values to collect. If `None`, all values will
+        be collected.
     """
     result: list[IN] = []
 
     async for value in values:
         result.append(value)
 
         if len(result) == limit:
@@ -33,14 +40,22 @@
     values: Iterable[IN],
     *,
     concurrency: int = 10,
 ) -> AsyncIterable[OUT]:
     """
     Asynchronously maps `func` over `values`, with at most `concurrency` items
     being processed simultaneously.
+
+    ## Parameters
+
+    `func`: The function to apply to each value.
+
+    `values`: The values to apply the function to.
+
+    `concurrency`: The maximum number of items to process simultaneously.
     """
     # TODO: Support async iterables for the input
 
     # Processes a single value. Returns both the index and the result.
     async def process_single(index: int, value: IN) -> tuple[int, OUT]:
         result = await func(value)
         return index, result
```

### Comparing `imy-0.2.8/imy/config.py` & `imy-0.3.0/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.8/imy/docstrings/data_models.py` & `imy-0.3.0/imy/docstrings/data_models.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.8/imy/docstrings/parsers.py` & `imy-0.3.0/imy/docstrings/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,29 @@
     if docstring.startswith("#") and not docstring.startswith("##"):
         docstring = docstring.split("\n", 1)[1]
 
     # Split the docstring into sections
     sections: dict[str, list[str]] = {}
     details: list[str] = []
     current_section: list[str] = details
+    currently_inside_code_block: bool = False
 
     # Process the individual lines
     for line in docstring.splitlines():
-        if line.startswith("#"):
+        # Code block?
+        if line.startswith("```"):
+            currently_inside_code_block = not currently_inside_code_block
+            current_section.append(line)
+
+        # Section Header
+        elif line.startswith("#") and not currently_inside_code_block:
             section_name = line.strip()
             current_section = sections.setdefault(section_name, [])
+
+        # Nothing to see here
         else:
             current_section.append(line)
 
     # Post-process the sections
     def postprocess(section: list[str]) -> str:
         return "\n".join(section).strip()
 
@@ -153,38 +162,14 @@
     if not long_description:
         long_description = None
 
     # Done
     return short_description, long_description
 
 
-def parse_docstring_basic(
-    docstring: str,
-) -> tuple[str | None, str | None, dict[str, str]]:
-    """
-    Parses a docstring into
-
-    - summary
-    - details
-    - sections
-    """
-
-    # Dedent & strip
-    docstring = textwrap.dedent(docstring).strip()
-
-    # Split the docstring into sections
-    details, sections = split_docstring_into_sections(docstring)
-
-    # Split into summary and details
-    summary, details = parse_details(details)
-
-    # Done
-    return summary, details, sections
-
-
 def parse_docstring(
     docstring: str,
     *,
     key_sections: Iterable[str],
 ) -> data_models.Docstring:
     """
     Parses a docstring into
@@ -196,16 +181,23 @@
     Any sections listed in `key_sections` will be parsed as key-value pairs and
     returned as sections. Any remaining sections will be re-joined into the
     details.
 
     Any sections listed in `key_sections` that are not present in the docstring
     will be imputed as empty.
     """
-    # Parse the docstring
-    summary, details, sections = parse_docstring_basic(docstring)
+    # Remove consistent indentation
+    docstring = textwrap.dedent(docstring).strip()
+
+    # Split the docstring into (summary + details) and sections
+    summary_and_details, sections = split_docstring_into_sections(docstring)
+
+    # Split into summary and details
+    summary, details = parse_details(summary_and_details)
+    del summary_and_details
 
     if details is None:
         details = ""
 
     # Find and parse all key-value sections
     key_sections = set(key_sections)
     key_value_sections: dict[str, dict[str, str]] = {}
@@ -245,17 +237,19 @@
 
 def parse_function(func: Callable[..., Any]) -> data_models.FunctionDocs:
     """
     Given a function, parse its signature and docstring into a `FunctionDocs`
     object.
     """
 
-    def parse_annotation(annotation: object) -> introspection.types.TypeAnnotation:
+    def parse_annotation(
+        annotation: object,
+    ) -> introspection.types.TypeAnnotation | data_models.Unset:
         if annotation is inspect.Parameter.empty:
-            return None
+            return data_models.UNSET
 
         # Recursive types can cause issues. In particular, we have `Jsonable`,
         # which is a recursive type, and `JsonDoc`, which references `Jsonable`.
         # So if a module imports `JsonDoc` but doesn't import `Jsonable`, it's
         # impossible to evaluate the forward reference `"Jsonable"` in that
         # module.
         #
@@ -281,60 +275,63 @@
 
     # Parse the parameters
     signature = inspect.signature(func)
     parameters: dict[str, data_models.FunctionParameter] = {}
 
     for param_name, param in signature.parameters.items():
         if param.default == inspect.Parameter.empty:
-            param_default = None
+            param_default = data_models.UNSET
         else:
-            param_default = repr(param.default)
+            param_default = param.default
 
         parameters[param_name] = data_models.FunctionParameter(
             name=param_name,
             type=parse_annotation(param.annotation),
             default=param_default,
             kw_only=param.kind == inspect.Parameter.KEYWORD_ONLY,
             collect_positional=param.kind == inspect.Parameter.VAR_POSITIONAL,
             collect_keyword=param.kind == inspect.Parameter.VAR_KEYWORD,
             description=None,
         )
 
-    # All our components are dataclasses, and all default values are
-    # converted into default factories. This results in the default
-    # values of `__init__` parameters being displayed as `<factory>`.
-    if any(param.default == "<factory>" for param in parameters.values()):
+    # FIXME: This is specific to rio.
+    #
+    # All our components are dataclasses, and all default values are converted
+    # into default factories. This results in the default values of `__init__`
+    # parameters being displayed as `<factory>`.
+    if any(repr(param.default) == "<factory>" for param in parameters.values()):
         # This is super hacky, but since the actual default value isn't
-        # accessible from the `__init__` function, we somehow have to
-        # get a hold of the class, then the field, the default factory,
-        # and finally the default value.
+        # accessible from the `__init__` function, we somehow have to get a hold
+        # of the class, then the field, the default factory, and finally the
+        # default value.
         cls = func.__globals__[func.__qualname__.split(".")[0]]
-        fields = {field.name: field for field in dataclasses.fields(cls)}
+        if isinstance(cls, type):
+            fields = {field.name: field for field in dataclasses.fields(cls)}
 
-        for param in parameters.values():
-            if param.default != "<factory>":
-                continue
-
-            default_factory = fields[param.name].default_factory
-
-            if not isinstance(default_factory, functools.partial):
-                continue
-
-            if default_factory.func not in (copy.copy, copy.deepcopy):
-                continue
-
-            default_value = default_factory.args[0]
-            if default_value is None or type(default_value) in (
-                bool,
-                int,
-                float,
-                bytes,
-                str,
-            ):
-                param.default = repr(default_value)
+            for param in parameters.values():
+                if repr(param.default) != "<factory>":
+                    continue
+
+                default_factory = fields[param.name].default_factory
+
+                if not isinstance(default_factory, functools.partial):
+                    continue
+
+                if default_factory.func not in (copy.copy, copy.deepcopy):
+                    continue
+
+                default_value = default_factory.args[0]
+                if default_value is None or type(default_value) in (
+                    bool,
+                    int,
+                    float,
+                    bytes,
+                    str,
+                ):
+                    param.default = repr(default_value)
 
     # Parse the docstring
     docstring = inspect.getdoc(func)
 
     if docstring is None:
         parsed = data_models.Docstring(summary=None, details=None, key_sections={})
         raises = []
```

### Comparing `imy-0.2.8/imy/inject.py` & `imy-0.3.0/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.8/imy/logs.py` & `imy-0.3.0/imy/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,21 +94,40 @@
             return set(LOG_LEVEL_NAMES[ii:])
 
     raise ValueError(f"Unknown log level: {level}")
 
 
 @dataclass
 class LogEntry(uniserde.Serde):
+    """
+    Represents a single log entry in the database.
+    """
+
+    # Unique identifier for the log entry
     id: ObjectId
+
+    # When this log entry was created
     timestamp: datetime
+
+    # Whether this log entry was created in development or production
     environment: Environment
+
+    # Which machine created this log entry
     host: str
+
+    # The app that created this log entry
     app: str
+
+    # The severity of this log entry
     level: LogLevel
+
+    # A human-readable message. This is the main content of the log entry
     message: str
+
+    # Arbitrary additional data
     payload: dict[str, Any]
 
 
 class MongoDbLogger(logging.StreamHandler):
     """
     Logger, which stores its entries in a MongoDB database.
 
@@ -351,88 +370,105 @@
 
 
 @overload
 def setup_logging(
     *,
     info_log_path: Path | None = None,
     debug_log_path: Path | None = None,
+    stdout_log_level: LogLevel = "debug",
 ) -> MongoDbLogger:
     ...
 
 
 @overload
 def setup_logging(
     *,
     info_log_path: Path | None = None,
     debug_log_path: Path | None = None,
     database_collection: pymongo.collection.Collection | None = None,
     database_environment: Environment,
-    database_host: str | None = None,
+    database_connection_string: str | None = None,
     database_app: str,
+    stdout_log_level: LogLevel = "debug",
     database_log_level: LogLevel = "debug",
 ) -> MongoDbLogger:
     ...
 
 
 def setup_logging(
     *,
     info_log_path: Path | None = None,
     debug_log_path: Path | None = None,
     database_collection: pymongo.collection.Collection | None = None,
     database_environment: Environment | None = None,
-    database_host: str | None = None,
+    database_connection_string: str | None = None,
     database_app: str | None = None,
+    stdout_log_level: LogLevel = "debug",
     database_log_level: LogLevel = "debug",
 ) -> MongoDbLogger | None:
     """
     Creates a nice logging setup. Any previously registered handlers are
     removed, which means it is safe to call this function multiple times without
     creating duplicate log entries.
 
     - INFO logs to `info_log_path`, keeping logs indefinitely
-    - DEBUG logs to `stdout`
+    - Configurable logs to `stdout`, DEBUG by default
     - DEBUG logs to `debug_log_path`, keeping a limited number of days
-    - DEBUG logs into the database
+    - DEBUG logs into the database, if a collection is provided
 
-    Persistence loggers can lose some log entries if they are not flushed before
-    closing the application. If every single entry is important to you, make
-    sure to flush the returned persistence logger before ending the script.
-
-    :param info_log_path: Path to the info log file
-    :param debug_log_path: Path to the debug log file
-    :param db: The persistence to store logs in
-    :return: The created PersistenceLogger
-    """
+    Returns the database logger, if one was created.
 
-    root_logger = logging.getLogger("")
-    root_logger.setLevel(logging.DEBUG)
+    ## Parameters
 
-    formatter = logging.Formatter("%(asctime)s  %(levelname)-8s  %(message)s")
+    `info_log_path`: Path to the info log file
+
+    `debug_log_path`: Path to the debug log file
+
+    `database_collection`: The MongoDB collection to store logs in
+
+    `database_environment`: The environment to mark log entries as
+
+    `database_connection_string`: The MongoDB connection string to connect to
+        the database
+
+    `database_app`: The running app's name. This will be added to logged
+        entries in the database
+
+    `stdout_log_level`: The minimum log level to display on stdout
+
+    `database_log_level`: The minimum log level to store in the database
+    """
 
     # Make sure not to add multiple handlers if the function is called multiple
     # times.
     reset_logging()
 
+    # Configure the root logger and prepare some values
+    root_logger = logging.getLogger("")
+    root_logger.setLevel(logging.DEBUG)
+
+    formatter = logging.Formatter("%(asctime)s  %(levelname)-8s  %(message)s")
+
     # Info -> file
     if info_log_path is not None:
         info_log_path.parent.mkdir(parents=True, exist_ok=True)
 
         handler = logging.handlers.TimedRotatingFileHandler(
             info_log_path,
             encoding="utf-8",
             when="midnight",
             utc=True,
         )
         handler.setLevel(logging.INFO)
         handler.setFormatter(formatter)
         root_logger.addHandler(handler)
 
-    # Debug -> stdout
+    # Stdout (configurable)
     handler = logging.StreamHandler()
-    handler.setLevel(logging.DEBUG)
+    handler.setLevel(_log_level_to_python(stdout_log_level))
     handler.setFormatter(formatter)
     root_logger.addHandler(handler)
 
     # Debug -> file
     if debug_log_path is not None:
         debug_log_path.parent.mkdir(parents=True, exist_ok=True)
 
@@ -457,15 +493,15 @@
 
         assert (
             database_app is not None
         ), "Must provide an app name when logging to a database"
 
         pers_logger = MongoDbLogger(
             database_collection,
-            host=database_host,
+            host=database_connection_string,
             environment=database_environment,
             app=database_app,
         )
 
         pers_logger.setLevel(_log_level_to_python(database_log_level))
         root_logger.addHandler(pers_logger)
```

### Comparing `imy-0.2.8/imy/package_metadata.py` & `imy-0.3.0/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.8/pyproject.toml` & `imy-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.8"
+version = "0.3.0"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 json5 = { version = "^0.9.22", optional = true }
 motor = { version = "^3.3.2", optional = true }
-uniserde = { version = "^0.3.12", optional = true }
-introspection = { version = "^1.7.12", optional = true }
+uniserde = { version = "^0.3.13", optional = true }
+introspection = { version = "^1.8.0", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.1.1"
 pytest = "^8.1.1"
```

### Comparing `imy-0.2.8/PKG-INFO` & `imy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.8
+Version: 0.3.0
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: introspection (>=1.7.12,<2.0.0)
+Requires-Dist: introspection (>=1.8.0,<2.0.0)
 Requires-Dist: json5 (>=0.9.22,<0.10.0)
 Requires-Dist: motor (>=3.3.2,<4.0.0)
-Requires-Dist: uniserde (>=0.3.12,<0.4.0)
+Requires-Dist: uniserde (>=0.3.13,<0.4.0)
 Project-URL: Repository, https://gitlab.com/Vivern/i-miss-you
 Description-Content-Type: text/markdown
 
 # I Miss You
 
 Utilities I can't go without.
```

