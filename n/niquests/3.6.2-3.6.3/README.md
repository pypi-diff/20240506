# Comparing `tmp/niquests-3.6.2.tar.gz` & `tmp/niquests-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May  2 06:04:54 2024, max compression
+gzip compressed data, last modified: Mon May  6 07:01:50 2024, max compression
```

## Comparing `niquests-3.6.2.tar` & `niquests-3.6.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      718 2024-05-02 06:04:54.000000 niquests-3.6.2/AUTHORS.rst
--rw-r--r--   0        0        0    86387 2024-05-02 06:04:54.000000 niquests-3.6.2/HISTORY.md
--rw-r--r--   0        0        0      377 2024-05-02 06:04:54.000000 niquests-3.6.2/Makefile
--rw-r--r--   0        0        0       38 2024-05-02 06:04:54.000000 niquests-3.6.2/NOTICE
--rw-r--r--   0        0        0      201 2024-05-02 06:04:54.000000 niquests-3.6.2/SECURITY.md
--rw-r--r--   0        0        0      220 2024-05-02 06:04:54.000000 niquests-3.6.2/requirements-dev.txt
--rw-r--r--   0        0        0        1 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/make.bat
--rw-r--r--   0        0        0      185 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7360 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/faq.rst
--rw-r--r--   0        0        0     2720 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52818 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-05-02 06:04:54.000000 niquests-3.6.2/docs/user/quickstart.rst
--rw-r--r--   0        0        0     3071 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/__version__.py
--rw-r--r--   0        0        0    47149 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_async.py
--rw-r--r--   0        0        0     2852 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/_typing.py
--rw-r--r--   0        0        0    86853 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/auth.py
--rw-r--r--   0        0        0    19797 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5248 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/hooks.py
--rw-r--r--   0        0        0    62438 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/py.typed
--rw-r--r--   0        0        0    69113 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/status_codes.py
--rw-r--r--   0        0        0     6973 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/structures.py
--rw-r--r--   0        0        0    37300 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    22348 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    21009 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-05-02 06:04:54.000000 niquests-3.6.2/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/__init__.py
--rw-r--r--   0        0        0     2193 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_multiplexed.py
--rw-r--r--   0        0        0    99099 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_requests.py
--rw-r--r--   0        0        0     2725 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-05-02 06:04:54.000000 niquests-3.6.2/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-05-02 06:04:54.000000 niquests-3.6.2/.gitignore
--rw-r--r--   0        0        0    10142 2024-05-02 06:04:54.000000 niquests-3.6.2/LICENSE
--rw-r--r--   0        0        0    10768 2024-05-02 06:04:54.000000 niquests-3.6.2/README.md
--rw-r--r--   0        0        0     3662 2024-05-02 06:04:54.000000 niquests-3.6.2/pyproject.toml
--rw-r--r--   0        0        0    13129 2024-05-02 06:04:54.000000 niquests-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-05-06 07:01:50.000000 niquests-3.6.3/AUTHORS.rst
+-rw-r--r--   0        0        0    86599 2024-05-06 07:01:50.000000 niquests-3.6.3/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-05-06 07:01:50.000000 niquests-3.6.3/Makefile
+-rw-r--r--   0        0        0       38 2024-05-06 07:01:50.000000 niquests-3.6.3/NOTICE
+-rw-r--r--   0        0        0      201 2024-05-06 07:01:50.000000 niquests-3.6.3/SECURITY.md
+-rw-r--r--   0        0        0      233 2024-05-06 07:01:50.000000 niquests-3.6.3/requirements-dev.txt
+-rw-r--r--   0        0        0        1 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-05-06 07:01:50.000000 niquests-3.6.3/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     3071 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47120 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_async.py
+-rw-r--r--   0        0        0     2852 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/_typing.py
+-rw-r--r--   0        0        0    86896 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/auth.py
+-rw-r--r--   0        0        0    19872 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5248 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62733 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/py.typed
+-rw-r--r--   0        0        0    69084 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     6973 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/structures.py
+-rw-r--r--   0        0        0    37300 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22348 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21009 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-05-06 07:01:50.000000 niquests-3.6.3/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/conftest.py
+-rw-r--r--   0        0        0     7540 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_hooks.py
+-rw-r--r--   0        0        0     4022 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_multiplexed.py
+-rw-r--r--   0        0        0    99906 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_requests.py
+-rw-r--r--   0        0        0     2725 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-05-06 07:01:50.000000 niquests-3.6.3/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-05-06 07:01:50.000000 niquests-3.6.3/.gitignore
+-rw-r--r--   0        0        0    10142 2024-05-06 07:01:50.000000 niquests-3.6.3/LICENSE
+-rw-r--r--   0        0        0    10884 2024-05-06 07:01:50.000000 niquests-3.6.3/README.md
+-rw-r--r--   0        0        0     3662 2024-05-06 07:01:50.000000 niquests-3.6.3/pyproject.toml
+-rw-r--r--   0        0        0    13245 2024-05-06 07:01:50.000000 niquests-3.6.3/PKG-INFO
```

### Comparing `niquests-3.6.2/AUTHORS.rst` & `niquests-3.6.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/HISTORY.md` & `niquests-3.6.3/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Release History
 ===============
 
