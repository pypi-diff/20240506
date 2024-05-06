# Comparing `tmp/pynetcheck-1.0.0.tar.gz` & `tmp/pynetcheck-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynetcheck-1.0.0.tar", max compression
+gzip compressed data, was "pynetcheck-1.0.1.tar", max compression
```

## Comparing `pynetcheck-1.0.0.tar` & `pynetcheck-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1094 2023-10-17 17:21:13.864484 pynetcheck-1.0.0/LICENSE
--rw-r--r--   0        0        0      261 2024-04-16 18:33:18.636607 pynetcheck-1.0.0/pynetcheck/__init__.py
--rw-r--r--   0        0        0    11226 2024-04-16 14:18:36.139811 pynetcheck-1.0.0/pynetcheck/archive/output_1713283371.388187.json
--rw-r--r--   0        0        0      817 2024-04-16 16:29:18.656699 pynetcheck-1.0.0/pynetcheck/archive/output_1713287098.9189737.json
--rw-r--r--   0        0        0     6750 2024-04-16 17:04:59.264998 pynetcheck-1.0.0/pynetcheck/archive/output_1713287258.6043513.json
--rw-r--r--   0        0        0     6750 2024-04-16 17:07:38.964406 pynetcheck-1.0.0/pynetcheck/archive/output_1713287738.6383476.json
--rw-r--r--   0        0        0     2669 2024-04-16 17:15:39.089976 pynetcheck-1.0.0/pynetcheck/archive/output_1713291137.528805.json
--rw-r--r--   0        0        0     4475 2024-04-16 18:12:17.905502 pynetcheck-1.0.0/pynetcheck/archive/output_1713291437.5512764.json
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.517432 pynetcheck-1.0.0/pynetcheck/models/__init__.py
--rw-r--r--   0        0        0     2769 2024-04-16 18:33:18.637606 pynetcheck-1.0.0/pynetcheck/models/device.py
--rw-r--r--   0        0        0      965 2024-04-16 16:43:18.234801 pynetcheck-1.0.0/pynetcheck/models/shared.py
--rw-r--r--   0        0        0      222 2024-04-16 18:33:18.638606 pynetcheck-1.0.0/pynetcheck/pytest.ini
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-1.0.0/pynetcheck/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-1.0.0/pynetcheck/tests/cisco/__init__.py
--rw-r--r--   0        0        0      819 2024-04-01 17:38:30.519511 pynetcheck-1.0.0/pynetcheck/tests/cisco/conftest.py
--rw-r--r--   0        0        0     2824 2024-04-01 17:38:30.520511 pynetcheck-1.0.0/pynetcheck/tests/cisco/test_servers.py
--rw-r--r--   0        0        0     1797 2024-04-17 18:07:19.984821 pynetcheck-1.0.0/pynetcheck/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.520511 pynetcheck-1.0.0/pynetcheck/tests/cve/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.521511 pynetcheck-1.0.0/pynetcheck/tests/cve/cisco/__init__.py
--rw-r--r--   0        0        0     6260 2024-04-17 18:07:19.985911 pynetcheck-1.0.0/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py
--rw-r--r--   0        0        0     2243 2024-04-17 18:07:19.986989 pynetcheck-1.0.0/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py
--rw-r--r--   0        0        0        0 2024-04-16 18:33:18.641609 pynetcheck-1.0.0/pynetcheck/tests/cve/paloalto/__init__.py
--rw-r--r--   0        0        0     3617 2024-04-17 18:07:19.988052 pynetcheck-1.0.0/pynetcheck/tests/cve/paloalto/test_cve_2024_3400.py
--rw-r--r--   0        0        0        0 2024-04-16 18:33:18.642622 pynetcheck-1.0.0/pynetcheck/tests/paloalto/__init__.py
--rw-r--r--   0        0        0      826 2024-04-16 18:33:18.643609 pynetcheck-1.0.0/pynetcheck/tests/paloalto/conftest.py
--rw-r--r--   0        0        0     1537 2024-04-17 18:07:19.989053 pynetcheck-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9996 2024-04-17 18:07:19.981552 pynetcheck-1.0.0/README.md
--rw-r--r--   0        0        0    11058 1970-01-01 00:00:00.000000 pynetcheck-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-10-17 17:21:13.864484 pynetcheck-1.0.1/LICENSE
+-rw-r--r--   0        0        0      261 2024-04-16 18:33:18.636607 pynetcheck-1.0.1/pynetcheck/__init__.py
+-rw-r--r--   0        0        0    11226 2024-04-16 14:18:36.139811 pynetcheck-1.0.1/pynetcheck/archive/output_1713283371.388187.json
+-rw-r--r--   0        0        0      817 2024-04-16 16:29:18.656699 pynetcheck-1.0.1/pynetcheck/archive/output_1713287098.9189737.json
+-rw-r--r--   0        0        0     6750 2024-04-16 17:04:59.264998 pynetcheck-1.0.1/pynetcheck/archive/output_1713287258.6043513.json
+-rw-r--r--   0        0        0     6750 2024-04-16 17:07:38.964406 pynetcheck-1.0.1/pynetcheck/archive/output_1713287738.6383476.json
+-rw-r--r--   0        0        0     2669 2024-04-16 17:15:39.089976 pynetcheck-1.0.1/pynetcheck/archive/output_1713291137.528805.json
+-rw-r--r--   0        0        0     4475 2024-04-16 18:12:17.905502 pynetcheck-1.0.1/pynetcheck/archive/output_1713291437.5512764.json
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.517432 pynetcheck-1.0.1/pynetcheck/models/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-16 18:33:18.637606 pynetcheck-1.0.1/pynetcheck/models/device.py
+-rw-r--r--   0        0        0      965 2024-04-16 16:43:18.234801 pynetcheck-1.0.1/pynetcheck/models/shared.py
+-rw-r--r--   0        0        0      222 2024-04-16 18:33:18.638606 pynetcheck-1.0.1/pynetcheck/pytest.ini
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-1.0.1/pynetcheck/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-1.0.1/pynetcheck/tests/cisco/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-01 17:38:30.519511 pynetcheck-1.0.1/pynetcheck/tests/cisco/conftest.py
+-rw-r--r--   0        0        0     2824 2024-04-01 17:38:30.520511 pynetcheck-1.0.1/pynetcheck/tests/cisco/test_servers.py
+-rw-r--r--   0        0        0     1931 2024-05-06 15:36:52.414296 pynetcheck-1.0.1/pynetcheck/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.520511 pynetcheck-1.0.1/pynetcheck/tests/cve/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.521511 pynetcheck-1.0.1/pynetcheck/tests/cve/cisco/__init__.py
+-rw-r--r--   0        0        0     6260 2024-04-17 18:07:19.985911 pynetcheck-1.0.1/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py
+-rw-r--r--   0        0        0     2243 2024-04-17 18:07:19.986989 pynetcheck-1.0.1/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:33:18.641609 pynetcheck-1.0.1/pynetcheck/tests/cve/paloalto/__init__.py
+-rw-r--r--   0        0        0     3617 2024-04-17 18:07:19.988052 pynetcheck-1.0.1/pynetcheck/tests/cve/paloalto/test_cve_2024_3400.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:33:18.642622 pynetcheck-1.0.1/pynetcheck/tests/paloalto/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-16 18:33:18.643609 pynetcheck-1.0.1/pynetcheck/tests/paloalto/conftest.py
+-rw-r--r--   0        0        0     1545 2024-05-06 15:36:52.414296 pynetcheck-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9996 2024-04-17 18:07:19.981552 pynetcheck-1.0.1/README.md
+-rw-r--r--   0        0        0    11058 1970-01-01 00:00:00.000000 pynetcheck-1.0.1/PKG-INFO
```

### Comparing `pynetcheck-1.0.0/LICENSE` & `pynetcheck-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/archive/output_1713283371.388187.json` & `pynetcheck-1.0.1/pynetcheck/archive/output_1713283371.388187.json`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/archive/output_1713287098.9189737.json` & `pynetcheck-1.0.1/pynetcheck/archive/output_1713287098.9189737.json`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/archive/output_1713287258.6043513.json` & `pynetcheck-1.0.1/pynetcheck/archive/output_1713287258.6043513.json`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/archive/output_1713287738.6383476.json` & `pynetcheck-1.0.1/pynetcheck/archive/output_1713287738.6383476.json`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/archive/output_1713291137.528805.json` & `pynetcheck-1.0.1/pynetcheck/archive/output_1713291137.528805.json`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/archive/output_1713291437.5512764.json` & `pynetcheck-1.0.1/pynetcheck/archive/output_1713291437.5512764.json`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/models/device.py` & `pynetcheck-1.0.1/pynetcheck/models/device.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/models/shared.py` & `pynetcheck-1.0.1/pynetcheck/models/shared.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/cisco/conftest.py` & `pynetcheck-1.0.1/pynetcheck/tests/cisco/conftest.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/cisco/test_servers.py` & `pynetcheck-1.0.1/pynetcheck/tests/cisco/test_servers.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/conftest.py` & `pynetcheck-1.0.1/pynetcheck/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from importlib import metadata
 from pathlib import Path
 from typing import Optional, Any
 
 from ipfabric import IPFClient
 from pydantic import BaseModel
 
 IPF, CONFIGS = None, []
