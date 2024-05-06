# Comparing `tmp/pkg_inspect-0.1.4.tar.gz` & `tmp/pkg_inspect-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.1.4.tar", last modified: Sat May  4 03:10:41 2024, max compression
+gzip compressed data, was "pkg_inspect-0.1.5.tar", last modified: Mon May  6 01:09:03 2024, max compression
```

## Comparing `pkg_inspect-0.1.4.tar` & `pkg_inspect-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.218563 pkg_inspect-0.1.4/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.4/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.4/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-04 03:10:41.218264 pkg_inspect-0.1.4/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.4/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-04 03:10:41.219300 pkg_inspect-0.1.4/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.4/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.210468 pkg_inspect-0.1.4/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      129 2024-05-04 02:58:20.000000 pkg_inspect-0.1.4/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.210762 pkg_inspect-0.1.4/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       66 2024-05-02 02:08:47.000000 pkg_inspect-0.1.4/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.213073 pkg_inspect-0.1.4/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       25 2024-04-24 00:55:56.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13151 2024-05-04 02:57:52.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.214537 pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-02 02:06:43.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48817 2024-05-04 03:03:29.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-01 23:52:03.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    43620 2024-05-04 02:54:19.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.216344 pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-04-22 02:40:00.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48618 2024-05-04 02:59:35.000000 pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.212198 pkg_inspect-0.1.4/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-04 03:10:41.000000 pkg_inspect-0.1.4/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      701 2024-05-04 03:10:41.000000 pkg_inspect-0.1.4/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-04 03:10:41.000000 pkg_inspect-0.1.4/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-04 03:10:41.000000 pkg_inspect-0.1.4/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-04 03:10:41.217384 pkg_inspect-0.1.4/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.4/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-04-29 03:16:50.000000 pkg_inspect-0.1.4/tests/test_pipinspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.772885 pkg_inspect-0.1.5/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.5/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.5/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-06 01:09:03.772595 pkg_inspect-0.1.5/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.5/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-06 01:09:03.773862 pkg_inspect-0.1.5/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.5/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.762380 pkg_inspect-0.1.5/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      193 2024-05-06 01:06:55.000000 pkg_inspect-0.1.5/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.762718 pkg_inspect-0.1.5/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      104 2024-05-05 20:43:34.000000 pkg_inspect-0.1.5/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.765812 pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-05 19:21:33.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13168 2024-05-06 00:56:09.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.767835 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-02 02:06:43.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47522 2024-05-05 20:43:35.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-05 18:27:31.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47426 2024-05-05 20:43:35.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.770755 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-05-05 19:26:25.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5393 2024-05-06 01:05:02.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/cli.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49212 2024-05-06 00:55:19.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.764759 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      735 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.771751 pkg_inspect-0.1.5/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.5/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-05-04 20:17:40.000000 pkg_inspect-0.1.5/tests/test_pkg_inspect.py
```

### Comparing `pkg_inspect-0.1.4/LICENSE.md` & `pkg_inspect-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.4/PKG-INFO` & `pkg_inspect-0.1.5/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pkg_inspect
-Version: 0.1.4
+Name: pkg-inspect
+Version: 0.1.5
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.4/README.md` & `pkg_inspect-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.4/setup.cfg` & `pkg_inspect-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.1.4
+version = 0.1.5
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A comprehensive tools to inspect Python packages and Python installations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,30 +116,30 @@
             )
 
 
 @__doc_handler(func_name="version_compare")
 def pkg_version_compare(
     package: str,
     first_pyversion: str,
-    other_pyversion,
+    other_pyversion: str,
     /,
     *,
-    item: str,
+    itemOrfile: str,
     opmethod: str = None,
 ):
     """
     Compare the items of a package between two different python versions.
 
     - If the `opmethod` is not provided, the function will return the items from both versions.
 
     - Please refer to the `pkg_version_compare.__doc__` for more information on comparing package data between Python versions.
 
     """
     return _PkgI(package, first_pyversion).version_compare(
-        other_pyversion, item, opmethod=opmethod
+        other_pyversion, itemOrfile, opmethod=opmethod
     )
 
 
 @__doc_handler()
 def get_version_packages(pyversion: str) -> DateTimeAndVersion:
     """
     Get all the packages installed in a python version.
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,19 @@
         """
         return "[Inspected Python Versions]\n" f"{(*self._get_installed_pythons(),)}\n"
 
     @staticmethod
     def _vparser(v) -> PackageVersion:
         return PkgV.parse_version(v)
 