+3.6.3 (2024-05-06)
+------------------
+
+**Fixed**
+- Fixed encoding data with None values and other objects. This was a regression introduced in our v3. #119
+
+**Changed**
+- Various minor performance improvements.
+
 3.6.2 (2024-05-02)
 ------------------
 
 **Fixed**
 - "Help" program `python -m niquests.help` that depended on h2 while not required anymore.
 - Minor performance regression in async while checking OCSP when certificate isn't eligible (e.g. no OCSP url provided).
```

### Comparing `niquests-3.6.2/docs/Makefile` & `niquests-3.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/api.rst` & `niquests-3.6.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/conf.py` & `niquests-3.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/index.rst` & `niquests-3.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/make.bat` & `niquests-3.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/_static/custom.css` & `niquests-3.6.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/_static/requests-sidebar.png` & `niquests-3.6.3/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/community/faq.rst` & `niquests-3.6.3/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/community/recommended.rst` & `niquests-3.6.3/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/community/release-process.rst` & `niquests-3.6.3/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/community/vulnerabilities.rst` & `niquests-3.6.3/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/dev/contributing.rst` & `niquests-3.6.3/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/dev/migrate.rst` & `niquests-3.6.3/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/user/advanced.rst` & `niquests-3.6.3/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/user/authentication.rst` & `niquests-3.6.3/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/user/install.rst` & `niquests-3.6.3/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/docs/user/quickstart.rst` & `niquests-3.6.3/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/__init__.py` & `niquests-3.6.3/src/niquests/__init__.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/__version__.py` & `niquests-3.6.3/src/niquests/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.6.2"
+__version__ = "3.6.3"
 
-__build__: int = 0x030602
+__build__: int = 0x030603
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.6.2/src/niquests/_async.py` & `niquests-3.6.3/src/niquests/_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,25 +436,28 @@
 
             r._resolve_redirect = _redirect_method_ref
 
             # in multiplexed mode, we are unable to forward this local function for safety reasons.
             kwargs["on_post_connection"] = None
 
             # we intentionally set 'niquests' as the prefix. urllib3.future have its own parameters.
