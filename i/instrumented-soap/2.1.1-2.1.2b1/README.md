# Comparing `tmp/instrumented-soap-2.1.1.tar.gz` & `tmp/instrumented_soap-2.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instrumented-soap-2.1.1.tar", last modified: Fri Oct  1 14:19:32 2021, max compression
+gzip compressed data, was "instrumented_soap-2.1.2b1.tar", max compression
```

## Comparing `instrumented-soap-2.1.1.tar` & `instrumented_soap-2.1.2b1.tar`

### file list

```diff
@@ -1,24 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-01 14:19:32.107432 instrumented-soap-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      749 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1744 2021-10-01 14:19:32.107432 instrumented-soap-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      990 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      672 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      126 2021-10-01 14:19:32.107432 instrumented-soap-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1629 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-01 14:19:32.100432 instrumented-soap-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-01 14:19:32.105432 instrumented-soap-2.1.1/src/instrumented_soap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1744 2021-10-01 14:19:31.000000 instrumented-soap-2.1.1/src/instrumented_soap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2021-10-01 14:19:32.000000 instrumented-soap-2.1.1/src/instrumented_soap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-01 14:19:31.000000 instrumented-soap-2.1.1/src/instrumented_soap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2021-10-01 14:19:31.000000 instrumented-soap-2.1.1/src/instrumented_soap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-10-01 14:19:31.000000 instrumented-soap-2.1.1/src/instrumented_soap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-01 14:19:32.106433 instrumented-soap-2.1.1/src/soap/
--rw-rw-rw-   0 root         (0) root         (0)     2730 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/src/soap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2857 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/src/soap/http.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/src/soap/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/src/soap/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-01 14:19:32.106433 instrumented-soap-2.1.1/src/soap/tests/
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/src/soap/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2021-10-01 14:19:22.000000 instrumented-soap-2.1.1/src/soap/tests/test_soap.py
--rw-r--r--   0 root         (0) root         (0)        6 2021-10-01 14:19:31.000000 instrumented-soap-2.1.1/version.txt
+-rw-r--r--   0        0        0      747 2024-05-06 18:19:02.927587 instrumented_soap-2.1.2b1/LICENSE.md
+-rw-r--r--   0        0        0      990 2024-05-06 18:19:02.927587 instrumented_soap-2.1.2b1/README.rst
+-rw-r--r--   0        0        0      753 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0     2730 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/src/soap/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/src/soap/http.py
+-rw-r--r--   0        0        0     1840 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/src/soap/settings.py
+-rw-r--r--   0        0        0     4232 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/src/soap/test.py
+-rw-r--r--   0        0        0      123 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/src/soap/tests/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 18:19:02.929587 instrumented_soap-2.1.2b1/src/soap/tests/test_soap.py
+-rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 instrumented_soap-2.1.2b1/PKG-INFO
```

### Comparing `instrumented-soap-2.1.1/LICENSE.md` & `instrumented_soap-2.1.2b1/LICENSE.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,5 +1,15 @@
-Copyright (c) 2016, Craig Weber <crgwbr@gmail.com>
+ISC License
 
-Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
+Copyright (c) 2016 - 2024 thelabnyc
 
-THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted, provided that the above
+copyright notice and this permission notice appear in all copies.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
+AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `instrumented-soap-2.1.1/PKG-INFO` & `instrumented_soap-2.1.2b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: instrumented-soap
-Version: 2.1.1
-Summary: Wrapper around suds-jurko that adds improved proxy support and testing tools.
+Version: 2.1.2b1
+Summary: Wrapper around suds-community that adds improved proxy support and testing tools.
 Home-page: https://gitlab.com/thelabnyc/instrumented-soap
-Author: Craig Weber
-Author-email: crgwbr@gmail.com
 License: ISC
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
+Author: thelabnyc
+Author-email: thelabdev@thelabnyc.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Provides-Extra: development
-License-File: LICENSE.md
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Django (>=3.2)
+Requires-Dist: requests (>=2.9.1)
+Requires-Dist: suds-community (>=0.8.5)
+Project-URL: Repository, https://gitlab.com/thelabnyc/instrumented-soap
+Description-Content-Type: text/x-rst
 
 Instrumented SOAP
 =================
 
 |  |license| |kit| |format| |downloads|
 
 .. |license| image:: https://img.shields.io/pypi/l/instrumented-soap.svg
@@ -40,8 +39,7 @@
 This package is a thin wrapper around the `suds <https://suds.readthedocs.io/en/latest/index.html>`_ library that adds several useful features.
 
 - Improved HTTP proxy support for SOAP Transports.
 - Useful SOAP API mocking and unit-testing tools.
 
 **Full Documentation**: https://instrumented-soap.readthedocs.io
 
-
```

### Comparing `instrumented-soap-2.1.1/README.rst` & `instrumented_soap-2.1.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `instrumented-soap-2.1.1/src/soap/__init__.py` & `instrumented_soap-2.1.2b1/src/soap/__init__.py`

 * *Files identical despite different names*

### Comparing `instrumented-soap-2.1.1/src/soap/http.py` & `instrumented_soap-2.1.2b1/src/soap/http.py`

 * *Files identical despite different names*

### Comparing `instrumented-soap-2.1.1/src/soap/settings.py` & `instrumented_soap-2.1.2b1/src/soap/settings.py`

 * *Files identical despite different names*

### Comparing `instrumented-soap-2.1.1/src/soap/test.py` & `instrumented_soap-2.1.2b1/src/soap/test.py`

 * *Files identical despite different names*

### Comparing `instrumented-soap-2.1.1/src/soap/tests/test_soap.py` & `instrumented_soap-2.1.2b1/src/soap/tests/test_soap.py`

 * *Files identical despite different names*