+    @staticmethod
+    def _fix_pkgname(pkg_name: str = None) -> str:
+        if pkg_name:
+            return stranslate(pkg_name, "_", "-")
+
     @classmethod
     @exception_handler("site-path version number", exceptions=StopIteration)
     def _get_version_num(
         cls,
         site_path: Union[Path, str],
         dist_ver: bool = False,
     ) -> Optional[PackageVersion]:
@@ -173,15 +178,15 @@
         self, distinfo_package: Path
     ) -> Generator[tuple[Any, str], Any, None]:
         def _check_version(d_package) -> tuple[Any, str]:
             package_name = get_package_name(d_package)
             package_ver = self._get_version_num(d_package, dist_ver=True)
             if package_ver is None:
                 # Import the version number if the version number is not found
-                # Otherwise, will return Version("0.0.0.0") by default.
+                # Otherwise, will return Version("0.0.0") by default.
                 package_ver = PkgV.import_version(package_name, parse_version=True)
             return package_name, package_ver
 
         packages = executor(
             _check_version,
             distinfo_package,
             max_workers=self._workers,
@@ -200,16 +205,16 @@
     def _get_package_names(
         self,
         py_version: str,
         *,
         return_total: bool = False,
         **kwargs,
     ) -> Union[list[str], Any]:
-        py_version = self._check_version(py_version)
-        raps = kwargs.pop("return_as_paths", True)
+        py_version: PackageVersion = self._check_version(py_version)
+        raps: bool = kwargs.pop("return_as_paths", True)
         pyver_packagenames = sorted(
             # Get the package names for the specified Python version
             py_pack if raps else get_package_name(py_pack)
             # pyver: Python version, pyver_packages: Package paths
             for pyver, pyver_packages in self._get_package_paths()
             # py_pack: Package path
             for py_pack in pyver_packages
@@ -243,16 +248,16 @@
         #### Returns:
             - `str`: The package name for the specified Python version.
 
         #### Raises:
             - `PkgException`: If the package is not found in the specified Python version.
 
         """
-        py_version = self._check_version(py_version)
-
+        py_version: PackageVersion = self._check_version(py_version)
+        package_name: str = self._fix_pkgname(package_name)
         try:
             # Check if the package is found in the specified Python version
             return next(
                 pkg
                 for pkg in self._get_package_names(
                     py_version=py_version, return_as_paths=False
                 )
@@ -415,82 +420,46 @@
         - `package` (PathOrStr): The package name to inspect.
         - `pyversion` (str): The Python version to inspect.
         - `generator` (bool): A boolean value indicating whether to return a generator or unpacked result.
         - `max_workers` (int): The maximum number of workers to use for concurrent execution.
             (`ThreadPoolExecutor`)
         - `sort_by` (Union[ZeroOrOne, Literal["reverse"]]): A value indicating whether to sort the distributions.
 
-    #### Attributes:
+    #### Properties:
         - `package_paths` (Iterable[Path]): Property for site-package paths for each python version.
         - `package_versions` (Generator[tuple[str, tuple[tuple[Any, str]]]]): Property for package versions installed for each python version.
         - `pyversions` (tuple[Path]): Property for installed python versions.
         - `site_packages` (Iterable[str]): Property for site packages installed for each python version.
 
     #### Methods:
         - `inspect_package`: Inspect details of an installed Python package.
-        - `_check_package`: Check the package name for the specified Python version.
-
-    #### Examples:
-        ```python
-        # The `inspect_package` method is called to inspect the details of the `pkgInspect` package.
-        PkgInspect().inspect_package(package="pkgInspect", item="short_meta")
-        # Output: {'Metadata-Version': 'x.x', 'Name': 'pkgInspect', 'Version': '1.x.x', 'Summary': 'A powerful data analysis and manipulation library for Python.', 'Home-page': 'https://pandas.pydata.org', 'Author': 'Wes McKinney', 'Author-email': '
-
-        PkgInspect().inspect_package(package="pkgInspect", item="version")
-        # Output: '1.x.x'
-
-        PkgInspect().inspect_package(package="pkgInspect", item="license")
-        # Output: 'Apache 2.0'
-
-        PkgInspect().inspect_package(package="pkgInspect", item="version_history")
-        # Output: (('1.x.x', 'Jan 1, 2021'), ('1.x.x', 'Dec 1, 2020'), ...)
-
-        # Attrbutes
-        PkgInspect().pyversions
-        # Output: ('3.8', '3.9', '3.10', ...)
-
-        PkgInspect().package_paths
-        # Output:
-        # ('3.8', <generator object PkgInspect._ver_executor at 0x...>, ...)
-        # ('3.8', [PosixPath('/usr/local/Cellar/python@3.8/3.8.2_2/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/pip-20.0.2.dist-info'), ...])
-
-        PkgInspect().site_packages
-        # Output:
-        # <generator object PkgInspect._get_site_packages at 0x...>
-        # (PosixPath('/usr/local/Cellar/python@3.8/3.8.2_2/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages'), ...)
-
-        PkgInspect().package_versions
-        # Output:
-        # ('3.8', <generator object PkgInspect._ver_executor at 0x...>)
-        # ('3.8', (('pip', '20.0.2'), ('setuptools', '46.1.3'), ('wheel', '0.34.2'), ...))
-        ```
     """
 
     __dict__ = {}
-    __slots__ = ("__weakrefs__", "_pyversion", "_pkg", "__pipv_pkg", "__pipm")
+    __slots__ = ("__weakrefs__", "_pyversion", "_pkg", "__pipm")
 
     def __init__(
         self, package: PathOrStr = None, pyversion: str = None, **kwargs
     ) -> None:
         # kwargs: 'generator', 'max_workers', 'sort_by'
         super().__init__(**kwargs)
         self._pyversion = self._check_version(pyversion, allow_none=True)
-        self._pkg = (
-            self._check_package(
-                py_version=self._pyversion,
-                package_name=get_package_name(package),
-            )
-            if all((self._pyversion, package))
-            else None
-        )
+        self._pkg = self._fix_pkgname(package)
         self.__pipm: PkgM = partial(PkgM, max_workers=self._workers)
-        if self._pkg:
-            self.__pipv_pkg: PkgV = lambda: PkgV(
-                package=self._pkg, generator=self._generator
-            )
+
+    def __pipv(self) -> PkgV:
+        if self.__validate_pkg():
+            return PkgV(package=self._pkg, generator=self._generator)
+
+    def __validate_pkg(self) -> Union[str, NoReturn]:
+        self.__check_attrs()
+        return self._check_package(
+            py_version=self._pyversion,
+            package_name=get_package_name(self._pkg),
+        )
 
     @recursive_repr(fillvalue="PkgInspect(...)")
     def __repr__(self) -> str:
         return PkgGenRepr(self).__str__()
 
     def __str__(self) -> str:
         """
@@ -512,14 +481,19 @@
         return self.__repr__()
 
     def __check_attrs(self, attr: str = None):
         _musthave = lambda at: musthave_attr(
             self, attr=at, item="Python {!r}".format(getattr(self, at))
         )
         if attr and attr in self.__slots__:
+            if attr == "_pkg":
+                if not isinstance(self._pkg, str):
+                    raise PkgException(
+                        f"The specified package must be a string type value."
+                    )
             _musthave(attr)
             return
         else:
             _musthave("_pyversion")
             _musthave("_pkg")
 
     @cache
@@ -705,14 +679,15 @@
                         - `PkgVersions fields`: Possible Fields from the `PkgVersions` class.
                             - `initial_version` (PackageVersion): Returns the initial version of the package.
                             - `installed_version` (PackageVersion): Returns the installed version of the package.
                             - `latest_version` (PackageVersion): Returns the latest version of the package.
                             - `total_versions` (int): Returns the total number of versions of the package.
                             - `version_history` (TupleOfPkgVersions): Returns the version history of the specified package.
                             - `package_url`: Returns the URL of the package on PyPI.
+                            - `downloads_history` (dict[str, int]): Returns the downloads history of the package.
                             - `github_stats_url` (str): Returns the GitHub statistics URL of the package.
                             - `github_stats` (dict[str, Any]): Returns the GitHub statistics of the package.
                                 - The GitHub statistics are returned as a dictionary \
                                     containing the following fields which can accessed using the `item` parameter:
                                     - `Forks` (int): Returns the number of forks on GitHub.
                                     - `Stars` (int): Returns the number of stars on GitHub.
                                     - `Watchers` (int): Returns the number of watchers on GitHub.
@@ -861,25 +836,25 @@
                         # Update the dictionary with the statistics
                         full_pypi_stats.update(**_get_pypistat(m))
                 # Return the full statistics
                 return full_pypi_stats
             # Otherwise, return the specified item from the 'pypistats' module
             return _get_pypistat(_item)
 
-        # The following options require the package to be specified
-        # and the Python version to be specified and validated.
-        self.__check_attrs()
+        # The following options require the package and/or Python version
+        # to be specified and validated.
+        self.__validate_pkg()
 
         if _item in pkgv_props:
-            get_pkgv = lambda it: getattr(self.__pipv_pkg(), it)
+            get_pkgv = lambda it: getattr(self.__pipv(), it)
             if _item in gh_keys or _item == (gh_stats_str := "github_stats"):
-                gh_stats = lambda x=gh_stats_str: get_pkgv(x)
+                gh_stats = get_pkgv(gh_stats_str)
                 if _item == gh_stats_str:
-                    return gh_stats()
-                return gh_stats()[_item.capitalize()]
+                    return gh_stats
+                return gh_stats[_item]
             # Check if the item is a property of the 'PkgVersions' class
             return get_pkgv(_item)
         elif _item in pkgi_props:
             return getattr(self, _item)
         elif _item in inspect_fields:
             # Return the source file for the specified package
             return self._import_meta(self._pkg, item=_item)
@@ -1082,21 +1057,21 @@
         except (*BASE_EXCEPTIONS, PkgException):
             return False
         return True
 
     @property
     def islatest_version(self) -> bool:
         """Return a boolean value indicating whether the package is the latest version."""
-        return self.__pipv_pkg().is_latest(self.installed_version)
+        return self.__pipv().is_latest(self.installed_version)
 
     @property
     @generator_handler(is_string=True)
     def available_updates(self) -> Optional[Iterator[PackageVersion]]:
         """Return the available updates for the specified package."""
-        return self.__pipv_pkg().get_updates(self.installed_version)
+        return self.__pipv().get_updates(self.installed_version)
 
     @property
     def installed_version(self) -> PackageVersion:
         """Return the installed version of the specified package."""
         return self._get_version_num(self.get_site_package(), dist_ver=True)
 
     @cached_property
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         return default_stats
 
     @os_exception_handler()
     def _os_stats(
         self, path: PathOrStr = None, keys_only: bool = False
     ) -> dict[str, IntOrFloat]:
         if not path:
-            path = DUMMY_FILE
+            path = DUMMY_PATH
         stats_results = self._path_stats(path, stats_results=True)
         metric_keys = set(k for k in dir(stats_results) if k.startswith("st"))
 
         if keys_only:
             for s in ("st_fsize", "st_vsize"):
                 metric_keys.add(s)
             return metric_keys
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -618,17 +618,18 @@
     ```python
     version_instance = PkgVersions("pandas")
     print(version_instance.version_history)
     # Output: (('2.25.1', 'Jan 1, 2021'), ('2.25.0', 'Dec 1, 2020'), ...)
     ```
     """
 
-    # The API endpoint for fetching package versions
+    # The API endpoint for fetching package stats & versions
     PYPI_API: str = "https://pypi.org/project/{}/#history"
     STATS_API: str = "https://libraries.io/{}/{}"
+    DOWNLOADS_API: str = "https://www.pepy.tech/projects/{}"
 
     # Pattern for matching release dates
     # Example: "Jan 1, 2021"
     # This pattern is specifically designed for the `PkgVersions` class to accurately match release dates
     # when parsing package version history release dates from PyPI.
     DATE_PATTERN: Pattern = r"[A-Z][a-z]{2}\s\d{1,2},\s\d{4}"
 
@@ -657,38 +658,46 @@
         "_pkg_url",
         "_pkg_path",
         "_sort_by",
         "_vhistory",
         "_initial",
         "_latest",
         "_gh_stats",
+        "_gh_url",
+        "_downloads_url",
+        "_dhistory",
     )
 
     def __init__(
         self,
         package: str,
         package_manager: str = None,
         *,
         sort_by: Union[DatesOrVersions, ZeroOrOne] = "versions",
     ) -> None:
         # Example: `PkgVersions("pandas") < PkgVersions("pandas")`
         # Compares the latest version of the specified package with the latest version of the other package
 
         # Parameters
-        self._pkg_name = package
+        self._pkg_name = stranslate(package, "_", "-")
         self._pkg_manager = package_manager
-        self._pkg_path = self._validate_package(self._pkg_name)
-        self._pkg_url = self._pkg_path.removesuffix("#history")
         self._sort_by = sort_by
+        self._pkg_path = self._validate_package(self._pkg_name)
 
-        # Properties
+        # Data Properties
         self._vhistory = None  # Version History
         self._initial = None  # Initial Version
         self._latest = None  # Latest Version
-        self._gh_stats = None
+        self._gh_stats = None  # GitHub Stats
+        self._dhistory = None  # Downloads History
+
+        # URL Properties
+        self._pkg_url = None
+        self._gh_url = None
+        self._downloads_url = None
 
     def __len__(self) -> int:
         """Return the total number of versions in the version history."""
         return len((*self._version_history(),))
 
     def __sizeof__(self) -> int:
         """Return the total number of versions in the version history."""
@@ -707,15 +716,15 @@
 
     def __hash__(self) -> int:
         """Return the hash value of the version history."""
         return hash(self.version_history)
 
     @classmethod
     def import_version(
-        cls, package_name: str, parse_version: bool = False
+        cls, package_name: str, *, parse_version: bool = False
     ) -> Union[PackageVersion, str]:
         """
         Retrieve the version of the specified package using the `importlib.metadata` module.
 
         ### Args:
             - `package_name` (str): The name of the package to retrieve the version.
             - `parse_version` (bool, optional): Whether to parse the version using the `packaging.version` module. Defaults to False.
@@ -918,44 +927,48 @@
             - `PkgException`: If the specified operator method is not valid.
         """
         return cls._compare_items(
             items=(current_dt, other_dt), op_method=op_method, item_type="dates"
         )
 
     @cache
-    def _main_request(self, url: PathOrStr) -> Union[str, Any]:
+    def _main_request(self, url: PathOrStr, parse_html: bool = True) -> Union[str, Any]:
         """Return the main asynchronous request for the version history page (#history) of the specified package."""
         try:
-            return asyncio.run(url_request(url))
-        except ClientResponseError:
+            url_contents = asyncio.run(url_request(url))
+            if parse_html:
+                url_contents = self._parse_html(url_contents)
+            return url_contents
+        except ClientResponseError as cre:
             raise RedPkgE(
                 f"An error occurred while trying to find {url!r}.",
                 "Please ensure the package name and manager is correct and is available on the following websites:"
                 f"\n- {self.package_url = }"
-                f"\n- {self.github_stats_url = }",
+                f"\n- {self.github_stats_url = }"
+                f"\n[ORG-ERROR]: {cre}",
             )
         except BASE_EXCEPTIONS as be_error:
             raise be_error
 
     def _parse_html(self, html_contents: str) -> BeautifulSoup:
         return BeautifulSoup(html_contents, "html.parser")
 
     def _history_page(self) -> Generator[Any, str, None]:
         # Parse the specified package history release page using BeautifulSoup.
         # Return the release distribution.
-        hsoup: BeautifulSoup = self._parse_html(self._main_request(self._pkg_path))
+        hsoup: BeautifulSoup = self._main_request(self._pkg_path)
         yield from (
             rd  # release-date
             for i in hsoup.find_all("div", class_="release")
             # Removes all instances of pre-releases
             if search(self.VERSION_PATTERN, rd := i.get_text(strip=True))
         )
 
     def _get_gh_stats(self, keys_only: bool = False):
-        gh_soup = self._parse_html(self._main_request(self.github_stats_url))
+        gh_soup = self._main_request(self.github_stats_url)
         stats_chart = [
             _j
             for i in gh_soup.find_all("dl", class_="row detail-card")
             for j in i.text.splitlines()
             if (_j := re.sub(r"\s{2,}", "", j))
         ]
         gh_stats = None
@@ -1006,22 +1019,94 @@
             )
         )
 
     def _get_dtv(self, method: MinOrMax = max) -> TupleDoubleStr:
         """Return the initial or latest release date and version of the package."""
         return [min, max][method == max](self._version_history(), key=itemgetter(1))
 
