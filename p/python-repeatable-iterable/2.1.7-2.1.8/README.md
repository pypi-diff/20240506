# Comparing `tmp/python_repeatable_iterable-2.1.7.tar.gz` & `tmp/python_repeatable_iterable-2.1.8.tar.gz`

## Comparing `python_repeatable_iterable-2.1.7.tar` & `python_repeatable_iterable-2.1.8.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/CONTRIBUTORS.md
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/README_printable.md
--rwxr-xr-x   0        0        0     1676 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/build_and_checks.sh
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/wget_sha512.sh
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/src/python_repeatable_iterable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/src/python_repeatable_iterable/py.typed
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/typing_test/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/COPYING.LESSER
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/README.md
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/pyproject.toml
--rw-r--r--   0        0        0    14587 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/README.md.tpl
+-rwxr-xr-x   0        0        0     1676 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/build_and_checks.sh
+-rw-r--r--   0        0        0    82028 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/python-repeatable-iterable.pdf
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/wget_sha512.sh
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/latex/python-repeatable-iterable.tex
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/latex/python-repeatable-iterable.tex.tpl
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/src/python_repeatable_iterable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/src/python_repeatable_iterable/py.typed
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/typing_test/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/COPYING.LESSER
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/README.md
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0    14587 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.8/PKG-INFO
```

### Comparing `python_repeatable_iterable-2.1.7/README_printable.md` & `python_repeatable_iterable-2.1.8/README.md.tpl`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/build_and_checks.sh` & `python_repeatable_iterable-2.1.8/build_and_checks.sh`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 subdir="build_and_checks_dependencies"
 
 personal_github="https://raw.githubusercontent.com/LLyaudet/"
 dependencies="DevOrSysAdminScripts/main/build_and_checks_dependencies"
 URL_beginning="$personal_github$dependencies"
 
 script="$URL_beginning/common_build_and_checks.sh"
-correct_sha512='528762e5fcd8a586c9fd5a471afeb9f306e7d47757fbf02f33c05'
-correct_sha512+='3f4eca41a8864cdb712c3e9af4e2ac07d916c10338638313ee7a'
-correct_sha512+='e1ff2aa724c4fe2649b90a9'
+correct_sha512='a46cd00d7b2d90fa1a3c7923244879fad28e789ff7dda791a0bd0'
+correct_sha512+='c723848c12cb73ccf2c4c5875cdb674237da9696ef9e4deac07d'
+correct_sha512+='c2b04aed6d90ffb98b9b0c4'
 wget_sha512 "./$subdir/common_build_and_checks.sh" "$script"\
   "$correct_sha512"
 chmod +x "./$subdir/common_build_and_checks.sh"
 
 cwd="."
 if [[ -n "$1" ]];
 then
```

### Comparing `python_repeatable_iterable-2.1.7/wget_sha512.sh` & `python_repeatable_iterable-2.1.8/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/src/python_repeatable_iterable/__init__.py` & `python_repeatable_iterable-2.1.8/src/python_repeatable_iterable/__init__.py`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/typing_test/__init__.py` & `python_repeatable_iterable-2.1.8/typing_test/__init__.py`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/COPYING` & `python_repeatable_iterable-2.1.8/COPYING`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/COPYING.LESSER` & `python_repeatable_iterable-2.1.8/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/README.md` & `python_repeatable_iterable-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.7/pyproject.toml` & `python_repeatable_iterable-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-repeatable-iterable"
-version = "2.1.7"
+version = "2.1.8"
 description = """\
 Add a RepeatableIterable type and a function to obtain it\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
@@ -29,15 +29,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 keywords = ["Python", "Iterable", "Repeatable", "RepeatableIterable"]
 dependencies = [
-   "python-none-objects==1.1.10",
+   "python-none-objects==1.1.11",
 ]
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "isort",
```

### Comparing `python_repeatable_iterable-2.1.7/PKG-INFO` & `python_repeatable_iterable-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-repeatable-iterable
-Version: 2.1.7
+Version: 2.1.8
 Summary: Add a RepeatableIterable type and a function to obtain it
 Project-URL: Homepage, https://github.com/LLyaudet/python-repeatable-iterable
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-repeatable-iterable/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -179,15 +179,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
-Requires-Dist: python-none-objects==1.1.10
+Requires-Dist: python-none-objects==1.1.11
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
```

