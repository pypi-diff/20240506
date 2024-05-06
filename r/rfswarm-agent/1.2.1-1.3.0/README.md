# Comparing `tmp/rfswarm-agent-1.2.1.tar.gz` & `tmp/rfswarm_agent-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-agent-1.2.1.tar", last modified: Mon Feb 19 03:36:33 2024, max compression
+gzip compressed data, was "rfswarm_agent-1.3.0.tar", last modified: Mon May  6 03:03:29 2024, max compression
```

## Comparing `rfswarm-agent-1.2.1.tar` & `rfswarm_agent-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,16 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.174565 rfswarm-agent-1.2.1/
--rw-r--r--   0 dave       (501) staff       (20)    35149 2019-11-02 13:28:40.000000 rfswarm-agent-1.2.1/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)     3152 2024-02-19 03:36:33.174226 rfswarm-agent-1.2.1/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     6597 2024-02-02 01:15:20.000000 rfswarm-agent-1.2.1/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.164932 rfswarm-agent-1.2.1/rfswarm_agent/
--rw-r--r--   0 dave       (501) staff       (20)       53 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/rfswarm_agent/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)    57833 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/rfswarm_agent/rfswarm_agent.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.168087 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)     3152 2024-02-19 03:36:33.000000 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      553 2024-02-19 03:36:33.000000 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2024-02-19 03:36:33.000000 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       71 2024-02-19 03:36:33.000000 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/entry_points.txt
--rw-r--r--   0 dave       (501) staff       (20)       44 2024-02-19 03:36:33.000000 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       21 2024-02-19 03:36:33.000000 rfswarm-agent-1.2.1/rfswarm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.173649 rfswarm-agent-1.2.1/robots/
--rw-r--r--   0 dave       (501) staff       (20)      818 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/PythonListener.py
--rw-r--r--   0 dave       (501) staff       (20)      466 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/RFSListener.py
--rw-r--r--   0 dave       (501) staff       (20)     3689 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/RFSListener2.py
--rw-r--r--   0 dave       (501) staff       (20)       32 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/myLibrary.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/myLibrary1.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/myLibrary2.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/myLibrary3.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/myvariables.py
--rw-r--r--   0 dave       (501) staff       (20)     6843 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/svg5.py
--rw-r--r--   0 dave       (501) staff       (20)     1863 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/robots/with_file_not_closed.py
--rw-r--r--   0 dave       (501) staff       (20)     1138 2024-02-19 03:36:30.000000 rfswarm-agent-1.2.1/setup-agent.py
--rw-r--r--   0 dave       (501) staff       (20)       38 2024-02-19 03:36:33.174714 rfswarm-agent-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.591906 rfswarm_agent-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 03:03:06.000000 rfswarm_agent-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-06 03:03:29.591906 rfswarm_agent-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-06 03:03:06.000000 rfswarm_agent-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.591906 rfswarm_agent-1.3.0/rfswarm_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 03:03:08.000000 rfswarm_agent-1.3.0/rfswarm_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76726 2024-05-06 03:03:28.000000 rfswarm_agent-1.3.0/rfswarm_agent/rfswarm_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.591906 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-06 03:03:29.000000 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 03:03:29.000000 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 03:03:29.000000 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 03:03:29.000000 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 03:03:29.000000 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 03:03:29.000000 rfswarm_agent-1.3.0/rfswarm_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-06 03:03:28.000000 rfswarm_agent-1.3.0/setup-agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 03:03:29.591906 rfswarm_agent-1.3.0/setup.cfg
```

### Comparing `rfswarm-agent-1.2.1/LICENSE` & `rfswarm_agent-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-agent-1.2.1/PKG-INFO` & `rfswarm_agent-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: rfswarm-agent
-Version: 1.2.1
+Version: 1.3.0
 Summary: rfswarm Agent
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
-License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
 Project-URL: Source, https://github.com/damies13/rfswarm
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser
+Requires-Dist: requests
+Requires-Dist: robotframework
+Requires-Dist: psutil
 
 # rfswarm (Robot Framework Swarm)
 
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
@@ -54,9 +56,7 @@
 
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13/)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
-
-
```

### Comparing `rfswarm-agent-1.2.1/README.md` & `rfswarm_agent-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.3.0&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.3.0&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.3.0&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.3.0&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-agent-1.2.1/rfswarm_agent.egg-info/PKG-INFO` & `rfswarm_agent-1.3.0/rfswarm_agent.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: rfswarm-agent
-Version: 1.2.1
+Version: 1.3.0
 Summary: rfswarm Agent
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
-License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
 Project-URL: Source, https://github.com/damies13/rfswarm
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser
+Requires-Dist: requests
+Requires-Dist: robotframework
+Requires-Dist: psutil
 
 # rfswarm (Robot Framework Swarm)
 
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
@@ -54,9 +56,7 @@
 
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13/)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
-
-
```

### Comparing `rfswarm-agent-1.2.1/setup-agent.py` & `rfswarm_agent-1.3.0/setup-agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-agent",
-	version="1.2.1",
+	version="1.3.0",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm Agent",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*rfswarm_manager*", "build/*"]),
```

