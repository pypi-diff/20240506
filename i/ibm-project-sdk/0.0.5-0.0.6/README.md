# Comparing `tmp/ibm-project-sdk-0.0.5.tar.gz` & `tmp/ibm-project-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-project-sdk-0.0.5.tar", last modified: Wed Apr  3 08:19:27 2024, max compression
+gzip compressed data, was "ibm-project-sdk-0.0.6.tar", last modified: Mon May  6 18:33:09 2024, max compression
```

## Comparing `ibm-project-sdk-0.0.5.tar` & `ibm-project-sdk-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4009 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/ibm_project_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)      895 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   495442 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/project_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4009 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      430 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 08:17:44.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      129 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-06 18:33:09.656918 ibm-project-sdk-0.0.6/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4009 2024-05-06 18:33:09.656918 ibm-project-sdk-0.0.6/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-06 18:33:09.656918 ibm-project-sdk-0.0.6/ibm_project_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      895 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/ibm_project_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/ibm_project_sdk/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   521085 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/ibm_project_sdk/project_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/ibm_project_sdk/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-06 18:33:09.656918 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4009 2024-05-06 18:33:09.000000 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      430 2024-05-06 18:33:09.000000 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-06 18:33:09.000000 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-05-06 18:33:09.000000 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2024-05-06 18:33:09.000000 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-06 18:31:14.000000 ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-06 18:33:09.656918 ibm-project-sdk-0.0.6/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-05-06 18:30:44.000000 ibm-project-sdk-0.0.6/setup.py
```

### Comparing `ibm-project-sdk-0.0.5/LICENSE` & `ibm-project-sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-project-sdk-0.0.5/PKG-INFO` & `ibm-project-sdk-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-project-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Project Services Python SDK
 Home-page: https://github.com/IBM/project-python-sdk
 Author: IBM
 Author-email: dvesperini@gmail.com
 License: Apache 2.0
 Keywords: ibm_project_sdk
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://api.travis-ci.com/IBM/project-python-sdk.svg?branch=main)](https://app.travis-ci.com/github/IBM/project-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# Project Services Python SDK Version 0.0.5
+# Project Services Python SDK Version 0.0.6
 
 Python client library to interact with various [IBM Cloud Platform Services APIs](https://cloud.ibm.com/apidocs?category=platform-services).
 
 Disclaimer: this SDK is being released initially as a **pre-release** version.
 Changes might occur which impact applications that use this SDK.
 
 ## Table of Contents
@@ -76,15 +76,15 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip`:
 
 ```bash
-pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.5
+pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.6
 ```
 
 Then in your code, you can import the appropriate service like this:
 ```
 from ibm_project_sdk.project_v1 import *
 ```
 where `<service-module-name>` is the service's module name from the table above
```

### Comparing `ibm-project-sdk-0.0.5/README.md` & `ibm-project-sdk-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Build Status](https://api.travis-ci.com/IBM/project-python-sdk.svg?branch=main)](https://app.travis-ci.com/github/IBM/project-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# Project Services Python SDK Version 0.0.5
+# Project Services Python SDK Version 0.0.6
 
 Python client library to interact with various [IBM Cloud Platform Services APIs](https://cloud.ibm.com/apidocs?category=platform-services).
 
 Disclaimer: this SDK is being released initially as a **pre-release** version.
 Changes might occur which impact applications that use this SDK.
 
 ## Table of Contents
@@ -51,15 +51,15 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip`:
 
 ```bash
-pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.5
+pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.6
 ```
 
 Then in your code, you can import the appropriate service like this:
 ```
 from ibm_project_sdk.project_v1 import *
 ```
 where `<service-module-name>` is the service's module name from the table above
```

### Comparing `ibm-project-sdk-0.0.5/ibm_project_sdk/__init__.py` & `ibm-project-sdk-0.0.6/ibm_project_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-project-sdk-0.0.5/ibm_project_sdk/common.py` & `ibm-project-sdk-0.0.6/ibm_project_sdk/common.py`

 * *Files identical despite different names*

### Comparing `ibm-project-sdk-0.0.5/ibm_project_sdk/project_v1.py` & `ibm-project-sdk-0.0.6/ibm_project_sdk/project_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -4061,14 +4061,108 @@
         The result of the last action.
         """
 
         FAILED = 'failed'
         PASSED = 'passed'
 
 
+class MemberOfDefinition:
+    """
+    The stack config parent of which this configuration is a member of.
+
+    :param str id: The unique ID.
+    :param StackConfigDefinitionSummary definition: The definition summary of the
+          stack configuration.
+    :param int version: The version of the stack configuration.
+    :param str href: A URL.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        definition: 'StackConfigDefinitionSummary',
+        version: int,
+        href: str,
+    ) -> None:
+        """
+        Initialize a MemberOfDefinition object.
+
+        :param str id: The unique ID.
+        :param StackConfigDefinitionSummary definition: The definition summary of
+               the stack configuration.
+        :param int version: The version of the stack configuration.
+        :param str href: A URL.
+        """
+        self.id = id
+        self.definition = definition
+        self.version = version
+        self.href = href
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'MemberOfDefinition':
+        """Initialize a MemberOfDefinition object from a json dictionary."""
+        args = {}
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
+        else:
+            raise ValueError('Required property \'id\' not present in MemberOfDefinition JSON')
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = StackConfigDefinitionSummary.from_dict(definition)
+        else:
+            raise ValueError('Required property \'definition\' not present in MemberOfDefinition JSON')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
+        else:
+            raise ValueError('Required property \'version\' not present in MemberOfDefinition JSON')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
+        else:
+            raise ValueError('Required property \'href\' not present in MemberOfDefinition JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a MemberOfDefinition object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'definition') and self.definition is not None:
+            if isinstance(self.definition, dict):
+                _dict['definition'] = self.definition
+            else:
+                _dict['definition'] = self.definition.to_dict()
+        if hasattr(self, 'version') and self.version is not None:
+            _dict['version'] = self.version
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this MemberOfDefinition object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'MemberOfDefinition') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'MemberOfDefinition') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class OutputValue:
     """
     OutputValue.
 
     :param str name: The variable name.
     :param str description: (optional) A short explanation of the output value.
     :param object value: (optional) This property can be any value - a string,
@@ -5010,16 +5104,21 @@
     :param dict references: (optional) The references that are used in the
           configuration to resolve input values.
     :param SchematicsMetadata schematics: (optional) A Schematics workspace that is
           associated to a project configuration, with scripts.
     :param str state: The state of the configuration.
     :param bool update_available: (optional) The flag that indicates whether a
           configuration update is available.
-    :param ProjectObjectReference template: (optional) The template reference.
+    :param str template_id: (optional) The stack definition identifier.
+    :param MemberOfDefinition member_of: (optional) The stack config parent of which
+          this configuration is a member of.
     :param str href: A URL.
+    :param str deployment_model: (optional) The configuration type.
+    :param str state_code: (optional) Computed state code clarifying the
+          prerequisites for validation for the configuration.
     :param ProjectConfigDefinitionResponse definition:
     :param ProjectConfigVersionSummary approved_version: (optional) A summary of a
           project configuration version.
     :param ProjectConfigVersionSummary deployed_version: (optional) A summary of a
           project configuration version.
     """
 