+    def _get_total_downloads(self, return_url: bool = False) -> str:
+        downloads_soup = self._main_request(self.DOWNLOADS_API.format(self._pkg_name))
+        downloads_url, total_downloads = [
+            d.text
+            for d in downloads_soup.find_all(
+                "div", class_="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 css-woiofv"
+            )
+        ]
+        if return_url:
+            return downloads_url
+        if (int_downloads := int(clean(total_downloads))) >= int(1e6):
+            return f"{abbreviate_number(int_downloads)} ({total_downloads})"
+        return total_downloads
+
+    def _get_downloads_history(self):
+        downloads_soup = self._main_request(self.DOWNLOADS_API.format(self._pkg_name))
+        soup_unpacker = lambda *args, **kwargs: [
+            i.text for i in downloads_soup.find_all(*args, **kwargs)
+        ]
+        version_columns = soup_unpacker(
+            "th",
+            class_="MuiTableCell-root MuiTableCell-head MuiTableCell-stickyHeader MuiTableCell-sizeMedium css-8coetn",
+        )[1:]
+
+        downloads_history = soup_unpacker(
+            "td",
+            class_="MuiTableCell-root MuiTableCell-body MuiTableCell-sizeMedium css-q34dxg",
+        )
+        dh_dict = {}
+        date = None
+        search_compiler = partial(search, compiler=True)
+        for d in downloads_history:
+            search_func = partial(search_compiler, obj=d)
+            if search_func("-"):
+                date = d
+                dh_dict[date] = []
+            else:
+                d = int(clean(d))
+                dh_dict[date].append(d)
+        total_downloads = soup_unpacker(
+            "td",
+            class_="MuiTableCell-root MuiTableCell-body MuiTableCell-alignRight MuiTableCell-sizeMedium css-1i36psw",
+        )[1::2]
+        return {
+            k: {
+                "versions": dict(
+                    zip(
+                        (
+                            self.parse_version(i)
+                            if search_compiler(r"^(?!.*\*).*$", i)
+                            else i
+                            for i in version_columns
+                        ),
+                        v,
+                    )
+                ),
+                "sum": (f"{sum_v:,}", abbreviate_number(sum_v))
+                if (sum_v := sum(v)) >= (million := int(1e6))
+                else sum_v,
+                "total_downloads": (td, abbreviate_number(td))
+                if (td := int(total_downloads[idx])) >= million
+                else td,
+            }
+            for idx, (k, v) in enumerate(dh_dict.items())
+        }
+
     @property
     def version_history(self) -> Generator[DateTimeAndVersion, Any, None]:
         """Cached property containing the version history of the specified package."""
         if self._vhistory is None:
             self._vhistory = self._version_history()
         return self._vhistory
 
     @property
