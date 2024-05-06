# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1139.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1139.tar", last modified: Tue Apr 30 04:19:24 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1140.tar", last modified: Mon May  6 08:21:13 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1140.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)     2032 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39983 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7419 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/hunyuan_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/setup.py
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-30 04:19:24.000000 tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39983 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/setup.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-06 08:21:13.000000 tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1140/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1139
+Version: 3.0.1140
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1139'
+__version__ = '3.0.1140'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1140/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1139"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1140"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1140/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1139
+Version: 3.0.1140
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1139/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1140/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*