@@ -5042,15 +5141,18 @@
         last_validated: Optional['LastValidatedActionWithSummary'] = None,
         last_deployed: Optional['LastActionWithSummary'] = None,
         last_undeployed: Optional['LastActionWithSummary'] = None,
         last_monitoring: Optional['LastMonitoringActionWithSummary'] = None,
         references: Optional[dict] = None,
         schematics: Optional['SchematicsMetadata'] = None,
         update_available: Optional[bool] = None,
-        template: Optional['ProjectObjectReference'] = None,
+        template_id: Optional[str] = None,
+        member_of: Optional['MemberOfDefinition'] = None,
+        deployment_model: Optional[str] = None,
+        state_code: Optional[str] = None,
         approved_version: Optional['ProjectConfigVersionSummary'] = None,
         deployed_version: Optional['ProjectConfigVersionSummary'] = None,
     ) -> None:
         """
         Initialize a ProjectConfig object.
 
         :param str id: The ID of the configuration. If this parameter is empty, an
@@ -5091,15 +5193,20 @@
                project configuration.
         :param dict references: (optional) The references that are used in the
                configuration to resolve input values.
         :param SchematicsMetadata schematics: (optional) A Schematics workspace
                that is associated to a project configuration, with scripts.
         :param bool update_available: (optional) The flag that indicates whether a
                configuration update is available.
-        :param ProjectObjectReference template: (optional) The template reference.
+        :param str template_id: (optional) The stack definition identifier.
+        :param MemberOfDefinition member_of: (optional) The stack config parent of
+               which this configuration is a member of.
+        :param str deployment_model: (optional) The configuration type.
+        :param str state_code: (optional) Computed state code clarifying the
+               prerequisites for validation for the configuration.
         :param ProjectConfigVersionSummary approved_version: (optional) A summary
                of a project configuration version.
         :param ProjectConfigVersionSummary deployed_version: (optional) A summary
                of a project configuration version.
         """
         self.id = id
         self.version = version
@@ -5115,16 +5222,19 @@
         self.last_monitoring = last_monitoring
         self.outputs = outputs
         self.project = project
         self.references = references
         self.schematics = schematics
         self.state = state
         self.update_available = update_available
-        self.template = template
+        self.template_id = template_id
+        self.member_of = member_of
         self.href = href
+        self.deployment_model = deployment_model
+        self.state_code = state_code
         self.definition = definition
         self.approved_version = approved_version
         self.deployed_version = deployed_version
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfig':
         """Initialize a ProjectConfig object from a json dictionary."""
@@ -5181,20 +5291,26 @@
             args['schematics'] = SchematicsMetadata.from_dict(schematics)
         if (state := _dict.get('state')) is not None:
             args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfig JSON')
         if (update_available := _dict.get('update_available')) is not None:
             args['update_available'] = update_available
-        if (template := _dict.get('template')) is not None:
-            args['template'] = ProjectObjectReference.from_dict(template)
+        if (template_id := _dict.get('template_id')) is not None:
+            args['template_id'] = template_id
+        if (member_of := _dict.get('member_of')) is not None:
+            args['member_of'] = MemberOfDefinition.from_dict(member_of)
         if (href := _dict.get('href')) is not None:
             args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectConfig JSON')
+        if (deployment_model := _dict.get('deployment_model')) is not None:
+            args['deployment_model'] = deployment_model
+        if (state_code := _dict.get('state_code')) is not None:
+            args['state_code'] = state_code
         if (definition := _dict.get('definition')) is not None:
             args['definition'] = definition
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfig JSON')
         if (approved_version := _dict.get('approved_version')) is not None:
             args['approved_version'] = ProjectConfigVersionSummary.from_dict(approved_version)
         if (deployed_version := _dict.get('deployed_version')) is not None:
@@ -5274,21 +5390,27 @@
                 _dict['schematics'] = self.schematics
             else:
                 _dict['schematics'] = self.schematics.to_dict()
         if hasattr(self, 'state') and self.state is not None:
             _dict['state'] = self.state
         if hasattr(self, 'update_available') and self.update_available is not None:
             _dict['update_available'] = self.update_available
-        if hasattr(self, 'template') and self.template is not None:
-            if isinstance(self.template, dict):
-                _dict['template'] = self.template
+        if hasattr(self, 'template_id') and self.template_id is not None:
+            _dict['template_id'] = self.template_id
+        if hasattr(self, 'member_of') and self.member_of is not None:
+            if isinstance(self.member_of, dict):
+                _dict['member_of'] = self.member_of
             else:
-                _dict['template'] = self.template.to_dict()
+                _dict['member_of'] = self.member_of.to_dict()
         if hasattr(self, 'href') and self.href is not None:
             _dict['href'] = self.href
