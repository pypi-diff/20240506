# Comparing `tmp/alibabacloud_cas20200407-1.2.0.tar.gz` & `tmp/alibabacloud_cas20200407-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cas20200407-1.2.0.tar", last modified: Wed Mar 13 17:19:06 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cas20200407-1.3.0.tar", last modified: Mon May  6 06:19:51 2024, max compression
```

## Comparing `alibabacloud_cas20200407-1.2.0.tar` & `alibabacloud_cas20200407-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1166 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2422 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183619 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407/client.py
--rw-r--r--   0 root         (0) root         (0)   231757 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2422 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2632 2024-03-13 17:19:06.000000 alibabacloud_cas20200407-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198437 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407/client.py
+-rw-r--r--   0 root         (0) root         (0)   267874 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-05-06 06:19:51.000000 alibabacloud_cas20200407-1.3.0/setup.py
```

### Comparing `alibabacloud_cas20200407-1.2.0/ChangeLog.md` & `alibabacloud_cas20200407-1.3.0/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+2024-03-13 Version: 1.2.0
+- Support API CreateCsr.
+- Support API CreateDeploymentJob.
+- Support API DeleteCsr.
+- Support API DeleteDeploymentJob.
+- Support API DeleteWorkerResource.
+- Support API DescribeDeploymentJobStatus.
+- Support API GetCsrDetail.
+- Support API ListCloudResources.
+- Support API ListCsr.
+- Support API ListDeploymentJob.
+- Support API ListDeploymentJobCert.
+- Support API ListDeploymentJobResource.
+- Support API UpdateCsr.
+- Support API UpdateDeploymentJob.
+- Support API UpdateDeploymentJobStatus.
+- Support API UpdateWorkerResourceStatus.
+- Support API UploadCsr.
+
+
 2024-02-27 Version: 1.1.0
 - Support API CreateCsr.
 - Support API DeleteCsr.
 - Support API GetCsrDetail.
 - Support API ListCsr.
 - Support API UpdateCsr.
 - Support API UploadCsr.
```

### Comparing `alibabacloud_cas20200407-1.2.0/LICENSE` & `alibabacloud_cas20200407-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cas20200407-1.2.0/PKG-INFO` & `alibabacloud_cas20200407-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cas20200407
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud SSL Certificates Service (20200407) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cas20200407-1.2.0/README-CN.md` & `alibabacloud_cas20200407-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cas20200407-1.2.0/README.md` & `alibabacloud_cas20200407-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407/client.py` & `alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1678,14 +1678,154 @@
         
         @param request: DescribeCertificateStateRequest
         @return: DescribeCertificateStateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_certificate_state_with_options_async(request, runtime)
 
