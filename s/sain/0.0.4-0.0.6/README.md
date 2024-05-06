# Comparing `tmp/sain-0.0.4.tar.gz` & `tmp/sain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sain-0.0.4.tar", max compression
+gzip compressed data, was "sain-0.0.6.tar", max compression
```

## Comparing `sain-0.0.4.tar` & `sain-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1540 2022-05-02 07:18:02.360097 sain-0.0.4/LICENSE
--rw-r--r--   0        0        0     2620 2023-08-13 19:51:49.311643 sain-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3153 2023-08-13 18:34:50.423059 sain-0.0.4/README.md
--rw-r--r--   0        0        0     3362 2023-08-13 18:32:28.457840 sain-0.0.4/sain/__init__.py
--rw-r--r--   0        0        0      700 2023-08-13 17:57:32.713547 sain-0.0.4/sain/__init__.pyi
--rw-r--r--   0        0        0    14569 2023-08-13 18:29:24.981777 sain-0.0.4/sain/cfg.py
--rw-r--r--   0        0        0     1666 2023-08-13 16:44:02.540806 sain-0.0.4/sain/cfg.pyi
--rw-r--r--   0        0        0     2637 2023-08-13 18:10:21.503640 sain-0.0.4/sain/default.py
--rw-r--r--   0        0        0     3941 2023-08-13 17:52:25.929860 sain-0.0.4/sain/futures.py
--rw-r--r--   0        0        0    16709 2023-08-13 18:27:58.544035 sain-0.0.4/sain/iter.py
--rw-r--r--   0        0        0     6691 2023-08-13 17:28:11.976465 sain-0.0.4/sain/macros.py
--rw-r--r--   0        0        0    14195 2023-08-13 18:26:55.047552 sain-0.0.4/sain/option.py
--rw-r--r--   0        0        0     3975 2023-08-13 17:46:49.495990 sain-0.0.4/sain/option.pyi
--rw-r--r--   0        0        0        2 2022-06-02 18:04:05.178246 sain-0.0.4/sain/py.typed
--rw-r--r--   0        0        0     3127 2023-08-13 18:27:09.151930 sain-0.0.4/sain/ref.py
--rw-r--r--   0        0        0     1640 2023-08-12 22:20:23.901846 sain-0.0.4/sain/result.py
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 sain-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1540 2022-05-02 07:18:02.360097 sain-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3204 2024-05-04 12:54:54.057875 sain-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3187 2024-05-04 13:27:49.628859 sain-0.0.6/README.md
+-rw-r--r--   0        0        0     4157 2024-05-04 12:54:43.329409 sain-0.0.6/sain/__init__.py
+-rw-r--r--   0        0        0     6477 2024-02-24 11:03:06.662718 sain-0.0.6/sain/boxed.py
+-rw-r--r--   0        0        0     4194 2024-05-04 12:50:57.114177 sain-0.0.6/sain/cell.py
+-rw-r--r--   0        0        0    13671 2024-03-26 18:32:29.160596 sain-0.0.6/sain/cfg.py
+-rw-r--r--   0        0        0      780 2024-02-16 17:23:45.344858 sain-0.0.6/sain/cfg.pyi
+-rw-r--r--   0        0        0     2639 2024-03-29 11:17:46.224624 sain-0.0.6/sain/default.py
+-rw-r--r--   0        0        0     4299 2024-03-29 11:17:46.224624 sain-0.0.6/sain/error.py
+-rw-r--r--   0        0        0     4273 2024-03-26 18:32:29.166584 sain-0.0.6/sain/futures.py
+-rw-r--r--   0        0        0    20606 2024-05-04 12:14:37.652604 sain-0.0.6/sain/iter.py
+-rw-r--r--   0        0        0    10815 2024-03-26 18:32:29.172583 sain-0.0.6/sain/macros.py
+-rw-r--r--   0        0        0    16084 2024-05-04 12:44:55.271854 sain-0.0.6/sain/option.py
+-rw-r--r--   0        0        0     3420 2024-03-26 18:32:29.178590 sain-0.0.6/sain/option.pyi
+-rw-r--r--   0        0        0        2 2023-12-24 19:54:40.817042 sain-0.0.6/sain/py.typed
+-rw-r--r--   0        0        0    16761 2024-02-16 18:12:49.666644 sain-0.0.6/sain/result.py
+-rw-r--r--   0        0        0     1833 2024-05-03 17:50:15.711666 sain-0.0.6/sain/sync/__init__.py
+-rw-r--r--   0        0        0     8398 2024-03-26 18:32:29.186587 sain-0.0.6/sain/sync/lazy.py
+-rw-r--r--   0        0        0     8484 2024-03-26 18:32:29.189593 sain-0.0.6/sain/sync/once.py
+-rw-r--r--   0        0        0    15039 2024-05-03 19:08:02.532865 sain-0.0.6/sain/vec.py
+-rw-r--r--   0        0        0     4612 1970-01-01 00:00:00.000000 sain-0.0.6/PKG-INFO
```

### Comparing `sain-0.0.4/LICENSE` & `sain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sain-0.0.4/pyproject.toml` & `sain-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,109 @@
 [tool.poetry]
 name = "sain"
-version = "0.0.4"
+version = "0.0.6"
 description = "Standard Rust core types implementations for Python."
 authors = ["nxtlo <dhmony-99@hotmail.com>"]
 license = "BSD-3-Clause license"
-keywords = ["Rust", "config"]
+keywords = ["Rust", "config", "typing", "utilities"]
 readme = "README.md"
 repository = "https://github.com/nxtlo/sain"
 packages = [{ include = "sain" }, { include = "sain/**/*.py" }]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
-[tool.poetry.dependencies]
-python = "^3.10"
+[tool.ruff]
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".git",
+    ".mypy_cache",
+    ".nox",
+    ".ruff_cache",
+    ".venv",
+    "__pypackages__",
+    "dist",
+    "node_modules",
+    "venv",
+    "aiobungie/_*.py",
+    "aiobungie/_*.pyi",
+    "aiobungie/crates/_*.py",
+    "aiobungie/crates/_*.pyi",
+]
+
+# Same as Black.
+line-length = 88
+indent-width = 4
+
+target-version = "py312"
+
+[tool.ruff.lint]
+# Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
+select = ["E4", "E7", "E9", "F"]
+ignore = []
+
+# Allow fix for all enabled rules (when `--fix`) is provided.
+fixable = ["ALL"]
+unfixable = []
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+[tool.ruff.format]
+# Like Black, use double quotes for strings.
+quote-style = "double"
+
+# Like Black, indent with spaces, rather than tabs.
+indent-style = "space"
 
-[tool.pytest.ini_options]
-xfail_strict = true
-norecursedirs = "docs *.egg-info .git .nox .pytest_cache .venv"
-
-[tool.black]
-line-length = 120
-target-version = ["py310"]
-include = ".*pyi?$"
+# Like Black, respect magic trailing commas.
+skip-magic-trailing-comma = false
+
+# Like Black, automatically detect the appropriate line ending.
+line-ending = "auto"
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 
-[tool.mypy]
-python_version = "3.10"
-pretty = true
-show_column_numbers = true
-show_error_codes = true
-show_error_context = true
-check_untyped_defs = true
-
-# Ignored
-ignore_missing_imports = true
-ignore_missing_imports_per_module = true
-
-# Warns
-warn_no_return = true
-warn_return_any = true
-
-# Disallowed
-disallow_any_generics = true
-disallow_subclassing_any = true
-disallow_untyped_calls = true
-disallow_untyped_defs = true
-disallow_incomplete_defs = true
-
-# Allowed
-allow_redefinition = true
-
 [tool.pyright]
-include = ["sain", "tests", "examples"]
-venvPath = "."
-venv = ".venv"
-pythonVersion = "3.10"
+include = ["sain", "examples"]
+pythonVersion = "3.12"
 typeCheckingMode = "strict"
-reportUnboundVariable = "none"
+
+reportUnnecessaryTypeIgnoreComment = "warning"
+reportMissingTypeStubs = "none"
+# This will always cause warnings above license.
+reportIncompatibleVariableOverride = "none"
+reportMissingImports = "error"
+reportImportCycles = "none"
+reportOverlappingOverload = "none"
+reportUnboundVariable = "error"
 reportUnknownParameterType = "error"
 reportUnknownLambdaType = "warning"
 reportUnknownMemberType = "warning"
 reportUnknownArgumentType = "warning"
 reportUnknownVariableType = "warning"
 reportMissingModuleSource = "error"
 reportMissingParameterType = "error"
 reportMissingTypeArgument = "error"
-reportMissingTypeStubs = "error"
-reportGeneralTypeIssues = "information"
-reportPrivateUsage = "warning"
+reportGeneralTypeIssues = "warning"
+reportPrivateUsage = "error"
 reportIncompatibleMethodOverride = "none"
-# This will always cause warnings above license.
-reportImportCycles = "warning"
-reportUnusedImport = "warning"
-
+reportUnusedVariable = "error"
+reportUnusedImport = "error"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sain-0.0.4/sain/__init__.py` & `sain-0.0.6/sain/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,81 +24,116 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-"""Standard Rust core types implementations for Python.
+"""sain is a set of minimal abstraction that brings Rust's ecosystem to Python.
+It offers a few of the core Rust features like `Vec<T>` and `Result<T, E>` and more.
+See the equivalent type section below.
 
-Equavilant types
+Equivalent types
 ----------------
-- `Option<T>` -> `sain.Option[T]` | `sain.Some[T]`
-- `Result<T, E>` -> `sain.Result[T, E]`. Not implemented yet.
-- `Default<T>` -> `sain.Default[T]`
-- `AsRef<T>` -> `sain.Ref[T]`.
-- `AsMut<T>` -> `sain.RefMut[T]`.
-- `Iter<Item>` -> `sain.Iter[Item]`
+- `Option<T>` -> `Option[T]` | `Some[T]`
+- `Result<T, E>` -> `Result[T, E]`
+- `Error` -> `Error`
+- `Vec<T>` -> `Vec[T]`
+- `Default<T>` -> `Default[T]`
+- `Iter<Item>` -> `Iter[Item]`
+- `Box<T>` -> `Box[T]`, not a heap box.
+- `cell::Cell<T>` -> `Cell[T]`, slightly different.
+- `cell::RefCell<T>` -> `RefCell[T]`, slightly different.
+- `sync::LazyLock<T>` -> `Lazy[T]`
+- `sync::OnceLock<T>` -> `Once[T]`
 
-Equavilant macros
+Equivalent macros
 -----------------
 As decorators.
 
-- `cfg!()` -> `sain.cfg`.
+- `cfg!()` -> `sain.cfg`
 - `todo!()` -> `sain.todo`. This is not a decorator.