+    def downloads_history(self) -> dict[str, dict[str, Any]]:
+        if self._dhistory is None:
+            self._dhistory = self._get_downloads_history()
+        return self._dhistory
+
+    @property
     def initial_version(self) -> TupleDoubleStr:
         """Return the initial release date and version of the package."""
         if self._initial is None:
             self._initial = self.create_dtv(*self._get_dtv(method=min))
         return self._initial
 
     @property
@@ -1033,28 +1118,42 @@
 
     @property
     def total_versions(self) -> int:
         """Return the total number of versions in the version history."""
         return self.__sizeof__()
 
     @property
+    def total_downloads(self) -> str:
+        return self._get_total_downloads()
+
+    @property
     def github_stats(self):
         if self._gh_stats is None:
             self._gh_stats = self._get_gh_stats()
         return self._gh_stats
 
     @property
-    def package_url(self):
+    def package_url(self) -> str:
+        if self._pkg_path and self._pkg_url is None:
+            self._pkg_url = self._pkg_path.removesuffix("#history")
         return self._pkg_url
 
     @property
-    def github_stats_url(self):
-        return self._validate_package(
-            self._pkg_name, self.STATS_API, package_manager=self._pkg_manager
-        )
+    def github_stats_url(self) -> str:
+        if self._pkg_name and self._gh_url is None:
+            self._gh_url = self._validate_package(
+                self._pkg_name, self.STATS_API, package_manager=self._pkg_manager
+            )
+        return self._gh_url
+
+    @property
+    def downloads_url(self) -> str:
+        if self._pkg_name and self._downloads_url is None:
+            self._downloads_url = self._get_total_downloads(return_url=True)
+        return self._downloads_url
 
     @_DateTimeVersions.operator_handler("==", version_only=True)
     def is_latest(self, other_py: PackageVersion) -> bool:
         """Check if the specified version is the latest version."""
         return self.latest_version, self.parse_version(other_py)
 
     def get_updates(self, current_version: str) -> Optional[Iterator[PackageVersion]]:
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 # MARK: - Constants, Variables, Functions and Exception Handling
 
 # Default 'DUMMY' values to be used for extracting
 #   1. package metadata
 #   2. Distribution Information
 #   3. GitHub Statistics
