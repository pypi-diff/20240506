# Comparing `tmp/shipper_shippy-2.36.6.tar.gz` & `tmp/shipper_shippy-2.36.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper_shippy-2.36.6.tar", last modified: Thu May  2 04:59:23 2024, max compression
+gzip compressed data, was "shipper_shippy-2.36.7.tar", last modified: Mon May  6 08:31:28 2024, max compression
```

## Comparing `shipper_shippy-2.36.6.tar` & `shipper_shippy-2.36.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:59:23.029810 shipper_shippy-2.36.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-02 04:59:23.029810 shipper_shippy-2.36.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 04:59:23.029810 shipper_shippy-2.36.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:59:23.029810 shipper_shippy-2.36.6/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-02 04:59:22.000000 shipper_shippy-2.36.6/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 04:59:23.000000 shipper_shippy-2.36.6/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 04:59:22.000000 shipper_shippy-2.36.6/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 04:59:22.000000 shipper_shippy-2.36.6/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 04:59:22.000000 shipper_shippy-2.36.6/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 04:59:22.000000 shipper_shippy-2.36.6/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:59:23.029810 shipper_shippy-2.36.6/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 04:59:14.000000 shipper_shippy-2.36.6/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:28.327365 shipper_shippy-2.36.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-06 08:31:28.327365 shipper_shippy-2.36.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:31:28.327365 shipper_shippy-2.36.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:28.327365 shipper_shippy-2.36.7/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-06 08:31:28.000000 shipper_shippy-2.36.7/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 08:31:28.000000 shipper_shippy-2.36.7/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:31:28.000000 shipper_shippy-2.36.7/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 08:31:28.000000 shipper_shippy-2.36.7/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 08:31:28.000000 shipper_shippy-2.36.7/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 08:31:28.000000 shipper_shippy-2.36.7/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:28.327365 shipper_shippy-2.36.7/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 08:31:19.000000 shipper_shippy-2.36.7/shippy/version.py
```

### Comparing `shipper_shippy-2.36.6/PKG-INFO` & `shipper_shippy-2.36.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.6
+Version: 2.36.7
 Summary: Client-side tool to interface with shipper
-Home-page: https://github.com/ericswpark/shippy
+Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
-Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
+Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
@@ -29,15 +29,16 @@
 Client-side tool to interface with shipper
 
 # Usage
 
 Get shippy from PyPI:
 
 ```shell
-pip3 install --upgrade shipper-shippy
+pipx install shipper-shippy             # pipx, recommended
+pip3 install --upgrade shipper-shippy   # or pip3
 ```
 
 Go to the directory with build files, and run:
 
 ```shell
 shippy
 ```
```

### Comparing `shipper_shippy-2.36.6/README.md` & `shipper_shippy-2.36.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 Client-side tool to interface with shipper
 
 # Usage
 
 Get shippy from PyPI:
 
 ```shell
-pip3 install --upgrade shipper-shippy
+pipx install shipper-shippy             # pipx, recommended
+pip3 install --upgrade shipper-shippy   # or pip3
 ```
 
 Go to the directory with build files, and run:
 
 ```shell
 shippy
 ```
```

### Comparing `shipper_shippy-2.36.6/setup.py` & `shipper_shippy-2.36.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     name="shipper-shippy",
     version=main_ns["__version__"],
     author="Eric Park",
     author_email="me@ericswpark.com",
     description="Client-side tool to interface with shipper",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ericswpark/shippy",
