# Comparing `tmp/alibabacloud_cas20200407_py2-1.2.0.tar.gz` & `tmp/alibabacloud_cas20200407_py2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cas20200407_py2-1.2.0.tar", last modified: Wed Mar 13 17:18:08 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cas20200407_py2-1.3.0.tar", last modified: Mon May  6 06:18:38 2024, max compression
```

## Comparing `alibabacloud_cas20200407_py2-1.2.0.tar` & `alibabacloud_cas20200407_py2-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2493 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81561 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407/client.py
--rw-r--r--   0 root         (0) root         (0)   232892 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2493 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2924 2024-03-13 17:18:08.000000 alibabacloud_cas20200407_py2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1645 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87462 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407/client.py
+-rw-r--r--   0 root         (0) root         (0)   269198 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-06 06:18:38.000000 alibabacloud_cas20200407_py2-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-05-06 06:18:37.000000 alibabacloud_cas20200407_py2-1.3.0/setup.py
```

### Comparing `alibabacloud_cas20200407_py2-1.2.0/LICENSE` & `alibabacloud_cas20200407_py2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cas20200407_py2-1.2.0/PKG-INFO` & `alibabacloud_cas20200407_py2-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cas20200407_py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud SSL Certificates Service (20200407) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cas20200407_py2-1.2.0/README-CN.md` & `alibabacloud_cas20200407_py2-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cas20200407_py2-1.2.0/README.md` & `alibabacloud_cas20200407_py2-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407/client.py` & `alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,14 +801,70 @@
         @param request: DescribeCertificateStateRequest
 
         @return: DescribeCertificateStateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_certificate_state_with_options(request, runtime)
 
+    def describe_cloud_resource_status_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.secret_id):
+            query['SecretId'] = request.secret_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCloudResourceStatus',
+            version='2020-04-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cas_20200407_models.DescribeCloudResourceStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_cloud_resource_status(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cloud_resource_status_with_options(request, runtime)
+
+    def describe_deployment_job_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDeploymentJob',
+            version='2020-04-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cas_20200407_models.DescribeDeploymentJobResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_deployment_job(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_deployment_job_with_options(request, runtime)
+
     def describe_deployment_job_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
@@ -1083,14 +1139,48 @@
             self.call_api(params, req, runtime)
         )
 
     def list_cert_warehouse(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_cert_warehouse_with_options(request, runtime)
 
+    def list_cloud_access_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cloud_name):
+            query['CloudName'] = request.cloud_name
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.secret_id):
+            query['SecretId'] = request.secret_id
+        if not UtilClient.is_unset(request.show_size):
+            query['ShowSize'] = request.show_size
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListCloudAccess',
+            version='2020-04-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cas_20200407_models.ListCloudAccessResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_cloud_access(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_cloud_access_with_options(request, runtime)
+
     def list_cloud_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cloud_name):
             query['CloudName'] = request.cloud_name
         if not UtilClient.is_unset(request.cloud_product):
             query['CloudProduct'] = request.cloud_product
@@ -1121,14 +1211,46 @@
             self.call_api(params, req, runtime)
         )
 
     def list_cloud_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_cloud_resources_with_options(request, runtime)
 
+    def list_contact_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.keyword):
+            query['Keyword'] = request.keyword
+        if not UtilClient.is_unset(request.show_size):
+            query['ShowSize'] = request.show_size
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListContact',
+            version='2020-04-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cas_20200407_models.ListContactResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_contact(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_contact_with_options(request, runtime)
+
     def list_csr_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.algorithm):
             query['Algorithm'] = request.algorithm
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
@@ -1305,14 +1427,50 @@
         @param request: ListUserCertificateOrderRequest
 
         @return: ListUserCertificateOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_user_certificate_order_with_options(request, runtime)
 
