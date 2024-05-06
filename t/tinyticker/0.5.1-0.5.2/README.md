# Comparing `tmp/tinyticker-0.5.1.tar.gz` & `tmp/tinyticker-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.1.tar", max compression
+gzip compressed data, was "tinyticker-0.5.2.tar", max compression
```

## Comparing `tinyticker-0.5.1.tar` & `tinyticker-0.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-06 08:53:00.961287 tinyticker-0.5.1/LICENSE
--rw-r--r--   0        0        0     3863 2024-05-06 08:53:00.961287 tinyticker-0.5.1/README.md
--rw-r--r--   0        0        0      899 2024-05-06 08:53:00.961287 tinyticker-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/__init__.py
--rw-r--r--   0        0        0     6196 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/__main__.py
--rw-r--r--   0        0        0     1773 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/config.py
--rw-r--r--   0        0        0     8880 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/paths.py
--rw-r--r--   0        0        0    15609 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/ticker.py
--rw-r--r--   0        0        0     3123 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/utils.py
--rw-r--r--   0        0        0      318 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1259 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     8376 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    11895 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14581 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10457 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     5835 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6627 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5690 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     3148 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epdconfig.py
--rw-r--r--   0        0        0     1283 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2547 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     7161 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    13954 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0      787 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1369 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-06 14:17:13.510182 tinyticker-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3863 2024-05-06 14:17:13.510182 tinyticker-0.5.2/README.md
+-rw-r--r--   0        0        0      899 2024-05-06 14:17:13.510182 tinyticker-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6196 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/__main__.py
+-rw-r--r--   0        0        0     1773 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/config.py
+-rw-r--r--   0        0        0     8880 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/paths.py
+-rw-r--r--   0        0        0    15609 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/ticker.py
+-rw-r--r--   0        0        0     2476 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/utils.py
+-rw-r--r--   0        0        0      318 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1259 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     8376 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    11895 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14581 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10457 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     5835 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6627 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5690 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     3148 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/epdconfig.py
+-rw-r--r--   0        0        0     1283 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6610 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15070 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0      787 2024-05-06 14:17:13.514182 tinyticker-0.5.2/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-06 14:17:13.518183 tinyticker-0.5.2/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-06 14:17:13.518183 tinyticker-0.5.2/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1369 2024-05-06 14:17:13.518183 tinyticker-0.5.2/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.2/PKG-INFO
```

### Comparing `tinyticker-0.5.1/LICENSE` & `tinyticker-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/README.md` & `tinyticker-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/pyproject.toml` & `tinyticker-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.1"
+version = "0.5.2"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.5.1/tinyticker/__main__.py` & `tinyticker-0.5.2/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/config.py` & `tinyticker-0.5.2/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/display.py` & `tinyticker-0.5.2/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/ticker.py` & `tinyticker-0.5.2/tinyticker/ticker.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/utils.py` & `tinyticker-0.5.2/tinyticker/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,33 +54,14 @@
 
 class RawTextArgumentDefaultsHelpFormatter(
     argparse.RawTextHelpFormatter, argparse.ArgumentDefaultsHelpFormatter
 ):
     pass
 
 