+        if hasattr(self, 'deployment_model') and self.deployment_model is not None:
+            _dict['deployment_model'] = self.deployment_model
+        if hasattr(self, 'state_code') and self.state_code is not None:
+            _dict['state_code'] = self.state_code
         if hasattr(self, 'definition') and self.definition is not None:
             if isinstance(self.definition, dict):
                 _dict['definition'] = self.definition
             else:
                 _dict['definition'] = self.definition.to_dict()
         if hasattr(self, 'approved_version') and self.approved_version is not None:
             if isinstance(self.approved_version, dict):
@@ -5339,14 +5461,35 @@
         UNDEPLOYING_FAILED = 'undeploying_failed'
         VALIDATED = 'validated'
         VALIDATING = 'validating'
         VALIDATING_FAILED = 'validating_failed'
         APPLIED = 'applied'
         APPLY_FAILED = 'apply_failed'
 
+    class DeploymentModelEnum(str, Enum):
+        """
+        The configuration type.
+        """
+
+        PROJECT_DEPLOYED = 'project_deployed'
+        USER_DEPLOYED = 'user_deployed'
+        STACK = 'stack'
+
+    class StateCodeEnum(str, Enum):
+        """
+        Computed state code clarifying the prerequisites for validation for the
+        configuration.
+        """
+
+        AWAITING_INPUT = 'awaiting_input'
+        AWAITING_PREREQUISITE = 'awaiting_prerequisite'
+        AWAITING_VALIDATION = 'awaiting_validation'
+        AWAITING_MEMBER_DEPLOYMENT = 'awaiting_member_deployment'
+        AWAITING_STACK_SETUP = 'awaiting_stack_setup'
+
 
 class ProjectConfigAuth:
     """
     The authorization details. You can authorize by using a trusted profile or an API key
     in Secrets Manager.
 
     :param str trusted_profile_id: (optional) The trusted profile ID.
@@ -5548,14 +5691,15 @@
 
         """
         msg = "Cannot instantiate base class. Instead, instantiate one of the defined subclasses: {0}".format(
             ", ".join(
                 [
                     'ProjectConfigDefinitionPatchDAConfigDefinitionPropertiesPatch',
                     'ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch',
+                    'ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch',
                 ]
             )
         )
         raise Exception(msg)
 
 
 class ProjectConfigDefinitionPrototype:
@@ -6721,16 +6865,21 @@
     :param dict references: (optional) The references that are used in the
           configuration to resolve input values.
     :param SchematicsMetadata schematics: (optional) A Schematics workspace that is
           associated to a project configuration, with scripts.
     :param str state: The state of the configuration.
     :param bool update_available: (optional) The flag that indicates whether a
           configuration update is available.
-    :param ProjectObjectReference template: (optional) The template reference.
+    :param str template_id: (optional) The stack definition identifier.
+    :param MemberOfDefinition member_of: (optional) The stack config parent of which
+          this configuration is a member of.
     :param str href: A URL.
+    :param str deployment_model: (optional) The configuration type.
+    :param str state_code: (optional) Computed state code clarifying the
+          prerequisites for validation for the configuration.
     :param ProjectConfigDefinitionResponse definition:
     """
 
     def __init__(
         self,
         id: str,
         version: int,
@@ -6749,15 +6898,18 @@
         last_validated: Optional['LastValidatedActionWithSummary'] = None,
         last_deployed: Optional['LastActionWithSummary'] = None,
         last_undeployed: Optional['LastActionWithSummary'] = None,
         last_monitoring: Optional['LastMonitoringActionWithSummary'] = None,
         references: Optional[dict] = None,
         schematics: Optional['SchematicsMetadata'] = None,
         update_available: Optional[bool] = None,
-        template: Optional['ProjectObjectReference'] = None,
+        template_id: Optional[str] = None,
+        member_of: Optional['MemberOfDefinition'] = None,
+        deployment_model: Optional[str] = None,
+        state_code: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigVersion object.
 
         :param str id: The ID of the configuration. If this parameter is empty, an
                ID is automatically created for the configuration.
         :param int version: The version of the configuration.
@@ -6796,15 +6948,20 @@
                project configuration.
         :param dict references: (optional) The references that are used in the
                configuration to resolve input values.
         :param SchematicsMetadata schematics: (optional) A Schematics workspace
                that is associated to a project configuration, with scripts.
         :param bool update_available: (optional) The flag that indicates whether a
                configuration update is available.
-        :param ProjectObjectReference template: (optional) The template reference.
+        :param str template_id: (optional) The stack definition identifier.
+        :param MemberOfDefinition member_of: (optional) The stack config parent of
+               which this configuration is a member of.
+        :param str deployment_model: (optional) The configuration type.
+        :param str state_code: (optional) Computed state code clarifying the
+               prerequisites for validation for the configuration.
         """
         self.id = id
         self.version = version
         self.is_draft = is_draft
         self.needs_attention_state = needs_attention_state
         self.created_at = created_at
         self.modified_at = modified_at
@@ -6816,16 +6973,19 @@
         self.last_monitoring = last_monitoring
         self.outputs = outputs
         self.project = project
         self.references = references
         self.schematics = schematics
         self.state = state
         self.update_available = update_available
-        self.template = template
+        self.template_id = template_id
+        self.member_of = member_of
         self.href = href
+        self.deployment_model = deployment_model
+        self.state_code = state_code
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigVersion':
         """Initialize a ProjectConfigVersion object from a json dictionary."""
         args = {}
         if (id := _dict.get('id')) is not None:
@@ -6880,20 +7040,26 @@
             args['schematics'] = SchematicsMetadata.from_dict(schematics)
         if (state := _dict.get('state')) is not None:
             args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfigVersion JSON')
         if (update_available := _dict.get('update_available')) is not None:
             args['update_available'] = update_available
-        if (template := _dict.get('template')) is not None:
-            args['template'] = ProjectObjectReference.from_dict(template)
+        if (template_id := _dict.get('template_id')) is not None:
+            args['template_id'] = template_id
+        if (member_of := _dict.get('member_of')) is not None:
+            args['member_of'] = MemberOfDefinition.from_dict(member_of)
         if (href := _dict.get('href')) is not None:
             args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectConfigVersion JSON')
