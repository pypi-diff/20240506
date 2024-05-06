# Comparing `tmp/cognite_extractor_utils-7.1.2.tar.gz` & `tmp/cognite_extractor_utils-7.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-7.1.2.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-7.1.3.tar", max compression
```

## Comparing `cognite_extractor_utils-7.1.2.tar` & `cognite_extractor_utils-7.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10173 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/LICENSE
--rw-r--r--   0        0        0     4090 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/README.md
--rw-r--r--   0        0        0      739 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    16148 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     3059 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    21334 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0    16317 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1084 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    15509 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0        0 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    18645 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3605 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/threading.py
--rw-r--r--   0        0        0     3110 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5282 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3247 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5628 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/assets.py
--rw-r--r--   0        0        0     5680 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    18417 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     6738 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26548 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7732 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1020 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    17198 2024-04-18 08:43:25.810994 cognite_extractor_utils-7.1.2/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2097 2024-04-18 08:43:25.814993 cognite_extractor_utils-7.1.2/pyproject.toml
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/LICENSE
+-rw-r--r--   0        0        0     4090 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/README.md
+-rw-r--r--   0        0        0      739 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    16148 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     3059 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    21334 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0    16317 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1084 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    15509 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    18645 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3605 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/threading.py
+-rw-r--r--   0        0        0     3110 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5282 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3247 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5628 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     5680 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    18417 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6738 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26817 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7732 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1020 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    17198 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2088 2024-05-06 08:50:33.620455 cognite_extractor_utils-7.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.3/PKG-INFO
```

### Comparing `cognite_extractor_utils-7.1.2/LICENSE` & `cognite_extractor_utils-7.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/README.md` & `cognite_extractor_utils-7.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "7.1.2"
+__version__ = "7.1.3"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/base.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/threading.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/threading.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/assets.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import (
     Sequence,
     SequenceData,
     SequenceRows,
+    StatusCode,
     TimeSeries,
 )
 from cognite.client.exceptions import CogniteDuplicatedError, CogniteNotFoundError
 from cognite.extractorutils.threading import CancellationToken
 from cognite.extractorutils.uploader._base import (
     RETRIES,
     RETRY_BACKOFF_FACTOR,
@@ -47,15 +48,18 @@
 MIN_DATAPOINT_TIMESTAMP = -2208988800000
 MAX_DATAPOINT_STRING_LENGTH = 255
 MAX_DATAPOINT_VALUE = 1e100
 MIN_DATAPOINT_VALUE = -1e100
 
 TimeStamp = Union[int, datetime]
 
-DataPoint = Union[Tuple[TimeStamp, float], Tuple[TimeStamp, str]]
+DataPointWithoutStatus = Union[Tuple[TimeStamp, float], Tuple[TimeStamp, str], Tuple[TimeStamp, int]]
+FullStatusCode = Union[StatusCode, int]
+DataPointWithStatus = Union[Tuple[TimeStamp, float, FullStatusCode], Tuple[TimeStamp, str, FullStatusCode]]
+DataPoint = Union[DataPointWithoutStatus, DataPointWithStatus]
 DataPointList = List[DataPoint]
 
 
 def default_time_series_factory(external_id: str, datapoints: DataPointList) -> TimeSeries:
     """
     Default time series factory used when create_missing in a TimeSeriesUploadQueue is given as a boolean.
 
@@ -279,15 +283,15 @@
 
         if len(self.upload_queue) == 0:
             return
 
         with self.lock:
             upload_this = _upload_batch(
                 [
-                    {either_id.type(): either_id.content(), "datapoints": datapoints}
+                    {either_id.type(): either_id.content(), "datapoints": list(datapoints)}
                     for either_id, datapoints in self.upload_queue.items()
                     if len(datapoints) > 0
                 ]
             )
 
             for _either_id, datapoints in self.upload_queue.items():
                 self.points_written.inc(len(datapoints))
```

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/cognite/extractorutils/util.py` & `cognite_extractor_utils-7.1.3/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.2/pyproject.toml` & `cognite_extractor_utils-7.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "7.1.2"
+version = "7.1.3"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
@@ -49,15 +49,15 @@
 show_error_codes = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 exclude = "tests/*"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-cognite-sdk = ">=7.28.1, <7.35.0"
+cognite-sdk = "^7.41.0"
 prometheus-client = ">0.7.0, <=1.0.0"
 arrow = "^1.0.0"
 pyyaml = ">=5.3.0, <7"
 dacite = "^1.6.0"
 psutil = "^5.7.0"
 decorator = "^5.1.1"
 more-itertools = "^10.0.0"
@@ -66,16 +66,16 @@
 azure-identity = "^1.14.0"
 azure-keyvault-secrets = "^4.7.0"
 
 [tool.poetry.extras]
 experimental = ["cognite-sdk-experimental"]
 
 [tool.poetry.group.dev.dependencies]
-mypy = "1.9.0"
-ruff = "^0.3.0"
+mypy = "1.10.0"
+ruff = "^0.4.0"
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 sphinx = "^7.0.0"
 sphinx-rtd-theme = "^2.0.0"
 pre-commit = "^3.3.0"
 SecretStorage = "^3.1.2"
 twine = "^5.0.0"
```

### Comparing `cognite_extractor_utils-7.1.2/PKG-INFO` & `cognite_extractor_utils-7.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 7.1.2
+Version: 7.1.3
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: experimental
 Requires-Dist: arrow (>=1.0.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.14.0,<2.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
-Requires-Dist: cognite-sdk (>=7.28.1,<7.35.0)
+Requires-Dist: cognite-sdk (>=7.41.0,<8.0.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
 Requires-Dist: prometheus-client (>0.7.0,<=1.0.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=5.3.0,<7)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.2 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.3 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: experimental Requires-Dist: arrow (>=1.0.0,<2.0.0) Requires-
 Dist: azure-identity (>=1.14.0,<2.0.0) Requires-Dist: azure-keyvault-secrets
-(>=4.7.0,<5.0.0) Requires-Dist: cognite-sdk (>=7.28.1,<7.35.0) Requires-Dist:
+(>=4.7.0,<5.0.0) Requires-Dist: cognite-sdk (>=7.41.0,<8.0.0) Requires-Dist:
 dacite (>=1.6.0,<2.0.0) Requires-Dist: decorator (>=5.1.1,<6.0.0) Requires-
 Dist: more-itertools (>=10.0.0,<11.0.0) Requires-Dist: prometheus-client
 (>0.7.0,<=1.0.0) Requires-Dist: psutil (>=5.7.0,<6.0.0) Requires-Dist: python-
 dotenv (>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=5.3.0,<7) Requires-Dist:
 typing-extensions (>=3.7.4,<5) Project-URL: Repository, https://github.com/
 cognitedata/python-extractor-utils Description-Content-Type: text/markdown
 _[_C_o_g_n_i_t_e_ _l_o_g_o_]Cognite Python `extractor-utils` ================================
```