-DUMMY_FILE: Path = Path(__file__)
+DUMMY_PATH: Path = Path(__file__).parents[3]  # Main Directory
 DUMMY_PKGNAME: str = "requests"
 
 
 # Field names and custom types to extract
 # from the package's METADATA file or dist-info ('site_path') directory.
 METADATA_FIELDS: tuple[str] = (
     # - 'METADATA' fieldnames
@@ -157,48 +157,49 @@
 # Unit Measurement Keys
 # ---------------------
 UNITS: tuple[str] = ("KB", "MB", "GB", "TB")
 
 
 # region OperatorUtils
 def get_opmethod(
-    opmethod: OperatorMethods, all_methods: bool = False, *, allow_none: bool = False
+    opmethod: OperatorMethods, *, allow_none: bool = False
 ) -> Optional[Any]:
     """Check the specified operator method is valid."""
     comparison_ops = {
         "==": "eq",
         ">=": "ge",
         ">": "gt",
         "<=": "le",
         "<": "lt",
         "!=": "ne",
+        "+": "add",
+        "**": "pow",
+        "*": "mul",
     }
-    if not allow_none:
-        if not all_methods:
-            if opmethod not in chain.from_iterable(zip(*comparison_ops.items())):
-                raise PkgException(
-                    f"The specified operator method {opmethod!r} is not a valid comparison operator."
-                )
 
-        elif all_methods and not hasattr(operator, opmethod):
-            raise PkgException(
-                f"The specified operator method {opmethod!r} is not a valid option."
-            )
-    # Return the operator method if valid
     # E.g `operator.gt`, `operator.lt`, `operator.eq`
-    return getattr(operator, comparison_ops.get(opmethod, opmethod), None)
+    opm = next(
+        (o for o in chain.from_iterable(zip(*comparison_ops.items())) if o == opmethod),
+        "",
+    )
+    if all((not allow_none, not opm, not hasattr(operator, opmethod))):
+        raise PkgException(
+            f"The specified operator method {opmethod = } is not a valid operator."
+        )
+    if opm:
+        # Return the operator method if valid
+        return getattr(operator, comparison_ops.get(opm, opmethod), None)
 
 
 # Default operator methods
-_gopm = partial(get_opmethod, all_methods=True)
-add_ = _gopm("add")
-multiply_ = _gopm("mul")
-pow_ = _gopm("pow")
-equal_ = get_opmethod("eq")
-lessthan_ = get_opmethod("lt")
+add_ = get_opmethod("+")
+multiply_ = get_opmethod("*")
+pow_ = get_opmethod("**")
+equal_ = get_opmethod("==")
+lessthan_ = get_opmethod("<")
 
 
 # region InspectUtils
 def is_function(c):
     """This function checks if the specified object is a function."""
     return inspect.isfunction(c)
 
@@ -479,54 +480,49 @@
     # Initialize the recursive function
     return create_id(length, ensure_unique)
 
 
 # endregion
 
 
-# region CleanUtils
-def clean(s: str, exclude: str = "", keep_punct: bool = False) -> str:
+# region StrUtils
+def stranslate(s: str, *args):
+    return s.translate(str.maketrans(*args))
+
+
+def clean(s: str, exclude: str = "") -> str:
     """
     Remove all instances of a specified character from a string.
 
     #### Args:
         - `s` (str): The string to clean.
         - `exclude` (str): The character(s) to exclude from the string.
-        - `keep_punct` (bool): A flag indicating whether to keep punctuation characters in the string.
 
     #### Returns:
         - `str`: The cleaned string.
 
     #### Note:
         - The function removes all instances of the specified character(s) from the string.
         - Punctuation characters are removed by default.
-
-    #### Example:
-    ```python
-    clean("ae9c3f4g5h6i7j8k9l0", "ae9c3")
-    # Output: 'f4g5h6i7j8k9l0'
-
-    clean("ae9c3f4g5h6i7j8k9l0", string.ascii_lowercase)
-    # Output: '93657890'
-    ```
-
     """
-
-    @base_exception_handler(item="the specified string.")
-    def clean_(s_):
-        return s_.translate(
-            str.maketrans("", "", add_(exclude, "" if keep_punct else punctuation))
-        )
-
-    return clean_(s)
+    return stranslate(
+        s,
+        *dup_obj(""),
+        add_(
+            # Remove punctuation by default
+            # if 'exclude' does not contain punctuation
+            exclude,
+            "" if search(exclude, punctuation, compiler=True) else punctuation,
+        ),
+    )
 
 
 def rm_period(s: str) -> str:
     """Remove all instances of a period from a string."""
-    return clean(s, ".", keep_punct=True)
+    return clean(s, ".")
 
 
 # endregion
 
 # region GenUtils
 
 
@@ -1443,28 +1439,54 @@
         )
     filtered = filterfalse(obj.__eq__, iter_obj)
     if sort_result:
         filtered = sorted(filtered)
     return filtered
 
 