+        if (deployment_model := _dict.get('deployment_model')) is not None:
+            args['deployment_model'] = deployment_model
+        if (state_code := _dict.get('state_code')) is not None:
+            args['state_code'] = state_code
         if (definition := _dict.get('definition')) is not None:
             args['definition'] = definition
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfigVersion JSON')
         return cls(**args)
 
     @classmethod
@@ -6969,21 +7135,27 @@
                 _dict['schematics'] = self.schematics
             else:
                 _dict['schematics'] = self.schematics.to_dict()
         if hasattr(self, 'state') and self.state is not None:
             _dict['state'] = self.state
         if hasattr(self, 'update_available') and self.update_available is not None:
             _dict['update_available'] = self.update_available
-        if hasattr(self, 'template') and self.template is not None:
-            if isinstance(self.template, dict):
-                _dict['template'] = self.template
+        if hasattr(self, 'template_id') and self.template_id is not None:
+            _dict['template_id'] = self.template_id
+        if hasattr(self, 'member_of') and self.member_of is not None:
+            if isinstance(self.member_of, dict):
+                _dict['member_of'] = self.member_of
             else:
-                _dict['template'] = self.template.to_dict()
+                _dict['member_of'] = self.member_of.to_dict()
         if hasattr(self, 'href') and self.href is not None:
             _dict['href'] = self.href
+        if hasattr(self, 'deployment_model') and self.deployment_model is not None:
+            _dict['deployment_model'] = self.deployment_model
+        if hasattr(self, 'state_code') and self.state_code is not None:
+            _dict['state_code'] = self.state_code
         if hasattr(self, 'definition') and self.definition is not None:
             if isinstance(self.definition, dict):
                 _dict['definition'] = self.definition
             else:
                 _dict['definition'] = self.definition.to_dict()
         return _dict
 
@@ -7024,14 +7196,35 @@
         UNDEPLOYING_FAILED = 'undeploying_failed'
         VALIDATED = 'validated'
         VALIDATING = 'validating'
         VALIDATING_FAILED = 'validating_failed'
         APPLIED = 'applied'
         APPLY_FAILED = 'apply_failed'
 
+    class DeploymentModelEnum(str, Enum):
+        """
+        The configuration type.
+        """
+
+        PROJECT_DEPLOYED = 'project_deployed'
+        USER_DEPLOYED = 'user_deployed'
+        STACK = 'stack'
+
+    class StateCodeEnum(str, Enum):
+        """
+        Computed state code clarifying the prerequisites for validation for the
+        configuration.
+        """
+
+        AWAITING_INPUT = 'awaiting_input'
+        AWAITING_PREREQUISITE = 'awaiting_prerequisite'
+        AWAITING_VALIDATION = 'awaiting_validation'
+        AWAITING_MEMBER_DEPLOYMENT = 'awaiting_member_deployment'
+        AWAITING_STACK_SETUP = 'awaiting_stack_setup'
+
 
 class ProjectConfigVersionDefinitionSummary:
     """
     A summary of the definition in a project configuration version.
 
     :param str environment_id: (optional) The ID of the project environment.
     :param str locator_id: (optional) A unique concatenation of the catalog ID and
@@ -7130,36 +7323,43 @@
 class ProjectConfigVersionSummary:
     """
     A summary of a project configuration version.
 
     :param ProjectConfigVersionDefinitionSummary definition: A summary of the
           definition in a project configuration version.
     :param str state: The state of the configuration.
+    :param str state_code: (optional) Computed state code clarifying the
+          prerequisites for validation for the configuration.
     :param int version: The version number of the configuration.
     :param str href: A URL.
     """
 
     def __init__(
         self,
         definition: 'ProjectConfigVersionDefinitionSummary',
         state: str,
         version: int,
         href: str,
+        *,
+        state_code: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigVersionSummary object.
 
         :param ProjectConfigVersionDefinitionSummary definition: A summary of the
                definition in a project configuration version.
         :param str state: The state of the configuration.
         :param int version: The version number of the configuration.
         :param str href: A URL.
+        :param str state_code: (optional) Computed state code clarifying the
+               prerequisites for validation for the configuration.
         """
         self.definition = definition
         self.state = state
+        self.state_code = state_code
         self.version = version
         self.href = href
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigVersionSummary':
         """Initialize a ProjectConfigVersionSummary object from a json dictionary."""
         args = {}
@@ -7167,14 +7367,16 @@
             args['definition'] = ProjectConfigVersionDefinitionSummary.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfigVersionSummary JSON')
         if (state := _dict.get('state')) is not None:
             args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfigVersionSummary JSON')
+        if (state_code := _dict.get('state_code')) is not None:
+            args['state_code'] = state_code
         if (version := _dict.get('version')) is not None:
             args['version'] = version
         else:
             raise ValueError('Required property \'version\' not present in ProjectConfigVersionSummary JSON')
         if (href := _dict.get('href')) is not None:
             args['href'] = href
         else:
@@ -7192,14 +7394,16 @@
         if hasattr(self, 'definition') and self.definition is not None:
             if isinstance(self.definition, dict):
                 _dict['definition'] = self.definition
             else:
                 _dict['definition'] = self.definition.to_dict()
         if hasattr(self, 'state') and self.state is not None:
             _dict['state'] = self.state
+        if hasattr(self, 'state_code') and self.state_code is not None:
+            _dict['state_code'] = self.state_code
         if hasattr(self, 'version') and self.version is not None:
             _dict['version'] = self.version
         if hasattr(self, 'href') and self.href is not None:
             _dict['href'] = self.href
         return _dict
 
     def _to_dict(self):
@@ -7239,14 +7443,26 @@
         UNDEPLOYING_FAILED = 'undeploying_failed'
         VALIDATED = 'validated'
         VALIDATING = 'validating'
         VALIDATING_FAILED = 'validating_failed'
         APPLIED = 'applied'
         APPLY_FAILED = 'apply_failed'
 