-def check_for_update(current_version: str, **kwargs) -> bool:
-    """Query the pypy index, returns True if an update is available.
-
-    Args:
-        current_version: the version string of the package.
-        **kwargs: passed to `urllib.request.urlopen`.
-
-    Returns:
-        True if an update is available, False otherwise.
-    """
-    url = "https://pypi.python.org/pypi/{package}/json"
-    response = json.loads(
-        urlopen(url.format(package="tinyticker"), **kwargs).read().decode("utf8")
-    )
-    pypy_version = Version(response["info"]["version"])
-    this_version = Version(current_version)
-    return pypy_version > this_version
-
-
 def now() -> pd.Timestamp:
     """Return the current timestamp."""
     return pd.to_datetime("now", utc=True)
 
 
 def set_verbosity(logger: logging.Logger, verbosity: int) -> logging.Logger:
     """Set the logger's verbosity.
```

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/epdconfig.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/epdconfig.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.2/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/__main__.py` & `tinyticker-0.5.2/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/app.py` & `tinyticker-0.5.2/tinyticker/web/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import logging
 import socket
 import subprocess
 import sys
 import threading
 from pathlib import Path
-from socket import timeout
 from typing import Optional
-from urllib.error import HTTPError, URLError
 
 from flask import Flask, abort, redirect, render_template, request, send_from_directory
 
 from .. import __version__
 from ..config import PLOT_TYPES, SequenceConfig, TickerConfig, TinytickerConfig
 from ..paths import CONFIG_FILE, LOG_DIR
 from ..ticker import INTERVAL_LOOKBACKS, INTERVAL_TIMEDELTAS, SYMBOL_TYPES
-from ..utils import check_for_update
 from ..waveshare_lib.models import MODELS
 from .command import COMMANDS, reboot
 
 LOGGER = logging.getLogger(__name__)
 TEMPLATE_PATH = str(Path(__file__).parent / "templates")
 INTERVAL_WAIT_TIMES = {k: v.value * 1e-9 for k, v in INTERVAL_TIMEDELTAS.items()}
 
@@ -69,32 +66,24 @@
     def add_header(response):
         response.cache_control.max_age = 0
         return response
 
     @app.route("/")
     def index():
         tt_config = TinytickerConfig.from_file(config_file)
-        # TODO: performing this query on the server will reduce responsiveness
-        try:
-            update_available = check_for_update(current_version=__version__, timeout=1)
-            LOGGER.info("Update available: %s", update_available)
-        except (HTTPError, URLError, timeout):
-            update_available = False
-            LOGGER.warning("Update check failed", exc_info=True)
         return render_template(
             "index.html",
             hostname=hostname,
             commands=commands,
             plot_type_options=PLOT_TYPES,
             symbol_type_options=SYMBOL_TYPES,
             interval_lookbacks=INTERVAL_LOOKBACKS,
             interval_wait_times=INTERVAL_WAIT_TIMES,
             interval_options=INTERVAL_LOOKBACKS.keys(),
             epd_model_options=MODELS.values(),
-            update_available=update_available,
             version=__version__,
             **tt_config.to_dict(),
         )
 
     @app.route("/logfiles")
     def logs():
         return render_template("logfiles.html", log_files=log_files)
```

### Comparing `tinyticker-0.5.1/tinyticker/web/command.py` & `tinyticker-0.5.2/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.2/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.2/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.2/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.2/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/index.html` & `tinyticker-0.5.2/tinyticker/web/templates/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -22,40 +22,72 @@
       href="img/favicon-16x16.png"
     />
     <!-- CSS FILES -->
     <link rel="stylesheet" type="text/css" href="css/uikit.min.css" />
     <!-- JS FILES -->
     <script src="js/uikit.min.js"></script>
     <script src="js/uikit-icons.min.js"></script>
+    <script>
+      /**
+       * Compares two semver strings.
+       *
+       * @param {string} v1 - The first version.
+       * @param {string} v2 - The second version.
+       * @returns {boolean} - Returns true if v1 is greater than v2, otherwise returns false.
+       */
+      function isGreater(v1, v2) {
+        let [v1major, v1minor, v1patch] = v1.split(".").map(Number);
+        let [v2major, v2minor, v2patch] = v2.split(".").map(Number);
+        return (
+          v1major > v2major ||
+          (v1major == v2major &&
+            (v1minor > v2minor || (v1minor == v2minor && v1patch > v2patch)))
+        );
+      }
+
+      async function checkForUpdate(currentVersion) {
+        const url = "https://pypi.org/pypi/tinyticker/json";
+        const response = await fetch(url);
+        const data = await response.json();
+        const pypiVersion = data.info.version;
+        return isGreater(pypiVersion, currentVersion);
+      }
+
+      checkForUpdate("{{version}}").then((isUpdateAvailable) => {
+        document.getElementById("updateDiv").style.display = isUpdateAvailable
+          ? "block"
+          : "none";
+      });
+    </script>
   </head>
   <body class="uk-background-muted uk-padding-small">
     <div class="uk-flex uk-flex-center uk-flex-middle">
       <div class="uk-width-large">
         <div class="uk-width-1-1 uk-text-center">
           <p class="uk-text-large">🚀 TinyTicker Dashboard 🚀</p>
         </div>
-        {% if update_available %}
-          <div
-            class="uk-background-default uk-alert uk-padding-small uk-margin-small"
-          >
-            <div class="uk-width-1-1 uk-text-center">
-              <p class="uk-text-large">🥳 Update available 🥳</p>
-            </div>
-            <form class="uk-form-stacked" action="/command">
-              <button
-                type="submit"
-                name="command"
-                value="update"
-                class="uk-button uk-button-primary uk-width-expand uk-margin-small-bottom"
-              >
-                Update
-              </button>
-            </form>
+        <div
+          id="updateDiv"
+          class="uk-background-default uk-alert uk-padding-small uk-margin-small"
+          style="display: none"
+        >
+          <div class="uk-width-1-1 uk-text-center">
+            <p class="uk-text-large">🥳 Update available 🥳</p>
           </div>
-        {% endif %}
+          <form class="uk-form-stacked" action="/command">
+            <button
+              type="submit"
+              name="command"
+              value="update"
+              class="uk-button uk-button-primary uk-width-expand uk-margin-small-bottom"
+            >
+              Update
+            </button>
+          </form>
+        </div>
         <div class="uk-width-large">
           <p class="uk-text-large">Config</p>
           <form action="/set_hostname">
             <label class="uk-form-label" for="hostname">Hostname: </label>
             <input
               class="uk-input uk-width-1-3 uk-width-1-2@m"
               type="text"
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
 🚀 TinyTicker Dashboard 🚀
-{% if update_available %}
 🥳 Update available 🥳
 Update
-{% endif %}
 Config
 Hostname:[{{ hostname }}      ][Set & Reboot]
 ===============================================================================
 ePaper display model
 {%- for epd_model_option in epd_model_options -%} {%- if epd_model_option.name
 == epd_model -%}
 {{ epd_model_option.desc }}
```

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.2/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.2/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.2/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.2/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.1/PKG-INFO` & `tinyticker-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.1 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.2 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

