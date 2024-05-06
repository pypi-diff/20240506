# Comparing `tmp/chyllonge-1.0.3.tar.gz` & `tmp/chyllonge-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyllonge-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "chyllonge-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `chyllonge-1.0.3.tar` & `chyllonge-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1683 2024-05-06 18:49:33.945206 chyllonge-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1356 2024-05-06 18:49:33.945206 chyllonge-1.0.3/README.md
--rw-r--r--   0        0        0     1140 2024-05-06 18:49:34.617212 chyllonge-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 18:49:33.945206 chyllonge-1.0.3/src/chyllonge/__init__.py
--rw-r--r--   0        0        0    39924 2024-05-06 18:49:33.945206 chyllonge-1.0.3/src/chyllonge/api.py
--rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 chyllonge-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1683 2024-05-06 20:04:37.449986 chyllonge-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     2253 2024-05-06 20:04:37.449986 chyllonge-1.0.4/README.md
+-rw-r--r--   0        0        0     1140 2024-05-06 20:04:37.857989 chyllonge-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 20:04:37.449986 chyllonge-1.0.4/src/chyllonge/__init__.py
+-rw-r--r--   0        0        0    40062 2024-05-06 20:04:37.449986 chyllonge-1.0.4/src/chyllonge/api.py
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 chyllonge-1.0.4/PKG-INFO
```

### Comparing `chyllonge-1.0.3/LICENSE.txt` & `chyllonge-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chyllonge-1.0.3/pyproject.toml` & `chyllonge-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "chyllonge"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = ["tzlocal>=5.2", "requests>=2.31.0"]
 requires-python = ">=3.8"
 authors = [{name = "Alex Fredrickson", email = "alex.q.fredrickson@gmail.com"}]
 maintainers = [{name = "Alex Fredrickson", email = "alex.q.fredrickson@gmail.com"}]
 description = "A Python 3.8+ implementation of the challonge.com API."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
```

### Comparing `chyllonge-1.0.3/src/chyllonge/api.py` & `chyllonge-1.0.4/src/chyllonge/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import ast
 import json
+import zoneinfo
 from datetime import datetime
 
 from typing import List
 
 import tzlocal
 import requests
 
@@ -20,40 +21,46 @@
 
 
 class ChallongeApi:
 
     def __init__(self):
         self.user = os.environ["CHALLONGE_USER"]
         self.key = os.environ["CHALLONGE_KEY"]
-        self.basic_auth_param = (self.user, self.key)
-        self.local_timezone = tzlocal.get_localzone()
-        self.now = datetime.now(tz=self.local_timezone)
-        self.now_utc_offset = self.now.strftime('%z')
-        self.local_timezone_utc_offset_string = self.now_utc_offset[0:-2] + ":" + self.now_utc_offset[-2:]
-
-        # note that the user agent string is required to get around Cloudflare issues
-        self.user_agent_param = {"User-Agent": "chyllonge"}
-
-        self.base_challonge_url = "https://api.challonge.com/v1/"
 
         if not self.user:
             raise ChallongeAPIException(
                 'ERROR: No API username was defined in the CHALLONGE_USER system environment variable.'
             )
 
-        if not self.user:
+        if not self.key:
             raise ChallongeAPIException(
                 'ERROR: No API key was defined in the CHALLONGE_KEY system environment variable.'
             )
 
-        if not self.local_timezone:
+        self.basic_auth_param = (self.user, self.key)
+
+        if "CHALLONGE_IANA_TZ_NAME" in os.environ:
+            self.timezone = zoneinfo.ZoneInfo(os.environ["CHALLONGE_IANA_TZ_NAME"])
+        else:
+            self.timezone = tzlocal.get_localzone()
+
+        if not self.timezone:
             raise ChallongeAPIException(
                 'ERROR: The local timezone could not be ascertained. This may create issues.'
             )
 
+        self.now = datetime.now(tz=self.timezone)
+        self.tz_utc_offset = self.now.strftime('%z')
+        self.tz_utc_offset_string = self.tz_utc_offset[0:-2] + ":" + self.tz_utc_offset[-2:]
+
+        # note that the user agent string is required to get around Cloudflare issues
+        self.user_agent_param = {"User-Agent": "chyllonge"}
+
+        self.base_challonge_url = "https://api.challonge.com/v1/"
+
     def get_heartbeat(self):
         """
         Invokes the most basic kind of API request.
         """
 
         response = requests.get(self.base_challonge_url, headers=self.user_agent_param, auth=self.basic_auth_param)
```

### Comparing `chyllonge-1.0.3/PKG-INFO` & `chyllonge-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyllonge
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python 3.8+ implementation of the challonge.com API.
 Keywords: challonge
 Author-email: Alex Fredrickson <alex.q.fredrickson@gmail.com>
 Maintainer-email: Alex Fredrickson <alex.q.fredrickson@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,18 @@
 ## Prerequisites
 
 `chyllonge` requires that the `CHALLONGE_KEY` and `CHALLONGE_USER` environment variables are set.
 
 * `CHALLONGE_USER` is your `challonge.com` username.
 * `CHALLONGE_KEY` is your `challonge.com` API key.  An API key can be generated [here](https://challonge.com/settings/developer).
 
+`chyllonge` also allows a `CHALLONGE_IANA_TZ_NAME` environment variable, which accepts an 
+[IANA-compliant time zone name](https://data.iana.org/time-zones/tzdb-2021a/zone1970.tab) - for 
+example: `Europe/Berlin`.
+
 ## Installation
 
 To install `chyllonge`, execute `pip install chyllonge`.
 
 ## Usage
 
 ```python
@@ -56,17 +60,39 @@
 
 `chyllonge` was inspired by `pychallonge` - developed by Russ Amos - which (in turn) includes `pychal`. 
 
 See `CONTRIBUTORS.txt` for the original authors.
 
 ## Testing
 
-To run local tests, run `python -m unittest tests.py`.
+To run local tests, run `python -m unittest tests/tests.py`.
 
 Note that the unit tests will create tournaments in your account, called `chyllonge-temp`.  It will try to delete them 
 afterward, but automated cleanup is not always guaranteed.
 
+## Contributing
+
+Please feel free to contribute, and to suggest updates to these contribution guidelines!
+
+The current guidelines are:
+
+* Functions should be documented in-line using `reStructuredText` format.
+* Support for older Python versions should be dropped as those minor updates approach end-of-life. 
+
+## Building
+
+`chyllonge` is built using [`flit`](https://flit.pypa.io/en/stable/) and [`build`](https://build.pypa.io/en/stable/).
+
+## Releases
+
+New versions of `chyllonge` are released to PyPI with the help of a GitHub Action workflow, which:
+
+1. Updates the `pyproject.toml` version
+2. Creates a GitHub release
+3. Invokes `build`, which publishes to PyPI
+
 ### Non-frequently Asked Questions
 
-Q: _How do you pronounce `chyllonge`_?
+**Q: How do you pronounce `chyllonge`?**
+
+**A:** Like "chill-ahnge".
 
-A: Like "chill-ahnge".
```