+    class StateCodeEnum(str, Enum):
+        """
+        Computed state code clarifying the prerequisites for validation for the
+        configuration.
+        """
+
+        AWAITING_INPUT = 'awaiting_input'
+        AWAITING_PREREQUISITE = 'awaiting_prerequisite'
+        AWAITING_VALIDATION = 'awaiting_validation'
+        AWAITING_MEMBER_DEPLOYMENT = 'awaiting_member_deployment'
+        AWAITING_STACK_SETUP = 'awaiting_stack_setup'
+
 
 class ProjectConfigVersionSummaryCollection:
     """
     The project configuration version list.
 
     :param List[ProjectConfigVersionSummary] versions: The collection list operation
           response schema that defines the array property with the name `versions`.
@@ -7712,83 +7928,14 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectEnvironmentSummaryDefinition') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
-class ProjectObjectReference:
-    """
-    ProjectObjectReference.
-
-    :param str id: The unique ID.
-    :param str href: A URL.
-    """
-
-    def __init__(
-        self,
-        id: str,
-        href: str,
-    ) -> None:
-        """
-        Initialize a ProjectObjectReference object.
-
-        :param str id: The unique ID.
-        :param str href: A URL.
-        """
-        self.id = id
-        self.href = href
-
-    @classmethod
-    def from_dict(cls, _dict: Dict) -> 'ProjectObjectReference':
-        """Initialize a ProjectObjectReference object from a json dictionary."""
-        args = {}
-        if (id := _dict.get('id')) is not None:
-            args['id'] = id
-        else:
-            raise ValueError('Required property \'id\' not present in ProjectObjectReference JSON')
-        if (href := _dict.get('href')) is not None:
-            args['href'] = href
-        else:
-            raise ValueError('Required property \'href\' not present in ProjectObjectReference JSON')
-        return cls(**args)
-
-    @classmethod
-    def _from_dict(cls, _dict):
-        """Initialize a ProjectObjectReference object from a json dictionary."""
-        return cls.from_dict(_dict)
-
-    def to_dict(self) -> Dict:
-        """Return a json dictionary representing this model."""
-        _dict = {}
-        if hasattr(self, 'id') and self.id is not None:
-            _dict['id'] = self.id
-        if hasattr(self, 'href') and self.href is not None:
-            _dict['href'] = self.href
-        return _dict
-
-    def _to_dict(self):
-        """Return a json dictionary representing this model."""
-        return self.to_dict()
-
-    def __str__(self) -> str:
-        """Return a `str` version of this ProjectObjectReference object."""
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __eq__(self, other: 'ProjectObjectReference') -> bool:
-        """Return `true` when self and other are equal, false otherwise."""
-        if not isinstance(other, self.__class__):
-            return False
-        return self.__dict__ == other.__dict__
-
-    def __ne__(self, other: 'ProjectObjectReference') -> bool:
-        """Return `true` when self and other are not equal, false otherwise."""
-        return not self == other
-
-
 class ProjectPatchDefinitionBlock:
     """
     The definition of the project.
 
     :param str name: (optional) The name of the project.  It's unique within the
           account across regions.
     :param bool destroy_on_delete: (optional) The policy that indicates whether the
@@ -8557,14 +8704,93 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Script') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class StackConfigDefinitionSummary:
+    """
+    The definition summary of the stack configuration.
+
+    :param str name: The configuration name. It's unique within the account across
+          projects and regions.
+    :param List[StackConfigMember] members: The member deployabe architectures that
+          are included in your stack.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        members: List['StackConfigMember'],
+    ) -> None:
+        """
+        Initialize a StackConfigDefinitionSummary object.
+
+        :param str name: The configuration name. It's unique within the account
+               across projects and regions.
+        :param List[StackConfigMember] members: The member deployabe architectures
+               that are included in your stack.
+        """
+        self.name = name
+        self.members = members
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackConfigDefinitionSummary':
+        """Initialize a StackConfigDefinitionSummary object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackConfigDefinitionSummary JSON')
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackConfigMember.from_dict(v) for v in members]
+        else:
+            raise ValueError('Required property \'members\' not present in StackConfigDefinitionSummary JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackConfigDefinitionSummary object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'members') and self.members is not None:
+            members_list = []
+            for v in self.members:
+                if isinstance(v, dict):
+                    members_list.append(v)
+                else:
+                    members_list.append(v.to_dict())
+            _dict['members'] = members_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackConfigDefinitionSummary object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackConfigDefinitionSummary') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackConfigDefinitionSummary') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class StackConfigMember:
     """
     A member deployable architecture that is included in your stack.
 
     :param str name: The name matching the alias in the stack definition.
     :param str config_id: The unique ID.
     """