-- `deprecated!()` -> `sain.deprecated`.
-- `unimplemented!()` -> `sain.unimplemented`.
-- `#[cfg_attr]` -> `sain.cfg_attr`.
+- `deprecated!()` -> `sain.deprecated`
+- `unimplemented!()` -> `sain.unimplemented`
+- `#[cfg_attr]` -> `sain.cfg_attr`
+- `#[doc()]` -> `sain.doc()`
 """
+
 from __future__ import annotations
 
 __all__ = (
     # cfg.py
     "cfg",
     "cfg_attr",
     # default.py
-    "Default",
     "default",
-    # ref.py
-    "Ref",
-    "RefMut",
-    "ref",
+    "Default",
     # option.py
-    "Some",
     "option",
+    "Some",
+    "Option",
+    "NOTHING",
     # iter.py
-    "into_iter",
     "Iter",
     "iter",
     # macros.py
+    "macros",
     "todo",
     "deprecated",
     "unimplemented",
+    "doc",
     # futures.py
     "futures",
+    # result.py
+    "result",
+    "Ok",
+    "Err",
+    "Result",
+    # vec.py
+    "vec",
+    "Vec",
+    # error.py
+    "error",
+    "Error",
+    # boxed.py
+    "boxed",
+    "Box",
+    # sync
+    "sync",
 )
 
-# Module top level. Required for pdoc.
+from . import boxed
 from . import default
+from . import error
+from . import futures
 from . import iter
+from . import macros
 from . import option
-from . import ref
-from . import futures
+from . import result
+from . import sync
+from .boxed import Box
 from .cfg import cfg
 from .cfg import cfg_attr
 from .default import Default
+from .error import Error
 from .iter import Iter
-from .iter import into_iter
 from .macros import deprecated
+from .macros import doc
 from .macros import todo
 from .macros import unimplemented
+from .option import NOTHING
+from .option import Option
 from .option import Some
-from .ref import Ref
-from .ref import RefMut
+from .result import Err
+from .result import Ok
+from .result import Result
+from .vec import Vec
+from .vec import vec
 
-__version__: str = "0.0.4"
+__version__: str = "0.0.6"
 __url__: str = "https://github.com/nxtlo/sain"
 __author__: str = "nxtlo"
 __about__: str = (
-    "Sain is a dependency-free library that implements some of the Rust core types. Which provides more abstraction."
+    "Sain is a dependency-free library that implements some of the Rust core"
+    "types which abstracts over common patterns in Rust for Python."
 )
 __license__: str = "BSD 3-Clause License"
```

### Comparing `sain-0.0.4/sain/cfg.py` & `sain-0.0.6/sain/cfg.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,44 +23,19 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-"""Runtime attr confuguration.
+"""Runtime attr configuration.
 
-Examples
---------
-```py
-from __futures__ import annotations
-import typing
-
-from sain import cfg_attr, cfg, Some
-
-# Required for typehints.
-if typing.TYPE_CHECKING:
-    from sain import Option
-
-# If a non windows machine runs this function, it will raise an error.
-@cfg_attr(target_os = "windows")
-def windows_only() -> Option[int]:
-    return sain.Some(1)
-
-@cfg_attr(requires_modules="uvloop", target_os = "unix")
-def run_uvloop() -> None:
-    import uvloop
-    uvloop.install()
-
-@cfg_attr(python_version = (3, 11, 0))
-class Tensor:
-    if cfg(target_os = "unix"):
-        def calculate(self, left: float, right: float) -> float:
-            ...
-```
+### Warning
+* The `cfg_attr` currently is buggy, Specifically when passing multiple modules into the
+`required_modules` parameter.
 
 Notes
 -----
 Target OS must be one of the following:
 * `linux`
 * `win32` | `windows`
 * `darwin`
@@ -81,93 +56,103 @@
 
 from __future__ import annotations
 
 __all__ = ("cfg_attr", "cfg")
 
 import collections.abc as collections
 import functools
+import importlib.util as importlib
 import inspect
 import platform
 import sys
 import typing
 
-from sain import macros
+from . import macros
+
+F = typing.TypeVar("F", bound=collections.Callable[..., object])
 
-SigT = collections.Callable[..., object]
-Signature = typing.TypeVar("Signature", bound=SigT)
-"""A type var hint for the decorated object signature."""
-
-TARGET_OS = typing.Literal["linux", "win32", "darwin", "unix", "windows"]
-TARGET_ARCH = typing.Literal["x86", "x64", "arm", "arm64"]
-PY_IMPL = typing.Literal["CPython", "PyPy", "IronPython", "Jython"]
+System = typing.Literal["linux", "win32", "darwin", "unix", "windows"]
+Arch = typing.Literal["x86", "x64", "arm", "arm64"]
+Python = typing.Literal["CPython", "PyPy", "IronPython", "Jython"]
+
+if typing.TYPE_CHECKING:
+    from typing_extensions import Self
 
 
 def _machine() -> str:
     return platform.machine()
 
 
 def _is_arm() -> bool:
-    return _machine().startswith("arm")
+    return "ARM" in _machine()
 
 
 def _is_arm_64() -> bool:
     return _is_arm() and _is_x64()
 
 
 def _is_x64() -> bool:
     return _machine().endswith("64")
 
 
+def _py_version() -> str:
+    return platform.python_version()
+
+
 def cfg_attr(
     *,
-    requires_modules: str | collections.Sequence[str] | None = None,
-    target_os: TARGET_OS | None = None,
+    requires: str | None = None,
+    target_os: System | None = None,
     python_version: tuple[int, int, int] | None = None,
-    target_arch: TARGET_ARCH | None = None,
-    impl: PY_IMPL | None = None,
-) -> collections.Callable[[Signature], Signature]:
+    target_arch: Arch | None = None,
+    impl: Python | None = None,
+) -> collections.Callable[[F], F]:
     """Conditional runtime object configuration based on passed arguments.
 
     If the decorated object gets called and one of the attributes returns `False`,
     `RuntimeError` will be raised and the object will not run.
 
+    .. warning::
+        The `requires` parameter is bugged and scheduled for deprecation
+        and will be removed in a future release.
+        Instead, directly import modules at the top of the file or function.
+
     Example
     -------
     ```py
     import sain
 
-    @sain.cfg_attr(target_os = "windows")
+    @sain.cfg_attr(target_os="windows")
     def windows_only():
         # Do stuff with Windows's API.
         ...
 
     # Mut be PyPy Python implementation or `RuntimeError` will be raised
     # when creating the instance.
     @sain.cfg_attr(impl="PyPy")
     class Zoo:
-        @sain.cfg_attr(target_os = "linux")
+        @sain.cfg_attr(target_os="linux")
         def bark(self) -> None:
             windows_only()  # RuntimeError("Windows OS only!)
 
     # An instance will not be created if raised.
     zoo = Zoo()
-    # RuntimError("class Zoo requires PyPy implementation")
+    # RuntimeError("class Zoo requires PyPy implementation")
     zoo.bark()
     # Whats zoo??
     ```
 
     Parameters
     ----------
-    requires_modules : `str | Sequence[str] | None`
-        A string or sequence of strings of the required modules for the object.
+    requires : `str | None`
+        A required module to run the object.
     target_os : `str | None`
         The targeted operating system thats required for the object.
     python_version : `tuple[int, int, int] | None`
-        The targeted Python version thats required for the object.
-        Format must be `(3, 9, 5)`.
+        The targeted Python version thats required for the object. Format must be `(3, 9, 5)`.
     target_arch : `str | None`
         The CPU targeted architecture thats required for the object.
     impl : `str | None`
         The Python implementation thats required for the object.
 
     Raises
     ------
@@ -175,192 +160,185 @@
         This fails if any of the attributes returns `False`. `required_modules` is not included.
     `ModuleNotFoundError`
         If the module check fails. i.e., if `required_modules` was provided and it returns `False`.
     `ValueError`
         If the passed Python implementation is unknown.
     """
 
-    def decorator(callback: Signature) -> Signature:
+    def decorator(callback: F) -> F:
         @functools.wraps(callback)
-        def wrapper(*args: typing.Any, **kwargs: typing.Any) -> Signature:
+        def wrapper(*args: typing.Any, **kwargs: typing.Any) -> F:
             checker = _AttrCheck(
                 callback,
-                requires_modules=requires_modules,
+                requires=requires,
                 target_os=target_os,
                 python_version=python_version,
                 target_arch=target_arch,
                 impl=impl,
             )
             return checker(*args, **kwargs)
 
-        return typing.cast(Signature, wrapper)
+        return typing.cast(F, wrapper)
 
     return decorator
 
 
 def cfg(
-    target_os: TARGET_OS | None = None,
-    requires_modules: str | collections.Sequence[str] | None = None,
+    target_os: System | None = None,
+    requires: str | None = None,
     python_version: tuple[int, int, int] | None = None,
-    target_arch: TARGET_ARCH | None = None,
-    impl: PY_IMPL | None = None,
+    target_arch: Arch | None = None,
+    impl: Python | None = None,
 ) -> bool:
     """A function that will run the code only if all predicate attributes returns `True`.
 
+    .. warning::
+        The `requires` parameter is bugged and scheduled for deprecation and will be removed in a future release.
+        Instead, directly import modules at the top of the file or function.
+
     The difference between this function and `cfg_attr` is that this function will not raise an exception.
     Instead it will return `False` if any of the attributes fails.
 
     Example
     -------
     ```py
     import sain
 
-    if sain.cfg(target_os = "windows"):
+    if sain.cfg(target_os="windows"):
         print("Windows")
-    elif sain.cfg(target_os = "linux"):
+    elif sain.cfg(target_os="linux"):
         print("Linux")
     else:
         print("Something else")
     ```
 
     Parameters
     ----------
-    requires_modules : `str | Sequence[str] | None`
-        A string or sequence of the required module names for the object to be ran.
+    requires : `str | None`
+        A required module to run the object.
     target_os : `str | None`
         The targeted operating system thats required for the object to be ran.
     python_version : `tuple[int, int, int] | None`