-async def url_request(url: PathOrStr) -> Union[str, Any]:
+def abbreviate_number(num: Union[int, str]):
+    """Converts a large number into an abbreviated form with common terms like Thousand, Million, Billion, etc."""
+    # Remove commas and convert to integer
+    if isinstance(num, str):
+        num = int(clean(num))
+
+    # Define abbreviations and their respective scales
+    abbrevs = (
+        (1_000_000_000_000, "Trillion"),
+        (1_000_000_000, "Billion"),
+        (1_000_000, "Million"),
+    )
+
+    for scale, abbrev in abbrevs:
+        if num >= scale:
+            # Convert to the appropriate scale and round to two decimal places
+            value = num / scale
+            # If rounded value is whole number, return it without decimal
+            if value == (int_val := int(value)):
+                return f"{int_val} {abbrev}"
+            return f"{value:.2f} {abbrev}"
+
+    # If less than 1000, return the number as is
+    return num
+
+
+async def url_request(url: PathOrStr, **kwargs) -> Union[str, Any]:
     try:
         async with ClientSession(
             connector=TCPConnector(
                 ssl=False,
                 enable_cleanup_closed=True,
                 force_close=True,
                 ttl_dns_cache=DEFAULT_TIMEOUT,
             ),
             raise_for_status=True,
         ) as session:
             if isinstance(url, Path):
                 url = url.as_posix()
