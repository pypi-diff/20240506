# Comparing `tmp/datagov_harvesting_logic-0.3.9.tar.gz` & `tmp/datagov_harvesting_logic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.3.9.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.4.0.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.3.9.tar` & `datagov_harvesting_logic-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,10 @@
--rw-r--r--   0        0        0     1878 2024-04-25 20:32:25.177374 datagov_harvesting_logic-0.3.9/LICENSE.md
--rw-r--r--   0        0        0     5265 2024-04-25 20:32:25.177374 datagov_harvesting_logic-0.3.9/README.md
--rw-r--r--   0        0        0      162 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/__init__.py
--rw-r--r--   0        0        0     4489 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/ckan_utils.py
--rw-r--r--   0        0        0     4464 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/arm.data.json
--rw-r--r--   0        0        0     7830 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
--rw-r--r--   0        0        0    14027 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
--rw-r--r--   0        0        0     7454 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/geospatial.data.json
--rw-r--r--   0        0        0   310979 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/large-spatial.data.json
--rw-r--r--   0        0        0      918 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-catalog.data.json
--rw-r--r--   0        0        0     1059 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
--rw-r--r--   0        0        0     3259 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-identifier-title.data.json
--rw-r--r--   0        0        0     1292 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/numerical-title.data.json
--rw-r--r--   0        0        0     2520 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/ny.data.json
--rw-r--r--   0        0        0     1314 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/reserved-title.data.json
--rw-r--r--   0        0        0     9562 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/usda.gov.data.json
--rw-r--r--   0        0        0     1604 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/schemas/catalog.json
--rw-r--r--   0        0        0    23811 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/schemas/dataset.json
--rw-r--r--   0        0        0     2158 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/exceptions.py
--rw-r--r--   0        0        0    25444 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/logger_config.py
--rw-r--r--   0        0        0     3859 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/utils.py
--rw-r--r--   0        0        0     2241 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-05-06 18:08:58.498361 datagov_harvesting_logic-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     5935 2024-05-06 18:08:58.498361 datagov_harvesting_logic-0.4.0/README.md
+-rw-r--r--   0        0        0      164 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/__init__.py
+-rw-r--r--   0        0        0     8369 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     2158 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/exceptions.py
+-rw-r--r--   0        0        0    14138 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/logger_config.py
+-rw-r--r--   0        0        0     4039 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/utils.py
+-rw-r--r--   0        0        0     2275 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.0/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.3.9/LICENSE.md` & `datagov_harvesting_logic-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.9/README.md` & `datagov_harvesting_logic-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 ## Requirements
 
 This project is using `poetry` to manage this project. Install [here](https://python-poetry.org/docs/#installation).
 
 Once installed, `poetry install` installs dependencies into a local virtual environment.
 
+We use [Ruff](https://github.com/astral-sh/ruff) to format and lint our Python files. If you use VS Code, you can install the formatter [here](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff).
+
 ## Testing
 
 ### CKAN load testing
 
 - CKAN load testing doesn't require the services provided in the `docker-compose.yml`.
 - [catalog-dev](https://catalog-dev.data.gov/) is used for ckan load testing.
 - Create an api-key by signing into catalog-dev.
@@ -111,18 +113,30 @@
    ```
 
    This will start the necessary services and execute the test.
 
 3. when there are database DDL changes, use following steps to generate migration scripts and update database:
 
     ```bash
-    docker compose db up
+    docker compose up -d db
     docker compose run app flask db migrate -m "migration description"
     docker compose run app flask db upgrade
     ```
+### Debugging
+*NOTE: To use the VS-Code debugger, you will first need to sacrifice the reloading support for flask*
+
+1. Build new containers with development requirements by running `make build-dev`
+
+2. Launch containers by running `make up-debug`
+
+3. In VS-Code, launch debug process `Python: Remote Attach`
+
+4. Set breakpoints
+
+5. Visit the site at `http://localhost:8080` and invoke the route which contains the code you've set the breakpoint on.
 
 ### Deployment to cloud.gov
 
 #### Database Service Setup
 
 A database service is required for use on cloud.gov.
```

### Comparing `datagov_harvesting_logic-0.3.9/harvester/exceptions.py` & `datagov_harvesting_logic-0.4.0/harvester/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from datetime import datetime
-from app.interface import HarvesterDBInterface
+
+from database.interface import HarvesterDBInterface
 
 
 # critical exceptions
 class HarvestCriticalException(Exception):
     def __init__(self, msg, harvest_job_id):
         super().__init__(msg, harvest_job_id)
 
@@ -24,19 +25,19 @@
             "date_created": datetime.utcnow(),
         }
 
         self.db_interface.add_harvest_error(error_data)
         self.logger.critical(self.msg, exc_info=True)
 
 
-class ExtractHarvestSourceException(HarvestCriticalException):
+class ExtractExternalException(HarvestCriticalException):
     pass
 
 
-class ExtractCKANSourceException(HarvestCriticalException):
+class ExtractInternalException(HarvestCriticalException):
     pass
 
 
 class CompareException(HarvestCriticalException):
     pass
 
 
@@ -56,15 +57,15 @@
 
         error_data = {
             "harvest_job_id": self.harvest_job_id,
             "message": self.msg,
             "severity": self.severity,
             "type": self.type,
             "date_created": datetime.utcnow(),
-            "harvest_record_id": self.title # to-do 
+            "harvest_record_id": self.title,  # to-do
         }
 
         self.db_interface.add_harvest_error(error_data)
         self.logger.error(self.msg, exc_info=True)
 
 
 class ValidationException(HarvestNonCriticalException):
```

### Comparing `datagov_harvesting_logic-0.3.9/harvester/logger_config.py` & `datagov_harvesting_logic-0.4.0/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.9/harvester/utils.py` & `datagov_harvesting_logic-0.4.0/harvester/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+import argparse
 import hashlib
 import json
 import os
-import argparse
+import xml.etree.ElementTree as ET
+from typing import Union
 
-import boto3
+import requests
+from bs4 import BeautifulSoup
 import sansjson
-
 from cloudfoundry_client.client import CloudFoundryClient
 from cloudfoundry_client.v3.tasks import TaskManager
 
 # ruff: noqa: F841
 
 
+def get_title_from_fgdc(xml_str: str) -> str:
+    tree = ET.ElementTree(ET.fromstring(xml_str))
+    return tree.find(".//title").text
+
+
 def parse_args(args):
 
     parser = argparse.ArgumentParser(
         prog="Harvest Runner", description="etl harvest sources"
     )
     parser.add_argument("-j", "--jobid")
 
@@ -42,65 +49,80 @@
     """open input json file as dictionary
     file_path (str)     :   json file path.
     """
     with open(file_path) as fp:
         return json.load(fp)
 
 
-class S3Handler:
-    def __init__(self):
-        self.access_key_id = os.getenv("S3FILESTORE__AWS_ACCESS_KEY_ID")
-        self.secret_access_key = os.getenv("S3FILESTORE__AWS_SECRET_ACCESS_KEY")
-        self.region_name = os.getenv("S3FILESTORE__REGION_NAME")
-        self.endpoint_url = os.getenv("S3FILESTORE__HOST_NAME")
-        self.bucket = os.getenv("S3FILESTORE__AWS_BUCKET_NAME")
-
-        # S3://{h20-bucket-prefix}/{harvest-source}/{harvest-job-id}/{ETL-process-step}/{example.json}
-        self.out_harvest_source = "{}/{}/{}/{ETL-process-step}/{example.json}"
-        self.out_harvest_record = None
-
-        self.config = {
-            "aws_access_key_id": self.access_key_id,
-            "aws_secret_access_key": self.secret_access_key,
-            "region_name": self.region_name,
-            "endpoint_url": self.endpoint_url,
-        }
-
-        self.client = boto3.client("s3", **self.config)
-
-    def create_bucket(self):
-        return self.client.create_bucket(Bucket=self.bucket)
-
-    def delete_object(self, object_key: str):
-        return self.client.delete_object(Bucket=self.bucket, Key=object_key)
-
-    def get_object(self, object_key: str):
-        return self.client.get_object(Bucket=self.bucket, Key=object_key)
-
-    def put_object(self, body: str, key_name: str):
-        return self.client.put_object(
-            **{
-                "Body": body,
-                "Bucket": self.bucket,
-                "Key": key_name,
-                "ContentType": "application/json",
-            }
-        )
+def download_file(url: str, file_type: str) -> Union[str, dict]:
+    resp = requests.get(url)
+    if 200 <= resp.status_code < 300:
+        if file_type == ".xml":
+            return resp.content
+        return resp.json()
 
 
-class CFHandler:
-    def __init__(self, url: str = None, user: str = None, password: str = None):
-        self.target_endpoint = url if url is not None else os.getenv("CF_API_URL")
-        self.client = CloudFoundryClient(self.target_endpoint)
-        self.client.init_with_user_credentials(
-            user if user is not None else os.getenv("CF_SERVICE_USER"),
-            password if password is not None else os.getenv("CF_SERVICE_AUTH"),
-        )
+def traverse_waf(
+    url, files=[], file_ext=".xml", folder="/", filters=["../", "dcatus/"]
+):
+    """Transverses WAF
+    Please add docstrings
+    """
+    # TODO: add exception handling
+    parent = os.path.dirname(url.rstrip("/"))
 
-        self.task_mgr = TaskManager(self.target_endpoint, self.client)
+    folders = []
+
+    res = requests.get(url)
+    if res.status_code == 200:
+        soup = BeautifulSoup(res.content, "html.parser")
+        anchors = soup.find_all("a", href=True)
+
+        for anchor in anchors:
+            if (
+                anchor["href"].endswith(folder)  # is the anchor link a folder?
+                and not parent.endswith(
+                    anchor["href"].rstrip("/")
+                )  # it's not the parent folder right?
+                and anchor["href"] not in filters  # and it's not on our exclusion list?
+            ):
+                folders.append(os.path.join(url, anchor["href"]))
+
+            if anchor["href"].endswith(file_ext):
+                # TODO: just download the file here
+                # instead of storing them and returning at the end.
+                files.append(os.path.join(url, anchor["href"]))
+
+    for folder in folders:
+        traverse_waf(folder, files=files, filters=filters)
+
+    return files
+
+
+def download_waf(files):
+    """Downloads WAF
+    Please add docstrings
+    """
+    output = []
+    for file in files:
+        output.append({"url": file, "content": download_file(file, ".xml")})
+
+    return output
+
+
+class CFHandler:
+    def __init__(self, url: str, user: str, password: str):
+        self.url = url
+        self.user = user
+        self.password = password
+
+    def setup(self):
+        self.client = CloudFoundryClient(self.url)
+        self.client.init_with_user_credentials(self.user, self.password)
+        self.task_mgr = TaskManager(self.url, self.client)
 
     def start_task(self, app_guuid, command, task_id):
         return self.task_mgr.create(app_guuid, command, task_id)
 
     def stop_task(self, task_id):
         return self.task_mgr.cancel(task_id)
```

### Comparing `datagov_harvesting_logic-0.3.9/pyproject.toml` & `datagov_harvesting_logic-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
@@ -18,32 +18,33 @@
 repository = "https://github.com/GSA/datagov-harvesting-logic"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 jsonschema = ">=4"
 python-dotenv = ">=1"
 deepdiff = ">=6"
-pytest = ">=7.3.2"
 ckanapi = ">=4.7"
 beautifulsoup4 = "^4.12.2"
 sansjson = "^0.3.0"
-boto3 = "^1.34.29"
 sqlalchemy = "^2.0.25"
 flask = "^3.0.2"
 psycopg2-binary = "^2.9.9"
 flask-sqlalchemy = "^3.1.1"
 flask-wtf = "^1.2.1"
 flask-migrate = "^4.0.7"
 flask-bootstrap = "^3.3.7.1"
 cloudfoundry-client = "^1.36.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.0"
-ruff = "^0.0.261"
+pytest = ">=7.3.2"
+ruff = "^0.0.291"
 pytest-cov = "^4.0.0"
+debugpy = "^1.8.1"
+isort = "^5.13.2"
+black = "^24.4.2"
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 ignore = []
 ignore-init-module-imports = true
 
@@ -69,14 +70,15 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "migrations"
 ]
 
 # Same as Black.
 line-length = 88
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
@@ -84,11 +86,10 @@
 # Assume Python 3.10.
 target-version = "py310"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datagov_harvesting_logic-0.3.9/PKG-INFO` & `datagov_harvesting_logic-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
 Requires-Python: >=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: boto3 (>=1.34.29,<2.0.0)
 Requires-Dist: ckanapi (>=4.7)
 Requires-Dist: cloudfoundry-client (>=1.36.0,<2.0.0)
 Requires-Dist: deepdiff (>=6)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
 Requires-Dist: flask-bootstrap (>=3.3.7.1,<4.0.0.0)
 Requires-Dist: flask-migrate (>=4.0.7,<5.0.0)
 Requires-Dist: flask-sqlalchemy (>=3.1.1,<4.0.0)
 Requires-Dist: flask-wtf (>=1.2.1,<2.0.0)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
-Requires-Dist: pytest (>=7.3.2)
 Requires-Dist: python-dotenv (>=1)
 Requires-Dist: sansjson (>=0.3.0,<0.4.0)
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
 Project-URL: Repository, https://github.com/GSA/datagov-harvesting-logic
 Description-Content-Type: text/markdown
 
 # datagov-harvesting-logic
@@ -54,14 +52,16 @@
 
 ## Requirements
 
 This project is using `poetry` to manage this project. Install [here](https://python-poetry.org/docs/#installation).
 
 Once installed, `poetry install` installs dependencies into a local virtual environment.
 
+We use [Ruff](https://github.com/astral-sh/ruff) to format and lint our Python files. If you use VS Code, you can install the formatter [here](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff).
+
 ## Testing
 
 ### CKAN load testing
 
 - CKAN load testing doesn't require the services provided in the `docker-compose.yml`.
 - [catalog-dev](https://catalog-dev.data.gov/) is used for ckan load testing.
 - Create an api-key by signing into catalog-dev.
@@ -146,18 +146,30 @@
    ```
 
    This will start the necessary services and execute the test.
 
 3. when there are database DDL changes, use following steps to generate migration scripts and update database:
 
     ```bash
-    docker compose db up
+    docker compose up -d db
     docker compose run app flask db migrate -m "migration description"
     docker compose run app flask db upgrade
     ```
+### Debugging
+*NOTE: To use the VS-Code debugger, you will first need to sacrifice the reloading support for flask*
+
+1. Build new containers with development requirements by running `make build-dev`
+
+2. Launch containers by running `make up-debug`
+
+3. In VS-Code, launch debug process `Python: Remote Attach`
+
+4. Set breakpoints
+
+5. Visit the site at `http://localhost:8080` and invoke the route which contains the code you've set the breakpoint on.
 
 ### Deployment to cloud.gov
 
 #### Database Service Setup
 
 A database service is required for use on cloud.gov.
```

