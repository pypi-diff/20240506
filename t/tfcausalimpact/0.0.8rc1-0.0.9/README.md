# Comparing `tmp/tfcausalimpact-0.0.8rc1.tar.gz` & `tmp/tfcausalimpact-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tfcausalimpact-0.0.8rc1.tar", last modified: Thu Sep 30 21:00:45 2021, max compression
+gzip compressed data, was "dist/tfcausalimpact-0.0.9.tar", last modified: Fri Oct  8 22:11:05 2021, max compression
```

## Comparing `tfcausalimpact-0.0.8rc1.tar` & `tfcausalimpact-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 21:00:45.600095 tfcausalimpact-0.0.8rc1/
--rw-rw-r--   0 root         (0) root         (0)    11357 2020-08-17 14:59:33.000000 tfcausalimpact-0.0.8rc1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       85 2020-12-16 13:32:50.000000 tfcausalimpact-0.0.8rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9287 2021-09-30 21:00:45.600095 tfcausalimpact-0.0.8rc1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8096 2021-09-20 13:04:07.000000 tfcausalimpact-0.0.8rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 21:00:45.596096 tfcausalimpact-0.0.8rc1/causalimpact/
--rw-rw-r--   0 root         (0) root         (0)      664 2020-12-31 01:14:51.000000 tfcausalimpact-0.0.8rc1/causalimpact/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      599 2021-09-30 19:20:24.000000 tfcausalimpact-0.0.8rc1/causalimpact/__version__.py
--rw-rw-r--   0 root         (0) root         (0)    18024 2021-09-30 20:01:09.000000 tfcausalimpact-0.0.8rc1/causalimpact/data.py
--rw-rw-r--   0 root         (0) root         (0)    14956 2021-09-29 14:27:06.000000 tfcausalimpact-0.0.8rc1/causalimpact/inferences.py
--rw-rw-r--   0 root         (0) root         (0)    14914 2021-09-29 00:52:59.000000 tfcausalimpact-0.0.8rc1/causalimpact/main.py
--rw-rw-r--   0 root         (0) root         (0)     3833 2021-02-26 22:28:06.000000 tfcausalimpact-0.0.8rc1/causalimpact/misc.py
--rw-rw-r--   0 root         (0) root         (0)    21280 2021-09-29 23:36:23.000000 tfcausalimpact-0.0.8rc1/causalimpact/model.py
--rw-rw-r--   0 root         (0) root         (0)     6345 2021-09-30 20:06:39.000000 tfcausalimpact-0.0.8rc1/causalimpact/plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 21:00:45.584096 tfcausalimpact-0.0.8rc1/causalimpact/summary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 21:00:45.596096 tfcausalimpact-0.0.8rc1/causalimpact/summary/templates/
--rw-rw-r--   0 root         (0) root         (0)     5026 2020-12-16 13:32:50.000000 tfcausalimpact-0.0.8rc1/causalimpact/summary/templates/report
--rw-rw-r--   0 root         (0) root         (0)     4181 2020-12-16 13:32:50.000000 tfcausalimpact-0.0.8rc1/causalimpact/summary/templates/summary
--rw-rw-r--   0 root         (0) root         (0)     2841 2021-02-27 00:57:02.000000 tfcausalimpact-0.0.8rc1/causalimpact/summary.py
--rw-rw-r--   0 root         (0) root         (0)      144 2021-09-30 21:00:45.600095 tfcausalimpact-0.0.8rc1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3549 2021-09-29 14:00:46.000000 tfcausalimpact-0.0.8rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-30 21:00:45.600095 tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     9287 2021-09-30 21:00:45.000000 tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      524 2021-09-30 21:00:45.000000 tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2021-09-30 21:00:45.000000 tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       91 2021-09-30 21:00:45.000000 tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2021-09-30 21:00:45.000000 tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-08 22:11:05.100309 tfcausalimpact-0.0.9/
+-rw-rw-r--   0 root         (0) root         (0)    11357 2020-08-17 14:59:33.000000 tfcausalimpact-0.0.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       85 2020-12-16 13:32:50.000000 tfcausalimpact-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9282 2021-10-08 22:11:05.100309 tfcausalimpact-0.0.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8096 2021-09-20 13:04:07.000000 tfcausalimpact-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-08 22:11:05.100309 tfcausalimpact-0.0.9/causalimpact/
+-rw-rw-r--   0 root         (0) root         (0)      664 2020-12-31 01:14:51.000000 tfcausalimpact-0.0.9/causalimpact/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      594 2021-10-08 22:08:17.000000 tfcausalimpact-0.0.9/causalimpact/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)    18024 2021-10-01 14:32:31.000000 tfcausalimpact-0.0.9/causalimpact/data.py
+-rw-rw-r--   0 root         (0) root         (0)    14956 2021-10-01 14:32:31.000000 tfcausalimpact-0.0.9/causalimpact/inferences.py
+-rw-rw-r--   0 root         (0) root         (0)    14914 2021-10-01 14:32:31.000000 tfcausalimpact-0.0.9/causalimpact/main.py
+-rw-rw-r--   0 root         (0) root         (0)     3833 2021-02-26 22:28:06.000000 tfcausalimpact-0.0.9/causalimpact/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    21280 2021-10-01 14:32:31.000000 tfcausalimpact-0.0.9/causalimpact/model.py
+-rw-rw-r--   0 root         (0) root         (0)     6345 2021-10-01 14:32:31.000000 tfcausalimpact-0.0.9/causalimpact/plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-08 22:11:05.092308 tfcausalimpact-0.0.9/causalimpact/summary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-08 22:11:05.100309 tfcausalimpact-0.0.9/causalimpact/summary/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5026 2020-12-16 13:32:50.000000 tfcausalimpact-0.0.9/causalimpact/summary/templates/report
+-rw-rw-r--   0 root         (0) root         (0)     4181 2020-12-16 13:32:50.000000 tfcausalimpact-0.0.9/causalimpact/summary/templates/summary
+-rw-rw-r--   0 root         (0) root         (0)     2841 2021-02-27 00:57:02.000000 tfcausalimpact-0.0.9/causalimpact/summary.py
+-rw-rw-r--   0 root         (0) root         (0)      144 2021-10-08 22:11:05.100309 tfcausalimpact-0.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3547 2021-10-08 22:07:51.000000 tfcausalimpact-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-08 22:11:05.100309 tfcausalimpact-0.0.9/tfcausalimpact.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9282 2021-10-08 22:11:05.000000 tfcausalimpact-0.0.9/tfcausalimpact.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2021-10-08 22:11:05.000000 tfcausalimpact-0.0.9/tfcausalimpact.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-08 22:11:05.000000 tfcausalimpact-0.0.9/tfcausalimpact.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2021-10-08 22:11:05.000000 tfcausalimpact-0.0.9/tfcausalimpact.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-10-08 22:11:05.000000 tfcausalimpact-0.0.9/tfcausalimpact.egg-info/top_level.txt
```

### Comparing `tfcausalimpact-0.0.8rc1/LICENSE` & `tfcausalimpact-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/PKG-INFO` & `tfcausalimpact-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfcausalimpact
-Version: 0.0.8rc1
+Version: 0.0.9
 Summary: Python version of Google's Causal Impact model on top of Tensorflow Probability.
 Home-page: https://github.com/WillianFuks/tfcausalimpact
 Author: Willian Fuks
 Author-email: willian.fuks@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WillianFuks/tfcausalimpact
 Keywords: causal impact
