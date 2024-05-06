# Comparing `tmp/tmdsclient-0.1.22.tar.gz` & `tmp/tmdsclient-0.2.0.tar.gz`

## Comparing `tmdsclient-0.1.22.tar` & `tmdsclient-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,53 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/README.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/domain-specific-terms.txt
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/requirements.txt
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/_tmdsclient_version.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/py.typed
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/client/__init__.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/client/config.py
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/client/tmdsclient.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/models/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/models/bo4e_stub.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/models/netzvertrag.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/src/tmdsclient/models/patches.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/pyproject.toml
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 tmdsclient-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/README.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/domain-specific-terms.txt
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/_tmdsclient_version.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/py.typed
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/client/__init__.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/client/config.py
+-rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/client/tmdsclient.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/bo4e_stub.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/messlokation.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/netzvertrag.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/partneradresse.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/patches.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/utils.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/zaehler.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/zaehler_bo_model.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/zaehlergroesse.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/zaehlerhersteller.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/zaehlwerk.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/src/tmdsclient/models/zeitscheibe.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tmdsclient-0.2.0/PKG-INFO
```

### Comparing `tmdsclient-0.1.22/.pre-commit-config.yaml` & `tmdsclient-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/README.md` & `tmdsclient-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/requirements.txt` & `tmdsclient-0.2.0/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile pyproject.toml
 #
-aiohttp[speedups]==3.9.3
+aiohttp[speedups]==3.9.4
     # via tmdsclient (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 annotated-types==0.6.0
     # via pydantic
 attrs==23.2.0
     # via aiohttp
+bo4e==202401.1.1
+    # via tmdsclient (pyproject.toml)
 brotli==1.1.0
     # via aiohttp
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-idna==3.6
+idna==3.7
     # via yarl
+iso3166==2.1.1
+    # via bo4e
 jsonpatch==1.33
     # via tmdsclient (pyproject.toml)
 jsonpointer==2.4
     # via jsonpatch
 more-itertools==10.2.0
     # via tmdsclient (pyproject.toml)
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 pydantic==2.6.4
-    # via tmdsclient (pyproject.toml)
+    # via
+    #   bo4e
+    #   tmdsclient (pyproject.toml)
 pydantic-core==2.16.3
     # via pydantic
+pyhumps==3.8.0
+    # via bo4e
 typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
 yarl==1.9.4
     # via aiohttp
```

### Comparing `tmdsclient-0.1.22/tox.ini` & `tmdsclient-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/dependabot.yml` & `tmdsclient-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/codeql-analysis.yml` & `tmdsclient-0.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/coverage.yml` & `tmdsclient-0.2.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/dependabot_automerge.yml` & `tmdsclient-0.2.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/dev_test.yml` & `tmdsclient-0.2.0/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/formatting.yml` & `tmdsclient-0.2.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/packaging_test.yml` & `tmdsclient-0.2.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/python-publish.yml` & `tmdsclient-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/pythonlint.yml` & `tmdsclient-0.2.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.github/workflows/unittests.yml` & `tmdsclient-0.2.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/dev_requirements/requirements-linting.txt` & `tmdsclient-0.2.0/dev_requirements/requirements-linting.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/dev_requirements/requirements-packaging.txt` & `tmdsclient-0.2.0/dev_requirements/requirements-packaging.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile dev_requirements/requirements-packaging.in
 #
 build==1.2.1
-    # via -r dev_requirements/requirements-packaging.in
+    # via -r requirements-packaging.in
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 cryptography==42.0.5
     # via secretstorage
 docutils==0.20.1
     # via readme-renderer
-idna==3.6
+idna==3.7
     # via requests
 importlib-metadata==7.0.2
     # via
     #   keyring
     #   twine
 jaraco-classes==3.3.1
     # via keyring
@@ -65,14 +65,14 @@
 secretstorage==3.3.3
     # via keyring
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
 twine==5.0.0
-    # via -r dev_requirements/requirements-packaging.in
+    # via -r requirements-packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `tmdsclient-0.1.22/dev_requirements/requirements-tests.txt` & `tmdsclient-0.2.0/dev_requirements/requirements-tests.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile requirements-tests.in
 #
-aiohttp==3.9.3
+aiohttp==3.9.4
     # via aioresponses
 aioresponses==0.7.6
-    # via -r dev_requirements/requirements-tests.in
+    # via -r requirements-tests.in
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 exceptiongroup==1.2.0
     # via pytest
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-idna==3.6
+idna==3.7
     # via yarl
 iniconfig==2.0.0
     # via pytest
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 packaging==23.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pytest==8.1.1
+pytest==8.2.0
     # via
-    #   -r dev_requirements/requirements-tests.in
+    #   -r requirements-tests.in
     #   pytest-asyncio
 pytest-asyncio==0.23.6
-    # via -r dev_requirements/requirements-tests.in
+    # via -r requirements-tests.in
 tomli==2.0.1
     # via pytest
 yarl==1.9.4
     # via aiohttp
