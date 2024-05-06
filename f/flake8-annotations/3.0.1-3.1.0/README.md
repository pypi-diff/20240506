# Comparing `tmp/flake8_annotations-3.0.1.tar.gz` & `tmp/flake8_annotations-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_annotations-3.0.1.tar", max compression
+gzip compressed data, was "flake8_annotations-3.1.0.tar", max compression
```

## Comparing `flake8_annotations-3.0.1.tar` & `flake8_annotations-3.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7437 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/LICENSE
--rw-r--r--   0        0        0    10787 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/README.md
--rw-r--r--   0        0        0       22 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/__init__.py
--rw-r--r--   0        0        0    17378 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/ast_walker.py
--rw-r--r--   0        0        0    12896 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/checker.py
--rw-r--r--   0        0        0      893 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/enums.py
--rw-r--r--   0        0        0     6046 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/error_codes.py
--rw-r--r--   0        0        0     2398 2023-05-03 02:44:35.954697 flake8_annotations-3.0.1/pyproject.toml
--rw-r--r--   0        0        0    12304 1970-01-01 00:00:00.000000 flake8_annotations-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7572 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/LICENSE
+-rw-r--r--   0        0        0    11348 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/__init__.py
+-rw-r--r--   0        0        0    17308 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/ast_walker.py
+-rw-r--r--   0        0        0    13831 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/checker.py
+-rw-r--r--   0        0        0      893 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/enums.py
+-rw-r--r--   0        0        0     6046 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/error_codes.py
+-rw-r--r--   0        0        0     2362 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12716 1970-01-01 00:00:00.000000 flake8_annotations-3.1.0/PKG-INFO
```

### Comparing `flake8_annotations-3.0.1/CHANGELOG.md` & `flake8_annotations-3.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 Versions follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (`<major>`.`<minor>`.`<patch>`)
 
+## [v3.1.0]
+### Added
+* #164 Add `--respect-type-ignore` to support suppression of errors for functions annotated with `type: ignore`
+
 ## [v3.0.1]
 ### Changed
 * #155 Remove upper bound on Python constraint
 
 ## [v3.0.0]
 ### Added
 * Add `ANN402` for the presence of type comments