-            async with session.get(url) as response:
+            async with session.get(url, **kwargs) as response:
                 # If the response is valid, return the response text.
                 return await response.text()
     except ContentTypeError as cte:
         # If the content type is not valid, raise a `ContentTypeError`.
         raise cte
     except (ClientConnectionError, ServerDisconnectedError):
         # If the client connection is not valid, recursively retry the request.
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pkg-inspect
-Version: 0.1.4
+Name: pkg_inspect
+Version: 0.1.5
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.4/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.1.5/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 src/pkg_inspect/pkg_functions/__init__.py
 src/pkg_inspect/pkg_functions/functions.py
 src/pkg_inspect/pkg_modules/__init__.py
 src/pkg_inspect/pkg_modules/pkg_inspect.py
 src/pkg_inspect/pkg_modules/pkg_metrics.py
 src/pkg_inspect/pkg_modules/pkg_versions.py
 src/pkg_inspect/pkg_utils/__init__.py
+src/pkg_inspect/pkg_utils/cli.py
 src/pkg_inspect/pkg_utils/exception.py
 src/pkg_inspect/pkg_utils/util_types.py
 src/pkg_inspect/pkg_utils/utils.py
 tests/__init__.py
-tests/test_pipinspect.py
+tests/test_pkg_inspect.py
```

### Comparing `pkg_inspect-0.1.4/tests/test_pipinspect.py` & `pkg_inspect-0.1.5/tests/test_pkg_inspect.py`

 * *Files identical despite different names*