+    url="https://github.com/shipperstack/shipper/tree/master/shippy",
     project_urls={
-        "Bug Tracker": "https://github.com/ericswpark/shippy/issues",
+        "Bug Tracker": "https://github.com/shipperstack/shipper/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=("tests",)),
```

### Comparing `shipper_shippy-2.36.6/shipper_shippy.egg-info/PKG-INFO` & `shipper_shippy-2.36.7/shipper_shippy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.6
+Version: 2.36.7
 Summary: Client-side tool to interface with shipper
-Home-page: https://github.com/ericswpark/shippy
+Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
-Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
+Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
@@ -29,15 +29,16 @@
 Client-side tool to interface with shipper
 
 # Usage
 
 Get shippy from PyPI:
 
 ```shell
-pip3 install --upgrade shipper-shippy
+pipx install shipper-shippy             # pipx, recommended
+pip3 install --upgrade shipper-shippy   # or pip3
 ```
 
 Go to the directory with build files, and run:
 
 ```shell
 shippy
 ```
```

### Comparing `shipper_shippy-2.36.6/shippy/__main__.py` & `shipper_shippy-2.36.7/shippy/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     find_checksum_file,
     Client,
 )
 from .config import get_config_value, set_config_value, get_optional_true_config_value
 from .constants import (
     SENTRY_SDK_URL,
     SERVER_COMPAT_ERROR_MSG,
+    SERVER_MISSING_SCHEMA_MSG,
     SHIPPY_COMPAT_ERROR_MSG,
     SHIPPY_OUTDATED_MSG,
     UNEXPECTED_SERVER_RESPONSE_ERROR_MSG,
     FAILED_TO_LOG_IN_ERROR_MSG,
     CANNOT_CONTACT_SERVER_ERROR_MSG,
     PRERELEASE_WARNING_MSG,
     NO_CONFIGURATION_WARNING_MSG,
@@ -198,18 +199,18 @@
         "Please wait while shippy contacts the remote server to check if the token is "
         "still valid... "
     ):
         if client.is_token_valid():
             print_success(
                 f"Successfully validated token! Hello, {client.get_username()}!"
             )
-        else:
-            # Token check failed, prompt for login again
-            print_warning("The saved token is invalid. Please sign-in again.")
-            prompt_login(client)
+            return
+    # Token check failed, prompt for login again
+    print_warning("The saved token is invalid. Please sign-in again.")
+    prompt_login(client)
 
 
 def check_shippy_update():
     with console.status("Please wait while shippy checks for updates... "):
         try:
             r = requests.get(
                 "https://api.github.com/repos/shipperstack/shipper/releases/latest"
@@ -312,15 +313,15 @@
 def get_server_url():
     try:
         while True:
             server_url = input("Enter the server URL: ")
             if not check_server_url_schema(server_url):
                 # noinspection HttpUrlsUsage
                 print_error(
-                    msg="Server URL is missing either http:// or https://.",
+                    msg=SERVER_MISSING_SCHEMA_MSG,
                     newline=True,
                     exit_after=False,
                 )
             else:
                 break
 
         set_config_value("shippy", "server", server_url)
```

### Comparing `shipper_shippy-2.36.6/shippy/client.py` & `shipper_shippy-2.36.7/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.6/shippy/config.py` & `shipper_shippy-2.36.7/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.6/shippy/constants.py` & `shipper_shippy-2.36.7/shippy/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,32 +20,27 @@
  * Compatible version: \t\t{}
 
 To prevent data corruption, shippy will not work with an outdated server. Exiting...
 """
 
 SHIPPY_COMPAT_ERROR_MSG = """\
 Error: shippy is out-of-date and will not with this server instance.
-Upgrade shippy with the following command:
-\tpip3 install --upgrade shipper-shippy
-
 Version information:
  * Reported compatible version by server: \t{}
  * Your current shippy version: \t\t{}
 """
 
 SHIPPY_OUTDATED_MSG = """\
 Warning: shippy is out-of-date.
  * Current version: \t{}
  * New version: \t{}
-
-We recommend updating shippy with the following command:
-\tpip3 install --upgrade shipper-shippy
 """
 
 SERVER_EMPTY_TOKEN_MSG = "Server returned an empty token."
+SERVER_MISSING_SCHEMA_MSG = "Server URL is missing either http:// or https://."
 SERVER_WRONG_SCHEMA_MSG = "Server uses HTTPS, but was supplied HTTP URL."
 BLANK_AUTH_DETAILS_MSG = "Username or password must not be blank."
 INVALID_CREDENTIALS_MSG = "The supplied credentials are invalid."
 GATEWAY_SERVER_UNAVAILABLE_MSG = "The gateway server is currently unavailable."
 SERVER_TEMPORARILY_UNAVAILABLE_MSG = "The server is temporarily unavailable."
 
 LOG_DEBUG_REQUEST_SEND_MSG = """\
```

### Comparing `shipper_shippy-2.36.6/shippy/helper.py` & `shipper_shippy-2.36.7/shippy/helper.py`

 * *Files identical despite different names*