-            r._promise.set_parameter("niquests_is_stream", stream)
-            r._promise.set_parameter("niquests_start", start)
-            r._promise.set_parameter("niquests_hooks", hooks)
-            r._promise.set_parameter("niquests_cookies", self.cookies)
-            r._promise.set_parameter("niquests_allow_redirect", allow_redirects)
-            r._promise.set_parameter("niquests_kwargs", kwargs)
-
-            # You may be wondering why we are setting redirect info in promise ctx.
-            # because in multiplexed mode, we are not fully aware of hop/redirect count
-            r._promise.set_parameter("niquests_redirect_count", 0)
-            r._promise.set_parameter("niquests_max_redirects", self.max_redirects)
+            r._promise.update_parameters(
+                {
+                    "niquests_is_stream": stream,
+                    "niquests_start": start,
+                    "niquests_hooks": hooks,
+                    "niquests_cookies": self.cookies,
+                    "niquests_allow_redirect": allow_redirects,
+                    "niquests_kwargs": kwargs,
+                    # You may be wondering why we are setting redirect info in promise ctx.
+                    # because in multiplexed mode, we are not fully aware of hop/redirect count
+                    "niquests_redirect_count": 0,
+                    "niquests_max_redirects": self.max_redirects,
+                }
+            )
 
             if not stream:
                 _swap_context(r)
 
             return r
 
         # Total elapsed time of the request (approximately)
```

### Comparing `niquests-3.6.2/src/niquests/_compat.py` & `niquests-3.6.3/src/niquests/_compat.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/_typing.py` & `niquests-3.6.3/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/adapters.py` & `niquests-3.6.3/src/niquests/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -964,34 +964,26 @@
                 raise
 
         return self.build_response(request, resp_or_promise)
 
     def _future_handler(
         self, response: Response, low_resp: BaseHTTPResponse
     ) -> Response | None:
-        stream = typing.cast(
-            bool, response._promise.get_parameter("niquests_is_stream")
-        )
-        start = typing.cast(float, response._promise.get_parameter("niquests_start"))
-        hooks = typing.cast(HookType, response._promise.get_parameter("niquests_hooks"))
-        session_cookies = typing.cast(
-            CookieJar, response._promise.get_parameter("niquests_cookies")
-        )
-        allow_redirects = typing.cast(
-            bool, response._promise.get_parameter("niquests_allow_redirect")
-        )
-        max_redirect = typing.cast(
-            int, response._promise.get_parameter("niquests_max_redirects")
-        )
-        redirect_count = typing.cast(
-            int, response._promise.get_parameter("niquests_redirect_count")
-        )
-        kwargs = typing.cast(
-            typing.MutableMapping[str, typing.Any],
-            response._promise.get_parameter("niquests_kwargs"),
+        stream: bool = response._promise.get_parameter("niquests_is_stream")  # type: ignore[assignment]
+        start: float = response._promise.get_parameter("niquests_start")  # type: ignore[assignment]
+
+        hooks: HookType = response._promise.get_parameter("niquests_hooks")  # type: ignore[assignment]
+        session_cookies: CookieJar = response._promise.get_parameter("niquests_cookies")  # type: ignore[assignment]
+        allow_redirects: bool = response._promise.get_parameter(  # type: ignore[assignment]
+            "niquests_allow_redirect"
+        )
+        max_redirect: int = response._promise.get_parameter("niquests_max_redirects")  # type: ignore[assignment]
+        redirect_count: int = response._promise.get_parameter("niquests_redirect_count")  # type: ignore[assignment]
+        kwargs: typing.MutableMapping[str, typing.Any] = (
+            response._promise.get_parameter("niquests_kwargs")  # type: ignore[assignment]
         )
 
         # This mark the response as no longer "lazy"
         response.raw = low_resp
         response_promise = response._promise
         del response._promise
 
@@ -1947,34 +1939,25 @@
         self, response: AsyncResponse | Response, low_resp: BaseAsyncHTTPResponse
     ) -> AsyncResponse | None:
         if not isinstance(response, AsyncResponse):
             _swap_context(response)
 
         assert isinstance(response, AsyncResponse)
 