-        The targeted Python version thats required for the object to be ran.
-
-        Format must be `(3, 9, 5)`.
+        The targeted Python version thats required for the object to be ran. Format must be `(3, 9, 5)``
     target_arch : `str | None`
         The CPU targeted architecture thats required for the object to be ran.
     impl : `str | None`
         The Python implementation thats required for the object to be ran.
 
     Returns
     -------
     `bool`
         The condition that was checked.
     """
     checker = _AttrCheck(
         lambda: None,
         no_raise=True,
-        requires_modules=requires_modules,
+        requires=requires,
         target_os=target_os,
         python_version=python_version,
         target_arch=target_arch,
         impl=impl,
     )
     return checker.internal_check()
 
 
-class _AttrCheck(typing.Generic[Signature]):
+@typing.final
+class _AttrCheck(typing.Generic[F]):
     __slots__ = (
-        "_modules",
+        "_requires",
         "_target_os",
         "_callback",
         "_py_version",
         "_no_raise",
         "_target_arch",
         "_py_impl",
         "_debugger",
     )
 
     def __init__(
         self,
-        callback: Signature,
-        requires_modules: str | collections.Iterable[str] | None = None,
-        target_os: TARGET_OS | None = None,
+        callback: F,
+        requires: str | None = None,
+        target_os: System | None = None,
         python_version: tuple[int, int, int] | None = None,
-        target_arch: TARGET_ARCH | None = None,
-        impl: PY_IMPL | None = None,
+        target_arch: Arch | None = None,
+        impl: Python | None = None,
         *,
         no_raise: bool = False,
     ) -> None:
         self._callback = callback
-        self._modules = requires_modules
+        self._requires = requires
         self._target_os = target_os
         self._py_version = python_version
         self._target_arch = target_arch
         self._no_raise = no_raise
         self._py_impl = impl
         self._debugger = _Debug(callback, no_raise)
 
-    def __call__(self, *args: typing.Any, **kwds: typing.Any) -> Signature:
+    def __call__(self, *args: typing.Any, **kwds: typing.Any) -> F:
         self._check_once()
-        return typing.cast(Signature, self._callback(*args, **kwds))
+        return typing.cast(F, self._callback(*args, **kwds))
 
     def internal_check(self) -> bool:
         return self._check_once()
 
-    # FIXME: fix this mess.
+    # FIXME: Can we impl this differently?
     def _check_once(self) -> bool:
         results: list[bool] = []
         if self._target_os is not None:
             results.append(self._check_platform())
 
         if self._py_version is not None:
             results.append(self._check_py_version())
 
-        if self._modules is not None:
+        if self._requires is not None:
             results.append(self._check_modules())
 
         if self._target_arch is not None:
             results.append(self._check_target_arch())
 
         if self._py_impl is not None:
             results.append(self._check_py_impl())
 
         # No checks are passed to cfg(), We return False.
         if not results:
             return False
 
         return all(results)
 
-    @macros.unstable(reason="The `requires_modules` attribute is buggy.")
+    @macros.unstable(reason="The function is buggy.")
+    @macros.deprecated(
+        since="0.0.4", use_instead="Self-Check the module locally", removed_in="0.0.6"
+    )
     def _check_modules(self) -> bool:
         """__intrinsics__"""
-        required_modules: set[str] = set()
+        assert self._requires
+
+        if importlib.find_spec(self._requires) is None:
+            if self._no_raise:
+                self._debugger.flag(True)
 
-        assert self._modules
-        if isinstance(modules := self._modules, str):
-            modules = (modules,)
-
-        for module in modules:
-            try:
-                # __import__  won't add expose of the modules to namespace.
-                mod = str(__import__(module)).split("'")[1]
-                # If the module gets added here, it means it raised the error below.
-                required_modules.add(mod)
-            except ModuleNotFoundError:
-                # We need to check the no raise flag to True
-                # to return a bool instead. This is usually for cfg() `if` checks.
-                if self._no_raise:
-                    self._debugger.flag(True)
-
-                needed = filter(lambda mod: mod not in required_modules, modules)
-                return (
-                    self._debugger.exception(ModuleNotFoundError)
-                    .message(f"requires modules {', '.join(needed)} to be installed")
-                    .finish()
-                )
-        return True
+        return (
+            self._debugger.exception(ModuleNotFoundError)
+            .message(f"Requires modules ({self._requires}) to be installed")
+            .finish()
+        )
 
     def _check_target_arch(self) -> bool:
-        if self._target_arch == "arm":
-            return _is_arm()
-        elif self._target_arch == "arm64":
-            return _is_arm_64()
-        elif self._target_arch == "x86":
-            return not _is_x64()
-        elif self._target_arch == "x64":
-            return _is_x64()
-        else:
-            raise ValueError(f"Unknown target arch: `{self._target_arch}`")
+        match self._target_arch:
+            case "arm":
+                return _is_arm()
+            case "arm64":
+                return _is_arm_64()
+            case "x86":
+                return not _is_x64()
+            case "x64":
+                return _is_x64()
+            case _:
+                raise ValueError(f"Unknown target arch: {self._target_arch}")
 
     def _check_platform(self) -> bool:
         is_unix = sys.platform in {"linux", "darwin"}
 
         # If the target os is unix, then we assume that it's either linux or darwin.
         if self._target_os == "unix" and is_unix:
             return True
@@ -372,77 +350,85 @@
         if sys.platform == self._target_os:
             return True
 
         # fmt: off
         return (
             self._debugger
             .exception(RuntimeError)
-            .message(f"requires `{self._target_os}` OS").finish()
+            .message(f"requires {self._target_os} OS").finish()
         )
         # fmt: on
 
     def _check_py_version(self) -> bool:
         if self._py_version and self._py_version <= sys.version_info:
             return True
 
         return (
             self._debugger.exception(RuntimeError)
-            .message(f"requires Python >=`{self._py_version}`. But found {platform.python_version()}")
+            .message(f"requires Python >={self._py_version}")
+            .and_then(f"But found {_py_version()}")
             .finish()
         )
 
     def _check_py_impl(self) -> bool:
         if platform.python_implementation() == self._py_impl:
             return True
 
         # fmt: off
         return (
             self._debugger.exception(RuntimeError)
-            .message(f"requires Python implementation `{self._py_impl}`")
+            .message(f"requires Python implementation {self._py_impl}")
             .finish()
         )
         # fmt: on
 
 
-class _Debug(typing.Generic[Signature]):
+class _Debug(typing.Generic[F]):
     def __init__(
         self,
-        callback: Signature,
+        callback: F,
         no_raise: bool,
         message: str | None = None,
         exception: type[BaseException] | None = None,
     ) -> None:
         self._callback = callback
         self._exception: type[BaseException] | None = exception
         self._no_raise = no_raise
         self._message = message
 
-    def exception(self, exc: type[BaseException]) -> _Debug[Signature]:
+    def exception(self, exc: type[BaseException]) -> Self:
         self._exception = exc
         return self
 
     @functools.cached_property
     def _obj_type(self) -> str:
         if inspect.isfunction(self._callback):
             return "function"
         elif inspect.isclass(self._callback):
             return "class"
 
         return "object"
 
-    def flag(self, cond: bool) -> _Debug[Signature]:
+    def flag(self, cond: bool) -> None:
         self._no_raise = cond
-        return self
 
-    def message(self, message: str) -> _Debug[Signature]:
+    def message(self, message: str) -> _Debug[F]:
         """Set a message to be included in the exception that is getting raised."""
-        fn_name = "" if self._callback.__name__ == "<lambda>" else self._callback.__name__
-        self._message = f"{self._obj_type} {fn_name} {message}."
+        fn_name = (
+            "" if self._callback.__name__ == "<lambda>" else self._callback.__name__
+        )
+        self._message = f"{self._obj_type} {fn_name} {message}"
+        return self
+
+    def and_then(self, message: str) -> Self:
+        """Append an extra str to the end of this debugger's message."""
+        assert self._message is not None
+        self._message += ", " + message
         return self
 
     def finish(self) -> bool:
         """Finish the result, Either returning a bool or raising an exception."""
         if self._no_raise:
             return False
-        else:
-            assert self._exception is not None
-            raise self._exception(self._message) from None
+
+        assert self._exception is not None
+        raise self._exception(self._message) from None
```

### Comparing `sain-0.0.4/sain/default.py` & `sain-0.0.6/sain/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     @staticmethod
     def default() -> str:
         return generator.random_str()
 
 DEFAULT_GENERATOR = Generator.default()
 ```
 """
+
 from __future__ import annotations
 
 __all__ = ("Default",)
 
 import typing
 
 _T_co = typing.TypeVar("_T_co", covariant=True)
```

### Comparing `sain-0.0.4/sain/futures.py` & `sain-0.0.6/sain/futures.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,83 +23,98 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-"""Abstractions for asynchronous programming."""
+"""Abstractions for threading / asynchronous programming."""
 
 from __future__ import annotations
 
 __all__ = ("spawn", "loop")
 
 import asyncio
+import enum
 import typing
 
+from . import result as _result
+
 if typing.TYPE_CHECKING:
     import collections.abc as collections
 
     T_co = typing.TypeVar("T_co", covariant=True)
     T = typing.TypeVar("T", bound=collections.Callable[..., typing.Any])
 
 
+class SpawnErr(enum.Enum):
+    EMPTY = 0
+    """No awaitables were passed."""
+    CANCELED = 1
+    """The future gatherer were canceled."""
+    TIMEOUT = 2
+    """The future gatherer timed-out."""
+
+
 async def spawn(
     *aws: collections.Awaitable[T_co],
     timeout: float | None = None,
-    with_exception: bool = True,
-) -> collections.Sequence[T_co]:
+) -> _result.Result[collections.Sequence[T_co], SpawnErr]:
     """Spawn all given awaitables concurrently.
 
     Example
     -------
     ```py
-    from sain import futures
-
     async def get(url: str) -> dict[str, Any]:
         return await http.get(url).json()
 
     async def main() -> None:
-        tasks = await futures.spawn(*(get("url.com") for _ in range(10)))
-        print(tasks)
+        tasks = await spawn(*(get("url.com") for _ in range(10)))
+        match tasks:
+            case Ok(tasks):
+                assert len(tasks) <= 10
+            case Err(why) if why.TIMEOUT:
+                print("couldn't make it in time :<")
+            case _:
+                ...
     ```
 
     Parameters
     ----------
     *aws : `collections.Awaitable[T]`
         The awaitables to gather.
     timeout : `float | None`
         An optional timeout.
-    with_exceptions : `bool`
-        If `True` then exceptions will be returned. Default to `True`.
 
     Returns
     -------
-    `Sequence[T]`
-        A sequence of the results of the awaited coros.
+    `sain.Result[T, SpawnErr]`:
+        The result of the gathered awaitables.
     """
 
     if not aws:
-        raise RuntimeError("No awaitables passed.", aws)
+        return _result.Err(SpawnErr.EMPTY)
 
     tasks: list[asyncio.Task[T_co]] = []
 
-    for future in aws:
-        tasks.append(asyncio.ensure_future(future))  # type: ignore
+    tasks.extend(asyncio.ensure_future(coro) for coro in aws)
+    gatherer = asyncio.gather(*tasks)
     try:
-        gatherer = asyncio.gather(*tasks, return_exceptions=with_exception)
-        return await asyncio.wait_for(gatherer, timeout=timeout)
+        return _result.Ok(await asyncio.wait_for(gatherer, timeout=timeout))
 
     except asyncio.CancelledError:
-        raise asyncio.CancelledError("Gathered Futures were cancelled.") from None
+        return _result.Err(SpawnErr.CANCELED)
+    except asyncio.TimeoutError:
+        return _result.Err(SpawnErr.TIMEOUT)
 
     finally:
         for task in tasks:
             if not task.done() and not task.cancelled():
                 task.cancel()
