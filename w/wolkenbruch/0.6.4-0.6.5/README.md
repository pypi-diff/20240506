# Comparing `tmp/wolkenbruch-0.6.4.tar.gz` & `tmp/wolkenbruch-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolkenbruch-0.6.4.tar", last modified: Tue Mar 16 19:40:42 2021, max compression
+gzip compressed data, was "wolkenbruch-0.6.5.tar", last modified: Mon May  6 08:29:13 2024, max compression
```

## Comparing `wolkenbruch-0.6.4.tar` & `wolkenbruch-0.6.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/
--rw-r--r--   0 root         (0) root         (0)     5801 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4428 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/extra/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/extra/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      129 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/extra/systemd/wolkenbruch.service
--rw-rw-rw-   0 root         (0) root         (0)       72 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/extra/systemd/wolkenbruch.timer
--rw-rw-rw-   0 root         (0) root         (0)       98 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      919 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2021-03-16 19:40:36.000000 wolkenbruch-0.6.4/wolkenbruch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch/lib/
--rw-rw-rw-   0 root         (0) root         (0)      997 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3510 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3289 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch/lib/emailsender.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch/lib/precipitationchecker.py
--rw-rw-rw-   0 root         (0) root         (0)     2903 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch/wolkenbruch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5801 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-03-16 19:40:42.000000 wolkenbruch-0.6.4/wolkenbruch.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      396 2021-03-16 19:39:59.000000 wolkenbruch-0.6.4/wolkenbruch.yml.example
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5062 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4428 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.440239 wolkenbruch-0.6.5/extra/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.442239 wolkenbruch-0.6.5/extra/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/extra/systemd/wolkenbruch.service
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/extra/systemd/wolkenbruch.timer
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.443239 wolkenbruch-0.6.5/wolkenbruch/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-05-06 08:29:11.000000 wolkenbruch-0.6.5/wolkenbruch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.445239 wolkenbruch-0.6.5/wolkenbruch/lib/
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3316 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/emailsender.py
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/precipitationchecker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/wolkenbruch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/wolkenbruch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5062 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      544 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch.yml.example
```

### Comparing `wolkenbruch-0.6.4/PKG-INFO` & `wolkenbruch-0.6.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,100 @@
-Metadata-Version: 2.1
-Name: wolkenbruch
-Version: 0.6.4
-Summary: Checks the weather forecast for your home town and sends an e-mail reminder to pack your rain gear if precipitation is forecast.
-Home-page: https://gitlab.com/christoph.fink/wolkenbruch
-Author: Christoph Fink
-Author-email: christoph.fink@helsinki.fi
-License: GPLv3
-Description: ![rain cloud](extra/img/wolkenbruch_256x160.svg)
-        
-        # Wolkenbruch
-        
-        Checks the weather forecast for a configurable place and sends an e-mail
-        reminder to pack your rain gear if precipitation is forecast.
-        
-        Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses [OpenStreetmap](https://osm.org/) to find the location from place names.
-        
-        ### Dependencies
-        
-        Wolkenbruch is written in Python 3, and depends on the Python modules [geocoder](https://geocoder.readthedocs.io/), [requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
-        
-        ### Installation
-        
-        - *using `pip` or similar:*
-        
-        ```shell
-        pip3 install wolkenbruch
-        ```
-        
-        - *OR: manually:*
-        
-            - Clone this repository
-        
-            ```shell
-            git clone https://gitlab.com/christoph.fink/wolkenbruch.git
-            ```
-        
-            - Change to the cloned directory
-            - Use the Python `setuptools` to install the package:
-        
-            ```shell
-            cd wolkenbruch
-            python3 ./setup.py install
-            ```
-        
-        ### Configuration
-        
-        Copy the example configuration file [wolkenbruch.yml.example](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/master/wolkenbruch.yml.example) to a suiteable location, depending on your operating system:
-        
-        - on Linux systems:
-            - system-wide configuration: `/etc/wolkenbruch.yml`
-            - per-user configuration: 
-                - `~/.config/wolkenbruch.yml` OR
-                - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
-        - on MacOS systems:
-            - per-user configuration:
-                - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
-        - on Microsoft Windows systems:
-            - per-user configuration:
-                `%APPDATA%\wolkenbruch.yml`
-        
-        Adapt the configuration:
-        
-        - Change the place the forecast searches for. For bigger cities their name might be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to smaller places, or places that share their name with other places in different parts of the world, you might have to add a country, state or county name, e.g. ”Springfield, Fife”.
-        - Adapt the SMTP host and credentials (leave user and password empty if not authentication is required). **Be careful:** the credentials are (obviously) saved in plain-text. Protect access to the configuration file, e.g. on a GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
-        - Set the sender and receiver e-mail address (they can and often will be the same address)
-        - If you feel like it, change the subject line and message body of the e-mail. The message body can contain [Python string formatting code](https://docs.python.org/3/library/string.html#formatstrings) for a float variables `a` and `m` (the average and maximum precipitation rates over the next 14 hours, in mm/h).
-        - Adjust the amount of rain you can stand: `average_precipitation_rate_threshold` is the average precipitation rate over the next 14 hours (in mm per hour) that has to be exceeded to send you a reminder, `max_precipitation_rate_threshold` the highest single hourly value that makes you want to not forget your rain gear.
-        - The verbose flag toggles whether `wolkenbruch` prints a status or operated silently.
-        
-        ```yaml
-        # example configuration file
-        # (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
-        #    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
-        smtp:
-            host:     localhost:587
-            user:     foobar
-            password: BARFOO
-        email:
-            from:     me@whereever.com
-            to:       myself@whereever.com
-            subject:  Pack your rain gear!
-            message:  The forecast precipitation rate for today is {a:.2f} mm/h, maximum {m:2f} mm/h.
-        place: Helsinki
-        average_precipitation_rate_threshold: 0.1
-        max_precipitation_rate_threshold: 0.5
-        verbose: False
-        ```
-        
-        ### Usage
-        
-        Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
-        
-        
-        #### Systemd timer
-        
-        Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/master/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
-        
-        ```sh
-        systemctl --user daemon-reload
-        systemctl --user enable --now wolkenbruch.timer 
-        ```
-        
-        If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
-        
-        ```sh
-        sudo loginctl enable-linger USERNAME
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+![rain cloud](extra/img/wolkenbruch_256x160.svg)
+
+# Wolkenbruch
+
+Checks the weather forecast for a configurable place and sends an e-mail
+reminder to pack your rain gear if precipitation is forecast.
+
+Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses [OpenStreetmap](https://osm.org/) to find the location from place names.
+
+### Dependencies
+
+Wolkenbruch is written in Python 3, and depends on the Python modules [geocoder](https://geocoder.readthedocs.io/), [requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
+
+### Installation
+
+- *using `pip` or similar:*
+
+```shell
+pip3 install wolkenbruch
+```
+
+- *OR: manually:*
+
+    - Clone this repository
+
+    ```shell
+    git clone https://gitlab.com/christoph.fink/wolkenbruch.git
+    ```
+
+    - Change to the cloned directory
+    - Use the Python `setuptools` to install the package:
+
+    ```shell
+    cd wolkenbruch
+    python3 ./setup.py install
+    ```
+
+### Configuration
+
+Copy the example configuration file [wolkenbruch.yml.example](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/master/wolkenbruch.yml.example) to a suiteable location, depending on your operating system:
+
+- on Linux systems:
+    - system-wide configuration: `/etc/wolkenbruch.yml`
+    - per-user configuration: 
+        - `~/.config/wolkenbruch.yml` OR
+        - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
+- on MacOS systems:
+    - per-user configuration:
+        - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
+- on Microsoft Windows systems:
+    - per-user configuration:
+        `%APPDATA%\wolkenbruch.yml`
+
+Adapt the configuration:
+
+- Change the place the forecast searches for. For bigger cities their name might be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to smaller places, or places that share their name with other places in different parts of the world, you might have to add a country, state or county name, e.g. ”Springfield, Fife”.
+- Adapt the SMTP host and credentials (leave user and password empty if not authentication is required). **Be careful:** the credentials are (obviously) saved in plain-text. Protect access to the configuration file, e.g. on a GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
+- Set the sender and receiver e-mail address (they can and often will be the same address)
+- If you feel like it, change the subject line and message body of the e-mail. The message body can contain [Python string formatting code](https://docs.python.org/3/library/string.html#formatstrings) for a float variables `a` and `m` (the average and maximum precipitation rates over the next 14 hours, in mm/h).
+- Adjust the amount of rain you can stand: `average_precipitation_rate_threshold` is the average precipitation rate over the next 14 hours (in mm per hour) that has to be exceeded to send you a reminder, `max_precipitation_rate_threshold` the highest single hourly value that makes you want to not forget your rain gear.
+- The verbose flag toggles whether `wolkenbruch` prints a status or operated silently.
+
+```yaml
+# example configuration file
+# (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
+#    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
+smtp:
+    host:     localhost:587
+    user:     foobar
+    password: BARFOO
+email:
+    from:     me@whereever.com
+    to:       myself@whereever.com
+    subject:  Pack your rain gear!
+    message:  The forecast precipitation rate for today is {a:.2f} mm/h, maximum {m:2f} mm/h.
+place: Helsinki
+average_precipitation_rate_threshold: 0.1
+max_precipitation_rate_threshold: 0.5
+verbose: False
+```
+
+### Usage
+
+Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
+
+
+#### Systemd timer
+
+Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/master/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
+
+```sh
+systemctl --user daemon-reload
+systemctl --user enable --now wolkenbruch.timer 
+```
+
+If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
+
+```sh
+sudo loginctl enable-linger USERNAME
+```
```

### Comparing `wolkenbruch-0.6.4/README.md` & `wolkenbruch-0.6.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wolkenbruch
+Version: 0.6.5
+Summary: Checks the weather forecast for your home town and sends an e-mail reminder to pack your rain gear if precipitation is forecast.
+Home-page: https://gitlab.com/christoph.fink/wolkenbruch
+Author: Christoph Fink
+Author-email: christoph.fink@helsinki.fi
+License: GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: geocoder
+Requires-Dist: PyYAML
+Requires-Dist: requests
+
 ![rain cloud](extra/img/wolkenbruch_256x160.svg)
 
 # Wolkenbruch
 
 Checks the weather forecast for a configurable place and sends an e-mail
 reminder to pack your rain gear if precipitation is forecast.
```

### Comparing `wolkenbruch-0.6.4/setup.cfg` & `wolkenbruch-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.6.4/wolkenbruch/__init__.py` & `wolkenbruch-0.6.5/wolkenbruch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Checks the forecast precipitation rate for the next 14h and sends
 an e-mail to remind me to take my rain gear with me
 """
 
 __all__ = [
     "__version__",
-    "remind_me_if_it_rains"
+    "remind_me_if_it_rains",
 ]
 
 
 from .wolkenbruch import remind_me_if_it_rains
 
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch/__main__.py` & `wolkenbruch-0.6.5/wolkenbruch/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,22 +12,26 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-""" Check the precipitation for the next 14h at a given location and send
-    an e-mail to remind me to pack rain gear """
+"""
+Check the precipitation for the next 14h at a given location and send an e-mail
+to remind me to pack rain gear
+"""
 
 
 from .wolkenbruch import remind_me_if_it_rains
 
 
 def main():
-    """ Check the precipitation for the next 14h at a given location and send
-        an e-mail to remind me to pack rain gear """
+    """
+    Check the precipitation for the next 14h at a given location and send an
+    e-mail to remind me to pack rain gear
+    """
     remind_me_if_it_rains()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch/lib/__init__.py` & `wolkenbruch-0.6.5/wolkenbruch/lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program; if not, see <http://www.gnu.org/licenses/>.
-""" Wolkenbruch library function """
+"""Wolkenbruch library function"""
 
 __all__ = [
     "Config",
     "EMailSender",
-    "PrecipitationChecker"
+    "PrecipitationChecker",
 ]
 
 from .config import Config
 from .emailsender import EMailSender
 from .precipitationchecker import PrecipitationChecker
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch/lib/config.py` & `wolkenbruch-0.6.5/wolkenbruch/lib/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,42 +26,36 @@
 import os.path
 import warnings
 
 import yaml
 
 
 class Config:
-    """ Global configuration object
+    """Global configuration object
 
-        Tries to load configuration from YAML files in default locations
-        (/etc/{module}.yml, ~/.config/{module}.yml, %APPDATA%/{module}.yml,
-        ${XDG_CONFIG_HOME}/{module}.yml).
-
-        Configuration file location can be overriden by specifying
-        `config_files` or a base name `config_filesBaseName` (replaces
-        “{module}” in the file locations listed above)
-
-        Arguments:
-            content of the config file
-
-        Args:
-            config_files (list of str, optional): override configuration
-                file locations
-            config_files_basename (str): override configuration file names
+    Tries to load configuration from YAML files in default locations
+    (/etc/{module}.yml, ~/.config/{module}.yml, %APPDATA%/{module}.yml,
+    ${XDG_CONFIG_HOME}/{module}.yml).
+
+    Configuration file location can be overriden by specifying
+    `config_files` or a base name `config_filesBaseName` (replaces
+    “{module}” in the file locations listed above)
+
+    Arguments:
+        content of the config file
+
+    Args:
+        config_files (list of str, optional): override configuration
+            file locations
+        config_files_basename (str): override configuration file names
     """
-    DEFAULT_CONFIG = os.path.join(
-        os.path.dirname(__file__),
-        "default.yml"
-    )
-
-    def __init__(
-            self,
-            config_files=None,
-            config_files_basename=None
-    ):
+
+    DEFAULT_CONFIG = os.path.join(os.path.dirname(__file__), "default.yml")
+
+    def __init__(self, config_files=None, config_files_basename=None):
         self._config = {}
         self._config_files = []
 
         if config_files is not None:
             if not isinstance(config_files, (list, tuple)):
                 config_files = [config_files]
             self._config_files = config_files
@@ -70,35 +64,31 @@
             config_files_basename = self.__module__.split(".")[0]
 
             self._config_files = [
                 "/etc/{:s}.yml".format(config_files_basename),
                 os.path.abspath(
                     os.path.join(
                         (
-                            os.environ.get('APPDATA')
-                            or os.environ.get('XDG_CONFIG_HOME')
-                            or os.path.join(os.environ['HOME'], '.config')
+                            os.environ.get("APPDATA")
+                            or os.environ.get("XDG_CONFIG_HOME")
+                            or os.path.join(os.environ["HOME"], ".config")
                         ),
-                        "{:s}.yml".format(config_files_basename)
+                        "{:s}.yml".format(config_files_basename),
                     )
-                )
+                ),
             ]
 
         self._config = self._load_config()
 
     def _load_config(self):
         config = {}
 
         for config_file in self._config_files:
             try:
-                config.update(
-                    yaml.safe_load(
-                        open(config_file, "r", encoding="utf-8")
-                    )
-                )
+                config.update(yaml.safe_load(open(config_file, "r", encoding="utf-8")))
             except FileNotFoundError:
                 pass
 
         if config == {}:
             warnings.warn(
                 "No configuration found in files {}".format(
                     ",".join(self._config_files)
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch/lib/emailsender.py` & `wolkenbruch-0.6.5/wolkenbruch/lib/emailsender.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,84 +19,76 @@
 """ Sends e-mails (convenience wrapper around `smtplib` and `email.message` """
 
 
 import email.message
 import smtplib
 
 
-__all__ = [
-    "EMailSender"
-]
+__all__ = ["EMailSender"]
 
 
 class EMailSender:
-    """ Sends e-mails
+    """Sends e-mails
+
+    Args:
+        from_addr:  Sender address
+        to_addr:    Receiver address
+        subject:    Subject line
+        body:       e-mail text
+        smtp_host:  host name/ip address to use as an SMTP server,
+                    can contain port in the form [host]:[port]
+        smtp_user:  SMTP user name if authentication required
+        smtp_password: SMTP password if authentication required
+        starttls:   use TLS (default: True)
+    """
+
+    def __init__(
+        self,
+        from_addr="",
+        to_addr="",
+        subject="",
+        body="",
+        smtp_host="",
+        smtp_user="",
+        smtp_password="",
+        starttls=True,
+        *args,
+        **kwargs
+    ):
+        """
+        Sends e-mails
 
         Args:
             from_addr:  Sender address
             to_addr:    Receiver address
             subject:    Subject line
             body:       e-mail text
             smtp_host:  host name/ip address to use as an SMTP server,
                         can contain port in the form [host]:[port]
             smtp_user:  SMTP user name if authentication required
             smtp_password: SMTP password if authentication required
             starttls:   use TLS (default: True)
-    """
-
-    def __init__(
-            self,
-            from_addr="",
-            to_addr="",
-            subject="",
-            body="",
-            smtp_host="",
-            smtp_user="",
-            smtp_password="",
-            starttls=True,
-            *args,
-            **kwargs
-    ):
-        """
-            Sends e-mails
-
-            Args:
-                from_addr:  Sender address
-                to_addr:    Receiver address
-                subject:    Subject line
-                body:       e-mail text
-                smtp_host:  host name/ip address to use as an SMTP server,
-                            can contain port in the form [host]:[port]
-                smtp_user:  SMTP user name if authentication required
-                smtp_password: SMTP password if authentication required
-                starttls:   use TLS (default: True)
         """
         self.from_addr = from_addr
         self.to_addr = to_addr
         self.subject = subject
         self.body = body
 
         self.smtp_host = smtp_host
         self.smtp_user = smtp_user
         self.smtp_password = smtp_password
         self.starttls = starttls
 
     def send_message(self):
-        """ Sends a message to `to_addr` """
+        """Sends a message to `to_addr`"""
         with smtplib.SMTP(self.smtp_host) as smtp:
             if self.starttls:
                 smtp.starttls()
-            if (
-                    self.smtp_user != ""
-                    and self.smtp_password != ""
-            ):
-                smtp.login(
-                    self.smtp_user,
-                    self.smtp_password
-                )
+            if self.smtp_user != "" and self.smtp_password != "":
+                smtp.login(self.smtp_user, self.smtp_password)
 
             message = email.message.EmailMessage()
             message["From"] = self.from_addr
             message["To"] = self.to_addr
             message["Subject"] = self.subject
             message.set_content(self.body)
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch/lib/precipitationchecker.py` & `wolkenbruch-0.6.5/wolkenbruch/lib/precipitationchecker.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,42 +18,36 @@
 
 """ Checks the precipitation over the next n hours at a given location """
 
 
 import requests
 
 
-__all__ = [
-    "PrecipitationChecker"
-]
+__all__ = ["PrecipitationChecker"]
 
 
 class PrecipitationChecker:
-    """ Check the forecast precipitation at a location
+    """Check the forecast precipitation at a location
 
-        Args:
-            lat:        Latitude
-            lon:        Longitude
-            n_hours:    calculate the average precipitation
-                        rate for the next `n_hours` hours
+    Args:
+        lat:        Latitude
+        lon:        Longitude
+        n_hours:    calculate the average precipitation
+                    rate for the next `n_hours` hours
     """
+
     API_VERSION = "2.0"
-    API_ENDPOINT = "https://api.met.no/weatherapi/locationforecast/{VERSION:s}/compact".format(VERSION=API_VERSION)
+    API_ENDPOINT = (
+        f"https://api.met.no/weatherapi/locationforecast/{API_VERSION:s}/compact"
+    )
     API_HEADERS = {
-        "User-agent": "python-wolkenbruch (https://gitlab.com/christoph.fink/wolkenbruch/"
+        "User-agent": "python-wolkenbruch (https://gitlab.com/christophfink/wolkenbruch/"
     }
 
-    def __init__(
-            self,
-            lat,
-            lon,
-            n_hours=14,
-            *args,
-            **kwargs
-    ):
+    def __init__(self, lat, lon, n_hours=14, *args, **kwargs):
         """
         Check the forecast precipitation at a location.
 
         Args:
             lat:        Latitude
             lon:        Longitude
             n_hours:    calculate the average precipitation
@@ -66,22 +60,23 @@
         self.precipitation = []
 
     def _fetch_weather_forecast(self):
         forecast = requests.get(
             self.API_ENDPOINT,
             params={
                 "lat": self.lat,
-                "lon": self.lon
+                "lon": self.lon,
             },
-            headers=self.API_HEADERS
+            headers=self.API_HEADERS,
         )
         forecast = forecast.json()
 
         with open("/tmp/wolkenbruch.json", "w") as f:
             import json
+
             f.write(json.dumps(forecast, sort_keys=True, indent=4))
 
         self.precipitation = [
             timestamp["data"]["next_1_hours"]["details"]["precipitation_amount"]
             for timestamp in forecast["properties"]["timeseries"]
             if "next_1_hours" in timestamp["data"]
         ]
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch/wolkenbruch.py` & `wolkenbruch-0.6.5/wolkenbruch/wolkenbruch.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,86 +19,81 @@
 """ Reminds me if it rains """
 
 import statistics
 import sys
 
 import geocoder
 
-from .lib import (
-    Config,
-    EMailSender,
-    PrecipitationChecker
-)
+from .lib import Config, EMailSender, PrecipitationChecker
 
 
-__all__ = [
-    "remind_me_if_it_rains"
-]
+__all__ = ["remind_me_if_it_rains"]
 
 # How many hours to look into the future?
 N_HOURS = 14
 
 
 def remind_me_if_it_rains():
-    """ Remind me if rain is forecast """
+    """Remind me if rain is forecast"""
     config = Config()
 
     try:
         verbose = config["verbose"]
     except KeyError:
         verbose = False
 
-    lat, lon = geocoder.osm(config["place"]).latlng
-
-    hourly_precipitation_rates = \
-        PrecipitationChecker(lat, lon).hourly_precipitation_rates[:N_HOURS]
+    try:
+        lat, lon = geocoder.osm(config["place"]).latlng
+    except (TypeError, ValueError) as exception:
+        raise RuntimeError(
+            f"Could not find location ‘{config['place']}’"
+        ) from exception
+
+    hourly_precipitation_rates = PrecipitationChecker(
+        lat, lon
+    ).hourly_precipitation_rates[:N_HOURS]
 
-    average_precipitation_rate = \
-        statistics.fmean(hourly_precipitation_rates)
-    max_precipitation_rate = \
-        max(hourly_precipitation_rates)
+    average_precipitation_rate = statistics.fmean(hourly_precipitation_rates)
+    max_precipitation_rate = max(hourly_precipitation_rates)
 
     if verbose:
         print(
             (
                 "Average precipitation rate in {place:s} is {a:0.2f} mm/h "
                 + "over the next 14 hours, maximum {m:0.2f}. "
             ).format(
                 place=config["place"],
                 a=average_precipitation_rate,
-                m=max_precipitation_rate
+                m=max_precipitation_rate,
             ),
             file=sys.stderr,
-            end=""
+            end="",
         )
 
     if (
-            average_precipitation_rate
-            > config["average_precipitation_rate_threshold"]
-
-            or max_precipitation_rate
-            > config["max_precipitation_rate_threshold"]
+        average_precipitation_rate > config["average_precipitation_rate_threshold"]
+        or max_precipitation_rate > config["max_precipitation_rate_threshold"]
     ):
         EMailSender(
             config["email"]["from"],
             config["email"]["to"],
             config["email"]["subject"],
             config["email"]["message"].format(
                 a=average_precipitation_rate,
-                m=max_precipitation_rate
+                m=max_precipitation_rate,
             ),
             config["smtp"]["host"],
             config["smtp"]["user"],
-            config["smtp"]["password"]
+            config["smtp"]["password"],
         ).send_message()
 
         if verbose:
             print(
                 "Sending reminder to {:s} ".format(config["email"]["to"]),
-                file=sys.stderr
+                file=sys.stderr,
             )
     else:
         if verbose:
             print(
                 "NOT sending reminder to {:s} ".format(config["email"]["to"]),
-                file=sys.stderr
+                file=sys.stderr,
             )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch.egg-info/PKG-INFO` & `wolkenbruch-0.6.5/wolkenbruch.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,117 @@
 Metadata-Version: 2.1
 Name: wolkenbruch
-Version: 0.6.4
+Version: 0.6.5
 Summary: Checks the weather forecast for your home town and sends an e-mail reminder to pack your rain gear if precipitation is forecast.
 Home-page: https://gitlab.com/christoph.fink/wolkenbruch
 Author: Christoph Fink
 Author-email: christoph.fink@helsinki.fi
 License: GPLv3
-Description: ![rain cloud](extra/img/wolkenbruch_256x160.svg)
-        
-        # Wolkenbruch
-        
-        Checks the weather forecast for a configurable place and sends an e-mail
-        reminder to pack your rain gear if precipitation is forecast.
-        
-        Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses [OpenStreetmap](https://osm.org/) to find the location from place names.
-        
-        ### Dependencies
-        
-        Wolkenbruch is written in Python 3, and depends on the Python modules [geocoder](https://geocoder.readthedocs.io/), [requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
-        
-        ### Installation
-        
-        - *using `pip` or similar:*
-        
-        ```shell
-        pip3 install wolkenbruch
-        ```
-        
-        - *OR: manually:*
-        
-            - Clone this repository
-        
-            ```shell
-            git clone https://gitlab.com/christoph.fink/wolkenbruch.git
-            ```
-        
-            - Change to the cloned directory
-            - Use the Python `setuptools` to install the package:
-        
-            ```shell
-            cd wolkenbruch
-            python3 ./setup.py install
-            ```
-        
-        ### Configuration
-        
-        Copy the example configuration file [wolkenbruch.yml.example](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/master/wolkenbruch.yml.example) to a suiteable location, depending on your operating system:
-        
-        - on Linux systems:
-            - system-wide configuration: `/etc/wolkenbruch.yml`
-            - per-user configuration: 
-                - `~/.config/wolkenbruch.yml` OR
-                - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
-        - on MacOS systems:
-            - per-user configuration:
-                - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
-        - on Microsoft Windows systems:
-            - per-user configuration:
-                `%APPDATA%\wolkenbruch.yml`
-        
-        Adapt the configuration:
-        
-        - Change the place the forecast searches for. For bigger cities their name might be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to smaller places, or places that share their name with other places in different parts of the world, you might have to add a country, state or county name, e.g. ”Springfield, Fife”.
-        - Adapt the SMTP host and credentials (leave user and password empty if not authentication is required). **Be careful:** the credentials are (obviously) saved in plain-text. Protect access to the configuration file, e.g. on a GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
-        - Set the sender and receiver e-mail address (they can and often will be the same address)
-        - If you feel like it, change the subject line and message body of the e-mail. The message body can contain [Python string formatting code](https://docs.python.org/3/library/string.html#formatstrings) for a float variables `a` and `m` (the average and maximum precipitation rates over the next 14 hours, in mm/h).
-        - Adjust the amount of rain you can stand: `average_precipitation_rate_threshold` is the average precipitation rate over the next 14 hours (in mm per hour) that has to be exceeded to send you a reminder, `max_precipitation_rate_threshold` the highest single hourly value that makes you want to not forget your rain gear.
-        - The verbose flag toggles whether `wolkenbruch` prints a status or operated silently.
-        
-        ```yaml
-        # example configuration file
-        # (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
-        #    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
-        smtp:
-            host:     localhost:587
-            user:     foobar
-            password: BARFOO
-        email:
-            from:     me@whereever.com
-            to:       myself@whereever.com
-            subject:  Pack your rain gear!
-            message:  The forecast precipitation rate for today is {a:.2f} mm/h, maximum {m:2f} mm/h.
-        place: Helsinki
-        average_precipitation_rate_threshold: 0.1
-        max_precipitation_rate_threshold: 0.5
-        verbose: False
-        ```
-        
-        ### Usage
-        
-        Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
-        
-        
-        #### Systemd timer
-        
-        Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/master/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
-        
-        ```sh
-        systemctl --user daemon-reload
-        systemctl --user enable --now wolkenbruch.timer 
-        ```
-        
-        If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
-        
-        ```sh
-        sudo loginctl enable-linger USERNAME
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: geocoder
+Requires-Dist: PyYAML
+Requires-Dist: requests
+
+![rain cloud](extra/img/wolkenbruch_256x160.svg)
+
+# Wolkenbruch
+
+Checks the weather forecast for a configurable place and sends an e-mail
+reminder to pack your rain gear if precipitation is forecast.
+
+Wolkenbruch makes use of the [MET Norway API](https://api.met.no/), and uses [OpenStreetmap](https://osm.org/) to find the location from place names.
+
+### Dependencies
+
+Wolkenbruch is written in Python 3, and depends on the Python modules [geocoder](https://geocoder.readthedocs.io/), [requests](https://2.python-requests.org/) and [yaml](https://pyyaml.org/).
+
+### Installation
+
+- *using `pip` or similar:*
+
+```shell
+pip3 install wolkenbruch
+```
+
+- *OR: manually:*
+
+    - Clone this repository
+
+    ```shell
+    git clone https://gitlab.com/christoph.fink/wolkenbruch.git
+    ```
+
+    - Change to the cloned directory
+    - Use the Python `setuptools` to install the package:
+
+    ```shell
+    cd wolkenbruch
+    python3 ./setup.py install
+    ```
+
+### Configuration
+
+Copy the example configuration file [wolkenbruch.yml.example](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/master/wolkenbruch.yml.example) to a suiteable location, depending on your operating system:
+
+- on Linux systems:
+    - system-wide configuration: `/etc/wolkenbruch.yml`
+    - per-user configuration: 
+        - `~/.config/wolkenbruch.yml` OR
+        - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
+- on MacOS systems:
+    - per-user configuration:
+        - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
+- on Microsoft Windows systems:
+    - per-user configuration:
+        `%APPDATA%\wolkenbruch.yml`
+
+Adapt the configuration:
+
+- Change the place the forecast searches for. For bigger cities their name might be sufficient (Unicode is supported), e.g. “Helsinki”. When it comes to smaller places, or places that share their name with other places in different parts of the world, you might have to add a country, state or county name, e.g. ”Springfield, Fife”.
+- Adapt the SMTP host and credentials (leave user and password empty if not authentication is required). **Be careful:** the credentials are (obviously) saved in plain-text. Protect access to the configuration file, e.g. on a GNU/Linux or MacOS system using `chmod 0600 "~/.config/wolkenbruch.yml"`.
+- Set the sender and receiver e-mail address (they can and often will be the same address)
+- If you feel like it, change the subject line and message body of the e-mail. The message body can contain [Python string formatting code](https://docs.python.org/3/library/string.html#formatstrings) for a float variables `a` and `m` (the average and maximum precipitation rates over the next 14 hours, in mm/h).
+- Adjust the amount of rain you can stand: `average_precipitation_rate_threshold` is the average precipitation rate over the next 14 hours (in mm per hour) that has to be exceeded to send you a reminder, `max_precipitation_rate_threshold` the highest single hourly value that makes you want to not forget your rain gear.
+- The verbose flag toggles whether `wolkenbruch` prints a status or operated silently.
+
+```yaml
+# example configuration file
+# (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
+#    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
+smtp:
+    host:     localhost:587
+    user:     foobar
+    password: BARFOO
+email:
+    from:     me@whereever.com
+    to:       myself@whereever.com
+    subject:  Pack your rain gear!
+    message:  The forecast precipitation rate for today is {a:.2f} mm/h, maximum {m:2f} mm/h.
+place: Helsinki
+average_precipitation_rate_threshold: 0.1
+max_precipitation_rate_threshold: 0.5
+verbose: False
+```
+
+### Usage
+
+Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
+
+
+#### Systemd timer
+
+Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/master/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
+
+```sh
+systemctl --user daemon-reload
+systemctl --user enable --now wolkenbruch.timer 
+```
+
+If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
+
+```sh
+sudo loginctl enable-linger USERNAME
+```
```

### Comparing `wolkenbruch-0.6.4/wolkenbruch.egg-info/SOURCES.txt` & `wolkenbruch-0.6.5/wolkenbruch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 wolkenbruch.yml.example
 extra/systemd/wolkenbruch.service
 extra/systemd/wolkenbruch.timer
 wolkenbruch/__init__.py
```