-        stream = typing.cast(
-            bool, response._promise.get_parameter("niquests_is_stream")
-        )
-        start = typing.cast(float, response._promise.get_parameter("niquests_start"))
-        hooks = typing.cast(HookType, response._promise.get_parameter("niquests_hooks"))
-        session_cookies = typing.cast(
-            CookieJar, response._promise.get_parameter("niquests_cookies")
-        )
-        allow_redirects = typing.cast(
-            bool, response._promise.get_parameter("niquests_allow_redirect")
-        )
-        max_redirect = typing.cast(
-            int, response._promise.get_parameter("niquests_max_redirects")
-        )
-        redirect_count = typing.cast(
-            int, response._promise.get_parameter("niquests_redirect_count")
-        )
-        kwargs = typing.cast(
-            typing.MutableMapping[str, typing.Any],
-            response._promise.get_parameter("niquests_kwargs"),
+        stream: bool = response._promise.get_parameter("niquests_is_stream")  # type: ignore[assignment]
+        start: float = response._promise.get_parameter("niquests_start")  # type: ignore[assignment]
+        hooks: HookType = response._promise.get_parameter("niquests_hooks")  # type: ignore[assignment]
+        session_cookies: CookieJar = response._promise.get_parameter("niquests_cookies")  # type: ignore[assignment]
+        allow_redirects: bool = response._promise.get_parameter(  # type: ignore[assignment]
+            "niquests_allow_redirect"
+        )
+        max_redirect: int = response._promise.get_parameter("niquests_max_redirects")  # type: ignore[assignment]
+        redirect_count: int = response._promise.get_parameter("niquests_redirect_count")  # type: ignore[assignment]
+        kwargs: typing.MutableMapping[str, typing.Any] = (
+            response._promise.get_parameter("niquests_kwargs")  # type: ignore[assignment]
         )
 
         # This mark the response as no longer "lazy"
         response.raw = low_resp
         response_promise = response._promise
         del response._promise
```

### Comparing `niquests-3.6.2/src/niquests/api.py` & `niquests-3.6.3/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/auth.py` & `niquests-3.6.3/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/cookies.py` & `niquests-3.6.3/src/niquests/cookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     if request is None or response is None:
         raise ValueError(
             "Attempt to extract cookie from undefined request and/or response"
         )
 
     if not (hasattr(response, "_original_response") and response._original_response):
         return
+    if "Set-Cookie" not in response._original_response.msg:
+        return
     # the _original_response field is the wrapped httplib.HTTPResponse object,
     req = MockRequest(request)
     # pull out the HTTPMessage with the headers and put it in the mock:
     res = MockResponse(response._original_response.msg)  # type: ignore[attr-defined]
     jar.extract_cookies(res, req)  # type: ignore[arg-type]
```

### Comparing `niquests-3.6.2/src/niquests/exceptions.py` & `niquests-3.6.3/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/help.py` & `niquests-3.6.3/src/niquests/help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/hooks.py` & `niquests-3.6.3/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/models.py` & `niquests-3.6.3/src/niquests/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,17 +738,26 @@
             return data
         elif hasattr(data, "read"):
             return data.read()
         elif hasattr(data, "__iter__"):
             result = []
             for k, vs in to_key_val_list(data):
                 iterable_vs: typing.Iterable[str | bytes]
-                if isinstance(vs, (str, bytes, int, float, bool)):
-                    # not officially supported, but some people maybe passing ints, float or bool.
-                    if isinstance(vs, (str, bytes)) is False:
+                if isinstance(vs, (str, bytes, int, float, bool)) or not hasattr(
+                    vs, "__iter__"
+                ):
+                    # not officially supported, but some people maybe passing ints, float, bool,
+                    # or other string serializable classes.
+                    if vs is not None and not isinstance(
+                        vs,
+                        (
+                            str,
+                            bytes,
+                        ),
+                    ):
                         iterable_vs = [str(vs)]
                     else:
                         iterable_vs = [vs]
                 else:
                     iterable_vs = vs
                 for v in iterable_vs:
                     if v is not None:
```

### Comparing `niquests-3.6.2/src/niquests/sessions.py` & `niquests-3.6.3/src/niquests/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1194,25 +1194,28 @@
                 None,
             )
 
             # in multiplexed mode, we are unable to forward this local function for safety reasons.
             kwargs["on_post_connection"] = None
 
             # we intentionally set 'niquests' as the prefix. urllib3.future have its own parameters.