+        gatherer.cancel()
 
 
 # source: hikari-py/aio.py
 def loop() -> asyncio.AbstractEventLoop:
     """Get the current usable event loop or create a new one.
 
     Returns
```

### Comparing `sain-0.0.4/sain/iter.py` & `sain-0.0.6/sain/iter.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,36 +23,53 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-"""Module contains a Standard functional iterator implementation."""
+"""Composable external iteration. See `Iter` for more details."""
 
 from __future__ import annotations
 
-__all__ = ("Iter", "into_iter", "Item")
+__all__ = ("Iter", "into_iter", "empty", "once")
 
+import collections.abc as collections
+import copy
 import itertools
 import typing
-import collections.abc as collections
+
+from . import default as _default
+from . import futures
+from . import option as _option
+from . import result as _result
+from .vec import Vec
 
 Item = typing.TypeVar("Item")
 """A type hint for the item type of the iterator."""
 
 if typing.TYPE_CHECKING:
-    import _typeshed as typeshed
+    import _typeshed
+    import typing_extensions as ty_ext
+
+    from .option import Option
 
     OtherItem = typing.TypeVar("OtherItem")
     _B = typing.TypeVar("_B", bound=collections.Callable[..., typing.Any])
 
 
-class Iter(collections.Iterator[Item]):
-    """Lazy, In-Memory iterator for sequence types with some functional methods.
+class Iter(
+    collections.Iterator[Item],
+    collections.Iterable[Item],
+    _default.Default["Iter[ty_ext.Never]"],
+):
+    """a lazy, in-memory functional iterator.
+
+    This is similar to Rust `Iterator` trait which iterables can build
+    from this via `.iter()` method.
 
     Example
     -------
     ```py
     iterator = Iter([1, 2, 3])
     # Limit the results to 2.
     for item in iterator.take(2):
@@ -80,112 +97,193 @@
     """
 
     __slots__ = ("_items",)
 
     def __init__(self, items: collections.Iterable[Item]) -> None:
         self._items = iter(items)
 
+    ###################
+    # const functions #
+    ###################
+
+    @staticmethod
+    @typing.final
+    def default() -> Iter[ty_ext.Never]:
+        """Return the default iterator for this type. It returns an empty iterator.
+
+        Example
+        -------
+        ```py
+        it = Iter.default()
+        assert t.next().is_none()
+        ```
+        """
+        return empty()
+
     @typing.overload
-    def collect(self) -> collections.Sequence[Item]:
-        ...
+    @typing.final
+    def collect(self) -> collections.Sequence[Item]: ...
 
     @typing.overload
-    def collect(self, *, casting: _B) -> collections.Sequence[_B]:
-        ...
+    @typing.final
+    def collect(self, *, cast: _B) -> collections.Sequence[_B]: ...
 
-    def collect(self, *, casting: _B | None = None) -> collections.Sequence[Item] | collections.Sequence[_B]:
-        """Collects all items in the iterator into a list.
+    @typing.final
+    def collect(
+        self, *, cast: _B | None = None
+    ) -> collections.Sequence[Item] | collections.Sequence[_B]:
+        """Collects all items in the iterator into an immutable sequence.
 
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> iterator.collect()
-        [1, 2, 3]
-        >>> iterator.collect(str)
-        ['1', '2', '3']
+        ```py
+        iterator = Iter(range(3))
+        iterator.collect()
+        # (0, 1, 2, 3)
+        iterator.collect(cast=str) # Map each element and collect it.
+        # ('0', '1', '2', '3')
+        ```
 
         Parameters
         ----------
-        casting: `T | None`
+        cast: `T | None`
             An optional type to cast the items into.
-            If not provided the items will be returned as a normal list.
+            If not provided the items will be returned as it's original type.
+        """
+        if cast is not None:
+            return tuple(map(cast, self._items))
 
-        Raises
-        ------
-        `StopIteration`
-            If no elements are left in the iterator.
+        return tuple(self._items)
+
+    @typing.final
+    def to_vec(self) -> Vec[Item]:
+        """Convert this iterator into `Vec[T]`.
+
+        Example
+        -------
+        ```py
+        it = sain.iter.once(0)
+        vc = it.to_vec()
+
+        assert to_vec == [0]
+        ```
         """
-        if casting is not None:
-            return typing.cast("collections.Sequence[_B]", list(map(casting, self._items)))
+        return Vec(self._items)
 
-        return list(self._items)
+    @typing.final
+    def copied(self) -> Iter[Item]:
+        """Creates an iterator which copies all of its elements by value.
 
-    def next(self) -> Item:
-        """Returns the next item in the iterator.
+        .. note::
+            If you only need a copy of the item reference, Use `by_ref` instead.
 
         Example
         -------
-        >>> iterator = Iter[str](["1", "2", "3"])
-        item = iterator.next()
-        assert item == "1"
-        item = iterator.next()
-        assert item == "2"
+        ```py
+        it = Iter([None, None, None])
+        copied = it.copied()
+        assert it.collect() == copied.collect()
+        ```
+        """
+        return Iter(copy.deepcopy(self._items))
 
-        Raises
-        ------
-        `StopIteration`
-            If no elements are left in the iterator.
+    @typing.final
+    def by_ref(self) -> Iter[Item]:
+        """Creates an iterator which shallow copies its elements by reference.
+
+        Example
+        -------
+        ```py
+        it = Iter([None, None, None])
+        for ref in it.by_ref():
+            ...
+
+        # Original not consumed.
+        assert it.count() == 3
+        ```
+        """
+        return Iter(copy.copy(self._items))
+
+    @typing.final
+    def sink(self) -> None:
+        """Consume all elements from this iterator, flushing it into the sink.
+
+        Example
+        -------
+        ```py
+        it = Iter((1, 2, 3))
+        it.sink()
+        assert it.next().is_none()
+        ```
+        """
+        for _ in self._items:
+            pass
+
+    ##################
+    # default impl's #
+    ##################
+
+    def next(self) -> Option[Item]:
+        """Returns the next item in the iterator, `Some(None)` if all items yielded.
+
+        Example
+        -------
+        ```py
+        iterator = Iter[str](["1", "2"])
+        assert iterator.next() == Some("1")
+        assert iterator.next() == Some("2")
+        assert iterator.next().is_none()
+        ```
         """
         try:
-            return self.__next__()
+            item = self.__next__()
         except StopIteration:
-            self._ok()
-
-    def map(self, predicate: collections.Callable[[Item], OtherItem]) -> Iter[OtherItem]:
+            # SAFETY: no items left.
+            return _option.nothing_unchecked()
+        return _option.Some(item)
+
+    def map(
+        self, predicate: collections.Callable[[Item], OtherItem]
+    ) -> Iter[OtherItem]:
         """Maps each item in the iterator to its predicated value.
 
         Example
         -------
-        >>> iterator = Iter[str](["1", "2", "3"]).map(lambda value: int(value))
-        <Iter([1, 2, 3])>
-        >>> for item in iterator:
-                assert isinstance(item, int)
+        ```py
+        iterator = Iter(["1", "2", "3"]).map(lambda value: int(value))
+
+        # <Iter([1, 2, 3])>
+        for item in iterator:
+            assert isinstance(item, int)
+        ```
 
         Parameters
         ----------
         predicate: `collections.Callable[[Item], Item]`
             The function to map each item in the iterator to its predicated value.
-
-        Raises
-        ------
-        `StopIteration`
-            If no elements are left in the iterator.
         """
-        return Iter(map(predicate, self._items))
+        return Iter(predicate(item) for item in self._items)
 
     def take(self, n: int) -> Iter[Item]:
         """Take the first number of items until the number of items are yielded or
         the end of the iterator is reached.
 
         Example
         -------
-        >>> iterator = Iter([RAID, STRIKE, GAMBIT])
-        >>> for mode in iterator.take(2):
-                assert mode in [RAID, STRIKE]
-        <Iter([RAID, STRIKE])>
+        ```py
+        iterator = Iter(['c', 'x', 'y'])
+        for mode in iterator.take(2):
+            assert mode in ['c', 'x']
+        # <Iter(['c', 'x'])>
+        ```
 
         Parameters
         ----------
         n: `int`
             The number of items to take.
-
-        Raises
-        ------
-        `StopIteration`
-            If no elements are left in the iterator.
         """
         return Iter(itertools.islice(self._items, n))
 
     def take_while(self, predicate: collections.Callable[[Item], bool]) -> Iter[Item]:
         """Yields items from the iterator while predicate returns `True`.
 
         Example
@@ -246,63 +344,44 @@
         for place in places.filter(lambda place: place.startswith('L')):
             print(place)
 
         # London
         # Los Angeles
         ```
         """
-        return Iter(filter(predicate, self._items))
+        return Iter(item for item in self._items if predicate(item))
 
     def skip(self, n: int) -> Iter[Item]:
         """Skips the first number of items in the iterator.
 
         Example
         -------
         ```py
         iterator = Iter([MembershipType.STEAM, MembershipType.XBOX, MembershipType.STADIA])
         for platform in iterator.skip(1):
-                print(platform)
+            print(platform)
         # Skip the first item in the iterator.
         # <Iter([MembershipType.XBOX, MembershipType.STADIA])>
+        ```
         """
         return Iter(itertools.islice(self._items, n, None))
 
-    def discard(self, predicate: collections.Callable[[Item], bool]) -> Iter[Item]:
-        """Discards all elements in the iterator for which the predicate function returns true.
-
-        Example
-        -------
-        >>> iterator = Iter([MembershipType.STEAM, MembershipType.XBOX, MembershipType.STADIA])
-        >>> for _ in iterator.discard(lambda platform: platform is not MembershipType.STEAM):
-                # Drops all memberships that are not steam.
-                print(iterator)
-        <Iter([MembershipType.XBOX, MembershipType.STADIA])>
-
-        Parameters
-        ----------
-        predicate: `collections.Callable[[Item], bool]`
-            The function to test each item in the iterator.
-
-        Raises
-        ------
-        `StopIteration`
-            If no elements are left in the iterator.
-        """
-        return Iter(filter(lambda x: not predicate(x), self._items))
-
-    def zip(self, other: Iter[OtherItem]) -> Iter[typing.Tuple[Item, OtherItem]]:
+    def zip(
+        self, other: collections.Iterable[OtherItem]
+    ) -> Iter[tuple[Item, OtherItem]]:
         """Zips the iterator with another iterable.
 
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> other = Iter([4, 5, 6])
-        >>> for item, other_item in iterator.zip(other):
-                assert item == other_item
+        ```py
+        iterator = Iter([1, 2, 3])
+        for item, other_item in iterator.zip([4, 5, 6]):
+            assert item == other_item
         <Iter([(1, 4), (2, 5), (3, 6)])>
+        ```
 
         Parameters
         ----------
         other: `Iter[OtherItem]`
             The iterable to zip with.
 
         Returns
@@ -318,144 +397,180 @@
         return Iter(zip(self._items, other))
 
     def all(self, predicate: collections.Callable[[Item], bool]) -> bool:
         """Return `True` if all items in the iterator match the predicate.
 
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> while iterator.all(lambda item: isinstance(item, int)):
-                print("Still all integers")
-                continue
+        ```py
+        iterator = Iter([1, 2, 3])
+        while iterator.all(lambda item: isinstance(item, int)):
+            print("Still all integers")
+            continue
             # Still all integers
+        ```
 
         Parameters
         ----------
         predicate: `collections.Callable[[Item], bool]`
             The function to test each item in the iterator.
 
         Raises
         ------
         `StopIteration`
             If no elements are left in the iterator.
         """
-        return all(predicate(item) for item in self)
+        return all(predicate(item) for item in self._items)
 
     def any(self, predicate: collections.Callable[[Item], bool]) -> bool:
         """`True` if any items in the iterator match the predicate.
 
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> if iterator.any(lambda item: isinstance(item, int)):
-                print("At least one item is an int.")
+        ```py
+        iterator = Iter([1, 2, 3])
+        if iterator.any(lambda item: isinstance(item, int)):
+            print("At least one item is an int.")
         # At least one item is an int.
+        ```
 
         Parameters
         ----------
         predicate: `collections.Callable[[Item], bool]`
             The function to test each item in the iterator.
 
         Raises
         ------
         `StopIteration`
             If no elements are left in the iterator.
         """
-        return any(predicate(item) for item in self)
+        return any(predicate(item) for item in self._items)
 
     def sort(
         self,
         *,
-        key: collections.Callable[[Item], typeshed.SupportsRichComparison],
+        key: collections.Callable[[Item], _typeshed.SupportsRichComparison],
         reverse: bool = False,
     ) -> Iter[Item]:
         """Sorts the iterator.
 
         Example
         -------
