# Comparing `tmp/picterra-1.2.2.tar.gz` & `tmp/picterra-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picterra-1.2.2.tar", last modified: Sat Jan 20 20:05:01 2024, max compression
+gzip compressed data, was "dist/picterra-2.0.0.tar", last modified: Mon May  6 09:24:32 2024, max compression
```

## Comparing `picterra-1.2.2.tar` & `picterra-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:05:01.000000 picterra-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-20 20:04:50.000000 picterra-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-20 20:05:01.000000 picterra-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-01-20 20:04:50.000000 picterra-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-20 20:05:01.000000 picterra-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-20 20:04:50.000000 picterra-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:05:01.000000 picterra-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-20 20:04:50.000000 picterra-1.2.2/src/picterra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36766 2024-01-20 20:04:50.000000 picterra-1.2.2/src/picterra/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-01-20 20:04:50.000000 picterra-1.2.2/src/picterra/nongeo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-20 20:05:01.000000 picterra-1.2.2/src/picterra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:05:01.000000 picterra-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-01-20 20:04:50.000000 picterra-1.2.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-01-20 20:04:50.000000 picterra-1.2.2/tests/test_nongeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:24:32.000000 picterra-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 09:24:28.000000 picterra-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-06 09:24:32.000000 picterra-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-06 09:24:28.000000 picterra-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 09:24:32.000000 picterra-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 09:24:28.000000 picterra-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:24:32.000000 picterra-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 09:24:28.000000 picterra-2.0.0/src/picterra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42069 2024-05-06 09:24:28.000000 picterra-2.0.0/src/picterra/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-06 09:24:28.000000 picterra-2.0.0/src/picterra/nongeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 09:24:32.000000 picterra-2.0.0/src/picterra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:24:32.000000 picterra-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    36903 2024-05-06 09:24:28.000000 picterra-2.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-06 09:24:28.000000 picterra-2.0.0/tests/test_nongeo.py
```

### Comparing `picterra-1.2.2/LICENSE` & `picterra-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picterra-1.2.2/PKG-INFO` & `picterra-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: picterra
-Version: 1.2.2
+Version: 2.0.0
 Summary: Picterra API client
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: lint
 License-File: LICENSE
 
 <a href="https://picterra.ch">
     <img
         src="https://storage.googleapis.com/cloud.picterra.ch/public/assets/logo/picterra_logo_640.png"
         alt="Picterra logo" title="Picterra" align="right" height="40" />
 </a>
 
 # Picterra Python API Client
 
 ![Tests](https://github.com/Picterra/picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/picterra-python/badge/?version=latest)](https://picterra-python.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/picterra)](https://pypi.org/project/picterra/)
 
 Easily integrate state-of-the-art machine learning models in your app
 
 ```python
 from picterra import APIClient
 
 # Replace this with the id of one of your detectors
@@ -35,15 +38,15 @@
 ```
 
 
 
 ## Installation
 
 ```
-pip install git+https://github.com/Picterra/picterra-python.git
+pip install picterra
 ```
 
 See the `examples` folder for examples.
 
 ## API Reference and User Guide available on [Read the Docs](https://picterra-python.readthedocs.io/)
 
 [![Read the Docs](https://storage.googleapis.com/cloud.picterra.ch/external/assets/python_api_docs_screenshot.png)](https://picterra-python.readthedocs.io/)
@@ -51,7 +54,17 @@
 
 ## Development
 
 In order to test locally, run:
 ```bash
 python setup.py test
 ```
+
+## Release process
+
+1. Bump the version number in `setup.py`
+2. Manually run the [publish to testpypi workflow](https://github.com/Picterra/picterra-python/actions/workflows/python-publish-testpypi.yml)
+3. Check the publication result on [testpypi](https://test.pypi.org/project/picterra/)
+4. Create a release through github
+5. The 'publish to pypi' workflow should automatically run
+6. Updated package should be available on [pypi](https://pypi.org/project/picterra/)
+
```

#### html2text {}

```diff
@@ -1,21 +1,29 @@
-Metadata-Version: 2.1 Name: picterra Version: 1.2.2 Summary: Picterra API
-client Description-Content-Type: text/markdown License-File: LICENSE _[_P_i_c_t_e_r_r_a
-_l_o_g_o_]# Picterra Python API Client ![Tests](https://github.com/Picterra/
-picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master) [!
-[Documentation Status](https://readthedocs.org/projects/picterra-python/badge/
-?version=latest)](https://picterra-python.readthedocs.io/en/latest/
-?badge=latest) Easily integrate state-of-the-art machine learning models in
-your app ```python from picterra import APIClient # Replace this with the id of
-one of your detectors detector_id = 'd552605b-6972-4a68-8d51-91e6cb531c24' #
-Set the PICTERRA_API_KEY environment variable to define your API key client =
-APIClient() print('Uploading raster...') raster_id = client.upload_raster
-('data/raster1.tif', name='a nice raster') print('Upload finished, starting
+Metadata-Version: 2.1 Name: picterra Version: 2.0.0 Summary: Picterra API
+client Description-Content-Type: text/markdown Provides-Extra: test Provides-
+Extra: lint License-File: LICENSE _[_P_i_c_t_e_r_r_a_ _l_o_g_o_]# Picterra Python API Client !
+[Tests](https://github.com/Picterra/picterra-python/workflows/
+lint%20and%20tests/badge.svg?branch=master) [![Documentation Status](https://
+readthedocs.org/projects/picterra-python/badge/?version=latest)](https://
+picterra-python.readthedocs.io/en/latest/?badge=latest) [![PyPI - Version]
+(https://img.shields.io/pypi/v/picterra)](https://pypi.org/project/picterra/
+) Easily integrate state-of-the-art machine learning models in your app
+```python from picterra import APIClient # Replace this with the id of one of
+your detectors detector_id = 'd552605b-6972-4a68-8d51-91e6cb531c24' # Set the
+PICTERRA_API_KEY environment variable to define your API key client = APIClient
+() print('Uploading raster...') raster_id = client.upload_raster('data/
+raster1.tif', name='a nice raster') print('Upload finished, starting
 detector...') result_id = client.run_detector(detector_id, raster_id)
 client.download_result_to_feature_collection(result_id, 'result.geojson') print
 ('Detection finished, results are in result.geojson') ``` ## Installation ```
-pip install git+https://github.com/Picterra/picterra-python.git ``` See the
-`examples` folder for examples. ## API Reference and User Guide available on
-[Read the Docs](https://picterra-python.readthedocs.io/) [![Read the Docs]
-(https://storage.googleapis.com/cloud.picterra.ch/external/assets/
-python_api_docs_screenshot.png)](https://picterra-python.readthedocs.io/) ##
-Development In order to test locally, run: ```bash python setup.py test ```
+pip install picterra ``` See the `examples` folder for examples. ## API
+Reference and User Guide available on [Read the Docs](https://picterra-
+python.readthedocs.io/) [![Read the Docs](https://storage.googleapis.com/
+cloud.picterra.ch/external/assets/python_api_docs_screenshot.png)](https://
+picterra-python.readthedocs.io/) ## Development In order to test locally, run:
+```bash python setup.py test ``` ## Release process 1. Bump the version number
+in `setup.py` 2. Manually run the [publish to testpypi workflow](https://
+github.com/Picterra/picterra-python/actions/workflows/python-publish-
+testpypi.yml) 3. Check the publication result on [testpypi](https://
+test.pypi.org/project/picterra/) 4. Create a release through github 5. The
+'publish to pypi' workflow should automatically run 6. Updated package should
+be available on [pypi](https://pypi.org/project/picterra/)
```

### Comparing `picterra-1.2.2/README.md` & `picterra-2.0.0/src/picterra.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+Metadata-Version: 2.1
+Name: picterra
+Version: 2.0.0
+Summary: Picterra API client
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: lint
+License-File: LICENSE
+
 <a href="https://picterra.ch">
     <img
         src="https://storage.googleapis.com/cloud.picterra.ch/public/assets/logo/picterra_logo_640.png"
         alt="Picterra logo" title="Picterra" align="right" height="40" />
 </a>
 
 # Picterra Python API Client
 
 ![Tests](https://github.com/Picterra/picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/picterra-python/badge/?version=latest)](https://picterra-python.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/picterra)](https://pypi.org/project/picterra/)
 
 Easily integrate state-of-the-art machine learning models in your app
 
 ```python
 from picterra import APIClient
 
 # Replace this with the id of one of your detectors
@@ -28,15 +38,15 @@
 ```
 
 
 
 ## Installation
 
 ```
-pip install git+https://github.com/Picterra/picterra-python.git
+pip install picterra
 ```
 
 See the `examples` folder for examples.
 
 ## API Reference and User Guide available on [Read the Docs](https://picterra-python.readthedocs.io/)
 
 [![Read the Docs](https://storage.googleapis.com/cloud.picterra.ch/external/assets/python_api_docs_screenshot.png)](https://picterra-python.readthedocs.io/)
@@ -44,7 +54,17 @@
 
 ## Development
 
 In order to test locally, run:
 ```bash
 python setup.py test
 ```
+
+## Release process
+
+1. Bump the version number in `setup.py`
+2. Manually run the [publish to testpypi workflow](https://github.com/Picterra/picterra-python/actions/workflows/python-publish-testpypi.yml)
+3. Check the publication result on [testpypi](https://test.pypi.org/project/picterra/)
+4. Create a release through github
+5. The 'publish to pypi' workflow should automatically run
+6. Updated package should be available on [pypi](https://pypi.org/project/picterra/)
+
```

#### html2text {}

```diff
@@ -1,19 +1,29 @@
-_[_P_i_c_t_e_r_r_a_ _l_o_g_o_]# Picterra Python API Client ![Tests](https://github.com/
-Picterra/picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master)
-[![Documentation Status](https://readthedocs.org/projects/picterra-python/
-badge/?version=latest)](https://picterra-python.readthedocs.io/en/latest/
-?badge=latest) Easily integrate state-of-the-art machine learning models in
-your app ```python from picterra import APIClient # Replace this with the id of
-one of your detectors detector_id = 'd552605b-6972-4a68-8d51-91e6cb531c24' #
-Set the PICTERRA_API_KEY environment variable to define your API key client =
-APIClient() print('Uploading raster...') raster_id = client.upload_raster
-('data/raster1.tif', name='a nice raster') print('Upload finished, starting
+Metadata-Version: 2.1 Name: picterra Version: 2.0.0 Summary: Picterra API
+client Description-Content-Type: text/markdown Provides-Extra: test Provides-
+Extra: lint License-File: LICENSE _[_P_i_c_t_e_r_r_a_ _l_o_g_o_]# Picterra Python API Client !
+[Tests](https://github.com/Picterra/picterra-python/workflows/
+lint%20and%20tests/badge.svg?branch=master) [![Documentation Status](https://
+readthedocs.org/projects/picterra-python/badge/?version=latest)](https://
+picterra-python.readthedocs.io/en/latest/?badge=latest) [![PyPI - Version]
+(https://img.shields.io/pypi/v/picterra)](https://pypi.org/project/picterra/
+) Easily integrate state-of-the-art machine learning models in your app
+```python from picterra import APIClient # Replace this with the id of one of
+your detectors detector_id = 'd552605b-6972-4a68-8d51-91e6cb531c24' # Set the
+PICTERRA_API_KEY environment variable to define your API key client = APIClient
+() print('Uploading raster...') raster_id = client.upload_raster('data/
+raster1.tif', name='a nice raster') print('Upload finished, starting
 detector...') result_id = client.run_detector(detector_id, raster_id)
 client.download_result_to_feature_collection(result_id, 'result.geojson') print
 ('Detection finished, results are in result.geojson') ``` ## Installation ```
-pip install git+https://github.com/Picterra/picterra-python.git ``` See the
-`examples` folder for examples. ## API Reference and User Guide available on
-[Read the Docs](https://picterra-python.readthedocs.io/) [![Read the Docs]
-(https://storage.googleapis.com/cloud.picterra.ch/external/assets/
-python_api_docs_screenshot.png)](https://picterra-python.readthedocs.io/) ##
-Development In order to test locally, run: ```bash python setup.py test ```
+pip install picterra ``` See the `examples` folder for examples. ## API
+Reference and User Guide available on [Read the Docs](https://picterra-
+python.readthedocs.io/) [![Read the Docs](https://storage.googleapis.com/
+cloud.picterra.ch/external/assets/python_api_docs_screenshot.png)](https://
+picterra-python.readthedocs.io/) ## Development In order to test locally, run:
+```bash python setup.py test ``` ## Release process 1. Bump the version number
+in `setup.py` 2. Manually run the [publish to testpypi workflow](https://
+github.com/Picterra/picterra-python/actions/workflows/python-publish-
+testpypi.yml) 3. Check the publication result on [testpypi](https://
+test.pypi.org/project/picterra/) 4. Create a release through github 5. The
+'publish to pypi' workflow should automatically run 6. Updated package should
+be available on [pypi](https://pypi.org/project/picterra/)
```

### Comparing `picterra-1.2.2/setup.py` & `picterra-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from setuptools import find_packages, setup
-
 # read the contents of your README file
 from pathlib import Path
+
+from setuptools import find_packages, setup
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+lint_deps = ["flake8", "mypy==1.8.0", "types-requests"]
+test_deps = ["pytest==7.1", "responses==0.22", "httpretty"]
+
 setup(
     name="picterra",
-    version="1.2.2",
+    version="2.0.0",
     description="Picterra API client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages("src"),
-    setup_requires=[
-        "pytest-runner",
-        "flake8",
-    ],
     install_requires=[
         "requests",
         # We use the new `allowed_methods` option
         "urllib3>=1.26.0",
     ],
-    tests_require=["pytest==7.1", "flake8", "responses==0.22", "httpretty"],
+    extras_require={
+        "test": test_deps,
+        "lint": lint_deps,
+    },
 )
```

### Comparing `picterra-1.2.2/src/picterra/client.py` & `picterra-2.0.0/src/picterra/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import logging
 import os
 import tempfile
 import time
 import warnings
-from typing import List, Optional
+from collections.abc import Callable
+from typing import Any, Generic, Iterator, Literal, TypedDict, TypeVar
 from urllib.parse import urlencode, urljoin
-from uuid import UUID
 
 import requests
 from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
+from urllib3.util.retry import Retry
 
 logger = logging.getLogger()
 
 CHUNK_SIZE_BYTES = 8192  # 8 KiB
 
 
 class APIError(Exception):
@@ -36,15 +36,15 @@
         )
 
     def request(self, *args, **kwargs):
         kwargs.setdefault("timeout", self.timeout)
         return super().request(*args, **kwargs)
 
 
-def _download_to_file(url, filename):
+def _download_to_file(url: str, filename: str):
     # Given we do not use self.sess the timeout is disabled (requests default), and this
     # is good as file download can take a long time
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(filename, "wb+") as f:
             logger.debug("Downloading to file %s.." % filename)
             for chunk in r.iter_content(chunk_size=CHUNK_SIZE_BYTES):
@@ -65,14 +65,73 @@
         # reading the (potentially large) layer GeoJSON in memory
         resp = requests.put(upload_url, data=f)
     if not resp.ok:
         logger.error("Error when uploading to blobstore %s" % upload_url)
         raise APIError(resp.text)
 
 
+T = TypeVar("T")
+
+
+class ResultsPage(Generic[T]):
+    """
+    Interface for a paginated response from the API
+
+    Typically the endpoint returning list of objects return them splitted
+    in pages (page 1, page 2, etc..) of a fixed dimension (eg 20). Thus
+    each `list_XX` function returns a ResultsPage (by default the first one);
+    once you have a ResultsPage for a given list of objects, you can:
+    * check its length with `len()` (eg `len(page)`)
+    * access a single element with the index operator `[]` (eg `page[5]`)
+    * turn it into a list of dictionaries with  `list()` (eg `list(page)`)
+    * get the next page with `.next()` (eg `page.next()`); this could return
+    None if the list is finished
+    You can also get a specific page passing the page number to the `list_XX` function
+    """
+
+    def __init__(self, url: str, fetch: Callable[[str], requests.Response]):
+        resp = fetch(url)
+        if not resp.ok:
+            raise APIError(resp.text)
+        r: dict[str, Any] = resp.json()
+        next_url: str | None = r["next"]
+        results: list[T] = r["results"]
+
+        self._fetch = fetch
+        self._next_url = next_url
+        self._results = results
+        self._url = url
+
+    def next(self):
+        return ResultsPage(self._next_url, self._fetch) if self._next_url else None
+
+    def __len__(self) -> int:
+        return len(self._results)
+
+    def __getitem__(self, key: int) -> T:
+        return self._results[key]
+
+    def __iter__(self) -> Iterator[T]:
+        return iter([self._results[i] for i in range(len(self._results))])
+
+    def __str__(self) -> str:
+        return f"{len(self._results)} results from {self._url}"
+
+
+class Feature(TypedDict):
+    type: Literal["Feature"]
+    properties: dict[str, Any]
+    geometry: dict[str, Any]
+
+
+class FeatureCollection(TypedDict):
+    type: Literal["FeatureCollection"]
+    features: list[Feature]
+
+
 class APIClient:
     """Main client class for the Picterra API"""
 
     def __init__(
         self, timeout: int = 30, max_retries: int = 3, backoff_factor: int = 10
     ):
         """
@@ -112,23 +171,25 @@
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         self.sess.mount("https://", adapter)
         self.sess.mount("http://", adapter)
         # Authentication
         self.sess.headers.update({"X-Api-Key": api_key})
 
-    def _api_url(self, path, params=None):
+    def _api_url(self, path: str, params: dict[str, Any] | None = None):
         base_url = urljoin(self.base_url, path)
         if not params:
             return base_url
         else:
             qstr = urlencode(params)
             return "%s?%s" % (base_url, qstr)
 
-    def _wait_until_operation_completes(self, operation_response: dict) -> dict:
+    def _wait_until_operation_completes(
+        self, operation_response: dict[str, Any]
+    ) -> dict[str, Any]:
         """Polls an operation an returns its data"""
         operation_id = operation_response["operation_id"]
         poll_interval = operation_response["poll_interval"]
         # Just sleep for a short while the first time
         time.sleep(poll_interval * 0.1)
         while True:
             logger.info("Polling operation id %s" % operation_id)
@@ -142,136 +203,144 @@
             if status == "success":
                 break
             if status == "failed":
                 raise APIError("Operation %s failed" % operation_id)
             time.sleep(poll_interval)
         return resp.json()
 
-    def _paginate_through_list(self, resource_endpoint: str, params=None):
+    def _return_results_page(
+        self, resource_endpoint: str, params: dict[str, Any] | None = None
+    ) -> ResultsPage:
         if params is None:
             params = {}
-        params["page_number"] = 1
-        data = []
+        if "page_number" not in params:
+            params["page_number"] = 1
+
         url = self._api_url("%s/" % resource_endpoint, params=params)
-        while url:
-            logger.debug("Fetching page url=%s", url)
-            resp = self.sess.get(url)
-            if not resp.ok:
-                raise APIError(resp.text)
-            r = resp.json()
-            url = r["next"]
-            data += r["results"]
-        return data
+        return ResultsPage(url, self.sess.get)
 
     def upload_raster(
         self,
         filename: str,
         name: str,
-        folder_id: Optional[str] = None,
-        captured_at: Optional[str] = None,
-        identity_key: Optional[str] = None,
+        folder_id: str | None = None,
+        captured_at: str | None = None,
+        identity_key: str | None = None,
         multispectral: bool = False,
-        cloud_coverage: Optional[int] = None,
-        user_tag: Optional[str] = None,
-    ):
+        cloud_coverage: int | None = None,
+        user_tag: str | None = None,
+    ) -> str:
         """
         Upload a raster to picterra.
 
         Args:
             filename: Local filename of raster to upload
             name: A human-readable name for this raster
             folder_id: Id of the folder this raster
                 belongs to; if not provided, the raster will be put in the
                 "Picterra API Project" folder
             captured_at: ISO-8601 date and time at which this
                 raster was captured, YYYY-MM-DDThh:mm[:ss[.uuuuuu]][+HH:MM|-HH:MM|Z];
                 e.g. "2020-01-01T12:34:56.789Z"
             identity_key: Personal identifier for this raster.
-            multispectral: If True, the raster is in multispectral mode and can have an associated band specification
+            multispectral: If True, the raster is in multispectral mode and can have
+                an associated band specification
             cloud_coverage: Raster cloud coverage %.
             user_tag (beta): Raster tag
 
         Returns:
-            raster_id (str): The id of the uploaded raster
+            raster_id: The id of the uploaded raster
         """
-        data = {"name": name, "multispectral": multispectral}
+        data: dict[str, Any] = {"name": name, "multispectral": multispectral}
         if folder_id is not None:
             data.update({"folder_id": folder_id})
         if captured_at is not None:
             data.update({"captured_at": captured_at})
         if identity_key is not None:
             data.update({"identity_key": identity_key})
         if cloud_coverage is not None:
             data.update({"cloud_coverage": cloud_coverage})
         if user_tag is not None:
             data.update({"user_tag": user_tag})
         resp = self.sess.post(self._api_url("rasters/upload/file/"), json=data)
         if not resp.ok:
             raise APIError(resp.text)
         data = resp.json()
-        upload_url = data["upload_url"]
-        raster_id = data["raster_id"]
+        upload_url = str(data["upload_url"])
+        raster_id: str = data["raster_id"]
         _upload_file_to_blobstore(upload_url, filename)
         resp = self.sess.post(self._api_url("rasters/%s/commit/" % raster_id))
         if not resp.ok:
             raise APIError(resp.text)
         self._wait_until_operation_completes(resp.json())
         return raster_id
 
-    def list_folder_detectors(self, folder_id: str):
+    def list_folder_detectors(self, folder_id: str, page_number: int | None = None):
         """
-        List of detectors assigned to a given folder
+        List of detectors assigned to a given folder, see `ResultsPage`
+        for the pagination access pattern.
 
         This a **beta** function, subject to change.
 
         Args:
-            folder_id (str): The id of the folder to obtain the detectors for
+            folder_id: The id of the folder to obtain the detectors for
+            page_number: Optional page (from 1) of the list we want to retrieve
 
         Returns:
-            A list of detector dictionaries
+            A ResultsPage object that contains a slice of the list of detector dictionaries,
+            plus methods to retrieve the other pages
 
         Example:
 
             ::
+
                 {
                     "id": "id1",
                     "name": "detector1",
                     "is_runnable": True,
                     "user_tag": "tag1",
                 },
                 {
                     "id": "id2",
                     "name": "detector2",
                     "is_runnable": False,
                     "user_tag": "tag2",
                 }
+
         """
-        return self._paginate_through_list("folders/%s/detectors" % folder_id)
+        return self._return_results_page(
+            "folders/%s/detectors" % folder_id,
+            {"page_number": page_number} if page_number is not None else None,
+        )
 
     def list_rasters(
         self,
-        folder_id: Optional[str] = None,
-        search_string: Optional[str] = None,
-        user_tag: Optional[str] = None,
-        max_cloud_coverage: Optional[int] = None,
-        captured_before: Optional[str] = None,
-        captured_after: Optional[str] = None,
-        has_vector_layers: Optional[bool] = None,
-    ) -> List[dict]:
-        """
-        List of rasters metadata
-
-        Args:
-            folder_id (str, optional): The id of the folder to search rasters in
-            search_string (str, optional): The search term used to filter rasters by name
-            user_tag (str, optional): [beta] The user tag to filter rasters by
-            max_cloud_coverage (int, optional): [beta] The max_cloud_coverage of the rasters (between 0 and 100)
-            captured_before (str, optional): ISO 8601 -formatted date / time of capture we want to list the rasters since
-            captured_after (str, optional): ISO 8601 -formatted date / time of capture we want to list the rasters from
-            has_vector_layers (bool, optional): [beta] Whether or not the rasters have at least one vector layer
+        folder_id: str | None = None,
+        search_string: str | None = None,
+        user_tag: str | None = None,
+        max_cloud_coverage: int | None = None,
+        captured_before: str | None = None,
+        captured_after: str | None = None,
+        has_vector_layers: bool | None = None,
+        page_number: int | None = None,
+    ):
+        """
+        List of rasters metadata, see `ResultsPage` for the pagination access pattern.
+
+        Args:
+            folder_id: The id of the folder to search rasters in
+            search_string: The search term used to filter rasters by name
+            user_tag: [beta] The user tag to filter rasters by
+            max_cloud_coverage: [beta] The max_cloud_coverage of the rasters (between 0 and 100)
+            captured_before: ISO 8601 -formatted date / time of capture
+                we want to list the rasters since
+            captured_after: ISO 8601 -formatted date / time of capture
+                we want to list the rasters from
+            has_vector_layers: [beta] Whether or not the rasters have at least one vector layer
+            page_number: Optional page (from 1) of the list we want to retrieve
 
         Returns:
             A list of rasters dictionaries
 
         Example:
 
             ::
@@ -286,37 +355,39 @@
                     'id': '43',
                     'status': 'ready',
                     'name': 'raster2',
                     'folder_id': 'def'
                 }
 
         """
-        params = {}
+        params: dict[str, Any] = {}
         if folder_id:
             params["folder"] = folder_id
         if search_string:
             params["search"] = search_string
         if user_tag is not None:
             params["user_tag"] = user_tag.strip()
         if max_cloud_coverage is not None:
             params["max_cloud_coverage"] = max_cloud_coverage
         if captured_before is not None:
             params["captured_before"] = captured_before
         if captured_after is not None:
             params["captured_after"] = captured_after
         if has_vector_layers is not None:
             params["has_vector_layers"] = bool(has_vector_layers)
-        return self._paginate_through_list("rasters", params)
+        if page_number is not None:
+            params["page_number"] = page_number
+        return self._return_results_page("rasters", params)
 
-    def get_raster(self, raster_id: str):
+    def get_raster(self, raster_id: str) -> dict[str, Any]:
         """
         Get raster information
 
         Args:
-            raster_id (str): id of the raster
+            raster_id: id of the raster
 
         Raises:
             APIError: There was an error while getting the raster information
 
         Returns:
             dict: Dictionary of the information
         """
@@ -324,107 +395,104 @@
         if not resp.ok:
             raise APIError(resp.text)
         return resp.json()
 
     def edit_raster(
         self,
         raster_id: str,
-        name: Optional[str] = None,
-        folder_id: Optional[str] = None,
-        captured_at: Optional[str] = None,
-        identity_key: Optional[str] = None,
-        multispectral_band_specification: Optional[dict] = None,
-        cloud_coverage: Optional[int] = None,
-        user_tag: Optional[str] = None,
+        name: str | None = None,
+        folder_id: str | None = None,
+        captured_at: str | None = None,
+        identity_key: str | None = None,
+        multispectral_band_specification: dict | None = None,
+        cloud_coverage: int | None = None,
+        user_tag: str | None = None,
     ):
         """
         Edits an already existing raster.
 
         Args:
             name: New human-readable name for this raster
             folder_id: Id of the new folder for this raster (move is in another project)
             captured_at: new ISO-8601 date and time at which this
                 raster was captured, YYYY-MM-DDThh:mm[:ss[.uuuuuu]][+HH:MM|-HH:MM|Z];
                 e.g. "2020-01-01T12:34:56.789Z"
             identity_key: New personal identifier for this raster.
-            multispectral_band_specification: The new band specification, see https://docs.picterra.ch/advanced-topics/multispectral
+            multispectral_band_specification: The new band specification,
+                see https://docs.picterra.ch/advanced-topics/multispectral
             cloud_coverage: Raster cloud coverage new percentage
             user_tag (beta): Raster tag
 
         Returns:
-            raster_id (str): The id of the edited raster
+            raster_id: The id of the edited raster
         """
-        data = {}
-        if name is not None:
-            if len(name) == 0:
-                raise ValueError("Invalid empty name")
+        data: dict[str, Any] = {}
+        if name:
             data.update({"name": name})
         if folder_id is not None:
             data.update({"folder_id": folder_id})
         if captured_at is not None:
             data.update({"captured_at": captured_at})
         if identity_key is not None:
             data.update({"identity_key": identity_key})
         if multispectral_band_specification is not None:
             data.update(
                 {"multispectral_band_specification": multispectral_band_specification}
             )
         if cloud_coverage is not None:
             data.update({"cloud_coverage": cloud_coverage})
-        if user_tag is not None:
+        if user_tag:
             data.update({"user_tag": user_tag})
-        if len(data) == 0:
-            raise ValueError("Nothing to edit")
         resp = self.sess.put(self._api_url("rasters/%s/" % raster_id), json=data)
         if not resp.ok:
             raise APIError(resp.text)
         return raster_id
 
-    def delete_raster(self, raster_id):
+    def delete_raster(self, raster_id: str):
         """
         Deletes a given raster by its identifier
 
         Args:
-            raster_id (str): The id of the raster to delete
+            raster_id: The id of the raster to delete
 
         Raises:
             APIError: There was an error while trying to delete the raster
         """
 
         resp = self.sess.delete(self._api_url("rasters/%s/" % raster_id))
         if not resp.ok:
             raise APIError(resp.text)
 
     def download_raster_to_file(self, raster_id: str, filename: str):
         """
         Downloads a raster to a local file
 
         Args:
-            raster_id (str): The id of the raster to download
-            filename (str): The local filename where to save the raster image
+            raster_id: The id of the raster to download
+            filename: The local filename where to save the raster image
 
         Raises:
             APIError: There was an error while trying to download the raster
         """
         resp = self.sess.get(self._api_url("rasters/%s/download/" % raster_id))
         if not resp.ok:
             raise APIError(resp.text)
         raster_url = resp.json()["download_url"]
         logger.debug("Trying to download raster %s from %s.." % (raster_id, raster_url))
         _download_to_file(raster_url, filename)
 
-    def set_raster_detection_areas_from_file(self, raster_id, filename):
+    def set_raster_detection_areas_from_file(self, raster_id: str, filename: str):
         """
         This is an experimental feature
 
         Set detection areas from a GeoJSON file
 
         Args:
-            raster_id (str): The id of the raster to which to assign the detection areas
-            filename (str): The filename of a GeoJSON file. This should contain a FeatureCollection
+            raster_id: The id of the raster to which to assign the detection areas
+            filename: The filename of a GeoJSON file. This should contain a FeatureCollection
                             of Polygon/MultiPolygon
 
         Raises:
             APIError: There was an error uploading the file to cloud storage
         """
         # Get upload URL
         resp = self.sess.post(
@@ -450,15 +518,15 @@
     def remove_raster_detection_areas(self, raster_id: str):
         """
         This is an experimental feature
 
         Remove the detection areas of a raster
 
         Args:
-            raster_id (str): The id of the raster whose detection areas will be removed
+            raster_id: The id of the raster whose detection areas will be removed
 
         Raises:
             APIError: There was an error during the operation
         """
         resp = self.sess.delete(
             self._api_url("rasters/%s/detection_areas/" % raster_id)
         )
@@ -468,30 +536,30 @@
     def add_raster_to_detector(self, raster_id: str, detector_id: str):
         """
         Associate a raster to a detector
 
         This a **beta** function, subject to change.
 
         Args:
-            detector_id (str): The id of the detector
-            raster_id (str): The id of the raster
+            detector_id: The id of the detector
+            raster_id: The id of the raster
 
         Raises:
             APIError: There was an error uploading the file to cloud storage
         """
         resp = self.sess.post(
             self._api_url("detectors/%s/training_rasters/" % detector_id),
             json={"raster_id": raster_id},
         )
         if not resp.status_code == 201:
             raise APIError(resp.text)
 
     def create_detector(
         self,
-        name: str = "",
+        name: str | None = None,
         detection_type: str = "count",
         output_type: str = "polygon",
         training_steps: int = 500,
         backbone: str = "resnet34",
         tile_size: int = 256,
         background_sample_ratio: float = 0.25,
     ) -> str:
@@ -509,21 +577,21 @@
             output_type: Output type of the detector (one of 'polygon', 'bbox')
             training_steps: Training steps the detector (integer between 500 & 40000)
             backbone: detector backbone (one of 'resnet18', 'resnet34', 'resnet50')
             tile_size: tile size (see HTTP API docs for the allowed values)
             background_sample_ratio: bg sample ratio (between 0 and 1)
 
         Returns:
-            detector_id (str): The id of the detector
+            The id of the detector
 
         Raises:
             APIError: There was an error while creating the detector
         """
         # Build request body
-        body_data = {"configuration": {}}
+        body_data: dict[str, Any] = {"configuration": {}}
         if name:
             body_data["name"] = name
         for i in (
             "detection_type",
             "output_type",
             "training_steps",
             "backbone",
@@ -535,23 +603,29 @@
         resp = self.sess.post(self._api_url("detectors/"), json=body_data)
         if not resp.status_code == 201:
             raise APIError(resp.text)
         return resp.json()["id"]
 
     def list_detectors(
         self,
-        search_string: Optional[str] = None,
-        user_tag: Optional[str] = None,
-        is_shared: Optional[bool] = None,
-    ) -> List[dict]:
+        search_string: str | None = None,
+        user_tag: str | None = None,
+        is_shared: bool | None = None,
+        page_number: int | None = None,
+    ):
         """
+        List all the detectors the user can access, see `ResultsPage`
+            for the pagination access pattern.
+
         Args:
             search_string: The term used to filter detectors by name
             user_tag: [beta] User tag to filter detectors by
             is_shared: [beta] Share status to filter detectors by
+            page_number: Optional page (from 1) of the list we want to retrieve
+
         Returns:
             A list of detectors dictionaries
 
         Example:
 
             ::
 
@@ -571,33 +645,35 @@
                         'detection_type': 'segmentation',
                         'output_type': 'polygon',
                         'training_steps': 500
                     }
                 }
 
         """
-        data = {}
+        data: dict[str, Any] = {}
         if search_string is not None:
             data["search"] = search_string.strip()
         if user_tag is not None:
             data["user_tag"] = user_tag.strip()
         if is_shared is not None:
             data["is_shared"] = is_shared
-        return self._paginate_through_list("detectors", data)
+        if page_number is not None:
+            data["page_number"] = page_number
+        return self._return_results_page("detectors", data)
 
     def edit_detector(
         self,
         detector_id: str,
-        name: Optional[str] = None,
-        detection_type: Optional[str] = None,
-        output_type: Optional[str] = None,
-        training_steps: Optional[int] = None,
-        backbone: Optional[str] = None,
-        tile_size: Optional[int] = None,
-        background_sample_ratio: Optional[float] = None,
+        name: str | None = None,
+        detection_type: str | None = None,
+        output_type: str | None = None,
+        training_steps: int | None = None,
+        backbone: str | None = None,
+        tile_size: int | None = None,
+        background_sample_ratio: float | None = None,
     ):
         """
         Edit a detector
 
         This a **beta** function, subject to change.
 
         Please note that depending on your plan some settings may not be editable.
@@ -612,15 +688,15 @@
             tile_size: tile size (see HTTP API docs for the allowed values)
             background_sample_ratio: bg sample ratio (between 0 and 1)
 
         Raises:
             APIError: There was an error while editing the detector
         """
         # Build request body
-        body_data = {"configuration": {}}
+        body_data: dict[str, Any] = {"configuration": {}}
         if name:
             body_data["name"] = name
         for i in (
             "detection_type",
             "output_type",
             "training_steps",
             "backbone",
@@ -637,81 +713,82 @@
             raise APIError(resp.text)
 
     def delete_detector(self, detector_id: str):
         """
         Deletes a given detector by its identifier
 
         Args:
-            detector_id (str): The id of the detector to delete
+            detector_id: The id of the detector to delete
 
         Raises:
             APIError: There was an error while trying to delete the detector
         """
 
         resp = self.sess.delete(self._api_url("detectors/%s/" % detector_id))
         if not resp.ok:
             raise APIError(resp.text)
 
     def run_detector(self, detector_id: str, raster_id: str) -> str:
         """
-        Runs a detector on a raster
+        Runs a detector on a raster: predictions are subject to a minimum charge
+        of 10 MP.
 
         Args:
-            detector_id (str): The id of the detector
-            raster_id (str): The id of the raster
+            detector_id: The id of the detector
+            raster_id: The id of the raster
 
         Returns:
-            operation_id (str): The id of the operation. You typically want to pass this
+            operation_id: The id of the operation. You typically want to pass this
                 to `download_result_to_feature_collection`
         """
         resp = self.sess.post(
             self._api_url("detectors/%s/run/" % detector_id),
             json={"raster_id": raster_id},
         )
         if not resp.ok:
             raise APIError(resp.text)
         operation_response = resp.json()
         self._wait_until_operation_completes(operation_response)
         return operation_response["operation_id"]
 
-    def download_result_to_file(self, operation_id, filename):
+    def download_result_to_file(self, operation_id: str, filename: str):
         """
         Downloads a set of results to a local GeoJSON file
 
         .. deprecated:: 1.0.0
            Use `download_result_to_feature_collection` instead
 
         Args:
-            operation_id (str): The id of the operation to download
-            filename (str): The local filename where to save the results
+            operation_id: The id of the operation to download
+            filename: The local filename where to save the results
         """
         warnings.warn(
             "This function is deprecated. Use download_result_to_feature_collection instead",
             DeprecationWarning,
         )
         result_url = self.get_operation_results(operation_id)["url"]
         logger.debug("Trying to download result %s.." % result_url)
         _download_to_file(result_url, filename)
 
-    def download_result_to_feature_collection(self, operation_id, filename):
+    def download_result_to_feature_collection(self, operation_id: str, filename: str):
         """
         Downloads the results from a detection operation to a local GeoJSON file.
 
         Results are stored as a FeatureCollection of Multipolygon. Each feature has a 'class_name'
         property indicating the corresponding class name
 
         Args:
-            operation_id (str): The id of the operation to download. This should be a
+            operation_id: The id of the operation to download. This should be a
                 detect operation
-            filename (str): The local filename where to save the results
+            filename: The local filename where to save the results
         """
         results = self.get_operation_results(operation_id)
         # We download results to a temporary directory and then assemble them into a
         # FeatureCollection
-        fc = {"type": "FeatureCollection", "features": []}
+        fc: FeatureCollection = {"type": "FeatureCollection", "features": []}
 
         for i, class_result in enumerate(results["by_class"]):
             with tempfile.NamedTemporaryFile() as f:
                 _download_to_file(class_result["result"]["url"], f.name)
                 # Reopen in read text
                 with open(f.name) as fr:
                     multipolygon = json.load(fr)
@@ -722,74 +799,70 @@
                             "geometry": multipolygon,
                         }
                     )
 
         with open(filename, "w") as f:
             json.dump(fc, f)
 
-    def download_operation_results_to_file(self, operation_id, filename):
+    def download_operation_results_to_file(self, operation_id: str, filename: str):
         """
         Downloads the results URL to a local GeoJSON file
 
         Args:
-            operation_id (str): The id of the operation to download
-            filename (str): The local filename where to save the results
+            operation_id: The id of the operation to download
+            filename: The local filename where to save the results
         """
         data = self.get_operation_results_url(operation_id)
         with open(filename, "w") as f:
             f.write(data)
 
-    def get_operation_results(self, operation_id: str) -> str:
+    def get_operation_results(self, operation_id: str) -> dict[str, Any]:
         """
         Return the 'results' dict of an operation
 
         This a **beta** function, subject to change.
 
         Args:
-            operation_id (str): The id of the operation
+            operation_id: The id of the operation
         """
         resp = self.sess.get(
             self._api_url("operations/%s/" % operation_id),
         )
         return resp.json()["results"]
 
     def get_operation_results_url(self, operation_id: str) -> str:
         """
-        Get the URL  of a set of results
+        Get the URL of a set of operation results
 
         This a **beta** function, subject to change.
 
         Args:
-            result_id (str): The id of the result
+            operation_id: The id of the result
         """
         return self.get_operation_results(operation_id)["url"]
 
-    def set_annotations(self, detector_id, raster_id, annotation_type, annotations):
+    def set_annotations(
+        self,
+        detector_id: str,
+        raster_id: str,
+        annotation_type: Literal[
+            "outline", "training_area", "testing_area", "validation_area"
+        ],
+        annotations: dict[str, Any],
+    ):
         """
         Replaces the annotations of type 'annotation_type' with 'annotations', for the
         given raster-detector pair.
 
         Args:
-            detector_id (str): The id of the detector
-            raster_id (str): The id of the raster
-            annotation_type (str): One of (outline, training_area, testing_area, validation_area)
-            annotations (dict): GeoJSON representation of the features to upload
-        """
-        annotation_type = annotation_type.lower()
-        valid_annotations = (
-            "outline",
-            "training_area",
-            "testing_area",
-            "validation_area",
-        )
-        if annotation_type not in valid_annotations:
-            raise ValueError(
-                'Invalid annotation type "%s"; allowed values are: %s.'
-                % (annotation_type, ", ".join(valid_annotations))
-            )
+            detector_id: The id of the detector
+            raster_id: The id of the raster
+            annotation_type: One of (outline, training_area, testing_area, validation_area)
+            annotations: GeoJSON representation of the features to upload
+        """
         # Get an upload url
         create_upload_resp = self.sess.post(
             self._api_url(
                 "detectors/%s/training_rasters/%s/%s/upload/bulk/"
                 % (detector_id, raster_id, annotation_type)
             )
         )
@@ -819,42 +892,46 @@
         )
         if not commit_upload_resp.ok:
             raise APIError(commit_upload_resp.text)
 
         # Poll for operation completion
         self._wait_until_operation_completes(commit_upload_resp.json())
 
-    def train_detector(self, detector_id):
+    def train_detector(self, detector_id: str):
         """
         Start the training of a detector
 
         Args:
-            detector_id (str): The id of the detector
+            detector_id: The id of the detector
         """
         resp = self.sess.post(self._api_url("detectors/%s/train/" % detector_id))
         if not resp.ok:
             raise APIError(resp.text)
         return self._wait_until_operation_completes(resp.json())
 
-    def run_dataset_recommendation(self, detector_id):
+    def run_dataset_recommendation(self, detector_id: str):
         """
         This is an **experimental** feature
 
         Runs dataset recommendation on a detector. Note that you currently have to use
         the UI to be able to view the recommendation markers/report.
 
         Args:
-            detector_id (str): The id of the detector
+            detector_id: The id of the detector
         """
-        resp = self.sess.post(self._api_url("detectors/%s/dataset_recommendation/" % detector_id))
+        resp = self.sess.post(
+            self._api_url("detectors/%s/dataset_recommendation/" % detector_id)
+        )
         if not resp.ok:
             raise APIError(resp.text)
         return self._wait_until_operation_completes(resp.json())
 
-    def run_advanced_tool(self, tool_id: UUID, inputs: dict, outputs: dict):
+    def run_advanced_tool(
+        self, tool_id: str, inputs: dict[str, Any], outputs: dict[str, Any]
+    ):
         """
         This is an experimental feature
 
         Runs a tool and waits for its execution, returning the finished operation metadata
 
         Args:
             tool_id: The id of the tool to run
@@ -870,19 +947,19 @@
         )
         if not resp.ok:
             raise APIError(resp.text)
         return self._wait_until_operation_completes(resp.json())
 
     def upload_vector_layer(
         self,
-        raster_id: UUID,
+        raster_id: str,
         filename: str,
-        name: Optional[str] = None,
-        color: Optional[str] = None,
-    ) -> UUID:
+        name: str | None = None,
+        color: str | None = None,
+    ) -> str:
         """
         Uploads a vector layer from a GeoJSON file
 
         This a **beta** function, subject to change.
 
         Args:
             raster_id: The id of the raster we want to attach the vector layer to
@@ -911,18 +988,15 @@
         )
         if not resp.ok:
             raise APIError(resp.text)
         op = self._wait_until_operation_completes(resp.json())
         return op["results"]["vector_layer_id"]
 
     def edit_vector_layer(
-        self,
-        vector_layer_id: UUID,
-        name: Optional[str] = None,
-        color: Optional[str] = None
+        self, vector_layer_id: str, name: str | None = None, color: str | None = None
     ):
         """
         Edits a vector layer
 
         This a **beta** function, subject to change.
 
         Args:
@@ -937,71 +1011,78 @@
             data.update({"color": color})
         resp = self.sess.put(
             self._api_url("vector_layers/%s/" % vector_layer_id), json=data
         )
         if not resp.ok:
             raise APIError(resp.text)
 
-    def delete_vector_layer(self, vector_layer_id: UUID):
+    def delete_vector_layer(self, vector_layer_id: str):
         """
         Removes a vector layer
 
         This a **beta** function, subject to change.
 
         Args:
             vector_layer_id: The id of the vector layer to remove
         """
         resp = self.sess.delete(self._api_url("vector_layers/%s/" % vector_layer_id))
         if not resp.ok:
             raise APIError(resp.text)
 
-    def download_vector_layer_to_file(self, vector_layer_id: UUID, filename: str):
+    def download_vector_layer_to_file(self, vector_layer_id: str, filename: str):
         """
         Downloads a vector layer
 
         This a **beta** function, subject to change.
 
         Args:
             vector_layer_id: The id of the vector layer to download
             filename: existing file to save the vector layer in
         """
         resp = self.sess.get(self._api_url("vector_layers/%s/" % vector_layer_id))
         if not resp.ok:
             raise APIError(resp.text)
         urls = resp.json()["geojson_urls"]
-        final_fc = {"type": "FeatureCollection", "features": []}
+        final_fc: FeatureCollection = {"type": "FeatureCollection", "features": []}
         for url in urls:
             with tempfile.NamedTemporaryFile("w+") as f:
                 _download_to_file(url, f.name)
                 fc = json.load(f)
                 for feature in fc["features"]:
                     final_fc["features"].append(feature)
         with open(filename, "w") as fp:
             json.dump(final_fc, fp)
 
-    def list_raster_markers(self, raster_id):
+    def list_raster_markers(
+        self,
+        raster_id: str,
+        page_number: int | None = None,
+    ):
         """
         This a **beta** function, subject to change.
 
-        List all the markers on a raster
+        List all the markers on a raster, see `ResultsPage` for the pagination access pattern.
 
         Args:
-            raster_id (str): The id of the raster
+            raster_id: The id of the raster
+            page_number: Optional page (from 1) of the list we want to retrieve
         """
-        url = "rasters/%s/markers/" % raster_id
-        return self._paginate_through_list(url)
+        return self._return_results_page(
+            "rasters/%s/markers/" % raster_id,
+            {"page_number": page_number} if page_number is not None else None,
+        )
 
     def create_marker(
         self,
-        raster_id: UUID,
-        detector_id: Optional[UUID],
+        raster_id: str,
+        detector_id: str | None,
         lng: float,
         lat: float,
         text: str,
-    ):
+    ) -> dict[str, Any]:
         """
         This is an **experimental** (beta) feature
 
         Creates a marker
 
         Args:
             raster_id: The id of the raster (belonging to detector) to create the marker on
@@ -1019,7 +1100,83 @@
             "marker": {"type": "Point", "coordinates": [lng, lat]},
             "text": text,
         }
         resp = self.sess.post(self._api_url(url), json=data)
         if not resp.ok:
             raise APIError(resp.text)
         return resp.json()
+
+    def import_raster_from_remote_source(
+        self,
+        raster_name: str,
+        folder_id: str,
+        source_id: str,
+        aoi_filename: str,
+        method: Literal["streaming"] = "streaming",
+    ) -> str:
+        """
+        This is an experimental feature
+
+        Import a raster from a remote imagery source given a GeoJSON file for the AOI
+
+        Args:
+            raster_name: Name of the new raster
+            folder_id: The id of the folder / project the raster will live in
+            source_id: The id of the remote imagery source to import from
+            filename: The filename of a GeoJSON file. This should contain a FeatureCollection of
+                Polygon/MultiPolygon representing the AOI of the new raster
+
+        Raises:
+            APIError: There was an error during import
+        """
+        # Get upload URL
+        resp = self.sess.post(self._api_url("rasters/import/"))
+        if not resp.ok:
+            raise APIError(resp.text)
+        data = resp.json()
+        upload_url = data["upload_url"]
+        upload_id = data["upload_id"]
+        # Upload to blobstore
+        _upload_file_to_blobstore(upload_url, aoi_filename)
+        # Commit upload
+        resp = self.sess.post(
+            self._api_url(f"rasters/import/{upload_id}/commit/"),
+            json={
+                "method": method,
+                "source_id": source_id,
+                "folder_id": folder_id,
+                "name": raster_name,
+            },
+        )
+        if not resp.ok:
+            raise APIError(resp.text)
+        # Poll operation and get raster identifier
+        operation = self._wait_until_operation_completes(resp.json())
+        return operation["metadata"]["raster_id"]
+
+    def list_raster_vector_layers(
+        self,
+        raster_id: str,
+        search: str | None = None,
+        detector_id: str | None = None,
+        page_number: int | None = None,
+    ):
+        """
+        This a **beta** function, subject to change.
+
+        List all the vector layers on a raster, see `ResultsPage`
+            for the pagination access pattern.
+
+        Args:
+            raster_id: The id of the raster
+            search: Optional string to search layers by name
+            page_number: Optional page (from 1) of the list we want to retrieve
+        """
+        params: dict[str, str | int] = {}
+        if search is not None:
+            params["search"] = search
+        if detector_id is not None:
+            params["detector"] = detector_id
+        if page_number is not None:
+            params["page_number"] = page_number
+        url = "rasters/%s/vector_layers/" % raster_id
+        return self._return_results_page(url, params)
```

### Comparing `picterra-1.2.2/src/picterra/nongeo.py` & `picterra-2.0.0/src/picterra/nongeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,25 +74,28 @@
     Note that this will NOT work if the image was georeferenced. So only use
     this function if you are uploading non-georeferenced image formats like
     PNG or JPEG
 
     This is currently in **beta** so let us know if you find any issues
 
     Args:
-        - result_filename (str): The file path to the GeoJSON file obtained by
-            `APIClient.download_result_to_file`
+        result_filename (str): The file path to the GeoJSON file obtained by
+                               `APIClient.download_result_to_file`
     Returns:
-        - polygons: A list of polygons. Each polygon is a list of rings and
-            each ring is a list of (x, y) tuples. For example:
-              [
+        A list of polygons. Each polygon is a list of rings and
+        each ring is a list of (x, y) tuples. For example:
+
+        ::
+
+            [
                 # This is a square with a square hole
                 [[(0, 0), (1, 0), (1, 1), (0, 1), (0, 0)],
                  [(0.4, 0.4), (0.5, 0.4), (0.5, 0.5), (0.4, 0.5), (0.4, 0.4)],
                 # A triangle
                 [[(0, 0), (1, 0), (1, 1), (0, 0)]]
-              ]
+            ]
     """
     with open(result_filename) as f:
         geojson = json.load(f)
     polygons = _load_polygons(geojson)
     polygons = [_polygon_to_xy(p) for p in polygons]
     return polygons
```

### Comparing `picterra-1.2.2/src/picterra.egg-info/PKG-INFO` & `picterra-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-Metadata-Version: 2.1
-Name: picterra
-Version: 1.2.2
-Summary: Picterra API client
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href="https://picterra.ch">
     <img
         src="https://storage.googleapis.com/cloud.picterra.ch/public/assets/logo/picterra_logo_640.png"
         alt="Picterra logo" title="Picterra" align="right" height="40" />
 </a>
 
 # Picterra Python API Client
 
 ![Tests](https://github.com/Picterra/picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/picterra-python/badge/?version=latest)](https://picterra-python.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/picterra)](https://pypi.org/project/picterra/)
 
 Easily integrate state-of-the-art machine learning models in your app
 
 ```python
 from picterra import APIClient
 
 # Replace this with the id of one of your detectors
@@ -35,15 +29,15 @@
 ```
 
 
 
 ## Installation
 
 ```
-pip install git+https://github.com/Picterra/picterra-python.git
+pip install picterra
 ```
 
 See the `examples` folder for examples.
 
 ## API Reference and User Guide available on [Read the Docs](https://picterra-python.readthedocs.io/)
 
 [![Read the Docs](https://storage.googleapis.com/cloud.picterra.ch/external/assets/python_api_docs_screenshot.png)](https://picterra-python.readthedocs.io/)
@@ -51,7 +45,17 @@
 
 ## Development
 
 In order to test locally, run:
 ```bash
 python setup.py test
 ```
+
+## Release process
+
+1. Bump the version number in `setup.py`
+2. Manually run the [publish to testpypi workflow](https://github.com/Picterra/picterra-python/actions/workflows/python-publish-testpypi.yml)
+3. Check the publication result on [testpypi](https://test.pypi.org/project/picterra/)
+4. Create a release through github
+5. The 'publish to pypi' workflow should automatically run
+6. Updated package should be available on [pypi](https://pypi.org/project/picterra/)
+
```

#### html2text {}

```diff
@@ -1,21 +1,27 @@
-Metadata-Version: 2.1 Name: picterra Version: 1.2.2 Summary: Picterra API
-client Description-Content-Type: text/markdown License-File: LICENSE _[_P_i_c_t_e_r_r_a
-_l_o_g_o_]# Picterra Python API Client ![Tests](https://github.com/Picterra/
-picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master) [!
-[Documentation Status](https://readthedocs.org/projects/picterra-python/badge/
-?version=latest)](https://picterra-python.readthedocs.io/en/latest/
-?badge=latest) Easily integrate state-of-the-art machine learning models in
-your app ```python from picterra import APIClient # Replace this with the id of
-one of your detectors detector_id = 'd552605b-6972-4a68-8d51-91e6cb531c24' #
-Set the PICTERRA_API_KEY environment variable to define your API key client =
-APIClient() print('Uploading raster...') raster_id = client.upload_raster
-('data/raster1.tif', name='a nice raster') print('Upload finished, starting
-detector...') result_id = client.run_detector(detector_id, raster_id)
-client.download_result_to_feature_collection(result_id, 'result.geojson') print
-('Detection finished, results are in result.geojson') ``` ## Installation ```
-pip install git+https://github.com/Picterra/picterra-python.git ``` See the
-`examples` folder for examples. ## API Reference and User Guide available on
-[Read the Docs](https://picterra-python.readthedocs.io/) [![Read the Docs]
-(https://storage.googleapis.com/cloud.picterra.ch/external/assets/
+_[_P_i_c_t_e_r_r_a_ _l_o_g_o_]# Picterra Python API Client ![Tests](https://github.com/
+Picterra/picterra-python/workflows/lint%20and%20tests/badge.svg?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/picterra-python/
+badge/?version=latest)](https://picterra-python.readthedocs.io/en/latest/
+?badge=latest) [![PyPI - Version](https://img.shields.io/pypi/v/picterra)]
+(https://pypi.org/project/picterra/) Easily integrate state-of-the-art machine
+learning models in your app ```python from picterra import APIClient # Replace
+this with the id of one of your detectors detector_id = 'd552605b-6972-4a68-
+8d51-91e6cb531c24' # Set the PICTERRA_API_KEY environment variable to define
+your API key client = APIClient() print('Uploading raster...') raster_id =
+client.upload_raster('data/raster1.tif', name='a nice raster') print('Upload
+finished, starting detector...') result_id = client.run_detector(detector_id,
+raster_id) client.download_result_to_feature_collection(result_id,
+'result.geojson') print('Detection finished, results are in result.geojson')
+``` ## Installation ``` pip install picterra ``` See the `examples` folder for
+examples. ## API Reference and User Guide available on [Read the Docs](https://
+picterra-python.readthedocs.io/) [![Read the Docs](https://
+storage.googleapis.com/cloud.picterra.ch/external/assets/
 python_api_docs_screenshot.png)](https://picterra-python.readthedocs.io/) ##
-Development In order to test locally, run: ```bash python setup.py test ```
+Development In order to test locally, run: ```bash python setup.py test ``` ##
+Release process 1. Bump the version number in `setup.py` 2. Manually run the
+[publish to testpypi workflow](https://github.com/Picterra/picterra-python/
+actions/workflows/python-publish-testpypi.yml) 3. Check the publication result
+on [testpypi](https://test.pypi.org/project/picterra/) 4. Create a release
+through github 5. The 'publish to pypi' workflow should automatically run 6.
+Updated package should be available on [pypi](https://pypi.org/project/
+picterra/)
```

### Comparing `picterra-1.2.2/tests/test_client.py` & `picterra-2.0.0/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,43 +55,57 @@
         match=matchers,
         status=expected_status,
     )
 
 
 def add_mock_rasters_list_response():
     data1 = {
-        "count": 4,
+        "count": 5,
         "next": api_url("rasters/?page_number=2"),
-        "previous": api_url("rasters/?page_number=1"),
+        "previous": None,
         "page_size": 2,
         "results": [
             {"id": "40", "status": "ready", "name": "raster1"},
             {"id": "41", "status": "ready", "name": "raster2"},
         ],
     }
     data2 = {
-        "count": 4,
-        "next": None,
+        "count": 5,
+        "next": api_url("rasters/?page_number=3"),
         "previous": None,
-        "page_size": 2,
+        "page_size": api_url("rasters/?page_number=1"),
         "results": [
             {"id": "42", "status": "ready", "name": "raster3"},
             {"id": "43", "status": "ready", "name": "raster4"},
         ],
     }
+    data3 = {
+        "count": 5,
+        "next": None,
+        "previous": api_url("rasters/?page_number=2"),
+        "page_size": 2,
+        "results": [
+            {"id": "44", "status": "ready", "name": "raster5"},
+        ],
+    }
     _add_api_response(
         "rasters/",
         json=data1,
         match=responses.matchers.query_param_matcher({"page_number": "1"}),
     )
     _add_api_response(
         "rasters/",
         json=data2,
         match=responses.matchers.query_param_matcher({"page_number": "2"}),
     )
+    _add_api_response(
+        "rasters/",
+        json=data3,
+        match=responses.matchers.query_param_matcher({"page_number": "3"}),
+    )
 
 
 def add_mock_rasters_in_folder_list_response(folder_id):
     data = {
         "count": 1,
         "next": None,
         "previous": None,
@@ -108,27 +122,27 @@
     qs = {"folder": folder_id, "page_number": "1"}
     _add_api_response(
         "rasters/", json=data, match=responses.matchers.query_param_matcher(qs)
     )
 
 
 def add_mock_rasters_in_filtered_list_response(
-    search=None, tag=None, cloud=None, before=None, after=None, has_layers=None
+    search=None, tag=None, cloud=None, before=None, after=None, has_layers=None, page=1
 ):
     name = (search + "_" if search else "") + "raster" + ("_" + tag if tag else "")
     data = {
         "count": 1,
         "next": None,
         "previous": None,
         "page_size": 2,
         "results": [
             {"id": "77", "status": "ready", "name": name},
         ],
     }
-    qs = {"page_number": 1}
+    qs = {"page_number": page}
     if search is not None:
         qs["search"] = search
     if tag is not None:
         qs["user_tag"] = tag
     if cloud is not None:
         qs["max_cloud_coverage"] = cloud
     if before:
@@ -138,14 +152,37 @@
     if has_layers is not None:
         qs["has_vector_layers"] = bool(has_layers)
     _add_api_response(
         "rasters/", match=responses.matchers.query_param_matcher(qs), json=data
     )
 
 
+def add_mock_vector_layers_filtered_list_response(
+    idx, raster, search=None, detector=None
+):
+    name = f"layer_{idx}"
+    data = {
+        "count": 1,
+        "next": None,
+        "previous": None,
+        "page_size": 1,
+        "results": [{"id": str(idx), "count": idx, "name": name}],
+    }
+    qs = {"page_number": 1}
+    if search is not None:
+        qs["search"] = search
+    if detector is not None:
+        qs["detector"] = detector
+    _add_api_response(
+        f"rasters/{raster}/vector_layers/",
+        match=responses.matchers.query_param_matcher(qs),
+        json=data,
+    )
+
+
 def add_mock_detectors_list_response(string=None, tag=None, shared=None):
     data1 = {
         "count": 4,
         "next": api_url("detectors/?page_number=2"),
         "previous": None,
         "page_size": 2,
         "results": [
@@ -198,16 +235,19 @@
     match = responses.json_params_matcher({"configuration": kwargs}) if kwargs else None
     _add_api_response("detectors/%s/" % d_id, responses.PUT, status=204, match=match)
 
 
 def add_mock_detector_train_responses(detector_id):
     _add_api_response("detectors/%s/train/" % detector_id, responses.POST, OP_RESP)
 
+
 def add_mock_run_dataset_recommendation_responses(detector_id):
-    _add_api_response("detectors/%s/dataset_recommendation/" % detector_id, responses.POST, OP_RESP)
+    _add_api_response(
+        "detectors/%s/dataset_recommendation/" % detector_id, responses.POST, OP_RESP
+    )
 
 
 def add_mock_operations_responses(status, **kwargs):
     data = {"type": "mock_operation_type", "status": status}
     if kwargs:
         data.update(kwargs)
     if status == "success":
@@ -305,14 +345,31 @@
     # Status, second check
     data = {"status": "ready"}
     _add_api_response(
         "rasters/%s/detection_areas/upload/%s/" % (raster_id, upload_id), json=data
     )
 
 
+def add_mock_remote_import_responses(upload_id, post_body):
+    match = responses.json_params_matcher(post_body)
+    # Upload initiation
+    data = {"upload_url": "http://storage.example.com", "upload_id": upload_id}
+    _add_api_response("rasters/import/", responses.POST, data)
+    # Storage PUT
+    responses.add(responses.PUT, "http://storage.example.com", status=200)
+    # Commit
+    _add_api_response(
+        f"rasters/import/{upload_id}/commit/",
+        responses.POST,
+        OP_RESP,
+        match=match,
+        status=200,
+    )
+
+
 def add_mock_detector_run_responses(detector_id):
     op_id = 43
     _add_api_response("detectors/%s/run/" % detector_id, responses.POST, OP_RESP)
     # First status check
     data = {"status": "running"}
     _add_api_response("operations/%s/" % op_id, json=data)
     # Second status check
@@ -661,19 +718,31 @@
     assert len(responses.calls) == 2
 
 
 @responses.activate
 def test_list_rasters():
     """Test the list of rasters, both generic and specifying the filters"""
     client = _client()
-    # Generic
+    # Generic (check pagination)
     add_mock_rasters_list_response()
-    rasters = client.list_rasters()
-    assert rasters[0]["name"] == "raster1"
-    assert rasters[2]["name"] == "raster3"
+    page1 = client.list_rasters()
+    assert len(page1) == 2
+    assert page1[0]["name"] == "raster1" and page1[1]["name"] == "raster2"
+    assert len(responses.calls) == 1
+    page2 = page1.next()
+    assert len(page2) == 2
+    assert page2[0]["name"] == "raster3" and page2[1]["name"] == "raster4"
+    page3 = page2.next()
+    assert len(responses.calls) == 3
+    assert len(page3) == 1 and page3.next() is None
+    assert page3[0]["name"] == "raster5"
+    assert len(responses.calls) == 3
+    pairs = zip(list(page2), list(client.list_rasters(page_number=2)))
+    assert all(x == y for x, y in pairs) is True
+    assert len(responses.calls) == 4
     # Folder list
     add_mock_rasters_in_folder_list_response("foobar")
     rasters = client.list_rasters("foobar")
     assert rasters[0]["name"] == "raster_in_folder1"
     assert rasters[0]["folder_id"] == "foobar"
     # Search list
     add_mock_rasters_in_filtered_list_response(search="spam")
@@ -703,14 +772,22 @@
     )
     rasters = client.list_rasters(
         search_string="bar",
         captured_after="2022-11-13T20:20:39+00:00",
         has_vector_layers=True,
     )
     assert rasters[0]["name"] == "bar_raster"
+    # Filter list with pagination
+    add_mock_rasters_in_filtered_list_response(page=3, search="spam")
+    rasters = client.list_rasters(
+        search_string="spam",
+        page_number=3,
+    )
+    assert rasters[0]["id"] == "77"
+    assert len(responses.calls) == 11
 
 
 @responses.activate
 def test_detector_creation():
     client = _client()
     args = [
         {"detection_type": "segmentation"},
@@ -733,25 +810,27 @@
 
 @responses.activate
 def test_list_detectors():
     client = _client()
     # Full list
     add_mock_detectors_list_response()
     detectors = client.list_detectors()
+    assert len(detectors) == 2  # 1st api call
     assert detectors[0]["name"] == "detector1"
     assert detectors[1]["name"] == "detector2"
+    assert detectors.next()[1]["id"] == "43"  # 2nd api call
     # Search list
     add_mock_detectors_list_response("spam")
-    detectors = client.list_detectors("spam")
+    detectors = client.list_detectors("spam")  # 3rd api call
     assert detectors[0]["name"] == "spam"
     # Filter list
     add_mock_detectors_list_response(None, "foobar", True)
-    detectors = client.list_detectors(user_tag="foobar", is_shared=True)
+    detectors = client.list_detectors(user_tag="foobar", is_shared=True)  # 4th api call
     assert detectors[1]["name"] == "detector2"
-    assert len(responses.calls) == 6
+    assert len(responses.calls) == 4
 
 
 @responses.activate
 def test_delete_detector():
     DETECTOR_ID = "foobar"
     client = _client()
     add_mock_delete_detector_response(DETECTOR_ID)
@@ -843,16 +922,14 @@
 )
 def test_upload_annotations(annotation_type):
     add_mock_annotations_responses(1, 2, annotation_type)
     add_mock_operations_responses("running")
     add_mock_operations_responses("running")
     add_mock_operations_responses("success")
     client = _client()
-    with pytest.raises(ValueError):
-        client.set_annotations(1, 2, "foobar", {})
     client.set_annotations(1, 2, annotation_type, {})
     assert len(responses.calls) == 6
 
 
 @responses.activate
 def test_train_detector():
     add_mock_detector_train_responses(1)
@@ -867,15 +944,15 @@
                 "training_areas_count": 2,
                 "assessment_areas_count": 10,
                 "validation_areas_count": 5,
                 "total_annotations_count": 4,
                 "training_annotations_count": 3,
                 "validation_annotations_count": 1,
             },
-        }
+        },
     )
     client = _client()
     op = client.train_detector(1)
     assert op["results"]["score"] == 92
     assert len(responses.calls) == 4
 
 
@@ -937,19 +1014,21 @@
 
 @responses.activate
 def test_list_raster_markers():
     client = _client()
     add_mock_raster_markers_list_response("spam")
     rasters = client.list_raster_markers("spam")
     assert rasters[0]["id"] == "1"
-    assert rasters[2]["id"] == "3"
+    rasters = client.list_raster_markers("spam", page_number=2)
+    assert rasters[0]["id"] == "3"
+    assert len(responses.calls) == 2
 
 
 @responses.activate
-def test_list_raster_markers():
+def test_raster_markers_creation():
     client = _client()
     add_mock_marker_creation_response("spam", "foo", "bar", [12.34, 56.78], "foobar")
     marker = client.create_marker("foo", "bar", 12.34, 56.78, "foobar")
     assert marker["id"] == "spam"
 
 
 @responses.activate
@@ -963,17 +1042,31 @@
 
 
 @responses.activate
 def test_list_folder_detectors():
     client = _client()
     add_mock_folder_detector_response("folder_id123")
     detector_list = client.list_folder_detectors("folder_id123")
-    assert len(detector_list) == 4
+    assert len(detector_list) == 2
     assert detector_list[0]["id"] == "id1"
-    assert detector_list[2]["id"] == "id3"
+    detector_list = detector_list.next()
+    assert detector_list[0]["id"] == "id3"
+    assert len(responses.calls) == 2
+
+
+@responses.activate
+def test_list_raster_vector_layers():
+    client = _client()
+    add_mock_vector_layers_filtered_list_response(0, "raster1")
+    add_mock_vector_layers_filtered_list_response(1, "raster1", "spam", "detector1")
+    assert client.list_raster_vector_layers("raster1")[0]["id"] == "0"
+    assert (
+        client.list_raster_vector_layers("raster1", "spam", "detector1")[0]["name"]
+        == "layer_1"
+    )
 
 
 # Cannot test Retry with responses, @see https://github.com/getsentry/responses/issues/135
 @httpretty.activate
 def test_backoff_success():
     data = {"count": 0, "next": None, "previous": None, "results": []}
     httpretty.register_uri(
@@ -1046,7 +1139,30 @@
     assert (
         client.run_advanced_tool(
             "foobar", {"foo": "bar"}, {"spam": [1, 2], "bar": {"foo": None, "bar": 4}}
         )["type"]
         == "mock_operation_type"
     )
     assert len(responses.calls) == 2
+
+
+@responses.activate
+def test_import_raster_from_remote_source():
+    body = {
+        "method": "streaming",
+        "source_id": "source",
+        "folder_id": "project",
+        "name": "image",
+    }
+    add_mock_remote_import_responses("upload_id", body)
+    add_mock_operations_responses("success")
+
+    client = _client()
+    # This just tests that this doesn't raise
+    with tempfile.NamedTemporaryFile() as f:
+        assert (
+            client.import_raster_from_remote_source(
+                "image", "project", "source", f.name
+            )
+            == "foo"
+        )
+    assert len(responses.calls) == 4
```

### Comparing `picterra-1.2.2/tests/test_nongeo.py` & `picterra-2.0.0/tests/test_nongeo.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from picterra.nongeo import _load_polygons, _nongeo_latlng2xy
 
 # The way to get the lat/lng is:
 # - Upload a non-georeferenced image to the platform
 # - Download the normalized.tif
 # - Open normalized.tif in QGIS, get the lat/lng coordinates of the 4 corners of the image
 
+
 # In this case, the image is 1520 x 1086
 @pytest.mark.parametrize(
     "latlng,xy",
     [
         # bottom-right corner
         ((-0.00097539, 0.00136530), (1520, 1086)),
         # bottom-left corner
```