@@ -19,15 +19,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3, <3.10.*
+Requires-Python: >=3, <3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 # tfcausalimpact
 [![Build Status](https://travis-ci.com/WillianFuks/tfcausalimpact.svg?branch=master)](https://travis-ci.com/WillianFuks/tfcausalimpact) [![Coverage Status](https://coveralls.io/repos/github/WillianFuks/tfcausalimpact/badge.svg?branch=master)](https://coveralls.io/github/WillianFuks/tfcausalimpact?branch=master) [![GitHub license](https://img.shields.io/github/license/WillianFuks/tfcausalimpact.svg)](https://github.com/WillianFuks/tfcausalimpact/blob/master/LICENSE) [![PyPI version](https://badge.fury.io/py/tfcausalimpact.svg)](https://badge.fury.io/py/tfcausalimpact) [![Pyversions](https://img.shields.io/pypi/pyversions/tfcausalimpact.svg)](https://pypi.python.org/pypi/tfcausalimpact)
```

### Comparing `tfcausalimpact-0.0.8rc1/README.md` & `tfcausalimpact-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/__init__.py` & `tfcausalimpact-0.0.9/causalimpact/__init__.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/__version__.py` & `tfcausalimpact-0.0.9/causalimpact/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '0.0.8-rc.1'
+__version__ = '0.0.9'
```

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/data.py` & `tfcausalimpact-0.0.9/causalimpact/data.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/inferences.py` & `tfcausalimpact-0.0.9/causalimpact/inferences.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/main.py` & `tfcausalimpact-0.0.9/causalimpact/main.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/misc.py` & `tfcausalimpact-0.0.9/causalimpact/misc.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/model.py` & `tfcausalimpact-0.0.9/causalimpact/model.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/plot.py` & `tfcausalimpact-0.0.9/causalimpact/plot.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/summary/templates/report` & `tfcausalimpact-0.0.9/causalimpact/summary/templates/report`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/summary/templates/summary` & `tfcausalimpact-0.0.9/causalimpact/summary/templates/summary`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/causalimpact/summary.py` & `tfcausalimpact-0.0.9/causalimpact/summary.py`

 * *Files identical despite different names*

### Comparing `tfcausalimpact-0.0.8rc1/setup.py` & `tfcausalimpact-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,10 +112,10 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering',
     ],
     project_urls={
         'Source': 'https://github.com/WillianFuks/tfcausalimpact'
     },
-    python_requires='>=3, <3.10.*',
+    python_requires='>=3, <3.10',
     test_suite='tests'
 )