-            r._promise.set_parameter("niquests_is_stream", stream)
-            r._promise.set_parameter("niquests_start", start)
-            r._promise.set_parameter("niquests_hooks", hooks)
-            r._promise.set_parameter("niquests_cookies", self.cookies)
-            r._promise.set_parameter("niquests_allow_redirect", allow_redirects)
-            r._promise.set_parameter("niquests_kwargs", kwargs)
-
-            # You may be wondering why we are setting redirect info in promise ctx.
-            # because in multiplexed mode, we are not fully aware of hop/redirect count
-            r._promise.set_parameter("niquests_redirect_count", 0)
-            r._promise.set_parameter("niquests_max_redirects", self.max_redirects)
+            r._promise.update_parameters(
+                {
+                    "niquests_is_stream": stream,
+                    "niquests_start": start,
+                    "niquests_hooks": hooks,
+                    "niquests_cookies": self.cookies,
+                    "niquests_allow_redirect": allow_redirects,
+                    "niquests_kwargs": kwargs,
+                    # You may be wondering why we are setting redirect info in promise ctx.
+                    # because in multiplexed mode, we are not fully aware of hop/redirect count
+                    "niquests_redirect_count": 0,
+                    "niquests_max_redirects": self.max_redirects,
+                }
+            )
 
             return r
 
         # Total elapsed time of the request (approximately)
         elapsed = preferred_clock() - start
         r.elapsed = timedelta(seconds=elapsed)
```

### Comparing `niquests-3.6.2/src/niquests/status_codes.py` & `niquests-3.6.3/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/structures.py` & `niquests-3.6.3/src/niquests/structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/utils.py` & `niquests-3.6.3/src/niquests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.3/src/niquests/extensions/_async_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/extensions/_ocsp.py` & `niquests-3.6.3/src/niquests/extensions/_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/src/niquests/extensions/_picotls.py` & `niquests-3.6.3/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/conftest.py` & `niquests-3.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_async.py` & `niquests-3.6.3/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_help.py` & `niquests-3.6.3/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_hooks.py` & `niquests-3.6.3/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_live.py` & `niquests-3.6.3/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_lowlevel.py` & `niquests-3.6.3/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_multiplexed.py` & `niquests-3.6.3/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_requests.py` & `niquests-3.6.3/tests/test_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2536,14 +2536,48 @@
     # urllib3 expects bodies as bytes-like objects
     body = {"key": "value"}
     p = PreparedRequest()
     p.prepare(method="GET", url="https://www.example.com/", json=body)
     assert isinstance(p.body, bytes)
 
 
+def test_data_encodes_noniterables(httpbin):
+    class Class:
+        pass
+
+    class ClassStringable:
+        def __str__(self):
+            return "🔥arbClassStringable🔥"
+
+    ClassObj = Class()
+
+    body = {
+        "string": "string",
+        "bytes": b"string",
+        "float": 0.01,
+        "int": 100,
+        "bool": True,
+        "None": None,
+        "plain_class": ClassObj,
+        "stringable_class": ClassStringable(),
+    }
+
+    expected_response = {
+        "bool": "True",
+        "float": "0.01",
+        "int": "100",
+        "plain_class": str(ClassObj),
+        "string": "string",
+        "bytes": "string",
+        "stringable_class": "🔥arbClassStringable🔥",
+    }
+    resp = niquests.post(httpbin("post"), data=body)
+    assert resp.json()["form"] == expected_response
+
+
 def test_requests_are_updated_each_time(httpbin):
     session = RedirectSession([303, 307])
     prep = niquests.Request("POST", httpbin("post")).prepare()
     r0 = session.send(prep)
     assert r0.request.method == "POST"
     assert session.calls[-1] == SendCall((r0.request,), {})
     redirect_generator = session.resolve_redirects(r0, prep)