```

### Comparing `flake8_annotations-3.0.1/LICENSE` & `flake8_annotations-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.1/README.md` & `flake8_annotations-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8-annotations
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.0.1?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.1.0?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)
 [![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)
 
 `flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.
 
@@ -28,15 +28,15 @@
 ver_str = out.stdout.replace("\n", "")
 cog.out(
     f"```bash\n$ flake8 --version\n{ver_str}\n```"
 )
 ]]] -->
 ```bash
 $ flake8 --version
-6.0.0 (flake8-annotations: 3.0.1, mccabe: 0.7.0, pycodestyle: 2.10.0, pyflakes: 3.0.1) CPython 3.11.0 on Darwin
+7.0.0 (flake8-annotations: 3.1.0, mccabe: 0.7.0, pycodestyle: 2.11.1, pyflakes: 3.2.0) CPython 3.12.3 on Darwin
 ```
 <!-- [[[end]]] -->
 
 ## Table of Warnings
 With the exception of `ANN4xx`-level warnings, all warnings are enabled by default.
 
 ### Function Annotations
@@ -136,14 +136,22 @@
 Default: `"overload"`
 
 ### `--allow-star-arg-any`
 Suppress `ANN401` for dynamically typed `*args` and `**kwargs`.
 
 Default: `False`
 
+### `--respect-type-ignore`
+Suppress linting errors for functions annotated with a `# type: ignore` comment.
+
+**NOTE:** Type ignore tags are not considered, e.g. `# type: ignore[arg-type]` is treated the same as `# type: ignore`.
+
+Default: `False`
+
+
 ## Generic Functions
 Per the Python Glossary, a [generic function](https://docs.python.org/3/glossary.html#term-generic-function) is defined as:
 
 > A function composed of multiple functions implementing the same operation for different types. Which implementation should be used during a call is determined by the dispatch algorithm.
 
 In the standard library we have some examples of decorators for implementing these generic functions: [`functools.singledispatch`](https://docs.python.org/3/library/functools.html#functools.singledispatch) and [`functools.singledispatchmethod`](https://docs.python.org/3/library/functools.html#functools.singledispatchmethod). In the spirit of the purpose of these decorators, errors for missing annotations for functions decorated with at least one of these are ignored.
 
@@ -196,14 +204,16 @@
   * `from typing import any; foo: Any`
   * `import typing; foo: typing.Any`
   * `import typing as <alias>; foo: <alias>.Any`
 
 Nested dynamic types (e.g. `typing.Tuple[typing.Any]`) and redefinition (e.g. `from typing import Any as Foo`) will not be identified.
 
 ## Contributing
+### Python Version Support
+A best attempt is made to support Python versions until they reach EOL, after which support will be formally dropped by the next minor or major release of this package, whichever arrives first. The status of Python versions can be found [here](https://devguide.python.org/versions/).
 
 ### Development Environment
 This project uses [Poetry](https://python-poetry.org/) to manage dependencies. With your fork cloned to your local machine, you can install the project and its dependencies to create a development environment using:
 
 ```bash
 $ poetry install
 ```
```

### Comparing `flake8_annotations-3.0.1/flake8_annotations/ast_walker.py` & `flake8_annotations-3.1.0/flake8_annotations/ast_walker.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,17 +398,16 @@
         Check each Return node to see if it returns anything other than `None`.
 
         If the node being visited returns anything other than `None`, its parent context is added to
         the set of non-returning child nodes of the parent node.
         """
         if node.value is not None:
             # In the event of an explicit `None` return (`return None`), the node body will be an
-            # instance of either `ast.Constant` (3.8+) or `ast.NameConstant`, which we need to check
-            # to see if it's actually `None`
-            if isinstance(node.value, (ast.Constant, ast.NameConstant)):  # pragma: no branch
+            # instance of `ast.Constant`, which we need to check to see if it's actually `None`
+            if isinstance(node.value, ast.Constant):  # pragma: no branch
                 if node.value.value is None:
                     return
 
             self._non_none_return_nodes.add(self._context[-1])
 
     def switch_context(self, node: AST_FUNCTION_TYPES) -> None:
         """
```

### Comparing `flake8_annotations-3.0.1/flake8_annotations/checker.py` & `flake8_annotations-3.1.0/flake8_annotations/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,26 @@
     def __init__(self, tree: t.Optional[ast.Module], lines: t.List[str]):
         # Request `tree` in order to ensure flake8 will run the plugin, even though we don't use it
         # Request `lines` here and join to allow for correct handling of input from stdin
         self.lines = lines
 
         self.tree = ast.parse("".join(lines), type_comments=True)  # flake8 doesn't strip newlines
 
+        # Type ignores are provided by ast at the module level & we'll need them later when deciding
+        # whether or not to emit errors for a given function
+        self._type_ignore_lineno = {ti.lineno for ti in self.tree.type_ignores}
+
         # Set by flake8's config parser
         self.suppress_none_returning: bool
         self.suppress_dummy_args: bool
         self.allow_untyped_defs: bool
         self.allow_untyped_nested: bool
         self.mypy_init_return: bool
         self.allow_star_arg_any: bool
+        self.respect_type_ignore: bool
         self.dispatch_decorators: t.Set[str]
         self.overload_decorators: t.Set[str]
 
     def run(self) -> t.Generator[FORMATTED_ERROR, None, None]:
         """
         This method is called by flake8 to perform the actual check(s) on the source code.
 
@@ -103,14 +108,19 @@
             if last_overload_decorated_function_name == function.name:
                 continue
 
             # If it's not, and it is overload decorated, store it for the next iteration
             if function.has_decorator(self.overload_decorators):
                 last_overload_decorated_function_name = function.name
 
+            # Optionally respect a type: ignore comment
+            # These are considered at the function level & tags are not considered
+            if self.respect_type_ignore and (function.lineno in self._type_ignore_lineno):
+                continue
+
             # Yield explicit errors for arguments that are missing annotations
             for arg in function.get_missed_annotations():
                 # Check for type comments here since we're not considering them as typed args
                 if arg.has_type_comment:
                     yield error_codes.ANN402.from_argument(arg).to_flake8()
 
                 if arg.argname == "return":
@@ -218,23 +228,35 @@
             "--allow-star-arg-any",
             default=False,
             action="store_true",
             parse_from_config=True,
             help="Suppress ANN401 for dynamically typed *args and **kwargs. (Default: %(default)s)",
         )
 
+        parser.add_option(
+            "--respect-type-ignore",
+            default=False,
+            action="store_true",
+            parse_from_config=True,
+            help=(
+                "Supress errors for functions annotated with a 'type: ignore' comment. (Default: "
+                "%(default)s)"
+            ),
+        )
+
     @classmethod
     def parse_options(cls, options: Namespace) -> None:  # pragma: no cover
         """Parse the custom configuration options given to flake8."""
         cls.suppress_none_returning = options.suppress_none_returning
         cls.suppress_dummy_args = options.suppress_dummy_args
         cls.allow_untyped_defs = options.allow_untyped_defs
         cls.allow_untyped_nested = options.allow_untyped_nested
         cls.mypy_init_return = options.mypy_init_return
         cls.allow_star_arg_any = options.allow_star_arg_any
+        cls.respect_type_ignore = options.respect_type_ignore
 
         # Store decorator lists as sets for easier lookup
         cls.dispatch_decorators = set(options.dispatch_decorators)
         cls.overload_decorators = set(options.overload_decorators)
 
 
 def classify_error(function: Function, arg: Argument) -> error_codes.Error:
```

### Comparing `flake8_annotations-3.0.1/flake8_annotations/enums.py` & `flake8_annotations-3.1.0/flake8_annotations/enums.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.1/flake8_annotations/error_codes.py` & `flake8_annotations-3.1.0/flake8_annotations/error_codes.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.1/pyproject.toml` & `flake8_annotations-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-annotations"
-version = "3.0.1"
+version = "3.1.0"
 description = "Flake8 Type Annotation Checks"
 license = "MIT"
 readme = "README.md"
 authors = ["S Co1 <sco1.git@gmail.com>"]
 homepage = "https://github.com/sco1/flake8-annotations"
 repository = "https://github.com/sco1/flake8-annotations"
 classifiers = [
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Typing :: Typed",
 ]
 
 include = [
@@ -36,28 +37,25 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 attrs = ">=21.4"
 flake8 = ">=5.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
+black = "^24.3"
 bump2version = "^1.0"
 cogapp = "^3.3"
-flake8-bugbear = "^23.1"
-flake8-docstrings = "^1.7"
-flake8-fixme = "^1.1"
 isort = "^5.10"
 mypy = "^1.0"
-pep8-naming = "^0.13"
 pre-commit = "^3.0"
-pytest = "^7.2"
+pytest = "^8.0"
 pytest-check = "^2.0"
-pytest-cov = "^4.0"
+pytest-cov = "^5.0"
 pytest-randomly = "^3.12"
+ruff = "^0.4"
 tox = { version = "^4.4", python = "<4.0" }
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
 "ANN" = "flake8_annotations.checker:TypeHintChecker"
 
 [tool.black]
```

### Comparing `flake8_annotations-3.0.1/PKG-INFO` & `flake8_annotations-3.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-annotations
-Version: 3.0.1
+Version: 3.1.0
 Summary: Flake8 Type Annotation Checks
 Home-page: https://github.com/sco1/flake8-annotations
 License: MIT
 Author: S Co1
 Author-email: sco1.git@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,32 +14,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=21.4)
 Requires-Dist: flake8 (>=5.0)
 Project-URL: Issue Tracker, https://github.com/sco1/flake8-annotations/issues
 Project-URL: Repository, https://github.com/sco1/flake8-annotations
 Description-Content-Type: text/markdown
 
 # flake8-annotations
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.0.1?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.1.0?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)
 [![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)
 
 `flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.
 
@@ -64,15 +61,15 @@
 ver_str = out.stdout.replace("\n", "")
 cog.out(
     f"```bash\n$ flake8 --version\n{ver_str}\n```"
 )
 ]]] -->
 ```bash
 $ flake8 --version
-6.0.0 (flake8-annotations: 3.0.1, mccabe: 0.7.0, pycodestyle: 2.10.0, pyflakes: 3.0.1) CPython 3.11.0 on Darwin
+7.0.0 (flake8-annotations: 3.1.0, mccabe: 0.7.0, pycodestyle: 2.11.1, pyflakes: 3.2.0) CPython 3.12.3 on Darwin
 ```
 <!-- [[[end]]] -->
 
 ## Table of Warnings
 With the exception of `ANN4xx`-level warnings, all warnings are enabled by default.
 
 ### Function Annotations
@@ -172,14 +169,22 @@
 Default: `"overload"`
 
 ### `--allow-star-arg-any`
 Suppress `ANN401` for dynamically typed `*args` and `**kwargs`.
 
 Default: `False`
 
+### `--respect-type-ignore`
+Suppress linting errors for functions annotated with a `# type: ignore` comment.
+
+**NOTE:** Type ignore tags are not considered, e.g. `# type: ignore[arg-type]` is treated the same as `# type: ignore`.
+
+Default: `False`
+
+
 ## Generic Functions
 Per the Python Glossary, a [generic function](https://docs.python.org/3/glossary.html#term-generic-function) is defined as:
 
 > A function composed of multiple functions implementing the same operation for different types. Which implementation should be used during a call is determined by the dispatch algorithm.
 
 In the standard library we have some examples of decorators for implementing these generic functions: [`functools.singledispatch`](https://docs.python.org/3/library/functools.html#functools.singledispatch) and [`functools.singledispatchmethod`](https://docs.python.org/3/library/functools.html#functools.singledispatchmethod). In the spirit of the purpose of these decorators, errors for missing annotations for functions decorated with at least one of these are ignored.
 
@@ -232,14 +237,16 @@
   * `from typing import any; foo: Any`
   * `import typing; foo: typing.Any`
   * `import typing as <alias>; foo: <alias>.Any`
 
 Nested dynamic types (e.g. `typing.Tuple[typing.Any]`) and redefinition (e.g. `from typing import Any as Foo`) will not be identified.
 
 ## Contributing
+### Python Version Support
+A best attempt is made to support Python versions until they reach EOL, after which support will be formally dropped by the next minor or major release of this package, whichever arrives first. The status of Python versions can be found [here](https://devguide.python.org/versions/).
 
 ### Development Environment
 This project uses [Poetry](https://python-poetry.org/) to manage dependencies. With your fork cloned to your local machine, you can install the project and its dependencies to create a development environment using:
 
 ```bash
 $ poetry install
 ```
```

