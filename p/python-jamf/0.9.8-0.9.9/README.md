# Comparing `tmp/python-jamf-0.9.8.tar.gz` & `tmp/python-jamf-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-jamf-0.9.8.tar", last modified: Mon Mar 25 20:55:34 2024, max compression
+gzip compressed data, was "python-jamf-0.9.9.tar", last modified: Mon May  6 21:14:56 2024, max compression
```

## Comparing `python-jamf-0.9.8.tar` & `python-jamf-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:55:34.644317 python-jamf-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-25 20:55:27.000000 python-jamf-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 20:55:27.000000 python-jamf-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-03-25 20:55:34.644317 python-jamf-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-03-25 20:55:27.000000 python-jamf-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:55:34.640317 python-jamf-0.9.8/python_jamf/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3205 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30052 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/package.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    74590 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4501 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/setconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-25 20:55:27.000000 python-jamf-0.9.8/python_jamf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:55:34.644317 python-jamf-0.9.8/python_jamf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 20:55:34.000000 python-jamf-0.9.8/python_jamf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 20:55:34.644317 python-jamf-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-25 20:55:27.000000 python-jamf-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 20:55:34.644317 python-jamf-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 20:55:27.000000 python-jamf-0.9.8/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-03-25 20:55:27.000000 python-jamf-0.9.8/tests/api_test_old.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5681 2024-03-25 20:55:27.000000 python-jamf-0.9.8/tests/config_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19267 2024-03-25 20:55:27.000000 python-jamf-0.9.8/tests/convert_json_xml_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5705 2024-03-25 20:55:27.000000 python-jamf-0.9.8/tests/test_records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:14:56.651532 python-jamf-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-06 21:14:49.000000 python-jamf-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 21:14:49.000000 python-jamf-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-06 21:14:56.651532 python-jamf-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-06 21:14:49.000000 python-jamf-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:14:56.647532 python-jamf-0.9.9/python_jamf/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3205 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30052 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/package.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74547 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5826 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/setconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 21:14:49.000000 python-jamf-0.9.9/python_jamf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:14:56.651532 python-jamf-0.9.9/python_jamf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 21:14:56.000000 python-jamf-0.9.9/python_jamf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:14:56.651532 python-jamf-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-06 21:14:49.000000 python-jamf-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:14:56.651532 python-jamf-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 21:14:49.000000 python-jamf-0.9.9/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-06 21:14:49.000000 python-jamf-0.9.9/tests/api_test_old.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5681 2024-05-06 21:14:49.000000 python-jamf-0.9.9/tests/config_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19267 2024-05-06 21:14:49.000000 python-jamf-0.9.9/tests/convert_json_xml_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5673 2024-05-06 21:14:49.000000 python-jamf-0.9.9/tests/test_records.py
```

### Comparing `python-jamf-0.9.8/LICENSE` & `python-jamf-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/PKG-INFO` & `python-jamf-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jamf
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python wrapper for Jamf Pro API
 Home-page: https://github.com/univ-of-utah-marriott-library-apple/python-jamf
 Author: The University of Utah
 Author-email: mlib-its-mac@lists.utah.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -137,44 +137,14 @@
 <img src="https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/images/MacAdmins_Slack_logo.png" alt="MacAdmin's Slack Logo">
 </p>
 
 ## Latest Status
 
 ### Releases
 