@@ -10093,14 +10319,196 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch(ProjectConfigDefinitionPatch):
+    """
+    The name and description of a project configuration.
+
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
+          is required for compliance.
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
+          the version ID that identify the deployable architecture in the catalog. I
+          you're importing from an existing Schematics workspace that is not backed by
+          cart, a `locator_id` is required. If you're using a Schematics workspace that is
+          backed by cart, a `locator_id` is not necessary because the Schematics workspace
+          has one.
+          > There are 3 scenarios:
+          > 1. If only a `locator_id` is specified, a new Schematics workspace is
+          instantiated with that `locator_id`.
+          > 2. If only a schematics `workspace_crn` is specified, a `400` is returned if a
+          `locator_id` is not found in the existing schematics workspace.
+          > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
+          `400` message is returned if the specified `locator_id` does not agree with the
+          `locator_id` in the existing Schematics workspace.
+          > For more information of creating a Schematics workspace, see [Creating
+          workspaces and importing your Terraform
+          template](/docs/schematics?topic=schematics-sch-create-wks).
+    :param List[StackConfigMember] members: (optional) The member deployabe
+          architectures that are included in your stack.
+    :param str description: (optional) A project configuration description.
+    :param str name: (optional) The configuration name. It's unique within the
+          account across projects and regions.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
+          You can authorize by using a trusted profile or an API key in Secrets Manager.
+    :param dict inputs: (optional) The input variables that are used for
+          configuration definition and environment.
+    :param dict settings: (optional) The Schematics environment variables to use to
+          deploy the configuration. Settings are only available if they are specified when
+          the configuration is initially created.
+    """
+
+    def __init__(
+        self,
+        *,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
+        locator_id: Optional[str] = None,
+        members: Optional[List['StackConfigMember']] = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
+    ) -> None:
+        """
+        Initialize a ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch object.
+
+        :param ProjectComplianceProfile compliance_profile: (optional) The profile
+               that is required for compliance.
+        :param str locator_id: (optional) A unique concatenation of the catalog ID
+               and the version ID that identify the deployable architecture in the
+               catalog. I you're importing from an existing Schematics workspace that is
+               not backed by cart, a `locator_id` is required. If you're using a
+               Schematics workspace that is backed by cart, a `locator_id` is not
+               necessary because the Schematics workspace has one.
+               > There are 3 scenarios:
+               > 1. If only a `locator_id` is specified, a new Schematics workspace is
+               instantiated with that `locator_id`.
+               > 2. If only a schematics `workspace_crn` is specified, a `400` is returned
+               if a `locator_id` is not found in the existing schematics workspace.
+               > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified,
+               a `400` message is returned if the specified `locator_id` does not agree
+               with the `locator_id` in the existing Schematics workspace.
+               > For more information of creating a Schematics workspace, see [Creating
+               workspaces and importing your Terraform
+               template](/docs/schematics?topic=schematics-sch-create-wks).
+        :param List[StackConfigMember] members: (optional) The member deployabe
+               architectures that are included in your stack.
+        :param str description: (optional) A project configuration description.
+        :param str name: (optional) The configuration name. It's unique within the
+               account across projects and regions.
+        :param str environment_id: (optional) The ID of the project environment.
+        :param ProjectConfigAuth authorizations: (optional) The authorization
+               details. You can authorize by using a trusted profile or an API key in
+               Secrets Manager.
+        :param dict inputs: (optional) The input variables that are used for
+               configuration definition and environment.
+        :param dict settings: (optional) The Schematics environment variables to
+               use to deploy the configuration. Settings are only available if they are
+               specified when the configuration is initially created.
+        """
+        # pylint: disable=super-init-not-called
+        self.compliance_profile = compliance_profile
+        self.locator_id = locator_id
+        self.members = members
+        self.description = description
+        self.name = name
+        self.environment_id = environment_id
+        self.authorizations = authorizations
+        self.inputs = inputs
+        self.settings = settings
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch':
+        """Initialize a ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch object from a json dictionary."""
+        args = {}
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackConfigMember.from_dict(v) for v in members]
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'compliance_profile') and self.compliance_profile is not None:
+            if isinstance(self.compliance_profile, dict):
+                _dict['compliance_profile'] = self.compliance_profile
+            else:
+                _dict['compliance_profile'] = self.compliance_profile.to_dict()
+        if hasattr(self, 'locator_id') and self.locator_id is not None:
+            _dict['locator_id'] = self.locator_id
+        if hasattr(self, 'members') and self.members is not None:
+            members_list = []
+            for v in self.members:
+                if isinstance(v, dict):
+                    members_list.append(v)
+                else:
+                    members_list.append(v.to_dict())
+            _dict['members'] = members_list
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'environment_id') and self.environment_id is not None:
+            _dict['environment_id'] = self.environment_id
+        if hasattr(self, 'authorizations') and self.authorizations is not None:
+            if isinstance(self.authorizations, dict):
+                _dict['authorizations'] = self.authorizations
+            else:
+                _dict['authorizations'] = self.authorizations.to_dict()
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            _dict['inputs'] = self.inputs
+        if hasattr(self, 'settings') and self.settings is not None:
+            _dict['settings'] = self.settings
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ProjectConfigDefinitionPatchStackConfigDefinitionPropertiesPatch') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype(ProjectConfigDefinitionPrototype):
     """
     The description of a project configuration.
 
     :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
     :param str locator_id: (optional) A unique concatenation of the catalog ID and
@@ -10394,17 +10802,16 @@
         return not self == other
 
 
 class ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties(ProjectConfigDefinitionPrototype):
     """
     The description of a project configuration.
 
-    :param str description: (optional) A project configuration description.
-    :param str name: (optional) The configuration name. It's unique within the
-          account across projects and regions.
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
+          is required for compliance.
     :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
@@ -10414,37 +10821,49 @@
           `locator_id` is not found in the existing schematics workspace.
           > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
           `400` message is returned if the specified `locator_id` does not agree with the
           `locator_id` in the existing Schematics workspace.
           > For more information of creating a Schematics workspace, see [Creating
           workspaces and importing your Terraform
           template](/docs/schematics?topic=schematics-sch-create-wks).
+    :param List[StackConfigMember] members: (optional) The member deployabe
+          architectures that are included in your stack.
+    :param str description: (optional) A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
+          projects and regions.
     :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
+          You can authorize by using a trusted profile or an API key in Secrets Manager.
     :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :param List[StackConfigMember] members: (optional) The member deployabe