-        >>> iterator = Iter([3, 1, 6, 7])
-        >>> for item in iterator.sort(key=lambda item: item < 3):
-                print(item)
+        ```py
+        iterator = Iter([3, 1, 6, 7])
+        for item in iterator.sort(key=lambda item: item < 3):
+            print(item)
         # 1
         # 3
         # 6
         # 7
+        ```
 
-        Parameters
         ----------
         key: `collections.Callable[[Item], Any]`
             The function to sort by.
         reverse: `bool`
             Whether to reverse the sort.
 
         Raises
         ------
         `StopIteration`
             If no elements are left in the iterator.
         """
         return Iter(sorted(self._items, key=key, reverse=reverse))
 
-    def first(self) -> Item:
+    def first(self) -> Option[Item]:
         """Returns the first item in the iterator.
 
         Example
         -------
-        >>> iterator = Iter([3, 1, 6, 7])
-        >>> iterator.first()
-        3
+        ```py
+        iterator = Iter([3, 1, 6, 7])
+        iterator.first().is_some_and(lambda x: x == 3)
+        ```
 
         Raises
         ------
         `StopIteration`
             If no elements are left in the iterator.
         """
         return self.take(1).next()
 
+    def last(self) -> Option[Item]:
+        """Returns the last item in the iterator.
+
+        Example
+        -------
+        ```py
+        iterator = Iter([3, 1, 6, 7])
+        iterator.last().is_some_and(lambda x: x == 7)
+        ```
+
+        Raises
+        ------
+        `StopIteration`
+        If no elements are left in the iterator.
+        """
+        return self.reversed().first()
+
     def reversed(self) -> Iter[Item]:
         """Returns a new iterator that yields the items in the iterator in reverse order.
 
         Example
         -------
-        >>> iterator = Iter([3, 1, 6, 7])
-        >>> for item in iterator.reversed():
-                print(item)
+        ```py
+        iterator = Iter([3, 1, 6, 7])
+        for item in iterator.reversed():
+            print(item)
         # 7
         # 6
         # 1
         # 3
+        ```
 
         Raises
         ------
         `StopIteration`
             If no elements are left in the iterator.
         """
         return Iter(reversed(self.collect()))
 
     def count(self) -> int:
+        """Return the count of elements in memory this iterator has.
+
+        Example
+        -------
+        ```py
+        it = Iter(range(3))
+        assert it.count() == 3
+        ```
+        """
         count = 0
         for _ in self:
             count += 1
 
         return count
 
     def union(self, other: Iter[Item]) -> Iter[Item]:
         """Returns a new iterator that yields all items from both iterators.
 
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> other = Iter([4, 5, 6])
-        >>> for item in iterator.union(other):
-                print(item)
+        ```py
+        iterator = Iter([1, 2, 3])
+        other = Iter([4, 5, 6])
+        for item in iterator.union(other):
+            print(item)
         # 1
         # 2
         # 3
         # 4
         # 5
         # 6
+        ```
 
         Parameters
         ----------
         other: `Iter[Item]`
             The iterable to union with.
 
         Raises
@@ -466,64 +581,109 @@
         return Iter(itertools.chain(self._items, other))
 
     def for_each(self, func: collections.Callable[[Item], typing.Any]) -> None:
         """Calls `func` on each item in the iterator.
 
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> iterator.for_each(lambda item: print(item))
+        ```py
+        iterator = Iter([1, 2, 3])
+        iterator.for_each(lambda item: print(item))
         # 1
         # 2
         # 3
+        ```
 
         Parameters
         ----------
         func: `collections.Callable[[Item], typing.Any]`
             The function to call on each item in the iterator.
         """
-        for item in self:
+        for item in self._items:
             func(item)
 
-    def enumerate(self, *, start: int = 0) -> Iter[typing.Tuple[int, Item]]:
+    async def async_for_each(
+        self,
+        func: collections.Callable[
+            [Item], collections.Coroutine[None, typing.Any, OtherItem]
+        ],
+    ) -> _result.Result[collections.Sequence[OtherItem], futures.SpawnErr]:
+        """Calls the async function on each item in the iterator concurrently.
+
+        Example
+        -------
+        ```py
+        async def create_user(username: str) -> None:
+            async with aiohttp.request("POST", f'.../{username}') as r:
+                return await r.json()
+
+        async def main():
+            users = sain.into_iter(["danny", "legalia"])
+            results = await users.async_for_each(lambda username: create_user(username))
+            for k, v in results.unwrap().items():
+                ...
+        ```
+
+        Parameters
+        ----------
+        func: `Callable[[Item], Coroutine[None, Any, Any]]`
+            The async function to call on each item in the iterator.
+        """
+        return await futures.spawn(*(func(item) for item in self._items))
+
+    def enumerate(self, *, start: int = 0) -> Iter[tuple[int, Item]]:
         """Returns a new iterator that yields tuples of the index and item.
+
         Example
         -------
-        >>> iterator = Iter([1, 2, 3])
-        >>> for index, item in iterator.enumerate():
-                print(index, item)
+        ```py
+        iterator = Iter([1, 2, 3])
+        for index, item in iterator.enumerate():
+            print(index, item)
         # 0, 1
         # 1, 2
         # 2, 3
+        ```
 
         Raises
         ------
         `StopIteration`
             If no elements are left in the iterator.
         """
         return Iter(enumerate(self._items, start=start))
 
     def _ok(self) -> typing.NoReturn:
         raise StopIteration("No more items in the iterator.") from None
 
-    def __getitem__(self, index: int) -> Item:
+    def __getitem__(self, index: int) -> Option[Item]:
         try:
             return self.skip(index).first()
         except IndexError:
             self._ok()
 
     # This is a never.
-    def __setitem__(self) -> typing.NoReturn:
-        raise TypeError(f"{type(self).__name__} doesn't support item assignment.") from None
+    def __setitem__(self, _: None, __: None) -> typing.NoReturn:
+        raise NotImplementedError(
+            f"{type(self).__name__} doesn't support item assignment."
+        ) from None
 
     def __contains__(self, item: Item) -> bool:
         return item in self._items
 
+    def __reversed__(self) -> Iter[Item]:
+        return self.reversed()
+
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__}({", ".join([str(item) for item in self._items])})>'
+        return f"<Iter: {type(self._items).__name__}>"
+
+    def __copy__(self) -> Iter[Item]:
+        return self.by_ref()
+
+    def __deepcopy__(self) -> Iter[Item]:
+        return self.copied()
 
     def __len__(self) -> int:
         return self.count()
 
     def __iter__(self) -> Iter[Item]:
         return self
 
@@ -532,33 +692,55 @@
             item = next(self._items)
         except StopIteration:
             self._ok()
 
         return item
 
 
+def empty() -> Iter[ty_ext.Never]:
+    """Create an iterator that yields nothing.
+
+    Example
+    -------
+    ```py
+    nope = sain.iter.empty()
+    assert nope.next().is_none()
+    ```
+    """
+    return Iter(_ for _ in ())
+
+
+def once(item: Item) -> Iter[Item]:
+    """Returns an iterator that yields exactly a single item.
+
+    Example
+    -------
+    ```py
+    iterator = sain.iter.once(1)
+    assert iterator.next() == Some(1)
+    assert iterator.next() == Some(None)
+    ```
+    """
+    return Iter((item,))
+
+
 def into_iter(
-    iterable: typing.Iterable[Item],
+    iterable: collections.Iterable[Item],
 ) -> Iter[Item]:
     """Convert an iterable into `Iter`.
     Example
     -------
     ```py
     sequence = [1,2,3]
-    for item in sain.into_iter(sequence).reversed():
-            print(item)
+    for item in sain.iter(sequence).reversed():
+        print(item)
     # 3
     # 2
     # 1
     ```
 
     Parameters
     ----------
-    iterable: `typing.Iterable[Item]`
+    iterable: `Iterable[Item]`
         The iterable to convert.
-
-    Raises
-    ------
-    `StopIteration`
-        If no elements are left in the iterator.
     """
     return Iter(iterable)
```

### Comparing `sain-0.0.4/sain/macros.py` & `sain-0.0.6/sain/boxed.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,178 +24,167 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-"""A module that contains useful decorators"""
+
+"""a `Box` is a wrapper around a value that expires after the given amount of time."""
 
 from __future__ import annotations
 
-__all__ = ("deprecated", "unimplemented", "todo", "unstable")
+__all__ = ("Box",)
 
-import functools
-import inspect
+import asyncio
+import datetime
+import math
+import time
 import typing
-import warnings
-
-if typing.TYPE_CHECKING:
-    import collections.abc as collections
-
-    T = typing.TypeVar("T", bound=collections.Callable[..., typing.Any])
-
-
-class Error(RuntimeWarning):
-    """A runtime error that is raised when the decorated object fails a check."""
-
-    __slots__ = ("message",)
-
-    def __init__(self, message: str | None = None, *args: typing.Any) -> None:
-        super().__init__(message, *args)
-        self.message = message
-
-
-def _warn(msg: str, stacklevel: int = 2) -> None:
-    warnings.warn(message=msg, stacklevel=stacklevel, category=Error)
-
-
-def unstable(*, reason: str) -> collections.Callable[[T], T]:
-    """A decorator that marks an internal object explicitly unstable."""
 
-    def decorator(obj: T) -> T:
-        @functools.wraps(obj)
-        def wrapper(*args: typing.Any, **kwargs: typing.Any) -> typing.Any:
-            obj_type = "class" if inspect.isclass(obj) else "function"
-            if not obj.__doc__ == "__intrinsics__":
-                # This has been used outside of the lib.
-                raise Error("Stability attributes may not be used outside of the core library")
-
-            name = obj.__name__
-            if name.startswith("_"):
-                name = obj.__name__.lstrip("_")
-
-            _warn(f"{obj_type} {name} is not stable: {reason}")
-            return obj(*args, **kwargs)
-
-        return typing.cast("T", wrapper)
-
-    return decorator
-
-
-def deprecated(
-    *,
-    since: str | None = None,
-    use_instead: str | None = None,
-) -> collections.Callable[[T], T]:
-    """A decorator that marks a function as deprecated.
-
-    An attemp to call the object that's marked will raise an `sain.macros.Error` exception.
-
-    Example
-    -------
-    ```py
-    from sain import deprecated
-
-    @deprecated(since = "1.0.0", use_instead = "UserImpl()")
-    class User:
-        ...
-
-    user = User() # This will raise an error at runtime.
-    ```
-
-    Parameters
-    ----------
-    since : `str`
-        The version that the function was deprecated.
-    removed_int : `str | None`
-        If provided, It will log when will the object will be removed in.
-    use_instead : `str | None`
-        If provided, This should be the alternaviate object name that should be used instead.
-    """
-
-    def decorator(func: T) -> T:
-        @functools.wraps(func)
-        def wrapper(*args: typing.Any, **kwargs: typing.Any) -> typing.Any:
-            obj_type = "class" if inspect.isclass(func) else "function"
-            msg = f"{obj_type} {func.__module__}.{func.__name__} is deprecated."
-
-            if since is not None:
-                msg += f" since {since}."
-
-            if use_instead is not None:
-                msg += f" Use {use_instead} instead."
-
-            _warn(msg)
-            return func(*args, **kwargs)
-
-        return typing.cast("T", wrapper)
-
-    return decorator
+from . import futures
+from . import option
 
