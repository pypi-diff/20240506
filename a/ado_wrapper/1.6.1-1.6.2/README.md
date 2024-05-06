# Comparing `tmp/ado_wrapper-1.6.1.tar.gz` & `tmp/ado_wrapper-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.6.1.tar", max compression
+gzip compressed data, was "ado_wrapper-1.6.2.tar", max compression
```

## Comparing `ado_wrapper-1.6.1.tar` & `ado_wrapper-1.6.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.6.1/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.6.1/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.6.1/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.6.1/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.6.1/ado_wrapper/client.py
--rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.6.1/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3427 2024-05-04 17:24:03.055237 ado_wrapper-1.6.1/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.6.1/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.6.1/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.6.1/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.6.1/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3704 2024-05-04 17:23:41.003500 ado_wrapper-1.6.1/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.6.1/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.6.1/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14870 2024-05-03 16:42:18.453223 ado_wrapper-1.6.1/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.6.1/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.6.1/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.6.1/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15327 2024-05-03 16:42:42.079759 ado_wrapper-1.6.1/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.6.1/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-03 16:42:47.416430 ado_wrapper-1.6.1/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.6.1/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10450 2024-05-05 11:05:13.008884 ado_wrapper-1.6.1/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0    10496 2024-05-05 13:08:03.080705 ado_wrapper-1.6.1/ado_wrapper/resources/repo_user_permission.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.6.1/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.6.1/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.6.1/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8314 2024-05-04 20:57:42.347047 ado_wrapper-1.6.1/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.6.1/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9437 2024-05-03 16:43:45.994580 ado_wrapper-1.6.1/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.6.1/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.6.1/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-05 13:08:28.204945 ado_wrapper-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.6.2/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.6.2/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.6.2/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.6.2/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.6.2/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.6.2/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3427 2024-05-04 17:24:03.055237 ado_wrapper-1.6.2/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.6.2/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.6.2/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.6.2/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.6.2/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.6.2/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.6.2/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.6.2/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3704 2024-05-04 17:23:41.003500 ado_wrapper-1.6.2/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.6.2/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.6.2/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14870 2024-05-03 16:42:18.453223 ado_wrapper-1.6.2/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.6.2/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.6.2/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.6.2/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15327 2024-05-03 16:42:42.079759 ado_wrapper-1.6.2/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.6.2/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-03 16:42:47.416430 ado_wrapper-1.6.2/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.6.2/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10450 2024-05-05 11:05:13.008884 ado_wrapper-1.6.2/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    10544 2024-05-05 13:11:57.297558 ado_wrapper-1.6.2/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.6.2/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.6.2/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.6.2/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8314 2024-05-04 20:57:42.347047 ado_wrapper-1.6.2/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.6.2/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9437 2024-05-03 16:43:45.994580 ado_wrapper-1.6.2/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.6.2/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.6.2/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-05 13:13:41.180639 ado_wrapper-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.6.2/PKG-INFO
```

### Comparing `ado_wrapper-1.6.1/LICENSE` & `ado_wrapper-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/README.md` & `ado_wrapper-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/__main__.py` & `ado_wrapper-1.6.2/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/client.py` & `ado_wrapper-1.6.2/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/dumps.py` & `ado_wrapper-1.6.2/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/generate_docs.py` & `ado_wrapper-1.6.2/ado_wrapper/generate_docs.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.6.2/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.6.2/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.6.2/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/agent_pools.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/branches.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/builds.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/commits.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/environment.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/groups.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/projects.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/releases.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/repo.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/repo_user_permission.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/repo_user_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,24 +53,25 @@
     "rename_repository": 1024,
 }
 
 @dataclass
 class UserPermission:
     namespace_id: str = field(repr=False)
     display_name: str
+    programmatic_name: str
     token: str = field(repr=False)
     bit: int = field(repr=False)
     can_edit: bool = field(repr=False)
     permission_display_string: str
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> UserPermission:
         return cls(
-            data["namespaceId"], external_to_internal_mapping.get(data["displayName"], data["displayName"]), data["token"], data["bit"],
-            data.get("canEdit", False), data["permissionDisplayString"]  # fmt: skip
+            data["namespaceId"], data["displayName"], external_to_internal_mapping.get(data["displayName"], data["displayName"]),
+            data["token"], data["bit"], data.get("canEdit", False), data["permissionDisplayString"]  # fmt: skip
         )
 
     @classmethod
     def get_by_subject_descriptor(cls, ado_client: AdoClient, subject_descriptor: str, repo_id: str) -> list[UserPermission]:
         requires_initialisation(ado_client)
         PAYLOAD = {"contributionIds": ["ms.vss-admin-web.security-view-permissions-data-provider"], "dataProviderContext": {"properties": {
             "subjectDescriptor": subject_descriptor,
```

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/searches.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/teams.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/users.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.6.2/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.6.2/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/state_manager.py` & `ado_wrapper-1.6.2/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/ado_wrapper/utils.py` & `ado_wrapper-1.6.2/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.6.1/pyproject.toml` & `ado_wrapper-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.6.1"
+version = "1.6.2"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.6.1/PKG-INFO` & `ado_wrapper-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.6.1
+Version: 1.6.2
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

