# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419-2.0.2.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-2.0.2.tar", last modified: Thu Mar 14 17:17:53 2024, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-2.0.3.tar", last modified: Mon May  6 17:08:37 2024, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2.tar` & `alibabacloud_resourcedirectorymaster20220419-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/
--rw-r--r--   0 root         (0) root         (0)      737 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2541 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1175 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1260 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   270913 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   411952 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2541 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2711 2024-03-14 17:17:53.000000 alibabacloud_resourcedirectorymaster20220419-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   270954 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   414060 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-05-06 17:08:37.000000 alibabacloud_resourcedirectorymaster20220419-2.0.3/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/LICENSE` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcedirectorymaster20220419
-Version: 2.0.2
+Version: 2.0.3
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/README.md` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419/client.py` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     *\
     """
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         self.check_config(config)
         self._endpoint = self.get_endpoint('resourcedirectorymaster', self._region_id, self._endpoint_rule, self._network, self._suffix, self._endpoint_map, self._endpoint)
 
     def get_endpoint(
         self,
         product_id: str,
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419/models.py` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1913,14 +1913,18 @@
         # 
         # The name must be 2 to 50 characters in length.
         # 
         # The name can contain letters, digits, underscores (\_), periods (.), hyphens (-), and spaces.
         # 
         # The name must be unique in the resource directory.
         self.display_name = display_name
+        # Specifies whether to perform only a dry run, without performing the actual request. Valid values:
+        # 
+        # *   true: performs only a dry run. The system checks whether an identity type can be specified for the member. If the request does not pass the dry run, an error code is returned.
+        # *   false (default): performs a dry run and performs the actual request.
         self.dry_run = dry_run
         # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
         # The ID of the billing account. If you leave this parameter empty, the member is used as its own billing account.
         self.payer_account_id = payer_account_id
         # The identity type of the member. Valid values:
         # 
@@ -3724,14 +3728,15 @@
     def __init__(
         self,
         account_id: str = None,
         account_name: str = None,
         display_name: str = None,
         email_status: str = None,
         folder_id: str = None,
+        has_secure_mobile_phone: bool = None,
         identity_information: str = None,
         join_method: str = None,
         join_time: str = None,
         location: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         resource_directory_path: str = None,
@@ -3750,14 +3755,15 @@
         # *   If the value of this parameter is empty, no modification is performed for the email address.
         # *   WAIT_MODIFY: The modification is being performed.
         # *   CANCELLED: The modification is canceled.
         # *   EXPIRED: The modification expires.
         self.email_status = email_status
         # The ID of the folder.
         self.folder_id = folder_id
+        self.has_secure_mobile_phone = has_secure_mobile_phone
         # The real-name verification information.
         self.identity_information = identity_information
         # The way in which the member joins the resource directory. Valid values:
         # 
         # *   invited: The member is invited to join the resource directory.
         # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
@@ -3807,14 +3813,16 @@
             result['AccountName'] = self.account_name
         if self.display_name is not None:
             result['DisplayName'] = self.display_name
         if self.email_status is not None:
             result['EmailStatus'] = self.email_status
         if self.folder_id is not None:
             result['FolderId'] = self.folder_id
+        if self.has_secure_mobile_phone is not None:
+            result['HasSecureMobilePhone'] = self.has_secure_mobile_phone
         if self.identity_information is not None:
             result['IdentityInformation'] = self.identity_information
         if self.join_method is not None:
             result['JoinMethod'] = self.join_method
         if self.join_time is not None:
             result['JoinTime'] = self.join_time
         if self.location is not None:
@@ -3843,14 +3851,16 @@
             self.account_name = m.get('AccountName')
         if m.get('DisplayName') is not None:
             self.display_name = m.get('DisplayName')
         if m.get('EmailStatus') is not None:
             self.email_status = m.get('EmailStatus')
         if m.get('FolderId') is not None:
             self.folder_id = m.get('FolderId')
+        if m.get('HasSecureMobilePhone') is not None:
+            self.has_secure_mobile_phone = m.get('HasSecureMobilePhone')
         if m.get('IdentityInformation') is not None:
             self.identity_information = m.get('IdentityInformation')
         if m.get('JoinMethod') is not None:
             self.join_method = m.get('JoinMethod')
         if m.get('JoinTime') is not None:
             self.join_time = m.get('JoinTime')
         if m.get('Location') is not None:
@@ -6094,17 +6104,18 @@
         self,
         include_tags: bool = None,
         page_number: int = None,
         page_size: int = None,
         query_keyword: str = None,
         tag: List[ListAccountsRequestTag] = None,
     ):
-        # Specifies whether to return the information of tags. Valid values:
+        # Specifies whether to return information about tags. Valid values:
         # 
-        # false (default value) true
+        # *   false (default value)
+        # *   true
         self.include_tags = include_tags
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
@@ -6163,17 +6174,17 @@
 
 class ListAccountsResponseBodyAccountsAccountTagsTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The tag key.