@@ -59,7 +60,8 @@
     else:
         IPF = IPFClient(
             base_url=config.getoption("--ipf-url"),
             auth=config.getoption("--ipf-token"),
             verify=config.getoption("--insecure", None),
             snapshot_id=config.getoption("--snapshot"),
         )
+        IPF._client.headers['user-agent'] += f'; python-pynetcheck/{metadata.version("pynetcheck")}'
```

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py` & `pynetcheck-1.0.1/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py` & `pynetcheck-1.0.1/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/cve/paloalto/test_cve_2024_3400.py` & `pynetcheck-1.0.1/pynetcheck/tests/cve/paloalto/test_cve_2024_3400.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pynetcheck/tests/paloalto/conftest.py` & `pynetcheck-1.0.1/pynetcheck/tests/paloalto/conftest.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/pyproject.toml` & `pynetcheck-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyNetCheck"
-version = "1.0.0"
+version = "1.0.1"
 license = "MIT"
 description = "Python Network device checker using Pytest and IP Fabric."
 authors = [
     "Solution Architecture <solution.architecture@ipfabric.io>",
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
 ]
 readme = "README.md"
@@ -16,15 +16,15 @@
 
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/pynetcheck/-/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-ipfabric = "^6.7.0"
+ipfabric = ">=6.7.0,<6.9.0"
 ciscoconfparse = "^1.9.0"
 pytest = "^8.0.0"
 pytest-html-reporter = "^0.2.9"
 netutils = "^1.8.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.0"
```

### Comparing `pynetcheck-1.0.0/README.md` & `pynetcheck-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pynetcheck-1.0.0/PKG-INFO` & `pynetcheck-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: PyNetCheck
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Network device checker using Pytest and IP Fabric.
 Home-page: https://gitlab.com/ip-fabric/integrations/pynetcheck
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ciscoconfparse (>=1.9.0,<2.0.0)
-Requires-Dist: ipfabric (>=6.7.0,<7.0.0)
+Requires-Dist: ipfabric (>=6.7.0,<6.9.0)
 Requires-Dist: netutils (>=1.8.0,<2.0.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: pytest-html-reporter (>=0.2.9,<0.3.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/pynetcheck/-/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://gitlab.com/ip-fabric/integrations/pynetcheck
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/pynetcheck
```

