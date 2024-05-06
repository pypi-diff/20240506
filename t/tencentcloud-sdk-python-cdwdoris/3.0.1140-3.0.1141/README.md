# Comparing `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1140.tar.gz` & `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1140.tar", last modified: Mon May  6 08:04:36 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1141.tar", last modified: Mon May  6 20:35:12 2024, max compression
```

## Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140.tar` & `tencentcloud-sdk-python-cdwdoris-3.0.1141.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/
--rw-r--r--   0 root         (0) root         (0)      703 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   129648 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16479 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/setup.py
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-06 08:04:36.000000 tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/
+-rw-r--r--   0 root         (0) root         (0)      703 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   129648 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16479 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/setup.py
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-06 20:35:12.000000 tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1140
+Version: 3.0.1141
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/errorcodes.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/models.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1140'
+__version__ = '3.0.1141'
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/setup.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdwdoris',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1140"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1141"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdwdoris SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/README.rst` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1140
+Version: 3.0.1141
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1140/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cdwdoris-3.0.1141/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