+        # The key of the tag.
         self.key = key
-        # The tag value.
+        # The value of the tag.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6248,14 +6259,22 @@
         tags: ListAccountsResponseBodyAccountsAccountTags = None,
         type: str = None,
     ):
         # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
         # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The deletion status of the member. Valid values:
+        # 
+        # *   Checking: A deletion check is being performed for the member.
+        # *   Deleting: The member is being deleted.
+        # *   CheckFailed: The deletion check for the member fails.
+        # *   DeleteFailed: The member fails to be deleted.
+        # 
+        # >  If deletion is not performed for the member, the value of this parameter is empty.
         self.deletion_status = deletion_status
         # The display name of the member.
         self.display_name = display_name
         # The ID of the folder.
         self.folder_id = folder_id
         # The way in which the member joins the resource directory. Valid values:
         # 
@@ -6264,20 +6283,20 @@
         self.join_method = join_method
         # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
         # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
         # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
-        # The path of the member in the resource directory.
+        # The RDPath of the member.
         self.resource_directory_path = resource_directory_path
         # The status of the member. Valid values:
         # 
         # *   CreateSuccess: The member is created.
-        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteVerifying: The upgrade of the member is under confirmation.
         # *   PromoteFailed: The upgrade of the member fails.
         # *   PromoteExpired: The upgrade of the member expires.
         # *   PromoteCancelled: The upgrade of the member is canceled.
         # *   PromoteSuccess: The member is upgraded.
         # *   InviteSuccess: The member accepts the invitation.
         self.status = status
         # The tags that are added to the member.
@@ -6398,15 +6417,15 @@
         self,
         accounts: ListAccountsResponseBodyAccounts = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The members returned.
+        # The information about the members.
         self.accounts = accounts
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
@@ -6533,17 +6552,18 @@
         include_tags: bool = None,
         page_number: int = None,
         page_size: int = None,
         parent_folder_id: str = None,
         query_keyword: str = None,
         tag: List[ListAccountsForParentRequestTag] = None,
     ):
-        # Specifies whether to return the information of tags. Valid values:
+        # Specifies whether to return information about tags. Valid values:
         # 
-        # false (default value) true
+        # *   false (default value)
+        # *   true
         self.include_tags = include_tags
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
@@ -6692,34 +6712,42 @@
         tags: ListAccountsForParentResponseBodyAccountsAccountTags = None,
         type: str = None,
     ):
         # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
         # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The deletion status of the member. Valid values:
+        # 
+        # *   Checking: A deletion check is being performed for the member.
+        # *   Deleting: The member is being deleted.
+        # *   CheckFailed: The deletion check for the member fails.
+        # *   DeleteFailed: The member fails to be deleted.
+        # 
+        # >  If deletion is not performed for the member, the value of this parameter is empty.
         self.deletion_status = deletion_status
         # The display name of the member.
         self.display_name = display_name
         # The ID of the folder.
         self.folder_id = folder_id
-        # The way in which the member joins the resource directory. Valid values:
+        # The way in which the member joins the resource directory.
         # 
         # *   invited: The member is invited to join the resource directory.
         # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
         # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
         # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
         # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
         # The status of the member. Valid values:
         # 
         # *   CreateSuccess: The member is created.
-        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteVerifying: The upgrade of the member is under confirmation.
         # *   PromoteFailed: The upgrade of the member fails.
         # *   PromoteExpired: The upgrade of the member expires.
         # *   PromoteCancelled: The upgrade of the member is canceled.
         # *   PromoteSuccess: The member is upgraded.
         # *   InviteSuccess: The member accepts the invitation.
         self.status = status
         # The tags that are added to the member.
@@ -6836,15 +6864,15 @@
         self,
         accounts: ListAccountsForParentResponseBodyAccounts = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The information of the members.
+        # The information about the members.
         self.accounts = accounts
         # The page number of the returned page.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
@@ -11755,14 +11783,18 @@
         account_id: str = None,
         dry_run: bool = None,
         new_account_type: str = None,
         new_display_name: str = None,
     ):
         # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # Specifies whether to perform only a dry run, without performing the actual request. Valid values:
+        # 
+        # *   true: performs only a dry run. The system checks items such as whether the member status can be modified and whether security information is configured for the member. If the request does not pass the dry run, an error code is returned.
+        # *   false (default): performs a dry run and performs the actual request.
         self.dry_run = dry_run
         # The new type of the member. Valid values:
         # 
         # *   ResourceAccount: resource account
         # *   CloudAccount: cloud account
         # 
         # > You can specify either `NewDisplayName` or `NewAccountType`.
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcedirectorymaster20220419
-Version: 2.0.2
+Version: 2.0.3
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-2.0.2/setup.py` & `alibabacloud_resourcedirectorymaster20220419-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419.
 
-Created on 14/03/2024
+Created on 06/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python"
```