-#### :new: [python-jamf - 0.8.2](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.8.2)
-
-- Much better error reporting when there's a connection failure to the server
-- Checks for "http://" or "https://" when setting a hostname and when connecting to a server
-- Added `conf-python-jamf -r` to remove the bearer token saved in the keychain
-- Unified server connection code
-- Replaced all `exit(1)` with `raise SystemExit`
-- pre-commit updated to 4.3.0
-- GitHub action updated action names
-- Updated README
-
-#### [python-jamf - 0.8.1](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.8.1)
-
-- This release includes the xml array fix described [here](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/blob/07378f0397744f52af54dbadb798e057d5e0c6cf/README.md#known-breaking-changes-on-the-roadmap).
-
-#### [python-jamf - 0.7.5](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.7.5)
-
-- Fixed trigger_logout removal from policies triggers
-- Fixed bearer token bug
-- Lots of automated reformatting and cleaning up
-- Adds pre-commit
-
-Thank you homebysix for your contributions.
-
-#### [python-jamf - 0.7.4](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.7.4-af4107c6)
-
- - Bearer token support
- - Fixed bug when creating records (shallow vs deep copy)
- - Fixed version in setup.py bug
- - Removed jamfnet from main docker-compose and move it to it's own file
- - Support smb mounting on linux
+Please see the [Changelog](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/blob/main/CHANGELOG.md) for all release notes.
 
 Thank you yairf-s1 and pythoninthegrass for your contributions.
 
 See `python-jamf` [upgrade](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/Installing#upgrading) documentation to upgrade to latest release.
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `python-jamf-0.9.8/README.md` & `python-jamf-0.9.9/python_jamf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: python-jamf
+Version: 0.9.9
+Summary: Python wrapper for Jamf Pro API
+Home-page: https://github.com/univ-of-utah-marriott-library-apple/python-jamf
+Author: The University of Utah
+Author-email: mlib-its-mac@lists.utah.edu
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # python-jamf
 _Programmatic Automation, Access & Control of Jamf Pro_
 
 ![python_jamf_logo](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/images/python_jamf_logo.png)
 
 ## Introduction
 
@@ -121,44 +137,14 @@
 <img src="https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/images/MacAdmins_Slack_logo.png" alt="MacAdmin's Slack Logo">
 </p>
 
 ## Latest Status
 
 ### Releases
 
-#### :new: [python-jamf - 0.8.2](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.8.2)
-
-- Much better error reporting when there's a connection failure to the server
-- Checks for "http://" or "https://" when setting a hostname and when connecting to a server
-- Added `conf-python-jamf -r` to remove the bearer token saved in the keychain
-- Unified server connection code
-- Replaced all `exit(1)` with `raise SystemExit`
-- pre-commit updated to 4.3.0
-- GitHub action updated action names
-- Updated README
-
-#### [python-jamf - 0.8.1](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.8.1)
-
-- This release includes the xml array fix described [here](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/blob/07378f0397744f52af54dbadb798e057d5e0c6cf/README.md#known-breaking-changes-on-the-roadmap).
-
-#### [python-jamf - 0.7.5](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.7.5)
-
-- Fixed trigger_logout removal from policies triggers
-- Fixed bearer token bug
-- Lots of automated reformatting and cleaning up
-- Adds pre-commit
-
-Thank you homebysix for your contributions.
-
-#### [python-jamf - 0.7.4](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.7.4-af4107c6)
-
- - Bearer token support
- - Fixed bug when creating records (shallow vs deep copy)
- - Fixed version in setup.py bug
- - Removed jamfnet from main docker-compose and move it to it's own file
- - Support smb mounting on linux
+Please see the [Changelog](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/blob/main/CHANGELOG.md) for all release notes.
 
 Thank you yairf-s1 and pythoninthegrass for your contributions.
 
 See `python-jamf` [upgrade](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/Installing#upgrading) documentation to upgrade to latest release.
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `python-jamf-0.9.8/python_jamf/api.py` & `python-jamf-0.9.9/python_jamf/api.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/python_jamf/config.py` & `python-jamf-0.9.9/python_jamf/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,32 +34,42 @@
 class Config:
     def __init__(
         self,
         config_path=None,
         hostname=None,
         username=None,
         password=None,
+        client=None,
         prompt=False,
     ):
         self.log = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
         self.prompt = prompt
         self.hostname = hostname
         self.username = username
         self.password = password
+        self.client = client
         self.config_path = resolve_config_path(config_path)
         if not self.hostname and not self.username and not self.password:
             self.load()
         # Prompt for any missing prefs
         if not self.hostname:
             if self.prompt:
                 self.hostname = prompt_hostname()
             else:
                 raise JamfConfigError(
                     "Config failed to obtain a hostname and prompt is off."
                 )
+        if self.client is None:
+            if self.prompt:
+                self.client = prompt_userauth()
+            else:
+                stderr.write(
+                    "No pref for API Client Auth and prompt is off. Using username and password auth.\n"
+                )
+                self.client = False
         if not self.username:
             if self.prompt:
                 self.username = input("Username: ")
             else:
                 raise JamfConfigError(
                     "Config failed to obtain a username and prompt is off."
                 )
@@ -95,33 +105,44 @@
 To improve security with storing credentials used with the jctl tool, we have
 deprecated the use of a property list file for storing configuration
 information and have migrated to use the Python keyring library provides an
 easy way to access the system keyring service from python. It can be used with
 the macOS Keychain and Linux KWallet.
 
 Please delete the the configuration at {self.config_path} and recreate it using
-the "./jamf/setconfig.py" script.
+the "conf-python-jamf" script.
 """
                     raise JamfConfigError(cmessage)
                 self.hostname = prefs["JSSHostname"]
                 self.username = prefs["Username"]
+                if "APIClientAuth" in prefs:
+                    self.client = prefs["APIClientAuth"]
+                else:
+                    stderr.write(
+                        "No pref for API Client Auth. Please recreate your prefs to add it.\n"
+                    )
+                    self.client = False
                 self.password = keyring.get_password(self.hostname, self.username)
             elif "JSS_URL" in prefs:
                 self.hostname = prefs["JSS_URL"]
                 self.username = prefs["API_USERNAME"]
                 self.password = prefs["API_PASSWORD"]
             elif "jss_url" in prefs:
                 self.hostname = prefs["jss_url"]
                 # No auth in that file
         else:
             raise JamfConfigError(f"Config file does not exist: {self.config_path}")
 
     def save(self):
         keyring.set_password(self.hostname, self.username, self.password)
-        data = {"JSSHostname": self.hostname, "Username": self.username}
+        data = {
+            "JSSHostname": self.hostname,
+            "Username": self.username,
+            "APIClientAuth": self.client,
+        }
         self.log.info(f"saving: {self.config_path}")
         fptr = open(self.config_path, "wb")
         plistlib.dump(data, fptr)
         fptr.close()
 
     def load_token(self):
         self.token = keyring.get_password(self.hostname, TOKEN_KEY)
@@ -191,7 +212,17 @@
     while not valid:
         hostname = input("Hostname (don't forget https:// and :8443): ")
         if hostname.startswith("https://") or hostname.startswith("http://"):
             valid = True
     while hostname[-1] == "/":
         hostname = hostname[:-1]
     return hostname
+
+
+def prompt_userauth():
+    valid = False
+    while not valid:
+        client = input("User Auth [0] or API Client Auth [1]: ")
+        if client == "0" or client == "no" or client == "false":
+            return False
+        if client == "1" or client == "yes" or client == "true":
+            return True
```

### Comparing `python-jamf-0.9.8/python_jamf/convert.py` & `python-jamf-0.9.9/python_jamf/convert.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/python_jamf/exceptions.py` & `python-jamf-0.9.9/python_jamf/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/python_jamf/package.py` & `python-jamf-0.9.9/python_jamf/package.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/python_jamf/records.py` & `python-jamf-0.9.9/python_jamf/records.py`

 * *Files 0% similar despite different names*

```diff
@@ -1937,18 +1937,17 @@
     singular_string = "script"
     refresh_method = "get_script"
     delete_method = "delete_script"
     update_method = "update_script"
 
     def script_contents_print_during(self):
         try:
-            printme = self.get_path("script_contents")
-            print(printme[0])
+            print(self.get_path("script_contents"))
         except JamfRecordNotFound:
-            printme = None
+            pass
 
 
 class Scripts(Records, metaclass=Singleton):
     # http://localhost/view/settings/computer/scripts
     singular_class = Script
     plural_string = "scripts"
     refresh_method = "get_scripts"
```

### Comparing `python-jamf-0.9.8/python_jamf/server.py` & `python-jamf-0.9.9/python_jamf/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,39 +16,45 @@
     def __init__(
         self,
         config_obj=None,
         config_path=None,
         hostname=None,
         username=None,
         password=None,
+        client=None,
         prompt=False,
         debug=False,
     ):
         """ """
         self.config = config_obj or config.Config(
             config_path=config_path,
             hostname=hostname,
             username=username,
             password=password,
+            client=client,
             prompt=prompt,
         )
         if (
             not self.config.hostname
             and not self.config.username
             and not self.config.password
+            and not self.config.client
         ):
             raise exceptions.JamfConfigError(
                 "No jamf hostname or credentials could be found."
             )
         self.classic = None
         self.debug = debug
         self.records = records
         try:
             self.classic = Classic(
-                self.config.hostname, self.config.username, self.config.password
+                self.config.hostname,
+                self.config.username,
+                self.config.password,
+                client=self.config.client,
             )
         except AuthResponseConnectionError:
             print("Could not connect to " + self.config.hostname)
             exit()
         except JamfAuthException:
             print("Incorrect username or password for " + self.config.hostname)
             exit()
```

### Comparing `python-jamf-0.9.8/python_jamf/setconfig.py` & `python-jamf-0.9.9/python_jamf/setconfig.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,104 +26,139 @@
         myplatform = platform.system()
         if myplatform == "Darwin":
             default_pref = python_jamf.config.MACOS_PREFS_TILDA
         elif myplatform == "Linux":
             default_pref = python_jamf.config.LINUX_PREFS_TILDA
         self.parser = argparse.ArgumentParser()
         self.parser.add_argument(
-            "-H", "--hostname", help="specify hostname (default: prompt)"
+            "-H", "--hostname", help="Specify hostname (default: prompt)"
         )
         self.parser.add_argument(
-            "-u", "--user", help="specify username (default: prompt)"
+            "-u", "--user", help="Specify username/Client ID (default: prompt)"
         )
         self.parser.add_argument(
-            "-p", "--passwd", help="specify password (default: prompt)"
+            "-p", "--passwd", help="Specify password/Client secret (default: prompt)"
         )
         self.parser.add_argument(
             "-r", "--revoke-token", action="store_true", help="Revoke Bearer token"
         )
         self.parser.add_argument(
+            "-c",
+            "--client",
+            help="Use API Client Auth instead of user auth (yes|true|1 or no|false|0, default is ask)",
+        )
+        self.parser.add_argument(
             "-C",
             "--config",
             dest="path",
             metavar="PATH",
             default=default_pref,
-            help=f"specify config file (default {default_pref})",
+            help=f"Specify config file (default {default_pref})",
         )
         self.parser.add_argument(
             "-P",
             "--print",
             action="store_true",
-            help="print existing config profile (except password!)",
+            help="Print existing config profile (except password/client secret!)",
         )
         self.parser.add_argument(
             "-t",
             "--test",
             action="store_true",
             help="Connect to the Jamf server using the config file",
         )
 
     def parse(self, argv):
         """
         :param argv:    list of arguments to parse
         :returns:       argparse.NameSpace object
         """
-        return self.parser.parse_args(argv)
+        args = self.parser.parse_args(argv)
+        if args.client:
+            if args.client not in ["0", "no", "false", "1", "yes", "true"]:
+                sys.stderr.write(
+                    "API Client Auth must be one of these vaules: yes, true, 1, no, false, or 0.\n"
+                )
+                exit(1)
+        return args
 
 
 def test(config_path):
     try:
-        api = python_jamf.API(config_path=config_path)
+        jps = python_jamf.server.Server(config_path=config_path)
     except python_jamf.exceptions.JamfConfigError:
         sys.stderr.write("Could not read config preferences, have you set them yet?\n")
         exit(1)
     try:
-        print(api.get("accounts"))
+        print(jps.classic.get_accounts())
         print("Connection successful")
     except SystemExit as error:
         print(f"Connection failed, check your settings\n{error}")
 
 
 def print_config(config_path):
     try:
         conf = python_jamf.config.Config(prompt=False, config_path=config_path)
     except python_jamf.exceptions.JamfConfigError:
         sys.stderr.write("Could not read config preferences, have you set them yet?\n")
         exit(1)
     print(conf.config_path)
-    print(conf.hostname)
-    print(conf.username)
+    if conf.client:
+        print("API Client Authentication")
+        username_type = "Client ID"
+        password_type = "Client Secret"
+    else:
+        print("User Authentication")
+        username_type = "Username"
+        password_type = "Password"
+    print(f"Hostname: {conf.hostname}")
+    print(f"{username_type}: {conf.username}")
     if conf.password:
-        print("Password is set")
+        print(f"{password_type} is set")
     else:
-        print("Password is not set")
+        print(f"{password_type} is not set")
 
 
 def revoke_token(config_path):
     api = python_jamf.API(config_path=config_path)
     api.revoke_token()
 
 
 def interactive(args, config_path):
     if args.hostname:
         hostname = args.hostname
     else:
         hostname = python_jamf.config.prompt_hostname()
+    if args.client is not None:
+        if args.client in ["0", "no", "false"]:
+            client = False
+        if args.client in ["1", "yes", "true"]:
+            client = True
+    else:
+        client = python_jamf.config.prompt_userauth()
+    if client:
+        username_type = "Client ID"
+        password_type = "Client Secret"
+    else:
+        username_type = "Username"
+        password_type = "Password"
     if args.user:
         user = args.user
     else:
-        user = input("username: ")
+        user = input(f"{username_type}: ")
+
     if args.passwd:
         passwd = args.passwd
     else:
-        passwd = getpass.getpass()
+        passwd = getpass.getpass(prompt=f"{password_type}: ")
     conf = python_jamf.config.Config(
         hostname=hostname,
         username=user,
         password=passwd,
+        client=client,
         prompt=False,
         config_path=config_path,
     )
     conf.save()
     print("Test the config by invoking `conf-python-jamf -t`")
```

### Comparing `python-jamf-0.9.8/python_jamf/version.py` & `python-jamf-0.9.9/python_jamf/version.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/python_jamf.egg-info/PKG-INFO` & `python-jamf-0.9.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: python-jamf
-Version: 0.9.8
-Summary: Python wrapper for Jamf Pro API
-Home-page: https://github.com/univ-of-utah-marriott-library-apple/python-jamf
-Author: The University of Utah
-Author-email: mlib-its-mac@lists.utah.edu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # python-jamf
 _Programmatic Automation, Access & Control of Jamf Pro_
 
 ![python_jamf_logo](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/images/python_jamf_logo.png)
 
 ## Introduction
 
@@ -137,44 +121,14 @@
 <img src="https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/images/MacAdmins_Slack_logo.png" alt="MacAdmin's Slack Logo">
 </p>
 
 ## Latest Status
 
 ### Releases
 
-#### :new: [python-jamf - 0.8.2](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.8.2)
-
-- Much better error reporting when there's a connection failure to the server
-- Checks for "http://" or "https://" when setting a hostname and when connecting to a server
-- Added `conf-python-jamf -r` to remove the bearer token saved in the keychain
-- Unified server connection code
-- Replaced all `exit(1)` with `raise SystemExit`
-- pre-commit updated to 4.3.0
-- GitHub action updated action names
-- Updated README
-
-#### [python-jamf - 0.8.1](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.8.1)
-
-- This release includes the xml array fix described [here](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/blob/07378f0397744f52af54dbadb798e057d5e0c6cf/README.md#known-breaking-changes-on-the-roadmap).
-
-#### [python-jamf - 0.7.5](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.7.5)
-
-- Fixed trigger_logout removal from policies triggers
-- Fixed bearer token bug
-- Lots of automated reformatting and cleaning up
-- Adds pre-commit
-
-Thank you homebysix for your contributions.
-
-#### [python-jamf - 0.7.4](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/releases/tag/0.7.4-af4107c6)
-
- - Bearer token support
- - Fixed bug when creating records (shallow vs deep copy)
- - Fixed version in setup.py bug
- - Removed jamfnet from main docker-compose and move it to it's own file
- - Support smb mounting on linux
+Please see the [Changelog](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/blob/main/CHANGELOG.md) for all release notes.
 
 Thank you yairf-s1 and pythoninthegrass for your contributions.
 
 See `python-jamf` [upgrade](https://github.com/univ-of-utah-marriott-library-apple/python-jamf/wiki/Installing#upgrading) documentation to upgrade to latest release.
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `python-jamf-0.9.8/python_jamf.egg-info/SOURCES.txt` & `python-jamf-0.9.9/python_jamf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/setup.py` & `python-jamf-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/tests/api_test_old.py` & `python-jamf-0.9.9/tests/api_test_old.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/tests/config_test.py` & `python-jamf-0.9.9/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/tests/convert_json_xml_test.py` & `python-jamf-0.9.9/tests/convert_json_xml_test.py`

 * *Files identical despite different names*

### Comparing `python-jamf-0.9.8/tests/test_records.py` & `python-jamf-0.9.9/tests/test_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,16 @@
         pkgItem = create(pkgObj)
         if pkgItem is None:
             print("Failed to create Package!")
             exit()
         pgkVer["package"] = {"id": pkgItem.data["id"], "name": pkgItem.data["name"]}
         pstItem.save()
     data = objType.stub_record()
-    data["patch_policy"]["software_title_configuration_id"] = pstItem.data["id"]
-    data["patch_policy"]["general"]["target_version"] = pgkVer["software_version"]
+    data["software_title_configuration_id"] = pstItem.data["id"]
+    data["general"]["target_version"] = pgkVer["software_version"]
     pprint(data)
     return data
 
 
 def post_patch_policy():
     pstObj = server.records.PatchSoftwareTitles()
     pstItem = pstObj.recordsWithName("Bare Bones BBEdit")[0]
```