+    def list_worker_resource_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cloud_product):
+            query['CloudProduct'] = request.cloud_product
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        if not UtilClient.is_unset(request.show_size):
+            query['ShowSize'] = request.show_size
+        if not UtilClient.is_unset(request.status):
+            query['Status'] = request.status
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListWorkerResource',
+            version='2020-04-07',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cas_20200407_models.ListWorkerResourceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_worker_resource(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_worker_resource_with_options(request, runtime)
+
     def renew_certificate_order_for_package_request_with_options(self, request, runtime):
         """
         You can call this operation to submit a renewal application for a certificate only when the order of the certificate is in the expiring state. After the renewal is complete, a new certificate order whose status is pending application is generated. You must submit a certificate application for the new certificate order and install the new certificate after the new certificate is issued.
         > You can call the [DescribeCertificateState](~~455800~~) operation to query the status of a certificate application order. If the value of the **Type** response parameter is **certificate**, the certificate is issued.
         
 
         @param request: RenewCertificateOrderForPackageRequestRequest
```

### Comparing `alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407/models.py` & `alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1893,14 +1893,368 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCertificateStateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCloudResourceStatusRequest(TeaModel):
+    def __init__(self, secret_id=None):
+        self.secret_id = secret_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCloudResourceStatusRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.secret_id is not None:
+            result['SecretId'] = self.secret_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('SecretId') is not None:
+            self.secret_id = m.get('SecretId')
+        return self
+
+
+class DescribeCloudResourceStatusResponseBodyData(TeaModel):
+    def __init__(self, cloud_name=None, cloud_product=None, total_count=None):
+        self.cloud_name = cloud_name  # type: str
+        self.cloud_product = cloud_product  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCloudResourceStatusResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cloud_name is not None:
+            result['CloudName'] = self.cloud_name
+        if self.cloud_product is not None:
+            result['CloudProduct'] = self.cloud_product
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CloudName') is not None:
+            self.cloud_name = m.get('CloudName')
+        if m.get('CloudProduct') is not None:
+            self.cloud_product = m.get('CloudProduct')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeCloudResourceStatusResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: list[DescribeCloudResourceStatusResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeCloudResourceStatusResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeCloudResourceStatusResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeCloudResourceStatusResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeCloudResourceStatusResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeCloudResourceStatusResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeCloudResourceStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDeploymentJobRequest(TeaModel):
+    def __init__(self, job_id=None):
+        self.job_id = job_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDeploymentJobRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        return self
+
+
+class DescribeDeploymentJobResponseBodyCasContacts(TeaModel):
+    def __init__(self, email=None, id=None, mobile=None, name=None):
+        self.email = email  # type: str
+        self.id = id  # type: str
+        self.mobile = mobile  # type: str
+        self.name = name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDeploymentJobResponseBodyCasContacts, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class DescribeDeploymentJobResponseBody(TeaModel):
+    def __init__(self, cas_contacts=None, cert_domain=None, cert_type=None, config=None, del_=None, end_time=None,
+                 gmt_create=None, gmt_modified=None, id=None, instance_id=None, job_type=None, name=None, product_name=None,
+                 request_id=None, rollback=None, schedule_time=None, start_time=None, status=None, user_id=None):
+        self.cas_contacts = cas_contacts  # type: list[DescribeDeploymentJobResponseBodyCasContacts]
+        self.cert_domain = cert_domain  # type: str
+        self.cert_type = cert_type  # type: str
+        self.config = config  # type: str
+        self.del_ = del_  # type: int
+        self.end_time = end_time  # type: str
+        self.gmt_create = gmt_create  # type: str
+        self.gmt_modified = gmt_modified  # type: str
+        self.id = id  # type: long
+        self.instance_id = instance_id  # type: str
+        self.job_type = job_type  # type: str
+        self.name = name  # type: str
+        self.product_name = product_name  # type: str
+        self.request_id = request_id  # type: str
+        self.rollback = rollback  # type: int
+        self.schedule_time = schedule_time  # type: str
+        self.start_time = start_time  # type: str
+        self.status = status  # type: str
+        self.user_id = user_id  # type: long
+
+    def validate(self):
+        if self.cas_contacts:
+            for k in self.cas_contacts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDeploymentJobResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['CasContacts'] = []
+        if self.cas_contacts is not None:
+            for k in self.cas_contacts:
+                result['CasContacts'].append(k.to_map() if k else None)
+        if self.cert_domain is not None:
+            result['CertDomain'] = self.cert_domain
+        if self.cert_type is not None:
+            result['CertType'] = self.cert_type
+        if self.config is not None:
+            result['Config'] = self.config
+        if self.del_ is not None:
+            result['Del'] = self.del_
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.job_type is not None:
+            result['JobType'] = self.job_type
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.product_name is not None:
+            result['ProductName'] = self.product_name
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.rollback is not None:
+            result['Rollback'] = self.rollback
+        if self.schedule_time is not None:
+            result['ScheduleTime'] = self.schedule_time
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.cas_contacts = []
+        if m.get('CasContacts') is not None:
+            for k in m.get('CasContacts'):
+                temp_model = DescribeDeploymentJobResponseBodyCasContacts()
+                self.cas_contacts.append(temp_model.from_map(k))
+        if m.get('CertDomain') is not None:
+            self.cert_domain = m.get('CertDomain')
+        if m.get('CertType') is not None:
+            self.cert_type = m.get('CertType')
+        if m.get('Config') is not None:
+            self.config = m.get('Config')
+        if m.get('Del') is not None:
+            self.del_ = m.get('Del')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('JobType') is not None:
+            self.job_type = m.get('JobType')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ProductName') is not None:
+            self.product_name = m.get('ProductName')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Rollback') is not None:
+            self.rollback = m.get('Rollback')
+        if m.get('ScheduleTime') is not None:
+            self.schedule_time = m.get('ScheduleTime')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class DescribeDeploymentJobResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDeploymentJobResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDeploymentJobResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeDeploymentJobResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDeploymentJobStatusRequest(TeaModel):
     def __init__(self, job_id=None):
         self.job_id = job_id  # type: long
 
     def validate(self):
         pass
 
@@ -3194,14 +3548,180 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListCertWarehouseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListCloudAccessRequest(TeaModel):
+    def __init__(self, cloud_name=None, current_page=None, secret_id=None, show_size=None):
+        self.cloud_name = cloud_name  # type: str
+        self.current_page = current_page  # type: int
+        self.secret_id = secret_id  # type: str
+        self.show_size = show_size  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListCloudAccessRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cloud_name is not None:
+            result['CloudName'] = self.cloud_name
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.secret_id is not None:
+            result['SecretId'] = self.secret_id
+        if self.show_size is not None:
+            result['ShowSize'] = self.show_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CloudName') is not None:
+            self.cloud_name = m.get('CloudName')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('SecretId') is not None:
+            self.secret_id = m.get('SecretId')
+        if m.get('ShowSize') is not None:
+            self.show_size = m.get('ShowSize')
+        return self
+
+
+class ListCloudAccessResponseBodyCloudAccessList(TeaModel):
+    def __init__(self, access_id=None, cloud_name=None, secret_id=None, service_status=None):
+        self.access_id = access_id  # type: long
+        self.cloud_name = cloud_name  # type: str
+        self.secret_id = secret_id  # type: str
+        self.service_status = service_status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListCloudAccessResponseBodyCloudAccessList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_id is not None:
+            result['AccessId'] = self.access_id
+        if self.cloud_name is not None:
+            result['CloudName'] = self.cloud_name
+        if self.secret_id is not None:
+            result['SecretId'] = self.secret_id
+        if self.service_status is not None:
+            result['ServiceStatus'] = self.service_status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AccessId') is not None:
+            self.access_id = m.get('AccessId')
+        if m.get('CloudName') is not None:
+            self.cloud_name = m.get('CloudName')
+        if m.get('SecretId') is not None:
+            self.secret_id = m.get('SecretId')
+        if m.get('ServiceStatus') is not None:
+            self.service_status = m.get('ServiceStatus')
+        return self
+
+
+class ListCloudAccessResponseBody(TeaModel):
+    def __init__(self, cloud_access_list=None, current_page=None, request_id=None, show_size=None, total_count=None):
+        self.cloud_access_list = cloud_access_list  # type: list[ListCloudAccessResponseBodyCloudAccessList]
+        self.current_page = current_page  # type: int
+        self.request_id = request_id  # type: str
+        self.show_size = show_size  # type: int
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.cloud_access_list:
+            for k in self.cloud_access_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListCloudAccessResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['CloudAccessList'] = []
+        if self.cloud_access_list is not None:
+            for k in self.cloud_access_list:
+                result['CloudAccessList'].append(k.to_map() if k else None)
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.show_size is not None:
+            result['ShowSize'] = self.show_size
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.cloud_access_list = []
+        if m.get('CloudAccessList') is not None:
+            for k in m.get('CloudAccessList'):
+                temp_model = ListCloudAccessResponseBodyCloudAccessList()
+                self.cloud_access_list.append(temp_model.from_map(k))
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ShowSize') is not None:
+            self.show_size = m.get('ShowSize')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListCloudAccessResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListCloudAccessResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListCloudAccessResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListCloudAccessResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListCloudResourcesRequest(TeaModel):
     def __init__(self, cloud_name=None, cloud_product=None, current_page=None, keyword=None, secret_id=None,
                  show_size=None):
         self.cloud_name = cloud_name  # type: str
         self.cloud_product = cloud_product  # type: str
         self.current_page = current_page  # type: int
         self.keyword = keyword  # type: str
@@ -3459,14 +3979,197 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListCloudResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListContactRequest(TeaModel):
+    def __init__(self, current_page=None, keyword=None, show_size=None):
+        self.current_page = current_page  # type: int
+        self.keyword = keyword  # type: str
+        self.show_size = show_size  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListContactRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.keyword is not None:
+            result['Keyword'] = self.keyword
+        if self.show_size is not None:
+            result['ShowSize'] = self.show_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('Keyword') is not None:
+            self.keyword = m.get('Keyword')
+        if m.get('ShowSize') is not None:
+            self.show_size = m.get('ShowSize')
+        return self
+
+
+class ListContactResponseBodyContactList(TeaModel):
+    def __init__(self, contact_id=None, email=None, email_status=None, mobile=None, mobile_status=None, name=None,
+                 webhooks=None):
+        self.contact_id = contact_id  # type: long
+        self.email = email  # type: str
+        self.email_status = email_status  # type: int
+        self.mobile = mobile  # type: str
+        self.mobile_status = mobile_status  # type: int
+        self.name = name  # type: str
+        self.webhooks = webhooks  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListContactResponseBodyContactList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.contact_id is not None:
+            result['ContactId'] = self.contact_id
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.email_status is not None:
+            result['EmailStatus'] = self.email_status
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.mobile_status is not None:
+            result['MobileStatus'] = self.mobile_status
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.webhooks is not None:
+            result['Webhooks'] = self.webhooks
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ContactId') is not None:
+            self.contact_id = m.get('ContactId')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('EmailStatus') is not None:
+            self.email_status = m.get('EmailStatus')
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('MobileStatus') is not None:
+            self.mobile_status = m.get('MobileStatus')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Webhooks') is not None:
+            self.webhooks = m.get('Webhooks')
+        return self
+
+
+class ListContactResponseBody(TeaModel):
+    def __init__(self, contact_list=None, current_page=None, keyword=None, request_id=None, show_size=None,
+                 total_count=None):
+        self.contact_list = contact_list  # type: list[ListContactResponseBodyContactList]
+        self.current_page = current_page  # type: int
+        self.keyword = keyword  # type: str
+        self.request_id = request_id  # type: str
+        self.show_size = show_size  # type: int
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.contact_list:
+            for k in self.contact_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListContactResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ContactList'] = []
+        if self.contact_list is not None:
+            for k in self.contact_list:
+                result['ContactList'].append(k.to_map() if k else None)
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.keyword is not None:
+            result['Keyword'] = self.keyword
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.show_size is not None:
+            result['ShowSize'] = self.show_size
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.contact_list = []
+        if m.get('ContactList') is not None:
+            for k in m.get('ContactList'):
+                temp_model = ListContactResponseBodyContactList()
+                self.contact_list.append(temp_model.from_map(k))
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('Keyword') is not None:
+            self.keyword = m.get('Keyword')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ShowSize') is not None:
+            self.show_size = m.get('ShowSize')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListContactResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListContactResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListContactResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListContactResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListCsrRequest(TeaModel):
     def __init__(self, algorithm=None, current_page=None, key_word=None, show_size=None):
         self.algorithm = algorithm  # type: str
         self.current_page = current_page  # type: long
         self.key_word = key_word  # type: str
         self.show_size = show_size  # type: long
 
@@ -4748,14 +5451,283 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListUserCertificateOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListWorkerResourceRequest(TeaModel):
+    def __init__(self, cloud_product=None, current_page=None, job_id=None, show_size=None, status=None):
+        self.cloud_product = cloud_product  # type: str
+        self.current_page = current_page  # type: int
+        self.job_id = job_id  # type: long
+        self.show_size = show_size  # type: int
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListWorkerResourceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cloud_product is not None:
+            result['CloudProduct'] = self.cloud_product
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.show_size is not None:
+            result['ShowSize'] = self.show_size
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CloudProduct') is not None:
+            self.cloud_product = m.get('CloudProduct')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('ShowSize') is not None:
+            self.show_size = m.get('ShowSize')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class ListWorkerResourceResponseBodyData(TeaModel):
+    def __init__(self, cert_domain=None, cert_id=None, cert_instance_id=None, cert_name=None, cloud_name=None,
+                 cloud_product=None, cloud_region=None, default_resource=None, gmt_create=None, gmt_modified=None, id=None,
+                 instance_id=None, job_id=None, listener_id=None, namespace_id=None, order_id=None, port=None, region_id=None,
+                 resource_cert_id=None, resource_domain=None, resource_id=None, status=None, user_id=None):
+        self.cert_domain = cert_domain  # type: str
+        self.cert_id = cert_id  # type: long
+        self.cert_instance_id = cert_instance_id  # type: str
+        self.cert_name = cert_name  # type: str
+        self.cloud_name = cloud_name  # type: str
+        self.cloud_product = cloud_product  # type: str
+        self.cloud_region = cloud_region  # type: str
+        self.default_resource = default_resource  # type: bool
+        self.gmt_create = gmt_create  # type: str
+        self.gmt_modified = gmt_modified  # type: str
+        self.id = id  # type: long
+        self.instance_id = instance_id  # type: str
+        self.job_id = job_id  # type: long
+        self.listener_id = listener_id  # type: str
+        self.namespace_id = namespace_id  # type: str
+        self.order_id = order_id  # type: long
+        self.port = port  # type: int
+        self.region_id = region_id  # type: str
+        self.resource_cert_id = resource_cert_id  # type: long
+        self.resource_domain = resource_domain  # type: str
+        self.resource_id = resource_id  # type: long
+        self.status = status  # type: str
+        self.user_id = user_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListWorkerResourceResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cert_domain is not None:
+            result['CertDomain'] = self.cert_domain
+        if self.cert_id is not None:
+            result['CertId'] = self.cert_id
+        if self.cert_instance_id is not None:
+            result['CertInstanceId'] = self.cert_instance_id
+        if self.cert_name is not None:
+            result['CertName'] = self.cert_name
+        if self.cloud_name is not None:
+            result['CloudName'] = self.cloud_name
+        if self.cloud_product is not None:
+            result['CloudProduct'] = self.cloud_product
+        if self.cloud_region is not None:
+            result['CloudRegion'] = self.cloud_region
+        if self.default_resource is not None:
+            result['DefaultResource'] = self.default_resource
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.listener_id is not None:
+            result['ListenerId'] = self.listener_id
+        if self.namespace_id is not None:
+            result['NamespaceId'] = self.namespace_id
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_cert_id is not None:
+            result['ResourceCertId'] = self.resource_cert_id
+        if self.resource_domain is not None:
+            result['ResourceDomain'] = self.resource_domain
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CertDomain') is not None:
+            self.cert_domain = m.get('CertDomain')
+        if m.get('CertId') is not None:
+            self.cert_id = m.get('CertId')
+        if m.get('CertInstanceId') is not None:
+            self.cert_instance_id = m.get('CertInstanceId')
+        if m.get('CertName') is not None:
+            self.cert_name = m.get('CertName')
+        if m.get('CloudName') is not None:
+            self.cloud_name = m.get('CloudName')
+        if m.get('CloudProduct') is not None:
+            self.cloud_product = m.get('CloudProduct')
+        if m.get('CloudRegion') is not None:
+            self.cloud_region = m.get('CloudRegion')
+        if m.get('DefaultResource') is not None:
+            self.default_resource = m.get('DefaultResource')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('ListenerId') is not None:
+            self.listener_id = m.get('ListenerId')
+        if m.get('NamespaceId') is not None:
+            self.namespace_id = m.get('NamespaceId')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceCertId') is not None:
+            self.resource_cert_id = m.get('ResourceCertId')
+        if m.get('ResourceDomain') is not None:
+            self.resource_domain = m.get('ResourceDomain')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class ListWorkerResourceResponseBody(TeaModel):
+    def __init__(self, current_page=None, data=None, request_id=None, show_size=None, total=None):
+        self.current_page = current_page  # type: int
+        self.data = data  # type: list[ListWorkerResourceResponseBodyData]
+        self.request_id = request_id  # type: str
+        self.show_size = show_size  # type: int
+        self.total = total  # type: long
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListWorkerResourceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.show_size is not None:
+            result['ShowSize'] = self.show_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListWorkerResourceResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ShowSize') is not None:
+            self.show_size = m.get('ShowSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListWorkerResourceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListWorkerResourceResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListWorkerResourceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListWorkerResourceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RenewCertificateOrderForPackageRequestRequest(TeaModel):
     def __init__(self, csr=None, order_id=None):
         # The content of the certificate signing request (CSR) file that is manually generated for the domain name by using OpenSSL or Keytool. The key algorithm in the CSR file must be Rivest-Shamir-Adleman (RSA) or elliptic-curve cryptography (ECC), and the key length of the RSA algorithm must be greater than or equal to 2,048 characters. For more information about how to create a CSR file, see [How do I create a CSR file?](~~42218~~)
         # 
         # If you do not specify this parameter, Certificate Management Service automatically generates a CSR file for the domain name in the certificate application order that you want to renew.
         # 
         # A CSR file contains the information about your server and company. When you apply for a certificate, you must submit the CSR file to the CA. The CA signs the CSR file by using the private key of the root certificate and generates a public key file to issue your certificate.
```

### Comparing `alibabacloud_cas20200407_py2-1.2.0/alibabacloud_cas20200407_py2.egg-info/PKG-INFO` & `alibabacloud_cas20200407_py2-1.3.0/alibabacloud_cas20200407_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cas20200407-py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud SSL Certificates Service (20200407) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cas20200407_py2-1.2.0/setup.py` & `alibabacloud_cas20200407_py2-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cas20200407_py2.
 
-Created on 13/03/2024
+Created on 06/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cas20200407"
 NAME = "alibabacloud_cas20200407_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud SSL Certificates Service (20200407) SDK Library for Python2"
```