+if typing.TYPE_CHECKING:
+    from collections import abc as collections
 
-def todo(message: str | None = None) -> typing.NoReturn:
-    """A place holder that indicates unfinished code.
+    from typing_extensions import Self
 
-    This is not a decorator. See example.
+    from . import Option
 
-    Example
-    -------
-    ```py
+T = typing.TypeVar("T", covariant=True)
 
-    @dataclass
-    class User:
-        name: str
-        id: int
-
-        @classmethod
-        def from_json(cls, payload: dict[str, Any]) -> Self:
-            # Calling this method will raise `Error`.
-            todo()
-    ```
 
-    Parameters
-    ----------
-    *args : object | None
-        Multiple optional arguments to pass if the error was raised.
-    """
-    raise Error(f"not yet implemented: {message}" if message else "not yet implemented")
+@typing.final
+class Box(typing.Generic[T]):
+    """The box object for expiring data. not thread-safe.
 
-
-def unimplemented(*, message: str | None = None, available_in: str | None = None) -> collections.Callable[[T], T]:
-    """A decorator that marks an object as unimplemented.
-
-    An attemp to call the object that's marked will cause a warn.
+    A box is an object that contains a value of type `T` which expires it after the given amount of time,
+    The box won't start expiring the data until its first access with `Box.get` method.
 
     Example
     -------
     ```py
-    from sain import unimplemented
-
-    @unimplemented("User object is not implemented yet.")
-    class User:
-        ...
+    # Initializing a box doesn't mean it started expiring. instead,
+    # getting the value the first time will start the process.
+    cache: dict[str, Box[int]] = {"sora": Box(999, timedelta(seconds=5)}
+
+    # first start expiring here.
+    cache["sora"].get().unwrap()
+    time.sleep(6)
+    assert cache["sora"].has_expired()
     ```
-
-    Parameters
-    ----------
-    message : `str | None`
-        An optional message to be displayed when the function is called. Otherwise default message will be used.
-    available_in : `str | None`
-        If provided, This will be shown as what release this object be implemented.
     """
 
-    def decorator(obj: T) -> T:
-        @functools.wraps(obj)
-        def wrapper(*args: typing.Any, **kwargs: typing.Any) -> typing.Any:
-            obj_type = "class" if inspect.isclass(obj) else "function"
-            msg = message or f"{obj_type} {obj.__module__}.{obj.__name__} is not yet implemented."  # noqa: W503
-
-            if available_in:
-                msg += f" Avaliable in {available_in}."
+    __slots__ = ("__inner", "_expire_in", "_on_expire", "_mono")
 
-            _warn(msg)
-            return obj(*args, **kwargs)
+    def __init__(self, value: T, expire_in: int | float | datetime.timedelta) -> None:
+        if isinstance(expire_in, datetime.timedelta):
+            expire_in = expire_in.total_seconds()
+        else:
+            expire_in = float(expire_in)
+
+        if expire_in <= 0:
+            raise ValueError("expire_in must be more than 0 seconds.")
+
+        # We set the last call on the first access to the value.
+        self._mono: float | None = None
+        self.__inner: Option[T] = option.Some(value)
+        self._on_expire: collections.Callable[[T], typing.Any] | None = None
+        self._expire_in = expire_in
+
+    @property
+    def has_expired(self) -> bool:
+        """Returns True if the value has expired."""
+        # return self._mono is not None and not self._expire_in <= (
+        # time.monotonic() - self._mono
+        # )
+        return self._mono is not None and (
+            not self._mono or self._expire_in <= (time.monotonic() - self._mono)
+        )
+
+    def on_expire(self, callback: collections.Callable[[T], typing.Any]) -> Self:
+        """Set a callback that will be invoked when this value gets expired.
+
+        Both async and sync callbacks are supported.
+
+        Example
+        -------
+        ```py
+        async def sink(message: str) -> None:
+            await client.create_message(message)
+            print("Sinked", message)
+
+        box = Box("bluh", 5).on_expire(sink)
+
+        while box.get().is_some():
+            time.sleep(5)
+        ```
+        First `.get` call on an expired box, the `sink` callback will be invoked,
+        also the inner value will be set to `Some(None)`.
+
+        After 5 seconds.
+        ```py
+        assert box.get() == Some("bluh") # This last call invokes the callback.
+        # Sinked bluh
+        assert box.get().is_none()
+        ```
+        """
+        self._on_expire = callback
+        return self
+
+    def remaining(self) -> float:
+        """Returns when this box will expire in seconds.
+
+        Example
+        --------
+        ```py
+        jogo = Box("jogo", 3)
+        assert jogo.get().unwrap() == "jogo"
+
+        time.sleep(1)
+        assert jogo.remaining() == 2
+        ```
+        """
+        if not self._mono:
+            return 0.0
+
+        return math.floor(
+            (self._expire_in - (time.monotonic() - self._mono) + 1) * 0.99
+        )
+
+    def get(self) -> Option[T]:
+        """Get the contained value if it was not expired, otherwise `Some(None)` is returned.
+
+        Example
+        -------
+        ```py
+        pizza = Box("pizza", timedelta(days=1))
+
+        while not pizza.get().is_none():
+            # Do stuff with the value while its not expired.
+
+        # After 1 day.
+        assert pizza.get().is_none()
+        ```
+        """
+        if self.has_expired:
+            if self._on_expire is not None:
+                try:
+                    if asyncio.iscoroutinefunction(self._on_expire):
+                        futures.loop().run_until_complete(
+                            self._on_expire(self.__inner.unwrap_unchecked())
+                        )
+                    else:
+                        self._on_expire(self.__inner.unwrap_unchecked())
+                finally:
+                    self._on_expire = None
+
+            self.__inner.take()
+            self._mono = None
+            # SAFETY: The value is expired, therefore we always return None.
+            return option.nothing_unchecked()
 
-        return typing.cast("T", wrapper)
+        if self._mono is None:
+            self._mono = time.monotonic()
 
-    return decorator
+        return self.__inner
```

### Comparing `sain-0.0.4/sain/option.py` & `sain-0.0.6/sain/option.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,43 +27,39 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Rust's `Option<T>` type. A value that can either be `T` or `None`"""
 
 from __future__ import annotations
 
-__all__ = ("Some", "Fn", "FnOnce", "ValueT")
+__all__ = ("Some", "Option", "NOTHING")
 
 import typing
 
+from . import cell
 from . import default as _default
-from . import ref as _ref
-
-ValueT = typing.TypeVar("ValueT")
-"""A type hint that represents the generic value of the `Some` type."""
+from . import iter
+from . import macros
 
 T = typing.TypeVar("T")
 T_co = typing.TypeVar("T_co", covariant=True)
 
 if typing.TYPE_CHECKING:
     import collections.abc as collections
 
-    from typing_extensions import Self
-
-    Fn = collections.Callable[[ValueT], T]
-    """A type hint for a function that can take a `ValueT` and return a `T`."""
-    FnOnce = collections.Callable[[], T]
-    """A type hint for a function that takes no arguments and return `T`"""
+    U = typing.TypeVar("U")
+    Fn = collections.Callable[[T], U]
+    FnOnce = collections.Callable[[], U]
 
 
 @typing.final
-class Some(typing.Generic[ValueT], _default.Default[None]):
+class Some(typing.Generic[T], _default.Default[None]):
     """The `Option` type. An object that might be `T` or `None`.
 
-    It is similar to `typing.Optional[T]`, But has proper methods to handle the contined value.
+    It is a drop-in replacement for `typing.Optional[T]`, But has proper methods to handle the contained value.
 
     Example
     -------
     ```py
     value = Some("Hello")
     print(value)
     # Some("Hello")
@@ -81,28 +77,30 @@
     print(none_value.unwrap_or(10))
     # 10
     ```
     """
 
     __slots__ = ("_value",)
 
-    def __init__(self, value: ValueT | None, /) -> None:
+    def __init__(self, value: T | None, /) -> None:
         self._value = value
 
     @staticmethod
     def default() -> None:
         """Default value for `Some`. Returns `None`."""
         return None
 
+    # *- Reading the value -*
+
     @property
-    def read(self) -> ValueT | None:
+    def read(self) -> T | None:
         """Read the contained value."""
         return self._value
 
-    def unwrap(self) -> ValueT:
+    def unwrap(self) -> T:
         """Unwrap the inner value either returning if its not `None` or raising a `RuntimeError`.
 
         Example
         -------
         ```py
         value = Some(5)
         print(value.unwrap())
@@ -115,268 +113,294 @@
 
         Raises
         ------
         `RuntimeError`
             If the inner value is `None`.
         """
         if self._value is None:
-            raise RuntimeError(f"Can't unwrap {type(self).__name__} value.") from None
+            raise RuntimeError(
+                f"Called `Option.unwrap()` on {type(self._value).__name__}."
+            ) from None
 
         return self._value
 
-    def unwrap_or(self, default: ValueT, /) -> ValueT:
+    def unwrap_or(self, default: T, /) -> T:
         """Unwrap the inner value either returning if its not `None` or returning `default`.
 
         Example
         -------
         ```py
         value = Some(5)
         print(value.unwrap_or(10))
         # 5
 
         # Type hint is required here.
-        value: Some[int] = Some(None)
+        value: Option[int] = Some(None)
         print(value.unwrap_or(10))
         # 10
         ```
         """
         if self._value is None:
             return default
 
         return self._value
 
-    def unwrap_or_else(self, f: FnOnce[ValueT], /) -> ValueT:
+    def unwrap_or_else(self, f: FnOnce[T], /) -> T:
         """Unwrap the inner value either returning if its not `None` or calling `f` to get a default value.
 
         Example
         -------
         ```py
         value = Some(5)
         print(value.unwrap_or_else(lambda: 10))
         # 5
 
-        value: Some[bool] = Some(None)
+        value: Option[bool] = Some(None)
         print(value.unwrap_or_else(lambda: True))
         # True
         ```
         """
         if self._value is None:
             return f()
 
         return self._value
 