+    def describe_cloud_resource_status_with_options(
+        self,
+        request: cas_20200407_models.DescribeCloudResourceStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.DescribeCloudResourceStatusResponse:
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
+    async def describe_cloud_resource_status_with_options_async(
+        self,
+        request: cas_20200407_models.DescribeCloudResourceStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.DescribeCloudResourceStatusResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_cloud_resource_status(
+        self,
+        request: cas_20200407_models.DescribeCloudResourceStatusRequest,
+    ) -> cas_20200407_models.DescribeCloudResourceStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cloud_resource_status_with_options(request, runtime)
+
+    async def describe_cloud_resource_status_async(
+        self,
+        request: cas_20200407_models.DescribeCloudResourceStatusRequest,
+    ) -> cas_20200407_models.DescribeCloudResourceStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_cloud_resource_status_with_options_async(request, runtime)
+
+    def describe_deployment_job_with_options(
+        self,
+        request: cas_20200407_models.DescribeDeploymentJobRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.DescribeDeploymentJobResponse:
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
+    async def describe_deployment_job_with_options_async(
+        self,
+        request: cas_20200407_models.DescribeDeploymentJobRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.DescribeDeploymentJobResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_deployment_job(
+        self,
+        request: cas_20200407_models.DescribeDeploymentJobRequest,
+    ) -> cas_20200407_models.DescribeDeploymentJobResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_deployment_job_with_options(request, runtime)
+
+    async def describe_deployment_job_async(
+        self,
+        request: cas_20200407_models.DescribeDeploymentJobRequest,
+    ) -> cas_20200407_models.DescribeDeploymentJobResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_deployment_job_with_options_async(request, runtime)
+
     def describe_deployment_job_status_with_options(
         self,
         request: cas_20200407_models.DescribeDeploymentJobStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cas_20200407_models.DescribeDeploymentJobStatusResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2326,14 +2466,96 @@
     async def list_cert_warehouse_async(
         self,
         request: cas_20200407_models.ListCertWarehouseRequest,
     ) -> cas_20200407_models.ListCertWarehouseResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_cert_warehouse_with_options_async(request, runtime)
 
+    def list_cloud_access_with_options(
+        self,
+        request: cas_20200407_models.ListCloudAccessRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.ListCloudAccessResponse:
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
+    async def list_cloud_access_with_options_async(
+        self,
+        request: cas_20200407_models.ListCloudAccessRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.ListCloudAccessResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_cloud_access(
+        self,
+        request: cas_20200407_models.ListCloudAccessRequest,
+    ) -> cas_20200407_models.ListCloudAccessResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_cloud_access_with_options(request, runtime)
+
+    async def list_cloud_access_async(
+        self,
+        request: cas_20200407_models.ListCloudAccessRequest,
+    ) -> cas_20200407_models.ListCloudAccessResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_cloud_access_with_options_async(request, runtime)
+
     def list_cloud_resources_with_options(
         self,
         request: cas_20200407_models.ListCloudResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cas_20200407_models.ListCloudResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2416,14 +2638,92 @@
     async def list_cloud_resources_async(
         self,
         request: cas_20200407_models.ListCloudResourcesRequest,
     ) -> cas_20200407_models.ListCloudResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_cloud_resources_with_options_async(request, runtime)
 
+    def list_contact_with_options(
+        self,
+        request: cas_20200407_models.ListContactRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.ListContactResponse:
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
+    async def list_contact_with_options_async(
+        self,
+        request: cas_20200407_models.ListContactRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.ListContactResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_contact(
+        self,
+        request: cas_20200407_models.ListContactRequest,
+    ) -> cas_20200407_models.ListContactResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_contact_with_options(request, runtime)
+
+    async def list_contact_async(
+        self,
+        request: cas_20200407_models.ListContactRequest,
+    ) -> cas_20200407_models.ListContactResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_contact_with_options_async(request, runtime)
+
     def list_csr_with_options(
         self,
         request: cas_20200407_models.ListCsrRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cas_20200407_models.ListCsrResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2844,14 +3144,100 @@
         
         @param request: ListUserCertificateOrderRequest
         @return: ListUserCertificateOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_certificate_order_with_options_async(request, runtime)
 
+    def list_worker_resource_with_options(
+        self,
+        request: cas_20200407_models.ListWorkerResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.ListWorkerResourceResponse:
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
+    async def list_worker_resource_with_options_async(
+        self,
+        request: cas_20200407_models.ListWorkerResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cas_20200407_models.ListWorkerResourceResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_worker_resource(
+        self,
+        request: cas_20200407_models.ListWorkerResourceRequest,
+    ) -> cas_20200407_models.ListWorkerResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_worker_resource_with_options(request, runtime)
+
+    async def list_worker_resource_async(
+        self,
+        request: cas_20200407_models.ListWorkerResourceRequest,
+    ) -> cas_20200407_models.ListWorkerResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_worker_resource_with_options_async(request, runtime)
+
     def renew_certificate_order_for_package_request_with_options(
         self,
         request: cas_20200407_models.RenewCertificateOrderForPackageRequestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cas_20200407_models.RenewCertificateOrderForPackageRequestResponse:
         """
         You can call this operation to submit a renewal application for a certificate only when the order of the certificate is in the expiring state. After the renewal is complete, a new certificate order whose status is pending application is generated. You must submit a certificate application for the new certificate order and install the new certificate after the new certificate is issued.
```

### Comparing `alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407/models.py` & `alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2137,14 +2137,418 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCertificateStateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCloudResourceStatusRequest(TeaModel):
+    def __init__(
+        self,
+        secret_id: str = None,
+    ):
+        self.secret_id = secret_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.secret_id is not None:
+            result['SecretId'] = self.secret_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SecretId') is not None:
+            self.secret_id = m.get('SecretId')
+        return self
+
+
+class DescribeCloudResourceStatusResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        cloud_name: str = None,
+        cloud_product: str = None,
+        total_count: int = None,
+    ):
+        self.cloud_name = cloud_name
+        self.cloud_product = cloud_product
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: List[DescribeCloudResourceStatusResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeCloudResourceStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        job_id: int = None,
+    ):
+        self.job_id = job_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        return self
+
+
+class DescribeDeploymentJobResponseBodyCasContacts(TeaModel):
+    def __init__(
+        self,
+        email: str = None,
+        id: str = None,
+        mobile: str = None,
+        name: str = None,
+    ):
+        self.email = email
+        self.id = id
+        self.mobile = mobile
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cas_contacts: List[DescribeDeploymentJobResponseBodyCasContacts] = None,
+        cert_domain: str = None,
+        cert_type: str = None,
+        config: str = None,
+        del_: int = None,
+        end_time: str = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        id: int = None,
+        instance_id: str = None,
+        job_type: str = None,
+        name: str = None,
+        product_name: str = None,
+        request_id: str = None,
+        rollback: int = None,
+        schedule_time: str = None,
+        start_time: str = None,
+        status: str = None,
+        user_id: int = None,
+    ):
+        self.cas_contacts = cas_contacts
+        self.cert_domain = cert_domain
+        self.cert_type = cert_type
+        self.config = config
+        self.del_ = del_
+        self.end_time = end_time
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.id = id
+        self.instance_id = instance_id
+        self.job_type = job_type
+        self.name = name
+        self.product_name = product_name
+        self.request_id = request_id
+        self.rollback = rollback
+        self.schedule_time = schedule_time
+        self.start_time = start_time
+        self.status = status
+        self.user_id = user_id
+
+    def validate(self):
+        if self.cas_contacts:
+            for k in self.cas_contacts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDeploymentJobResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         job_id: int = None,
     ):
         self.job_id = job_id
 
@@ -3609,14 +4013,204 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListCertWarehouseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListCloudAccessRequest(TeaModel):
+    def __init__(
+        self,
+        cloud_name: str = None,
+        current_page: int = None,
+        secret_id: str = None,
+        show_size: int = None,
+    ):
+        self.cloud_name = cloud_name
+        self.current_page = current_page
+        self.secret_id = secret_id
+        self.show_size = show_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        access_id: int = None,
+        cloud_name: str = None,
+        secret_id: str = None,
+        service_status: str = None,
+    ):
+        self.access_id = access_id
+        self.cloud_name = cloud_name
+        self.secret_id = secret_id
+        self.service_status = service_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cloud_access_list: List[ListCloudAccessResponseBodyCloudAccessList] = None,
+        current_page: int = None,
+        request_id: str = None,
+        show_size: int = None,
+        total_count: int = None,
+    ):
+        self.cloud_access_list = cloud_access_list
+        self.current_page = current_page
+        self.request_id = request_id
+        self.show_size = show_size
+        self.total_count = total_count
+
+    def validate(self):
+        if self.cloud_access_list:
+            for k in self.cloud_access_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListCloudAccessResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         cloud_name: str = None,
         cloud_product: str = None,
         current_page: int = None,
         keyword: str = None,
@@ -3913,14 +4507,222 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListCloudResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListContactRequest(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        keyword: str = None,
+        show_size: int = None,
+    ):
+        self.current_page = current_page
+        self.keyword = keyword
+        self.show_size = show_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        contact_id: int = None,
+        email: str = None,
+        email_status: int = None,
+        mobile: str = None,
+        mobile_status: int = None,
+        name: str = None,
+        webhooks: str = None,
+    ):
+        self.contact_id = contact_id
+        self.email = email
+        self.email_status = email_status
+        self.mobile = mobile
+        self.mobile_status = mobile_status
+        self.name = name
+        self.webhooks = webhooks
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        contact_list: List[ListContactResponseBodyContactList] = None,
+        current_page: int = None,
+        keyword: str = None,
+        request_id: str = None,
+        show_size: int = None,
+        total_count: int = None,
+    ):
+        self.contact_list = contact_list
+        self.current_page = current_page
+        self.keyword = keyword
+        self.request_id = request_id
+        self.show_size = show_size
+        self.total_count = total_count
+
+    def validate(self):
+        if self.contact_list:
+            for k in self.contact_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListContactResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         algorithm: str = None,
         current_page: int = None,
         key_word: str = None,
         show_size: int = None,
@@ -5377,14 +6179,324 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListUserCertificateOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListWorkerResourceRequest(TeaModel):
+    def __init__(
+        self,
+        cloud_product: str = None,
+        current_page: int = None,
+        job_id: int = None,
+        show_size: int = None,
+        status: str = None,
+    ):
+        self.cloud_product = cloud_product
+        self.current_page = current_page
+        self.job_id = job_id
+        self.show_size = show_size
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cert_domain: str = None,
+        cert_id: int = None,
+        cert_instance_id: str = None,
+        cert_name: str = None,
+        cloud_name: str = None,
+        cloud_product: str = None,
+        cloud_region: str = None,
+        default_resource: bool = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        id: int = None,
+        instance_id: str = None,
+        job_id: int = None,
+        listener_id: str = None,
+        namespace_id: str = None,
+        order_id: int = None,
+        port: int = None,
+        region_id: str = None,
+        resource_cert_id: int = None,
+        resource_domain: str = None,
+        resource_id: int = None,
+        status: str = None,
+        user_id: int = None,
+    ):
+        self.cert_domain = cert_domain
+        self.cert_id = cert_id
+        self.cert_instance_id = cert_instance_id
+        self.cert_name = cert_name
+        self.cloud_name = cloud_name
+        self.cloud_product = cloud_product
+        self.cloud_region = cloud_region
+        self.default_resource = default_resource
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.id = id
+        self.instance_id = instance_id
+        self.job_id = job_id
+        self.listener_id = listener_id
+        self.namespace_id = namespace_id
+        self.order_id = order_id
+        self.port = port
+        self.region_id = region_id
+        self.resource_cert_id = resource_cert_id
+        self.resource_domain = resource_domain
+        self.resource_id = resource_id
+        self.status = status
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        current_page: int = None,
+        data: List[ListWorkerResourceResponseBodyData] = None,
+        request_id: str = None,
+        show_size: int = None,
+        total: int = None,
+    ):
+        self.current_page = current_page
+        self.data = data
+        self.request_id = request_id
+        self.show_size = show_size
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListWorkerResourceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         csr: str = None,
         order_id: int = None,
     ):
         # The content of the certificate signing request (CSR) file that is manually generated for the domain name by using OpenSSL or Keytool. The key algorithm in the CSR file must be Rivest-Shamir-Adleman (RSA) or elliptic-curve cryptography (ECC), and the key length of the RSA algorithm must be greater than or equal to 2,048 characters. For more information about how to create a CSR file, see [How do I create a CSR file?](~~42218~~)
```

### Comparing `alibabacloud_cas20200407-1.2.0/alibabacloud_cas20200407.egg-info/PKG-INFO` & `alibabacloud_cas20200407-1.3.0/alibabacloud_cas20200407.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cas20200407
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud SSL Certificates Service (20200407) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cas20200407-1.2.0/setup.py` & `alibabacloud_cas20200407-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cas20200407.
 
-Created on 13/03/2024
+Created on 06/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cas20200407"
 NAME = "alibabacloud_cas20200407" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud SSL Certificates Service (20200407) SDK Library for Python"
```