-          architectures that are included in your stack.
+    :param dict settings: (optional) The Schematics environment variables to use to
+          deploy the configuration. Settings are only available if they are specified when
+          the configuration is initially created.
     """
 
     def __init__(
         self,
+        name: str,
         *,
-        description: Optional[str] = None,
-        name: Optional[str] = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
         locator_id: Optional[str] = None,
+        members: Optional[List['StackConfigMember']] = None,
+        description: Optional[str] = None,
         environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
         inputs: Optional[dict] = None,
-        members: Optional[List['StackConfigMember']] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object.
 
-        :param str description: (optional) A project configuration description.
-        :param str name: (optional) The configuration name. It's unique within the
-               account across projects and regions.
+        :param str name: The configuration name. It's unique within the account
+               across projects and regions.
+        :param ProjectComplianceProfile compliance_profile: (optional) The profile
+               that is required for compliance.
         :param str locator_id: (optional) A unique concatenation of the catalog ID
                and the version ID that identify the deployable architecture in the
                catalog. I you're importing from an existing Schematics workspace that is
                not backed by cart, a `locator_id` is required. If you're using a
                Schematics workspace that is backed by cart, a `locator_id` is not
                necessary because the Schematics workspace has one.
                > There are 3 scenarios:
@@ -10454,72 +10873,104 @@
                if a `locator_id` is not found in the existing schematics workspace.
                > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified,
                a `400` message is returned if the specified `locator_id` does not agree
                with the `locator_id` in the existing Schematics workspace.
                > For more information of creating a Schematics workspace, see [Creating
                workspaces and importing your Terraform
                template](/docs/schematics?topic=schematics-sch-create-wks).
+        :param List[StackConfigMember] members: (optional) The member deployabe
+               architectures that are included in your stack.
+        :param str description: (optional) A project configuration description.
         :param str environment_id: (optional) The ID of the project environment.
+        :param ProjectConfigAuth authorizations: (optional) The authorization
+               details. You can authorize by using a trusted profile or an API key in
+               Secrets Manager.
         :param dict inputs: (optional) The input variables that are used for
                configuration definition and environment.
-        :param List[StackConfigMember] members: (optional) The member deployabe
-               architectures that are included in your stack.
+        :param dict settings: (optional) The Schematics environment variables to
+               use to deploy the configuration. Settings are only available if they are
+               specified when the configuration is initially created.
         """
         # pylint: disable=super-init-not-called
+        self.compliance_profile = compliance_profile
+        self.locator_id = locator_id
+        self.members = members
         self.description = description
         self.name = name
-        self.locator_id = locator_id
         self.environment_id = environment_id
+        self.authorizations = authorizations
         self.inputs = inputs
-        self.members = members
+        self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties':
         """Initialize a ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object from a json dictionary."""
         args = {}
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackConfigMember.from_dict(v) for v in members]
         if (description := _dict.get('description')) is not None:
             args['description'] = description
         if (name := _dict.get('name')) is not None:
             args['name'] = name
-        if (locator_id := _dict.get('locator_id')) is not None:
-            args['locator_id'] = locator_id
+        else:
+            raise ValueError(
+                'Required property \'name\' not present in ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties JSON'
+            )
         if (environment_id := _dict.get('environment_id')) is not None:
             args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
         if (inputs := _dict.get('inputs')) is not None:
             args['inputs'] = inputs
-        if (members := _dict.get('members')) is not None:
-            args['members'] = [StackConfigMember.from_dict(v) for v in members]
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, 'description') and self.description is not None:
-            _dict['description'] = self.description
-        if hasattr(self, 'name') and self.name is not None:
-            _dict['name'] = self.name
+        if hasattr(self, 'compliance_profile') and self.compliance_profile is not None:
+            if isinstance(self.compliance_profile, dict):
+                _dict['compliance_profile'] = self.compliance_profile
+            else:
+                _dict['compliance_profile'] = self.compliance_profile.to_dict()
         if hasattr(self, 'locator_id') and self.locator_id is not None:
             _dict['locator_id'] = self.locator_id