-    def unwrap_unchecked(self) -> ValueT:
-        """Unwrap the inner value immdiently returning it, passing if its `None`.
+    @macros.unsafe
+    def unwrap_unchecked(self) -> T:
+        """Unwrap the inner value immediately returning it.
 
         Example
         -------
         ```py
+        v: Option[float] = Some(1.2)
+        v.unwrap_unchecked() # 1.2
+
         v: Option[float] = Some(None)
-        print(v.unwrap_unchecked())
-        # ...
+        print(v.unwrap_unchecked()) # Undefined Behavior
+        ```
+        """
+        #! SAFETY: The caller guarantees that the value is not None.
+        return self._value  # type: ignore
+
+    def expect(self, message: str, /) -> T:
+        """Returns the contained value if it is not `None` otherwise raises a `RuntimeError`.
+
+        Example
+        -------
+        ```py
+        value = Some("Hello")
+
+        print(value.expect("Value is None"))
+        # "Hello"
+
+        value: Option[str] = Some(None)
+        print(value.expect("Value is None"))
+        # RuntimeError("Value is None")
         ```
         """
         if self._value is None:
-            pass
+            raise RuntimeError(message)
+
         return self._value
 
-    # Functional.
-    def map(self, f: Fn[ValueT, T], /) -> Some[T]:
-        """Map the inner value to a new value. Returning `Some[None]` if `ValueT` is `None`.
+    # *- Functional operations -*
+    def map(self, f: Fn[T, U], /) -> Some[U]:
+        """Map the inner value to another type. Returning `Some(None)` if `T` is `None`.
 
         Example
         -------
         ```py
         value = Some(5.0)
 
         print(value.map(lambda x: x * 2.0))
         # Some(10.0)
 
-        value: Some[bool] = Some(None)
+        value: Option[bool] = Some(None)
         print(value)
         # Some(None)
         ```
         """
         if self._value is None:
-            return Some(None)
+            return nothing_unchecked()
 
         return Some(f(self._value))
 
-    def map_or(self, default: T, f: Fn[ValueT, T], /) -> T:
-        """Map the inner value to a new value or return `default` if its `None`.
+    def map_or(self, default: U, f: Fn[T, U], /) -> U:
+        """Map the inner value to another type or return `default` if its `None`.
 
         Example
         -------
         ```py
-        value = Some(5.0)
+        value: Option[float] = Some(5.0)
 
-        # Since the value is not `None` this will get mapped.
-        print(value.map_or(10.0, lambda x: x + 1.0))
-        # 6.0
-
-        # This is `None`, so the default value will be returned.
-        value: Some[str] = Some(None)
-        print(value.map_or("5", lambda x: str(x)))
-        # "5"
+        # map to int.
+        print(value.map_or(0, int))
+        # 6
+
+        value: Option[float] = Some(None)
+        print(value.map_or(0, int)
+        # 0
         ```
         """
         if self._value is None:
             return default
 
         return f(self._value)
 
-    def map_or_else(self, default: FnOnce[T], f: Fn[ValueT, T], /) -> T:
-        """Map the inner value to a new value, Or return default which maps to `default()` if its `None`.
+    def map_or_else(self, default: FnOnce[U], f: Fn[T, U], /) -> U:
+        """Map the inner value to another type, or return `default()` if its `None`.
 
         Example
         -------
         ```py
-        value = Some(5.0)
+        def default() -> int:
+            return sys.getsizeof(object())
 
-        # Since the value is not `None` this will get mapped.
-        print(value.map_or_else(lambda: 10.0, lambda x: x + 1.0))
-        # 6.0
+        value: Option[float] = Some(5.0)
 
-        # This is `None`, so the default func will be returned.
-        value: Option[str] = Some(None)
-        print(value.map_or_else(lambda: "5", lambda x: str(x)))
-        # "5"
+        # map to int.
+        print(value.map_or_else(default, int))
+        # 6
+
+        value: Option[float] = Some(None)
+        print(value.map_or_else(default, int)
+        # 28 <- size of object()
         ```
         """
         if self._value is None:
             return default()
 
         return f(self._value)
 
-    def filter(self, predicate: Fn[ValueT, bool]) -> Self:
-        """Returns `Some[None]` if the contained value is `None`,
+    def filter(self, predicate: Fn[T, bool]) -> Some[T]:
+        """Returns `Some(None)` if the contained value is `None`,
 
-        otherwise calls the predicate and returns `Some[ValueT]` if the predicate returns `True`.
+        otherwise calls the predicate and returns `Some(T)` if the predicate returns `True`.
 
         Example
         -------
         ```py
         value = Some([1, 2, 3])
 
-        print(value.filter(lambda x: len(x) >= 2))
+        print(value.filter(lambda x: 1 in x))
         # Some([1, 2, 3])
 
-        value: Some[int] = Some(None)
-        print(value.filter(lambda x: x > 3))
+        value: Option[int] = Some([1, 2, 3]) # or Some(None)
+        print(value.filter(lambda x: 1 not in x))
         # None
         ```
         """
         if (value := self._value) is not None:
             if predicate(value):
                 return Some(value)
 
-        # We could return `None` here, but we want to return `Some[None]` instead.
-        return Some(None)
+        return nothing_unchecked()
+
+    # *- Inner operations *-
 
     def take(self) -> None:
-        """Take the value from the `Some` object setting it to `None`.
+        """Take the value from `Some` object setting it to `None`.
 
         Example
         -------
         ```py
         value = Some("Hi")
         value = value.take()
         print(value)
         # None
         ```
         """
+        if self._value is None:
+            return
+
         self._value = None
 
-    def replace(self, value: ValueT) -> Self:
+    def replace(self, value: T) -> Some[T]:
         """Replace the contained value with another value.
 
         Example
         -------
         ```py
-        value = Some("Hi")
+        value: Option[str] = Some(None)
         value = value.replace("Hello")
-
-        print(value)
         # Some("Hello")
         ```
         """
         self._value = value
-        return Some(self._value)
+        return self
 
-    # Boolean checkings.
-    def expect(self, message: str, /) -> ValueT:
-        """Returns `ValueT` if the contained value is not `None` otherwise raises a `RuntimeError`.
+    def and_ok(self, optb: Some[T]) -> Some[T]:
+        """Returns `Some(None)` if either contained value is `None`,
+
+        Otherwise return `optb`.
 
         Example
         -------
         ```py
-        value = Some("Hello")
-
-        print(value.expect("Value is None"))
-        # "Hello"
+        x: Option[int] = Some(None)
+        y: Option[str] = Some("bye")
+        assert x.and_ok(y).is_none()
 
-        value: Some[str] = Some(None)
-        print(value.expect("Value is None"))
-        # RuntimeError("Value is None")
+        x: Option[int] = Some(10)
+        y: Option[str] = Some("bye")
+        assert value.and_ok(y) == Some("bye")
         ```
         """
-        if self._value is None:
-            raise RuntimeError(message)
-
-        return self._value
+        if self._value is None or optb.is_none():
+            return nothing_unchecked()
 
-    def and_ok(self, optb: Some[T]) -> Some[T]:
-        """Returns `Some[None]` if the contained value is `None`,
+        return optb
 
-        Otherwise return optb as `Some[T | None]` if optb is `Some[T]`.
+    def and_then(self, f: Fn[T, Some[T]]) -> Some[T]:
+        """Returns `Some(None)` if the contained value is `None`, otherwise call `f()`
+        on `T` and return `Option[T]` if it's value not `None`.
 
         Example
         -------
         ```py
         value = Some(5)
-
-        print(value.and_ok(Some(10)))
+        print(value.and_then(lambda x: Some(x * 2)))
         # Some(10)
 
-        value: Some[int] = Some(10)
-        print(value.and_ok(Some(None)))  # optb is `None`.
+        value: Option[int] = Some(10)
+        print(value.and_then(lambda x: Some(None)))
         # Some(None)
         ```
         """
         if self._value is None:
-            return Some(None)
+            return nothing_unchecked()
 
-        return optb
+        return f(self._value)
 
-    def and_then(self, f: Fn[ValueT, Some[T]]) -> Some[T]:
-        """Returns `Some[None]` if the contained value is `None`,
+    # *- Builder methods *-
 
-        otherwise call `f` on `ValueT` and return `Some[T]` if it's value not `None`.
+    def iter(self) -> iter.Iter[T]:
+        """Returns an iterator over the contained value.
 
         Example
         -------
         ```py
-        value = Some(5)
-        print(value.and_then(lambda x: Some(x * 2)))
-        # Some(10)
+        from sain import Some
+        value = Some("gg")
+        value.next() == Some("gg")
 
-        value: Some[int] = Some(10)
-        print(value.and_then(lambda x: Some(None)))
-        # Some(None)
+        value: Option[int] = Some(None)
+        value.next().is_none()
         ```
         """
         if self._value is None:
-            return Some(None)
+            #! SAFETY: We know the value is None here.
+            return iter.empty()  # pyright: ignore
 
-        return f(self._value)
+        return iter.once(self._value)
 
-    def as_ref(self) -> Some[_ref.Ref[ValueT]]:
-        """Returns immutable `Some[Ref[ValueT]]` if the contained value is not `None`,
+    def as_ref(self) -> Some[cell.Cell[T]]:
+        """Returns immutable `Some[sain.cell.Cell[T]]` if the contained value is not `None`,
 
-        Otherwise returns `Some[None]`.
+        Otherwise returns `Some(None)`.
 
         Example
         -------
         ```py
         value = Some(5).as_ref().unwrap()
         value.object = 0 # FrozenError!
 
@@ -385,83 +409,87 @@
 
         # Create a copy of object.
         clone = value.copy()
         clone = 0  # Thats fine.
         print(clone == owned) # False, 0 != 5
 
         # None object.
-        value: Some[int] = Some(None)
+        value: Option[int] = Some(None)
         print(value.as_ref())
-        # Some(Ref(None))
+        # Some(None)
         ```
 
         Raises
         ------
         `dataclasses.FrozenInstanceError`
-            When attempting to modify the contained value. Use `sain.Ref.copy()` method to create a copy.
+            When attempting to modify the contained value. Use `sain.AsRef.copy()` method to create a copy.
 
-            Or just use `Some.as_ref_mut()` if you're dealing with mutable objects.
+            Or just use `.as_mut()` if you're dealing with mutable objects.
         """
         if self._value is not None:
-            return Some(_ref.Ref(self._value))
+            return Some(cell.Cell(self._value))
 
-        return Some(None)
+        # SAFETY: self._value is None.
+        return NOTHING  # pyright: ignore
 
-    def as_mut(self) -> Some[_ref.RefMut[ValueT]]:
-        """Returns mutable `Some[RefMut[ValueT]]` if the contained value is not `None`,
+    def as_mut(self) -> Some[cell.RefCell[T]]:
+        """Returns mutable `Some[sain.cell.RefCell[T]]` if the contained value is not `None`,
 