```

### Comparing `niquests-3.6.2/tests/test_structures.py` & `niquests-3.6.3/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_testserver.py` & `niquests-3.6.3/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/test_utils.py` & `niquests-3.6.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/utils.py` & `niquests-3.6.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/tests/testserver/server.py` & `niquests-3.6.3/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/LICENSE` & `niquests-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/README.md` & `niquests-3.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 _Scenario:_ Fetch a thousand requests using 10 tasks or threads, each with a hundred requests using a single pool of connection.
 
 **High-Level APIs**
 
 | Client   | Average Delay to Complete | Notes                        |
 |----------|---------------------------|------------------------------|
 | requests | 987 ms                    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx    | 735 ms                    | Asyncio. HTTP/2              |
-| niquests | 400 ms                    | Asyncio. HTTP/2              |
+| httpx    | 720 ms                    | Asyncio. HTTP/2              |
+| niquests | 390 ms                    | Asyncio. HTTP/2              |
 
 **Simplified APIs**
 
 | Client        | Average Delay to Complete | Notes                        |
 |---------------|---------------------------|------------------------------|
 | requests core | 643 ms                    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx core    | 550 ms                    | Asyncio. HTTP/2              |
-| aiohttp       | 220 ms                    | Asyncio. HTTP/1.1            |
+| httpx core    | 530 ms                    | Asyncio. HTTP/2              |
+| aiohttp       | 210 ms                    | Asyncio. HTTP/1.1            |
 | niquests core | 190 ms                    | Asyncio. HTTP/2              |
 
-Did you give up on HTTP/2 due to performance concerns? Think again! Multiplexing and response lazyness open up a wide range
-of possibilities! Want to learn more about the tests? scripts? reasoning?
+Did you give up on HTTP/2 due to performance concerns? Think again! Do you realize that you can get 2.53 times faster with the same CPU if you ever switched to Niquests from Requests?
+Multiplexing and response lazyness open up a wide range of possibilities! Want to learn more about the tests? scripts? reasoning?
 
 Take a deeper look at https://github.com/Ousret/niquests-stats
 
 ⚠️ Do the responsible thing with this library and do not attempt DoS remote servers using its abilities.
 </details>
 
 ```python
```

### Comparing `niquests-3.6.2/pyproject.toml` & `niquests-3.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `niquests-3.6.2/PKG-INFO` & `niquests-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.6.2
+Version: 3.6.3
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -96,28 +96,28 @@
 _Scenario:_ Fetch a thousand requests using 10 tasks or threads, each with a hundred requests using a single pool of connection.
 
 **High-Level APIs**
 
 | Client   | Average Delay to Complete | Notes                        |
 |----------|---------------------------|------------------------------|
 | requests | 987 ms                    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx    | 735 ms                    | Asyncio. HTTP/2              |
-| niquests | 400 ms                    | Asyncio. HTTP/2              |
+| httpx    | 720 ms                    | Asyncio. HTTP/2              |
+| niquests | 390 ms                    | Asyncio. HTTP/2              |
 
 **Simplified APIs**
 
 | Client        | Average Delay to Complete | Notes                        |
 |---------------|---------------------------|------------------------------|
 | requests core | 643 ms                    | ThreadPoolExecutor. HTTP/1.1 |
-| httpx core    | 550 ms                    | Asyncio. HTTP/2              |
-| aiohttp       | 220 ms                    | Asyncio. HTTP/1.1            |
+| httpx core    | 530 ms                    | Asyncio. HTTP/2              |
+| aiohttp       | 210 ms                    | Asyncio. HTTP/1.1            |
 | niquests core | 190 ms                    | Asyncio. HTTP/2              |
 
-Did you give up on HTTP/2 due to performance concerns? Think again! Multiplexing and response lazyness open up a wide range
-of possibilities! Want to learn more about the tests? scripts? reasoning?
+Did you give up on HTTP/2 due to performance concerns? Think again! Do you realize that you can get 2.53 times faster with the same CPU if you ever switched to Niquests from Requests?
+Multiplexing and response lazyness open up a wide range of possibilities! Want to learn more about the tests? scripts? reasoning?
 
 Take a deeper look at https://github.com/Ousret/niquests-stats
 
 ⚠️ Do the responsible thing with this library and do not attempt DoS remote servers using its abilities.
 </details>
 
 ```python
```