-        if hasattr(self, 'environment_id') and self.environment_id is not None:
-            _dict['environment_id'] = self.environment_id
-        if hasattr(self, 'inputs') and self.inputs is not None:
-            _dict['inputs'] = self.inputs
         if hasattr(self, 'members') and self.members is not None:
             members_list = []
             for v in self.members:
                 if isinstance(v, dict):
                     members_list.append(v)
                 else:
                     members_list.append(v.to_dict())
             _dict['members'] = members_list
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'environment_id') and self.environment_id is not None:
+            _dict['environment_id'] = self.environment_id
+        if hasattr(self, 'authorizations') and self.authorizations is not None:
+            if isinstance(self.authorizations, dict):
+                _dict['authorizations'] = self.authorizations
+            else:
+                _dict['authorizations'] = self.authorizations.to_dict()
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            _dict['inputs'] = self.inputs
+        if hasattr(self, 'settings') and self.settings is not None:
+            _dict['settings'] = self.settings
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
@@ -10842,17 +11293,16 @@
         return not self == other
 
 
 class ProjectConfigDefinitionResponseStackConfigDefinitionProperties(ProjectConfigDefinitionResponse):
     """
     The description of a project configuration.
 
-    :param str description: (optional) A project configuration description.
-    :param str name: (optional) The configuration name. It's unique within the
-          account across projects and regions.
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
+          is required for compliance.
     :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
@@ -10862,37 +11312,49 @@
           `locator_id` is not found in the existing schematics workspace.
           > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
           `400` message is returned if the specified `locator_id` does not agree with the
           `locator_id` in the existing Schematics workspace.
           > For more information of creating a Schematics workspace, see [Creating
           workspaces and importing your Terraform
           template](/docs/schematics?topic=schematics-sch-create-wks).
+    :param List[StackConfigMember] members: (optional) The member deployabe
+          architectures that are included in your stack.
+    :param str description: (optional) A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
+          projects and regions.
     :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
+          You can authorize by using a trusted profile or an API key in Secrets Manager.
     :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :param List[StackConfigMember] members: (optional) The member deployabe
-          architectures that are included in your stack.
+    :param dict settings: (optional) The Schematics environment variables to use to
+          deploy the configuration. Settings are only available if they are specified when
+          the configuration is initially created.
     """
 
     def __init__(
         self,
+        name: str,
         *,
-        description: Optional[str] = None,
-        name: Optional[str] = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
         locator_id: Optional[str] = None,
+        members: Optional[List['StackConfigMember']] = None,
+        description: Optional[str] = None,
         environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
         inputs: Optional[dict] = None,
-        members: Optional[List['StackConfigMember']] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionResponseStackConfigDefinitionProperties object.
 
-        :param str description: (optional) A project configuration description.
-        :param str name: (optional) The configuration name. It's unique within the
-               account across projects and regions.
+        :param str name: The configuration name. It's unique within the account
+               across projects and regions.
+        :param ProjectComplianceProfile compliance_profile: (optional) The profile
+               that is required for compliance.
         :param str locator_id: (optional) A unique concatenation of the catalog ID
                and the version ID that identify the deployable architecture in the
                catalog. I you're importing from an existing Schematics workspace that is
                not backed by cart, a `locator_id` is required. If you're using a
                Schematics workspace that is backed by cart, a `locator_id` is not
                necessary because the Schematics workspace has one.
                > There are 3 scenarios:
@@ -10902,72 +11364,104 @@
                if a `locator_id` is not found in the existing schematics workspace.
                > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified,
                a `400` message is returned if the specified `locator_id` does not agree
                with the `locator_id` in the existing Schematics workspace.
                > For more information of creating a Schematics workspace, see [Creating
                workspaces and importing your Terraform
                template](/docs/schematics?topic=schematics-sch-create-wks).
+        :param List[StackConfigMember] members: (optional) The member deployabe
+               architectures that are included in your stack.
+        :param str description: (optional) A project configuration description.
         :param str environment_id: (optional) The ID of the project environment.
+        :param ProjectConfigAuth authorizations: (optional) The authorization
+               details. You can authorize by using a trusted profile or an API key in
+               Secrets Manager.
         :param dict inputs: (optional) The input variables that are used for
                configuration definition and environment.
-        :param List[StackConfigMember] members: (optional) The member deployabe
-               architectures that are included in your stack.
+        :param dict settings: (optional) The Schematics environment variables to
+               use to deploy the configuration. Settings are only available if they are
+               specified when the configuration is initially created.
         """
         # pylint: disable=super-init-not-called
+        self.compliance_profile = compliance_profile
+        self.locator_id = locator_id
+        self.members = members
         self.description = description
         self.name = name
-        self.locator_id = locator_id
         self.environment_id = environment_id
+        self.authorizations = authorizations
         self.inputs = inputs
-        self.members = members
+        self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionResponseStackConfigDefinitionProperties':
         """Initialize a ProjectConfigDefinitionResponseStackConfigDefinitionProperties object from a json dictionary."""
         args = {}
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackConfigMember.from_dict(v) for v in members]
         if (description := _dict.get('description')) is not None:
             args['description'] = description
         if (name := _dict.get('name')) is not None:
             args['name'] = name
-        if (locator_id := _dict.get('locator_id')) is not None:
-            args['locator_id'] = locator_id
+        else:
+            raise ValueError(
+                'Required property \'name\' not present in ProjectConfigDefinitionResponseStackConfigDefinitionProperties JSON'
+            )
         if (environment_id := _dict.get('environment_id')) is not None:
             args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
         if (inputs := _dict.get('inputs')) is not None:
             args['inputs'] = inputs
-        if (members := _dict.get('members')) is not None:
-            args['members'] = [StackConfigMember.from_dict(v) for v in members]
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionResponseStackConfigDefinitionProperties object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
-        if hasattr(self, 'description') and self.description is not None:
-            _dict['description'] = self.description
-        if hasattr(self, 'name') and self.name is not None:
-            _dict['name'] = self.name
+        if hasattr(self, 'compliance_profile') and self.compliance_profile is not None:
+            if isinstance(self.compliance_profile, dict):
+                _dict['compliance_profile'] = self.compliance_profile
+            else:
+                _dict['compliance_profile'] = self.compliance_profile.to_dict()
         if hasattr(self, 'locator_id') and self.locator_id is not None:
             _dict['locator_id'] = self.locator_id
-        if hasattr(self, 'environment_id') and self.environment_id is not None:
-            _dict['environment_id'] = self.environment_id
-        if hasattr(self, 'inputs') and self.inputs is not None:
-            _dict['inputs'] = self.inputs
         if hasattr(self, 'members') and self.members is not None:
             members_list = []
             for v in self.members:
                 if isinstance(v, dict):
                     members_list.append(v)
                 else:
                     members_list.append(v.to_dict())
             _dict['members'] = members_list
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'environment_id') and self.environment_id is not None:
+            _dict['environment_id'] = self.environment_id
+        if hasattr(self, 'authorizations') and self.authorizations is not None:
+            if isinstance(self.authorizations, dict):
+                _dict['authorizations'] = self.authorizations
+            else:
+                _dict['authorizations'] = self.authorizations.to_dict()
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            _dict['inputs'] = self.inputs
+        if hasattr(self, 'settings') and self.settings is not None:
+            _dict['settings'] = self.settings
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
```

### Comparing `ibm-project-sdk-0.0.5/ibm_project_sdk/version.py` & `ibm-project-sdk-0.0.6/ibm_project_sdk/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of project
 """
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

### Comparing `ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/PKG-INFO` & `ibm-project-sdk-0.0.6/ibm_project_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-project-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Project Services Python SDK
 Home-page: https://github.com/IBM/project-python-sdk
 Author: IBM
 Author-email: dvesperini@gmail.com
 License: Apache 2.0
 Keywords: ibm_project_sdk
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://api.travis-ci.com/IBM/project-python-sdk.svg?branch=main)](https://app.travis-ci.com/github/IBM/project-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# Project Services Python SDK Version 0.0.5
+# Project Services Python SDK Version 0.0.6
 
 Python client library to interact with various [IBM Cloud Platform Services APIs](https://cloud.ibm.com/apidocs?category=platform-services).
 
 Disclaimer: this SDK is being released initially as a **pre-release** version.
 Changes might occur which impact applications that use this SDK.
 
 ## Table of Contents
@@ -76,15 +76,15 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip`:
 
 ```bash
-pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.5
+pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.6
 ```
 
 Then in your code, you can import the appropriate service like this:
 ```
 from ibm_project_sdk.project_v1 import *
 ```
 where `<service-module-name>` is the service's module name from the table above
```

### Comparing `ibm-project-sdk-0.0.5/setup.py` & `ibm-project-sdk-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 PACKAGE_NAME = 'ibm_project_sdk'
 PACKAGE_DESC = 'Project Services Python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