-        Otherwise returns `Some[None]`.
+        Otherwise returns `Some(None)`.
 
         Example
         -------
         ```py
-        value = Some(5).as_ref_mut().unwrap()
+        value = Some(5).as_mut().unwrap()
         value.object = 0
-        print(value.object) # 0
+        print(value) # Some(RefCell(0))
 
         # None object.
-        value: Some[int] = Some(None)
-        print(value.as_ref_mut())
-        # Some(RefMut(None))
+        value: Option[int] = Some(None)
+        print(value.as_mut())
+        # Some(None)
         ```
         """
         if self._value is not None:
-            return Some(_ref.RefMut(self._value))
+            return Some(cell.RefCell(self._value))
+
+        # SAFETY: self._value is None.
+        return NOTHING  # pyright: ignore
 
-        return Some(None)
+    # *- Boolean checks *-
 
     def is_some(self) -> bool:
         """Returns `True` if the contained value is not `None`, otherwise returns `False`.
 
         Example
         -------
         ```py
         value = Some(5)
         print(value.is_some())
         # True
 
-        value: Some[int] = Some(None)
+        value: Option[int] = Some(None)
         print(value.is_some())
         # False
         ```
         """
         return self._value is not None
 
-    def is_some_and(self, predicate: Fn[ValueT, bool]) -> bool:
+    def is_some_and(self, predicate: Fn[T, bool]) -> bool:
         """Returns `True` if the contained value is not `None` and
         the predicate returns `True`, otherwise returns `False`.
 
         Example
         -------
         ```py
         value = Some(5)
         print(value.is_some_and(lambda x: x > 3))
         # True
 
-        value: Some[int] = Some(None)
+        value: Option[int] = Some(None)
         print(value.is_some_and(lambda x: x > 3))
         # False
         ```
         """
         return self._value is not None and predicate(self._value)
 
     def is_none(self) -> bool:
@@ -470,34 +498,97 @@
         Example
         -------
         ```py
         value = Some(5)
         print(value.is_none())
         # False
 
-        value: Some[int] = Some(None)
+        value: Option[int] = Some(None)
         print(value.is_none())
         # True
         ```
         """
-        return not self.is_some()
-
-    def __str__(self) -> str:
-        return f"Some({self._value!r})"
+        return self._value is None
 
     def __repr__(self) -> str:
         return f"Some({self._value!r})"
 
+    __str__ = __repr__
+
+    def __invert__(self) -> T:
+        return self.unwrap()
+
+    def __or__(self, other: T) -> T:
+        return self.unwrap_or(other)
+
     def __bool__(self) -> bool:
         return self.is_some()
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Some):
             return NotImplemented
 
-        return self._value == other.read
+        return self._value == other._value  # pyright: ignore[reportUnknownVariableType, reportUnknownMemberType]
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return hash(self._value)
+
+
+Option: typing.TypeAlias = Some[T]
+"""A type hint for a value that can be `Some<T>`.
+
+Example
+-------
+```py
+from __future__ import annotations
+
+import typing
+from sain import Some
+
+if typing.CHECKING:
+    from sain import Option
+
+foo: Option[str] = Some(None)
+```
+"""
+
+NOTHING: typing.Final[Some[None]] = Some(None)
+"""A constant that is always `Option<None>`.
+
+Example
+-------
+```py
+from sain import NOTHING, Some
+
+place_holder = NOTHING
+assert NOTHING == Some(None) # True
+```
+"""
+
+
+@typing.no_type_check
+@macros.unsafe
+def nothing_unchecked() -> Option[T]:
+    """A placeholder that always returns `sain.NOTHING` but acts like it returns `Option[T]`.
+
+    This is useful to avoid constructing new `Some(None)` and want to return `T` in the future.
+
+    Example
+    -------
+    ```py
+    class User:
+        username: str
+
+        def name(self) -> Option[str]:
+            if '@' not in self.username:
+                # even though the type of `NOTHING` is `Option[None]`.
+                # we trick the type checker into thinking
+                # that its an `Option[str]`.
+                return nothing_unchecked()
+
+            return Some(self.username.split('@')[0])
+    ```
+    """
+    return typing.cast("Option[T]", NOTHING)
```

### Comparing `sain-0.0.4/sain/result.py` & `sain-0.0.6/sain/sync/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,8 +23,17 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-"""Error handling with the `Result` type."""
+"""Synchronization primitives."""
+
+from __future__ import annotations
+
+__all__ = ("Lazy", "Once", "LazyFuture", "AsyncOnce")
+
+from .lazy import Lazy
+from .lazy import LazyFuture
+from .once import Once
+from .once import AsyncOnce
```

### Comparing `sain-0.0.4/PKG-INFO` & `sain-0.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,143 @@
 Metadata-Version: 2.1
 Name: sain
-Version: 0.0.4
+Version: 0.0.6
 Summary: Standard Rust core types implementations for Python.
 Home-page: https://github.com/nxtlo/sain
 License: BSD-3-Clause license
-Keywords: Rust,config
+Keywords: Rust,config,typing,utilities
 Author: nxtlo
 Author-email: dhmony-99@hotmail.com
-Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/nxtlo/sain
 Description-Content-Type: text/markdown
 
 # sain
-Sain is a dependency-free library that implements some of the Rust core standard types.
 
+a dependency-free library which implements a set of minimal abstraction that brings Rust's ecosystem to Python.
+It offers a few of the core Rust features like `Vec<T>` and `Result<T, E>` and more. See the equivalent type section below.
+
+This library provides a type-safe mechanism for writing Python code, such as the `Result<T, E>` and `Option<T>` types,
+which provides zero exception handling, where you simply return errors as values.
+
+multiple `core`/`std` types are implemented in Python. Check the [project documentation](https://nxtlo.github.io/sain/sain.html)
 
 ## Install
+
 You'll need Python 3.10 or higher.
 
 PyPI
+
 ```sh
-$ pip install sain
+pip install sain
 ```
 
 ## Overview
-More examples in [examples](https://github.com/nxtlo/sain/tree/master/examples)
-
-### `cfg`, `cfg_attr` and Marking objects.
-Conditionally include code at runtime and mark objects.
 
-```py
-from sain import cfg, cfg_attr
+Advanced examples in [examples](https://github.com/nxtlo/sain/tree/master/examples)
 
-@cfg_attr(target_os="unix")
-# Calling this on a non-unix system will raise a RuntimeError
-# and the function will not run.
-def run_when_unix() -> None:
-    import uvloop
-    uvloop.install()
-
-if cfg(target_arch="arm64"):
-    run_when_unix()
-
-# If `cfg` returns True, Function will be in scope.
-if cfg(requires_modules="aiohttp"):
-    def create_app() -> aiohttp.web.Application:
-        # Calling this will raise a runtime error. its marked as `TODO`.
-        sain.todo("Finish me!")
-
-# Assuming aiohttp is not installed.
-# Calling the function will raise `NameError` since its not in scope.
-create_app()
-
-# Those will only warn at runtime and will not raise anything. They're just markers.
-@sain.unimplemented(message="User is not fully implemented.")
-class User:
-
-    @property
-    @sain.deprecated(since = "1.0.4", use_instead="use `get_id` instead.")
-    def id(self) -> int:
-        ...
-```
+### no `try/except`
 
-### `Option<T>` and `Some<T>`
-Implements the standard `Option` and `Some` types. An object that may be `None` or `T`.
+Exceptions suck, `Result` and `Option` is a much better way to avoid runtime exceptions.
 
 ```py
-import sain
-import os
+from sain import Ok, Err
+from sain import Some
+from sain import Vec
 
-if typing.TYPE_CHECKING:
-    # Avaliable only during type checking.
-    from sain import Option
+import typing
+from dataclasses import dataclass
 
-# Stright up replace typing.Optional[str]
-def get_token(key: str) -> Option[str]:
-    # What os.getenv returns may be str or None.
-    return sain.Some(os.environ.get(key))
-
-# Raises RuntimeError("No token found.") if os.getenv return None.
-token = get_token().expect("No token found.")
-
-# The classic way to handle this in Python would be.
-if token is None:
-    token = "..."
-else:
-    ...
-
-# Replace this with `unwrap_or`.
-# Returning DEFAULT_TOKEN if it was None.
-env_or_default = get_token().unwrap_or("DEFAULT_TOKEN")
-
-# Type hint is fine.
-as_none: Option[str] = sain.Some(None)
-as_none.uwnrap_or(123)  # Error: Must be type `str`!
-assert as_none.is_none() # True
-```
-
-### Defaults
-An interface that types can implement which have a default value.
-
-```py
-import sain
-import requests
-
-class Session(sain.Default[requests.Session]):
-    # One staticmethod must be implemented and must return the same type.
-    @staticmethod
-    def default() -> requests.Session:
-        return requests.Session()
+if typing.TYPE_CHECKING:
+    # These are just type aliases that have no cost at runtime.
+    from sain import Result, Option
 
-DEFAULT_SESSION = Session.default()
+@dataclass
+class Chunk:
+    name: str
+    description: Option[str] = Some(None)
+
+@dataclass
+class BlobStore:
+    buffer: Vec[Chunk] = Vec()
+    size: int = 1024
+
+    def put(self, tag: str) -> Result[Chunk, str]:
+        if self.buffer.len() >= self.size:
+            # The return type of the error doesn't have to be a str.
+            # its much better to have it an opaque type such as enums
+            # or any data type with more context.
+            return Err("Reached maximum capacity sry :3")
+
+        chunk = Chunk(tag, Some("Evil within."))
+        self.buffer.push(chunk)
+        return Ok(chunk)
+
+    def next_chunk(self, filtered: str = "") -> Option[Chunk]:
+        # this code makes you feel right at home.
+        return self
+            .buffer
+            .iter()
+            .filter(lambda tag: tag in filtered)
+            .next()
+
+storage = BlobStore()
+match storage.put("wiped"):
+    case Ok(chunk):
+        # Success
+        ...
+    case Err(why):
+        print(why)
 ```
 
-### Iter
-Turns normal iterables into `Iter` type.
-
-```py
-import sain
+## Equivalent types
 
-f = sain.Iter([1,2,3])
-# or f = sain.into_iter([1,2,3])
-assert 1 in f
+- `Option<T>` -> `Option[T]` | `Some(T)`
+- `Result<T, E>` -> `Result[T, E]` | `Ok(T)` | `Err(T)`
+- `&dyn Error` -> `Error`
+- `Vec<T>` -> `Vec[T]`
+- `Default<T>` -> `Default[T]`
+- `AsRef<T>` -> `AsRef[T]`
+- `AsMut<T>` -> `AsMut[T]`
+- `Iterator<Item>` -> `Iter[Item]`
+- `OnceLock<T>` -> `Once[T]`
+- `N/A` -> `Box[T]`, This is different from a rust box.
+
+## Equivalent functions / macros
+
+- `cfg!()` -> `sain.cfg`
+- `todo!()` -> `sain.todo`. This is not a decorator.
+- `deprecated!()` -> `sain.deprecated`
+- `unimplemented!()` -> `sain.unimplemented`
+- `std::iter::once()` -> `sain.iter.once`
+- `std::iter::empty()` -> `sain.iter.empty`
+- `#[cfg_attr]` -> `sain.cfg_attr`
+- `#[doc(...)]` -> `sain.doc(...)`
 
-for item in f.map(lambda i: str(i)):
-    print(item)
-```
+## Notes
 
-### Notes
 Since Rust is a compiled language, Whatever predict in `cfg` and `cfg_attr` returns False will not compile.
 
 But there's no such thing as this in Python, So `RuntimeError` will be raised and whatever was predicated will not run.
```

