# Comparing `tmp/wolkenbruch-0.6.5.tar.gz` & `tmp/wolkenbruch-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolkenbruch-0.6.5.tar", last modified: Mon May  6 08:29:13 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `wolkenbruch-0.6.5.tar` & `wolkenbruch-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5062 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4428 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.440239 wolkenbruch-0.6.5/extra/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.442239 wolkenbruch-0.6.5/extra/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/extra/systemd/wolkenbruch.service
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/extra/systemd/wolkenbruch.timer
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.443239 wolkenbruch-0.6.5/wolkenbruch/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2024-05-06 08:29:11.000000 wolkenbruch-0.6.5/wolkenbruch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.445239 wolkenbruch-0.6.5/wolkenbruch/lib/
--rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3316 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/emailsender.py
--rw-rw-rw-   0 root         (0) root         (0)     2869 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/lib/precipitationchecker.py
--rw-rw-rw-   0 root         (0) root         (0)     3014 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch/wolkenbruch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:29:13.446239 wolkenbruch-0.6.5/wolkenbruch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5062 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      544 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 08:29:13.000000 wolkenbruch-0.6.5/wolkenbruch.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-06 08:28:57.000000 wolkenbruch-0.6.5/wolkenbruch.yml.example
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.flake8
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.pylintrc
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/img/wolkenbruch.svg
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/img/wolkenbruch_256x160.svg
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/img/wolkenbruch_bw_256x256.svg
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/systemd/wolkenbruch.service
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/extra/systemd/wolkenbruch.timer
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/__init__.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/__main__.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/config.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/emailsender.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/precipitationchecker.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/wolkenbruch.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/src/wolkenbruch/wolkenbruch.yml.template
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/README.md
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 wolkenbruch-0.7.0/PKG-INFO
```

### Comparing `wolkenbruch-0.6.5/LICENSE` & `wolkenbruch-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.6.5/PKG-INFO` & `wolkenbruch-0.7.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wolkenbruch
-Version: 0.6.5
-Summary: Checks the weather forecast for your home town and sends an e-mail reminder to pack your rain gear if precipitation is forecast.
-Home-page: https://gitlab.com/christoph.fink/wolkenbruch
-Author: Christoph Fink
-Author-email: christoph.fink@helsinki.fi
-License: GPLv3
-Classifier: Programming Language :: Python :: 3
+Version: 0.7.0
+Summary: Send an e-mail reminder if precipitation is forecast
+Project-URL: Documentation, https://gitlab.com/christophfink/wolkenbruch/
+Project-URL: Repository, https://gitlab.com/christophfink/wolkenbruch/
+Project-URL: Change log, https://gitlab.com/christophfink/wolkenbruch/-/blob/master/CHANGELOG.md
+Project-URL: Bug tracker, https://gitlab.com/christophfink/wolkenbruch/-/issues
+Author-email: Christoph Fink <christoph.fink@gmail.com>
+License: GPL-3.0-or-later or MIT
+License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
 Requires-Dist: geocoder
-Requires-Dist: PyYAML
+Requires-Dist: importlib-resources
+Requires-Dist: pyyaml
 Requires-Dist: requests
+Description-Content-Type: text/markdown
 
 ![rain cloud](extra/img/wolkenbruch_256x160.svg)
 
 # Wolkenbruch
 
 Checks the weather forecast for a configurable place and sends an e-mail
 reminder to pack your rain gear if precipitation is forecast.
@@ -50,15 +54,15 @@
     ```shell
     cd wolkenbruch
     python3 ./setup.py install
     ```
 
 ### Configuration
 
-Copy the example configuration file [wolkenbruch.yml.example](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/master/wolkenbruch.yml.example) to a suiteable location, depending on your operating system:
+Copy the example configuration file [wolkenbruch.yml.template](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/main/src/wolkenbruch/wolkenbruch.yml.template) to a suiteable location, depending on your operating system:
 
 - on Linux systems:
     - system-wide configuration: `/etc/wolkenbruch.yml`
     - per-user configuration: 
         - `~/.config/wolkenbruch.yml` OR
         - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
 - on MacOS systems:
@@ -99,15 +103,15 @@
 ### Usage
 
 Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
 
 
 #### Systemd timer
 
-Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/master/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
+Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/main/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
 
 ```sh
 systemctl --user daemon-reload
 systemctl --user enable --now wolkenbruch.timer 
 ```
 
 If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
```

### Comparing `wolkenbruch-0.6.5/README.md` & `wolkenbruch-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ```shell
     cd wolkenbruch
     python3 ./setup.py install
     ```
 
 ### Configuration
 
-Copy the example configuration file [wolkenbruch.yml.example](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/master/wolkenbruch.yml.example) to a suiteable location, depending on your operating system:
+Copy the example configuration file [wolkenbruch.yml.template](https://gitlab.com/christoph.fink/wolkenbruch/-/raw/main/src/wolkenbruch/wolkenbruch.yml.template) to a suiteable location, depending on your operating system:
 
 - on Linux systems:
     - system-wide configuration: `/etc/wolkenbruch.yml`
     - per-user configuration: 
         - `~/.config/wolkenbruch.yml` OR
         - `${XDG_CONFIG_HOME}/wolkenbruch.yml`
 - on MacOS systems:
@@ -82,15 +82,15 @@
 ### Usage
 
 Run `wolkenbruch` to check the precipitation for the next 14 hours and send you an e-mail reminder. Ideally, set up a cron job or a systemd timer to run `wolkenbruch` e.g. every morning.
 
 
 #### Systemd timer
 
-Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/master/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
+Copy `wolkenbruch.service` and `wolkenbruch.timer` from [extra/systemd/](https://gitlab.com/christoph.fink/wolkenbruch/-/tree/main/extra/systemd/) to `/etc/systemd/user/` or `~/.config/systemd/user/` and enable the timer to run wolkenbruch at 6:30 every morning:
 
 ```sh
 systemctl --user daemon-reload
 systemctl --user enable --now wolkenbruch.timer 
 ```
 
 If you want the systemd timer to trigger when you’re not logged in, enable [_lingering_](https://wiki.archlinux.org/index.php/Systemd/User#Automatic_start-up_of_systemd_user_instances) for your user:
```

### Comparing `wolkenbruch-0.6.5/wolkenbruch/__init__.py` & `wolkenbruch-0.7.0/src/wolkenbruch/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     "remind_me_if_it_rains",
 ]
 
 
 from .wolkenbruch import remind_me_if_it_rains
 
 
-__version__ = "0.6.5"
+__version__ = "0.7.0"
```

### Comparing `wolkenbruch-0.6.5/wolkenbruch/__main__.py` & `wolkenbruch-0.7.0/src/wolkenbruch/__main__.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.6.5/wolkenbruch/lib/emailsender.py` & `wolkenbruch-0.7.0/src/wolkenbruch/emailsender.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         subject="",
         body="",
         smtp_host="",
         smtp_user="",
         smtp_password="",
         starttls=True,
         *args,
-        **kwargs
+        **kwargs,
     ):
         """
         Sends e-mails
 
         Args:
             from_addr:  Sender address
             to_addr:    Receiver address
```

### Comparing `wolkenbruch-0.6.5/wolkenbruch/lib/precipitationchecker.py` & `wolkenbruch-0.7.0/src/wolkenbruch/precipitationchecker.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.6.5/wolkenbruch/wolkenbruch.py` & `wolkenbruch-0.7.0/src/wolkenbruch/wolkenbruch.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 """ Reminds me if it rains """
 
 import statistics
 import sys
 
 import geocoder
 
-from .lib import Config, EMailSender, PrecipitationChecker
+from config import Config
+from emailsender import EMailSender
+from precipitationchecker import PrecipitationChecker
 
 
 __all__ = ["remind_me_if_it_rains"]
 
 # How many hours to look into the future?
 N_HOURS = 14
```

