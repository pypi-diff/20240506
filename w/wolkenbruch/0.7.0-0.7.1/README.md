# Comparing `tmp/wolkenbruch-0.7.0.tar.gz` & `tmp/wolkenbruch-0.7.1.tar.gz`

## Comparing `wolkenbruch-0.7.0.tar` & `wolkenbruch-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.flake8
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.pylintrc
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/img/wolkenbruch.svg
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/img/wolkenbruch_256x160.svg
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/img/wolkenbruch_bw_256x256.svg
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/systemd/wolkenbruch.service
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/systemd/wolkenbruch.timer
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/__init__.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/__main__.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/config.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/emailsender.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/precipitationchecker.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/wolkenbruch.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/wolkenbruch.yml.template
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/LICENSE
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/README.md
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.flake8
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.pylintrc
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/extra/img/wolkenbruch.svg
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/extra/img/wolkenbruch_256x160.svg
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/extra/img/wolkenbruch_bw_256x256.svg
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/extra/systemd/wolkenbruch.service
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/extra/systemd/wolkenbruch.timer
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/__init__.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/__main__.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/config.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/emailsender.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/precipitationchecker.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/wolkenbruch.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/src/wolkenbruch/wolkenbruch.yml.template
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 wolkenbruch-0.7.1/PKG-INFO
```

### Comparing `wolkenbruch-0.7.0/CHANGELOG.md` & `wolkenbruch-0.7.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+- **0.7.1** (2024-05-06):
+    - migrate source repository and build toolchain to GitHub
+
 - **0.7.0** (2024-05-06):
     - migrate to clean pyproject.toml and hatchling
     - change default config file handling
     - rename git default branch
 
 - **0.6.5** (2024-05-06):
     - catch geocoder error
```

### Comparing `wolkenbruch-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `wolkenbruch-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `wolkenbruch-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/.github/workflows/build.yml` & `wolkenbruch-0.7.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/.github/workflows/release.yml` & `wolkenbruch-0.7.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/extra/img/wolkenbruch.svg` & `wolkenbruch-0.7.1/extra/img/wolkenbruch.svg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/extra/img/wolkenbruch_256x160.svg` & `wolkenbruch-0.7.1/extra/img/wolkenbruch_256x160.svg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/extra/img/wolkenbruch_bw_256x256.svg` & `wolkenbruch-0.7.1/extra/img/wolkenbruch_bw_256x256.svg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/src/wolkenbruch/__init__.py` & `wolkenbruch-0.7.1/src/wolkenbruch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     "remind_me_if_it_rains",
 ]
 
 
 from .wolkenbruch import remind_me_if_it_rains
 
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `wolkenbruch-0.7.0/src/wolkenbruch/__main__.py` & `wolkenbruch-0.7.1/src/wolkenbruch/__main__.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/src/wolkenbruch/config.py` & `wolkenbruch-0.7.1/src/wolkenbruch/config.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/src/wolkenbruch/emailsender.py` & `wolkenbruch-0.7.1/src/wolkenbruch/emailsender.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/src/wolkenbruch/precipitationchecker.py` & `wolkenbruch-0.7.1/src/wolkenbruch/precipitationchecker.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """
 
     API_VERSION = "2.0"
     API_ENDPOINT = (
         f"https://api.met.no/weatherapi/locationforecast/{API_VERSION:s}/compact"
     )
     API_HEADERS = {
-        "User-agent": "python-wolkenbruch (https://gitlab.com/christophfink/wolkenbruch/"
+        "User-agent": "python-wolkenbruch (https://github.com/christophfink/wolkenbruch/"
     }
 
     def __init__(self, lat, lon, n_hours=14, *args, **kwargs):
         """
         Check the forecast precipitation at a location.
 
         Args:
```

### Comparing `wolkenbruch-0.7.0/src/wolkenbruch/wolkenbruch.py` & `wolkenbruch-0.7.1/src/wolkenbruch/wolkenbruch.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/LICENSE` & `wolkenbruch-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.0/README.md` & `wolkenbruch-0.7.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 ![rain cloud](extra/img/wolkenbruch_256x160.svg)
 
 # Wolkenbruch
 
 Checks the weather forecast for a configurable place and sends an e-mail
 reminder to pack your rain gear if precipitation is forecast.
 
-Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses [OpenStreetmap](https://osm.org/) to find the location from place names.
+Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses
+[OpenStreetmap](https://osm.org/) to find the location from place names.
 
 ### Dependencies
 
-Wolkenbruch is written in Python 3, and depends on the Python modules [geocoder](https://geocoder.readthedocs.io/), [requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
+Wolkenbruch is written in Python 3, and depends on the Python modules
+[geocoder](https://geocoder.readthedocs.io/),
+[requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
 
 ### Installation
 
 - *using `pip` or similar:*
 
 ```shell
-pip3 install wolkenbruch
+pip install wolkenbruch
 ```
 
-- *OR: manually:*
-
-    - Clone this repository
-
-    ```shell
-    git clone https://gitlab.com/christoph.fink/wolkenbruch.git
-    ```
-
-    - Change to the cloned directory
-    - Use the Python `setuptools` to install the package:
-
-    ```shell
-    cd wolkenbruch
-    python3 ./setup.py install
-    ```
-
 ### Configuration
 
-Copy the example configuration file [wolkenbruch.yml.template](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/main/src/wolkenbruch/wolkenbruch.yml.template) to a suiteable location, depending on your operating system:
+Copy the example configuration file
+[wolkenbruch.yml.template](https://raw.githubusercontent.com/christophfink/wolkenbruch/main/src/wolkenbruch/wolkenbruch.yml.template)
+to a suiteable location, depending on your operating system:
 
 - on Linux systems:
     - system-wide configuration: `/etc/wolkenbruch.yml`
     - per-user configuration: 
         - `~/.config/wolkenbruch.yml` OR
         - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
 - on MacOS systems:
@@ -49,20 +38,37 @@
         - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
 - on Microsoft Windows systems:
     - per-user configuration:
         `%APPDATA%\wolkenbruch.yml`
 
 Adapt the configuration:
 
-- Change the place the forecast searches for. For bigger cities their name might be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to smaller places, or places that share their name with other places in different parts of the world, you might have to add a country, state or county name, e.g. ”Springfield, Fife”.
-- Adapt the SMTP host and credentials (leave user and password empty if not authentication is required). **Be careful:** the credentials are (obviously) saved in plain-text. Protect access to the configuration file, e.g. on a GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
-- Set the sender and receiver e-mail address (they can and often will be the same address)
-- If you feel like it, change the subject line and message body of the e-mail. The message body can contain [Python string formatting code](https://docs.python.org/3/library/string.html#formatstrings) for a float variables `a` and `m` (the average and maximum precipitation rates over the next 14 hours, in mm/h).
-- Adjust the amount of rain you can stand: `average_precipitation_rate_threshold` is the average precipitation rate over the next 14 hours (in mm per hour) that has to be exceeded to send you a reminder, `max_precipitation_rate_threshold` the highest single hourly value that makes you want to not forget your rain gear.
-- The verbose flag toggles whether `wolkenbruch` prints a status or operated silently.
+- Change the place the forecast searches for. For bigger cities their name might
+  be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to
+  smaller places, or places that share their name with other places in different
+  parts of the world, you might have to add a country, state or county name,
+  e.g. ”Springfield, Fife”.
+- Adapt the SMTP host and credentials (leave user and password empty if not
+  authentication is required). **Be careful:** the credentials are (obviously)
+  saved in plain-text. Protect access to the configuration file, e.g. on a
+  GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
+- Set the sender and receiver e-mail address (they can and often will be the
+  same address)
+- If you feel like it, change the subject line and message body of the e-mail.
+  The message body can contain [Python string formatting
+  code](https://docs.python.org/3/library/string.html#formatstrings) for a float
+  variables `a` and `m` (the average and maximum precipitation rates over the
+  next 14 hours, in mm/h).
+- Adjust the amount of rain you can stand:
+  `average_precipitation_rate_threshold` is the average precipitation rate over
+  the next 14 hours (in mm per hour) that has to be exceeded to send you a
+  reminder, `max_precipitation_rate_threshold` the highest single hourly value
+  that makes you want to not forget your rain gear.
+- The verbose flag toggles whether `wolkenbruch` prints a status or operated
+  silently.
 
 ```yaml
 # example configuration file
 # (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
 #    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
 smtp:
     host:     localhost:587
@@ -77,24 +83,35 @@
 average_precipitation_rate_threshold: 0.1
 max_precipitation_rate_threshold: 0.5
 verbose: False
 ```
 
 ### Usage
 
-Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
+Run `wolkenbruch` to check the precipitation for the next 14 hours and send you
+an e-mail reminder. Ideally, set up a cron job or a systemd timer to run
+`wolkenbruch` e.g. every morning.
 
 
 #### Systemd timer
 
-Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/main/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
+Copy
+[`wolkenbruch.service`](https://raw.githubusercontent.com/christophfink/wolkenbruch/main/extra/systemd/wolkenbruch.service)
+and
+[`wolkenbruch.timer`](https://raw.githubusercontent.com/christophfink/wolkenbruch/main/extra/systemd/wolkenbruch.timer)
+from
+[extra/systemd/](https://github.com/christophfink/wolkenbruch/tree/main/extra/systemd)
+to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run
+wolkenbruch at 6:30 every morning:
 
 ```sh
 systemctl --user daemon-reload
 systemctl --user enable --now wolkenbruch.timer 
 ```
 
-If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
+If you want the systemd timer to trigger when you’re not logged in, enable
+[_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances)
+for your user:
 
 ```sh
 sudo loginctl enable-linger USERNAME
 ```
```

### Comparing `wolkenbruch-0.7.0/pyproject.toml` & `wolkenbruch-0.7.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 
 dynamic = ["version"]
 
 [project.scripts]
 wolkenbruch = "wolkenbruch.__main__:main"
 
 [project.urls]
-Documentation = "https://gitlab.com/christophfink/wolkenbruch/"
-Repository = "https://gitlab.com/christophfink/wolkenbruch/"
-"Change log" = "https://gitlab.com/christophfink/wolkenbruch/-/blob/master/CHANGELOG.md"
-"Bug tracker" = "https://gitlab.com/christophfink/wolkenbruch/-/issues"
+Documentation = "https://github.com/christophfink/wolkenbruch/"
+Repository = "https://github.com/christophfink/wolkenbruch/"
+"Change log" = "https://github.com/christophfink/wolkenbruch/blob/main/CHANGELOG.md"
+"Bug tracker" = "https://github.com/christophfink/wolkenbruch/issues"
 
 [tool.hatch.version]
 path = "src/wolkenbruch/__init__.py"
```

### Comparing `wolkenbruch-0.7.0/PKG-INFO` & `wolkenbruch-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: wolkenbruch
-Version: 0.7.0
+Version: 0.7.1
 Summary: Send an e-mail reminder if precipitation is forecast
-Project-URL: Documentation, https://gitlab.com/christophfink/wolkenbruch/
-Project-URL: Repository, https://gitlab.com/christophfink/wolkenbruch/
-Project-URL: Change log, https://gitlab.com/christophfink/wolkenbruch/-/blob/master/CHANGELOG.md
-Project-URL: Bug tracker, https://gitlab.com/christophfink/wolkenbruch/-/issues
+Project-URL: Documentation, https://github.com/christophfink/wolkenbruch/
+Project-URL: Repository, https://github.com/christophfink/wolkenbruch/
+Project-URL: Change log, https://github.com/christophfink/wolkenbruch/blob/main/CHANGELOG.md
+Project-URL: Bug tracker, https://github.com/christophfink/wolkenbruch/issues
 Author-email: Christoph Fink <christoph.fink@gmail.com>
 License: GPL-3.0-or-later or MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -22,47 +22,36 @@
 ![rain cloud](extra/img/wolkenbruch_256x160.svg)
 
 # Wolkenbruch
 
 Checks the weather forecast for a configurable place and sends an e-mail
 reminder to pack your rain gear if precipitation is forecast.
 
-Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses [OpenStreetmap](https://osm.org/) to find the location from place names.
+Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses
+[OpenStreetmap](https://osm.org/) to find the location from place names.
 
 ### Dependencies
 
-Wolkenbruch is written in Python 3, and depends on the Python modules [geocoder](https://geocoder.readthedocs.io/), [requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
+Wolkenbruch is written in Python 3, and depends on the Python modules
+[geocoder](https://geocoder.readthedocs.io/),
+[requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
 
 ### Installation
 
 - *using `pip` or similar:*
 
 ```shell
-pip3 install wolkenbruch
+pip install wolkenbruch
 ```
 
-- *OR: manually:*
-
-    - Clone this repository
-
-    ```shell
-    git clone https://gitlab.com/christoph.fink/wolkenbruch.git
-    ```
-
-    - Change to the cloned directory
-    - Use the Python `setuptools` to install the package:
-
-    ```shell
-    cd wolkenbruch
-    python3 ./setup.py install
-    ```
-
 ### Configuration
 
-Copy the example configuration file [wolkenbruch.yml.template](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/main/src/wolkenbruch/wolkenbruch.yml.template) to a suiteable location, depending on your operating system:
+Copy the example configuration file
+[wolkenbruch.yml.template](https://raw.githubusercontent.com/christophfink/wolkenbruch/main/src/wolkenbruch/wolkenbruch.yml.template)
+to a suiteable location, depending on your operating system:
 
 - on Linux systems:
     - system-wide configuration: `/etc/wolkenbruch.yml`
     - per-user configuration: 
         - `~/.config/wolkenbruch.yml` OR
         - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
 - on MacOS systems:
@@ -70,20 +59,37 @@
         - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
 - on Microsoft Windows systems:
     - per-user configuration:
         `%APPDATA%\wolkenbruch.yml`
 
 Adapt the configuration:
 
-- Change the place the forecast searches for. For bigger cities their name might be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to smaller places, or places that share their name with other places in different parts of the world, you might have to add a country, state or county name, e.g. ”Springfield, Fife”.
-- Adapt the SMTP host and credentials (leave user and password empty if not authentication is required). **Be careful:** the credentials are (obviously) saved in plain-text. Protect access to the configuration file, e.g. on a GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
-- Set the sender and receiver e-mail address (they can and often will be the same address)
-- If you feel like it, change the subject line and message body of the e-mail. The message body can contain [Python string formatting code](https://docs.python.org/3/library/string.html#formatstrings) for a float variables `a` and `m` (the average and maximum precipitation rates over the next 14 hours, in mm/h).
-- Adjust the amount of rain you can stand: `average_precipitation_rate_threshold` is the average precipitation rate over the next 14 hours (in mm per hour) that has to be exceeded to send you a reminder, `max_precipitation_rate_threshold` the highest single hourly value that makes you want to not forget your rain gear.
-- The verbose flag toggles whether `wolkenbruch` prints a status or operated silently.
+- Change the place the forecast searches for. For bigger cities their name might
+  be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to
+  smaller places, or places that share their name with other places in different
+  parts of the world, you might have to add a country, state or county name,
+  e.g. ”Springfield, Fife”.
+- Adapt the SMTP host and credentials (leave user and password empty if not
+  authentication is required). **Be careful:** the credentials are (obviously)
+  saved in plain-text. Protect access to the configuration file, e.g. on a
+  GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
+- Set the sender and receiver e-mail address (they can and often will be the
+  same address)
+- If you feel like it, change the subject line and message body of the e-mail.
+  The message body can contain [Python string formatting
+  code](https://docs.python.org/3/library/string.html#formatstrings) for a float
+  variables `a` and `m` (the average and maximum precipitation rates over the
+  next 14 hours, in mm/h).
+- Adjust the amount of rain you can stand:
+  `average_precipitation_rate_threshold` is the average precipitation rate over
+  the next 14 hours (in mm per hour) that has to be exceeded to send you a
+  reminder, `max_precipitation_rate_threshold` the highest single hourly value
+  that makes you want to not forget your rain gear.
+- The verbose flag toggles whether `wolkenbruch` prints a status or operated
+  silently.
 
 ```yaml
 # example configuration file
 # (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
 #    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
 smtp:
     host:     localhost:587
@@ -98,24 +104,35 @@
 average_precipitation_rate_threshold: 0.1
 max_precipitation_rate_threshold: 0.5
 verbose: False
 ```
 
 ### Usage
 
-Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
+Run `wolkenbruch` to check the precipitation for the next 14 hours and send you
+an e-mail reminder. Ideally, set up a cron job or a systemd timer to run
+`wolkenbruch` e.g. every morning.
 
 
 #### Systemd timer
 
-Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/main/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
+Copy
+[`wolkenbruch.service`](https://raw.githubusercontent.com/christophfink/wolkenbruch/main/extra/systemd/wolkenbruch.service)
+and
+[`wolkenbruch.timer`](https://raw.githubusercontent.com/christophfink/wolkenbruch/main/extra/systemd/wolkenbruch.timer)
+from
+[extra/systemd/](https://github.com/christophfink/wolkenbruch/tree/main/extra/systemd)
+to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run
+wolkenbruch at 6:30 every morning:
 
 ```sh
 systemctl --user daemon-reload
 systemctl --user enable --now wolkenbruch.timer 
 ```
 
-If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
+If you want the systemd timer to trigger when you’re not logged in, enable
+[_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances)
+for your user:
 
 ```sh
 sudo loginctl enable-linger USERNAME
 ```
```