```

### Comparing `tmdsclient-0.1.22/src/tmdsclient/client/config.py` & `tmdsclient-0.2.0/src/tmdsclient/client/config.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/src/tmdsclient/client/tmdsclient.py` & `tmdsclient-0.2.0/src/tmdsclient/client/tmdsclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 from aiohttp import BasicAuth, ClientResponseError, ClientSession, ClientTimeout
 from more_itertools import chunked
 from yarl import URL
 
 from tmdsclient.client.config import TmdsConfig
 from tmdsclient.models import AllIdsResponse
+from tmdsclient.models.messlokation import Messlokation
 from tmdsclient.models.netzvertrag import Netzvertrag, _ListOfNetzvertraege
 from tmdsclient.models.patches import build_json_patch_document
+from tmdsclient.models.zaehler import Zaehler
 
 _logger = logging.getLogger(__name__)
 
 _DEFAULT_CHUNK_SIZE = 100
 
 
 def _log_chunk_success(chunk_size: int, total_size: int, chunk_idx: int, chunk_length: int) -> None:
@@ -279,7 +281,45 @@
             request_url, json=patch_document.patch, headers={"Content-Type": "application/json-patch+json"}
         ) as response:
             response.raise_for_status()
             _logger.debug("[%s] response status: %s", str(request_uuid), response.status)
             response_json = await response.json()
             result = Netzvertrag.model_validate(response_json)
         return result
+
+    async def get_messlokation(self, messlokation_id: str) -> Messlokation | None:
+        """
+        provide a Messlokation-ID, get the matching MeLo in return (or None, if 404)
+        """
+        session = await self._get_session()
+        request_url = self._config.server_url / "api" / "Messlokation" / messlokation_id
+        request_uuid = uuid.uuid4()
+        _logger.debug("[%s] requesting %s", str(request_uuid), request_url)
+        async with session.get(request_url) as response:
+            try:
+                if response.status == 404:
+                    return None
+                response.raise_for_status()
+            finally:
+                _logger.debug("[%s] response status: %s", str(request_uuid), response.status)
+            response_json = await response.json()
+            result = Messlokation.model_validate(response_json)
+        return result
+
+    async def get_zaehler(self, zaehler_id: uuid.UUID) -> Zaehler | None:
+        """
+        provide a Zaehler-ID, get the matching Zaehler in return (or None, if 404)
+        """
+        session = await self._get_session()
+        request_url = self._config.server_url / "api" / "Zaehler" / str(zaehler_id)
+        request_uuid = uuid.uuid4()
+        _logger.debug("[%s] requesting %s", str(request_uuid), request_url)
+        async with session.get(request_url) as response:
+            try:
+                if response.status == 404:
+                    return None
+                response.raise_for_status()
+            finally:
+                _logger.debug("[%s] response status: %s", str(request_uuid), response.status)
+            response_json = await response.json()
+            result = Zaehler.model_validate(response_json)
+        return result
```

### Comparing `tmdsclient-0.1.22/src/tmdsclient/models/bo4e_stub.py` & `tmdsclient-0.2.0/src/tmdsclient/models/bo4e_stub.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/src/tmdsclient/models/netzvertrag.py` & `tmdsclient-0.2.0/src/tmdsclient/models/netzvertrag.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/src/tmdsclient/models/patches.py` & `tmdsclient-0.2.0/src/tmdsclient/models/patches.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/.gitignore` & `tmdsclient-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/LICENSE` & `tmdsclient-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.22/pyproject.toml` & `tmdsclient-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pydantic>=2.0.0",
-    "aiohttp[speedups]>=3.9.3",
+    "aiohttp[speedups]>=3.9.4",
     "jsonpatch",
     "more_itertools",
+    "bo4e>=202401.1.1",
 ] # add all the dependencies here
 dynamic = ["readme", "version"]
 
 [project.urls]
 Changelog = "https://github.com/Hochfrequenz/tmdsclient.py/releases"
 Homepage = "https://github.com/Hochfrequenz/tmdsclient.py"
```

### Comparing `tmdsclient-0.1.22/PKG-INFO` & `tmdsclient-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tmdsclient
-Version: 0.1.22
+Version: 0.2.0
 Summary: Fully typed, async client library for Technical Master Data Service (TMDS)
 Project-URL: Changelog, https://github.com/Hochfrequenz/tmdsclient.py/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/tmdsclient.py
 Author-email: Hochfreuqenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: technical master data,tmds
@@ -14,15 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
-Requires-Dist: aiohttp[speedups]>=3.9.3
+Requires-Dist: aiohttp[speedups]>=3.9.4
+Requires-Dist: bo4e>=202401.1.1
 Requires-Dist: jsonpatch
 Requires-Dist: more-itertools
 Requires-Dist: pydantic>=2.0.0
 Description-Content-Type: text/markdown
 
 # tmdsclient.py
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
```

