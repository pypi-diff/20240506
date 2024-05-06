# Comparing `tmp/pyalicat-0.0.1.tar.gz` & `tmp/pyalicat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalicat-0.0.1.tar", max compression
+gzip compressed data, was "pyalicat-0.0.2.tar", max compression
```

## Comparing `pyalicat-0.0.1.tar` & `pyalicat-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2024-03-14 17:40:14.065679 pyalicat-0.0.1/LICENSE
--rw-r--r--   0        0        0     6349 2024-04-04 18:41:03.386845 pyalicat-0.0.1/README.md
--rw-r--r--   0        0        0      472 2024-03-14 17:40:14.069679 pyalicat-0.0.1/pyalicat/__init__.py
--rw-r--r--   0        0        0    15732 2024-04-04 17:46:44.027066 pyalicat-0.0.1/pyalicat/codes.json
--rw-r--r--   0        0        0     7596 2024-04-04 17:46:44.028066 pyalicat-0.0.1/pyalicat/comm.py
--rw-r--r--   0        0        0     1905 2024-04-04 17:46:44.028066 pyalicat-0.0.1/pyalicat/daq.py
--rw-r--r--   0        0        0    53159 2024-04-04 17:46:44.028066 pyalicat-0.0.1/pyalicat/device.py
--rw-r--r--   0        0        0      708 2024-04-04 17:46:44.028066 pyalicat-0.0.1/pyalicat/example.py
--rw-r--r--   0        0        0      281 2024-04-04 17:46:44.028066 pyalicat-0.0.1/pyalicat/util.py
--rw-r--r--   0        0        0     2858 2024-04-04 18:37:41.764597 pyalicat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7393 1970-01-01 00:00:00.000000 pyalicat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-03-14 19:50:17.719635 pyalicat-0.0.2/LICENSE
+-rw-r--r--   0        0        0      491 2024-03-14 19:50:17.729972 pyalicat-0.0.2/pyalicat/__init__.py
+-rw-r--r--   0        0        0    16371 2024-04-03 20:55:16.187178 pyalicat-0.0.2/pyalicat/codes.json
+-rw-r--r--   0        0        0     7708 2024-05-06 00:00:52.786672 pyalicat-0.0.2/pyalicat/comm.py
+-rw-r--r--   0        0        0     4346 2024-05-06 00:00:52.792672 pyalicat-0.0.2/pyalicat/daq.py
+-rw-r--r--   0        0        0    65629 2024-05-06 00:00:52.797675 pyalicat-0.0.2/pyalicat/device.py
+-rw-r--r--   0        0        0      740 2024-03-29 22:10:35.930094 pyalicat-0.0.2/pyalicat/example.py
+-rw-r--r--   0        0        0     2782 2024-05-06 00:00:52.804673 pyalicat-0.0.2/pyalicat/util.py
+-rw-r--r--   0        0        0     2971 2024-05-06 00:00:52.809672 pyalicat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6479 2024-04-07 19:19:18.216851 pyalicat-0.0.2/README.md
+-rw-r--r--   0        0        0     7574 1970-01-01 00:00:00.000000 pyalicat-0.0.2/PKG-INFO
```

### Comparing `pyalicat-0.0.1/LICENSE` & `pyalicat-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-Copyright (c) 2024 ulfsri
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
+The MIT License (MIT)
+Copyright (c) 2024 ulfsri
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pyalicat-0.0.1/README.md` & `pyalicat-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # pyAlicat
+![pyAlicat](docs/assets/images/logo_pyalicat.svg)
 
 <div align="center">
 
 [![Build status](https://github.com/ulfsri/pyAlicat/workflows/build/badge.svg?branch=main&event=push)](https://github.com/ulfsri/pyAlicat/actions?query=workflow%3Abuild)
-[![Python Version](https://img.shields.io/pypi/pyversions/pyAlicat.svg)](https://pypi.org/project/pyAlicat/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyalicat.svg)](https://pypi.org/project/pyAlicat/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ulfsri/pyAlicat/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ulfsri/pyAlicat/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ulfsri/pyAlicat/releases)
-[![License](https://img.shields.io/github/license/ulfsri/pyAlicat)](https://github.com/ulfsri/pyAlicat/blob/main/LICENSE)
+[![License](https://img.shields.io/github/license/ulfsri/pyalicat)](https://github.com/ulfsri/pyAlicat/blob/main/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 Python API for acquisition and control of Alicat mass flow meters and controllers.
 
 See [Alicat Serial Communications Guide](https://www.alicat.com/wp-content/documents/Alicat-Serial-Primer.pdf) for reference
 
 </div>
@@ -269,7 +270,9 @@
   howpublished = {\url{https://github.com/ulfsri/pyAlicat}}
 }
 ```
 
 ## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
 This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
+
+Logo design by [Natalya England](https://www.instagram.com/natalya.england22/)
```

### Comparing `pyalicat-0.0.1/PKG-INFO` & `pyalicat-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
-Name: pyalicat
-Version: 0.0.1
+Name: pyAlicat
+Version: 0.0.2
 Summary: Python API for acquisition and control of Alicat mass flow meters and controllers.
 Home-page: https://github.com/ulfsri/pyAlicat
 License: MIT
 Author: ulfsri
 Author-email: grayson.bellamy@ul.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: trio (>=0.25.0,<0.26.0)
 Requires-Dist: trio-serial (>=0.4.0,<0.5.0)
 Project-URL: Repository, https://github.com/ulfsri/pyAlicat
 Description-Content-Type: text/markdown
 
 # pyAlicat
+![pyAlicat](docs/assets/images/logo_pyalicat.svg)
 
 <div align="center">
 
 [![Build status](https://github.com/ulfsri/pyAlicat/workflows/build/badge.svg?branch=main&event=push)](https://github.com/ulfsri/pyAlicat/actions?query=workflow%3Abuild)
-[![Python Version](https://img.shields.io/pypi/pyversions/pyAlicat.svg)](https://pypi.org/project/pyAlicat/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyalicat.svg)](https://pypi.org/project/pyAlicat/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ulfsri/pyAlicat/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ulfsri/pyAlicat/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ulfsri/pyAlicat/releases)
-[![License](https://img.shields.io/github/license/ulfsri/pyAlicat)](https://github.com/ulfsri/pyAlicat/blob/main/LICENSE)
+[![License](https://img.shields.io/github/license/ulfsri/pyalicat)](https://github.com/ulfsri/pyAlicat/blob/main/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 Python API for acquisition and control of Alicat mass flow meters and controllers.
 
 See [Alicat Serial Communications Guide](https://www.alicat.com/wp-content/documents/Alicat-Serial-Primer.pdf) for reference
 
 </div>
@@ -296,7 +298,9 @@
 }
 ```
 
 ## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
 This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
 
+Logo design by [Natalya England](https://www.instagram.com/natalya.england22/)
+
```

