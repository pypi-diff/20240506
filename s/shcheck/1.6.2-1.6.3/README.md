# Comparing `tmp/shcheck-1.6.2.tar.gz` & `tmp/shcheck-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shcheck-1.6.2.tar", last modified: Sun May  5 10:55:25 2024, max compression
+gzip compressed data, was "shcheck-1.6.3.tar", last modified: Mon May  6 13:08:27 2024, max compression
```

## Comparing `shcheck-1.6.2.tar` & `shcheck-1.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:55:25.605190 shcheck-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-05 10:55:21.000000 shcheck-1.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-05 10:55:25.605190 shcheck-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-05 10:55:21.000000 shcheck-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:55:25.605190 shcheck-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-05 10:55:21.000000 shcheck-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:55:25.605190 shcheck-1.6.2/shcheck/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:55:21.000000 shcheck-1.6.2/shcheck/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16290 2024-05-05 10:55:21.000000 shcheck-1.6.2/shcheck/shcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:55:25.605190 shcheck-1.6.2/shcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-05 10:55:25.000000 shcheck-1.6.2/shcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-05 10:55:25.000000 shcheck-1.6.2/shcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:55:25.000000 shcheck-1.6.2/shcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 10:55:25.000000 shcheck-1.6.2/shcheck.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      818 2024-05-05 10:55:21.000000 shcheck-1.6.2/shcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:55:25.605190 shcheck-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 10:55:21.000000 shcheck-1.6.2/tests/test_shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:08:27.724183 shcheck-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-06 13:08:23.000000 shcheck-1.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-06 13:08:27.724183 shcheck-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 13:08:23.000000 shcheck-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:08:27.724183 shcheck-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-06 13:08:23.000000 shcheck-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:08:27.720183 shcheck-1.6.3/shcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:08:23.000000 shcheck-1.6.3/shcheck/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16352 2024-05-06 13:08:23.000000 shcheck-1.6.3/shcheck/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:08:27.724183 shcheck-1.6.3/shcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-06 13:08:27.000000 shcheck-1.6.3/shcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 13:08:27.000000 shcheck-1.6.3/shcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:08:27.000000 shcheck-1.6.3/shcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 13:08:27.000000 shcheck-1.6.3/shcheck.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      818 2024-05-06 13:08:23.000000 shcheck-1.6.3/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:08:27.724183 shcheck-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 13:08:23.000000 shcheck-1.6.3/tests/test_shcheck.py
```

### Comparing `shcheck-1.6.2/LICENSE.txt` & `shcheck-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shcheck-1.6.2/PKG-INFO` & `shcheck-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.6.2
+Version: 1.6.3
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.6.2 Summary: A basic tool to
+Metadata-Version: 2.1 Name: shcheck Version: 1.6.3 Summary: A basic tool to
 check security headers of a website Home-page: https://github.com/santoru/
 shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
 Security Header Check
                    _[_P_y_P_I_]_[_P_y_p_i_]_[_U_p_d_a_t_e_d_][Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
```

### Comparing `shcheck-1.6.2/README.md` & `shcheck-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `shcheck-1.6.2/setup.py` & `shcheck-1.6.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
 PACKAGE_NAME = "shcheck"
-VERSION = "1.6.2"
+VERSION = "1.6.3"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def parse_requirements(filename):
     """Load requirements from a pip requirements file."""
```

### Comparing `shcheck-1.6.2/shcheck/shcheck.py` & `shcheck-1.6.3/shcheck/shcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         log("[*] Effective URL: {}".format(colorize(rUrl, 'info')))
         parse_headers(response.getheaders())
         json_headers[f"{rUrl}"] = json_results
         json_results["present"] = {}
         json_results["missing"] = []
 
         # Before parsing, remove X-Frame-Options if there's CSP with frame-ancestors directive
-        if "frame-ancestors" in headers.get('Content-Security-Policy'.lower()).lower():
+        if "Content-Security-Policy".lower() in str(headers).lower() and "frame-ancestors" in headers.get('Content-Security-Policy'.lower()).lower():
             sec_headers.pop("X-Frame-Options")
             headers.pop("X-Frame-Options".lower())
 
         for safeh in sec_headers:
             lsafeh = safeh.lower()
             if lsafeh in headers:
                 safe += 1
```

### Comparing `shcheck-1.6.2/shcheck.egg-info/PKG-INFO` & `shcheck-1.6.3/shcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.6.2
+Version: 1.6.3
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.6.2 Summary: A basic tool to
+Metadata-Version: 2.1 Name: shcheck Version: 1.6.3 Summary: A basic tool to
 check security headers of a website Home-page: https://github.com/santoru/
 shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
 Security Header Check
                    _[_P_y_P_I_]_[_P_y_p_i_]_[_U_p_d_a_t_e_d_][Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
```

### Comparing `shcheck-1.6.2/shcheck.py` & `shcheck-1.6.3/shcheck.py`

 * *Files identical despite different names*