```

### Comparing `tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/PKG-INFO` & `tfcausalimpact-0.0.9/tfcausalimpact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfcausalimpact
-Version: 0.0.8rc1
+Version: 0.0.9
 Summary: Python version of Google's Causal Impact model on top of Tensorflow Probability.
 Home-page: https://github.com/WillianFuks/tfcausalimpact
 Author: Willian Fuks
 Author-email: willian.fuks@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WillianFuks/tfcausalimpact
 Keywords: causal impact
@@ -19,15 +19,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3, <3.10.*
+Requires-Python: >=3, <3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 # tfcausalimpact
 [![Build Status](https://travis-ci.com/WillianFuks/tfcausalimpact.svg?branch=master)](https://travis-ci.com/WillianFuks/tfcausalimpact) [![Coverage Status](https://coveralls.io/repos/github/WillianFuks/tfcausalimpact/badge.svg?branch=master)](https://coveralls.io/github/WillianFuks/tfcausalimpact?branch=master) [![GitHub license](https://img.shields.io/github/license/WillianFuks/tfcausalimpact.svg)](https://github.com/WillianFuks/tfcausalimpact/blob/master/LICENSE) [![PyPI version](https://badge.fury.io/py/tfcausalimpact.svg)](https://badge.fury.io/py/tfcausalimpact) [![Pyversions](https://img.shields.io/pypi/pyversions/tfcausalimpact.svg)](https://pypi.python.org/pypi/tfcausalimpact)
```

### Comparing `tfcausalimpact-0.0.8rc1/tfcausalimpact.egg-info/SOURCES.txt` & `tfcausalimpact-0.0.9/tfcausalimpact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

