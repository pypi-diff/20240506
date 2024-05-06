# Comparing `tmp/cost-monitoring-construct-1.2.2.tar.gz` & `tmp/cost-monitoring-construct-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-monitoring-construct-1.2.2.tar", last modified: Fri May  3 13:06:36 2024, max compression
+gzip compressed data, was "cost-monitoring-construct-1.2.3.tar", last modified: Mon May  6 09:00:49 2024, max compression
```

## Comparing `cost-monitoring-construct-1.2.2.tar` & `cost-monitoring-construct-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/
--rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79199 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:06:26.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:06:36.965151 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-03 13:06:36.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 13:06:36.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:06:36.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 13:06:36.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 13:06:36.000000 cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:00:49.082642 cost-monitoring-construct-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-06 09:00:49.082642 cost-monitoring-construct-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:00:49.082642 cost-monitoring-construct-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:00:49.078642 cost-monitoring-construct-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:00:49.082642 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/
+-rw-r--r--   0 runner    (1001) docker     (127)    71864 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:00:49.082642 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79217 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:00:35.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:00:49.082642 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-06 09:00:49.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-06 09:00:49.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:00:49.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 09:00:49.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 09:00:49.000000 cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/top_level.txt
```

### Comparing `cost-monitoring-construct-1.2.2/LICENSE` & `cost-monitoring-construct-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cost-monitoring-construct-1.2.2/PKG-INFO` & `cost-monitoring-construct-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.2.2
+Version: 1.2.3
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cost-monitoring-construct-1.2.2/README.md` & `cost-monitoring-construct-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cost-monitoring-construct-1.2.2/setup.py` & `cost-monitoring-construct-1.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cost-monitoring-construct",
-    "version": "1.2.2",
+    "version": "1.2.3",
     "description": "A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage",
     "license": "Apache-2.0",
     "url": "https://github.com/DataChefHQ/cost-monitoring-construct.git",
     "long_description_content_type": "text/markdown",
     "author": "DataChef<support@datachef.co>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cost_monitoring_construct",
         "cost_monitoring_construct._jsii"
     ],
     "package_data": {
         "cost_monitoring_construct._jsii": [
-            "cost-monitoring-construct@1.2.2.jsii.tgz"
+            "cost-monitoring-construct@1.2.3.jsii.tgz"
         ],
         "cost_monitoring_construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cost-monitoring-construct-1.2.2/src/cost_monitoring_construct/__init__.py` & `cost-monitoring-construct-1.2.3/src/cost_monitoring_construct/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,29 +537,29 @@
         ...
 
     @monthly_limit_in_dollars.setter
     def monthly_limit_in_dollars(self, value: jsii.Number) -> None:
         ...
 
     @builtins.property
-    @jsii.member(jsii_name="defaultTopic")
-    def default_topic(self) -> typing.Optional[builtins.str]:
+    @jsii.member(jsii_name="subscribers")
+    def subscribers(self) -> typing.List[builtins.str]:
         ...
 
-    @default_topic.setter
-    def default_topic(self, value: typing.Optional[builtins.str]) -> None:
+    @subscribers.setter
+    def subscribers(self, value: typing.List[builtins.str]) -> None:
         ...
 
     @builtins.property
-    @jsii.member(jsii_name="subscribers")
-    def subscribers(self) -> typing.Optional[typing.List[builtins.str]]:
+    @jsii.member(jsii_name="defaultTopic")
+    def default_topic(self) -> typing.Optional[builtins.str]:
         ...
 
-    @subscribers.setter
-    def subscribers(self, value: typing.Optional[typing.List[builtins.str]]) -> None:
+    @default_topic.setter
+    def default_topic(self, value: typing.Optional[builtins.str]) -> None:
         ...
 
 
 class _IBudgetStrategyPropsProxy:
     __jsii_type__: typing.ClassVar[str] = "cost-monitoring-construct.IBudgetStrategyProps"
 
     @builtins.property
@@ -571,37 +571,37 @@
     def monthly_limit_in_dollars(self, value: jsii.Number) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d3c41c81462322c9b6739b44cf119d812e914ce08ff18786aff1ba9fc132d07d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "monthlyLimitInDollars", value)
 
     @builtins.property
+    @jsii.member(jsii_name="subscribers")
+    def subscribers(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "subscribers"))
+
+    @subscribers.setter
+    def subscribers(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7097f679e2b7535ab4395d449452bc902f33d9088d3294c3a999153b5df55fc8)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "subscribers", value)
+
+    @builtins.property
     @jsii.member(jsii_name="defaultTopic")
     def default_topic(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "defaultTopic"))
 
     @default_topic.setter
     def default_topic(self, value: typing.Optional[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a2072df5054cedd9785787c9e96d3ad7f9897375df6988c2471bddba94a014f6)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "defaultTopic", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="subscribers")
-    def subscribers(self) -> typing.Optional[typing.List[builtins.str]]:
-        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "subscribers"))
-
-    @subscribers.setter
-    def subscribers(self, value: typing.Optional[typing.List[builtins.str]]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7097f679e2b7535ab4395d449452bc902f33d9088d3294c3a999153b5df55fc8)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "subscribers", value)
-
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IBudgetStrategyProps).__jsii_proxy_class__ = lambda : _IBudgetStrategyPropsProxy
 
 
 @jsii.interface(jsii_type="cost-monitoring-construct.IOptionalBudgetAlertCondition")
 class IOptionalBudgetAlertCondition(typing_extensions.Protocol):
     @builtins.property
@@ -1199,36 +1199,36 @@
     metaclass=jsii.JSIIMeta,
     jsii_type="cost-monitoring-construct.ApplicationCostMonitoringProps",
 ):
     def __init__(
         self,
         application_name: builtins.str,
         monthly_limit_in_dollars: jsii.Number,
+        subscribers: typing.Sequence[builtins.str],
         other_stacks_included_in_budget: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.Stack]] = None,
         default_topic: typing.Optional[builtins.str] = None,
-        subscribers: typing.Optional[typing.Sequence[builtins.str]] = None,
         cost_allocation_tag: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param application_name: - the name of application to label resources with it.
         :param monthly_limit_in_dollars: - montly limit in US Dollors.
+        :param subscribers: - list of email address that the CostMonitoring will use to send alerts to.
         :param other_stacks_included_in_budget: - optional other stack to track their resources alog with the default stack.
         :param default_topic: - default SNS topic name. Only if provided, the BudgetStratgy creates an SNS topic and send notifications to it.
-        :param subscribers: - list of email address that the CostMonitoring will use to send alerts to.
         :param cost_allocation_tag: - Tag key used to track resources' expenditure. Only if provided, it will be used to tag the application resources. Defaults to ``cm:application``
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__016611925949da4facbba95bcddcf14217d235eea769e2db3a3d240c6ca86d73)
             check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
             check_type(argname="argument monthly_limit_in_dollars", value=monthly_limit_in_dollars, expected_type=type_hints["monthly_limit_in_dollars"])
+            check_type(argname="argument subscribers", value=subscribers, expected_type=type_hints["subscribers"])
             check_type(argname="argument other_stacks_included_in_budget", value=other_stacks_included_in_budget, expected_type=type_hints["other_stacks_included_in_budget"])
             check_type(argname="argument default_topic", value=default_topic, expected_type=type_hints["default_topic"])
-            check_type(argname="argument subscribers", value=subscribers, expected_type=type_hints["subscribers"])
             check_type(argname="argument cost_allocation_tag", value=cost_allocation_tag, expected_type=type_hints["cost_allocation_tag"])
-        jsii.create(self.__class__, self, [application_name, monthly_limit_in_dollars, other_stacks_included_in_budget, default_topic, subscribers, cost_allocation_tag])
+        jsii.create(self.__class__, self, [application_name, monthly_limit_in_dollars, subscribers, other_stacks_included_in_budget, default_topic, cost_allocation_tag])
 
     @builtins.property
     @jsii.member(jsii_name="applicationName")
     def application_name(self) -> builtins.str:
         '''- the name of application to label resources with it.'''
         return typing.cast(builtins.str, jsii.get(self, "applicationName"))
 
@@ -1249,14 +1249,27 @@
     def monthly_limit_in_dollars(self, value: jsii.Number) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__57b7dbe15daa64f31317dedf1362713156a13c2d526b10bae05bb824fb1852b5)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "monthlyLimitInDollars", value)
 
     @builtins.property
+    @jsii.member(jsii_name="subscribers")
+    def subscribers(self) -> typing.List[builtins.str]:
+        '''- list of email address that the CostMonitoring will use to send alerts to.'''
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "subscribers"))
+
+    @subscribers.setter
+    def subscribers(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "subscribers", value)
+
+    @builtins.property
     @jsii.member(jsii_name="costAllocationTag")
     def cost_allocation_tag(self) -> typing.Optional[builtins.str]:
         '''- Tag key used to track resources' expenditure.
 
         Only if provided, it will be used to tag the application resources. Defaults to ``cm:application``
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "costAllocationTag"))
@@ -1298,27 +1311,14 @@
         value: typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__27ca7aaaa6cac405f55855e5078ed65603a6f03c771242fe182f13cf406a81a0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "otherStacksIncludedInBudget", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="subscribers")
-    def subscribers(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''- list of email address that the CostMonitoring will use to send alerts to.'''
-        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "subscribers"))
-
-    @subscribers.setter
-    def subscribers(self, value: typing.Optional[typing.List[builtins.str]]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "subscribers", value)
-
 
 __all__ = [
     "AccountCostMonitoring",
     "ApplicationCostMonitoring",
     "ApplicationCostMonitoringProps",
     "Budget",
     "ComparisonOperator",
@@ -1450,22 +1450,22 @@
 
 def _typecheckingstub__d3c41c81462322c9b6739b44cf119d812e914ce08ff18786aff1ba9fc132d07d(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a2072df5054cedd9785787c9e96d3ad7f9897375df6988c2471bddba94a014f6(
-    value: typing.Optional[builtins.str],
+def _typecheckingstub__7097f679e2b7535ab4395d449452bc902f33d9088d3294c3a999153b5df55fc8(
+    value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7097f679e2b7535ab4395d449452bc902f33d9088d3294c3a999153b5df55fc8(
-    value: typing.Optional[typing.List[builtins.str]],
+def _typecheckingstub__a2072df5054cedd9785787c9e96d3ad7f9897375df6988c2471bddba94a014f6(
+    value: typing.Optional[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e9d072ebf62d46641c750811e356317d82231f397276302d0a3eb26b8ece143a(
     value: typing.Optional[ComparisonOperator],
 ) -> None:
@@ -1619,17 +1619,17 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__016611925949da4facbba95bcddcf14217d235eea769e2db3a3d240c6ca86d73(
     application_name: builtins.str,
     monthly_limit_in_dollars: jsii.Number,
+    subscribers: typing.Sequence[builtins.str],
     other_stacks_included_in_budget: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.Stack]] = None,
     default_topic: typing.Optional[builtins.str] = None,
-    subscribers: typing.Optional[typing.Sequence[builtins.str]] = None,
     cost_allocation_tag: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4fd4ce542700b2deac40811890f4429d90eac081bd29d08415e6ce8667697422(
     value: builtins.str,
@@ -1639,14 +1639,20 @@
 
 def _typecheckingstub__57b7dbe15daa64f31317dedf1362713156a13c2d526b10bae05bb824fb1852b5(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__3bd683e50b33baeaf6f59fc99784ce52773a612c0f5a480e422ab4972f7f6e2b(
     value: typing.Optional[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a36b5adee3e84bbffda1fbfb9801304b1780cd8ef3dc089586a0aeee043a09a7(
@@ -1656,13 +1662,7 @@
     pass
 
 def _typecheckingstub__27ca7aaaa6cac405f55855e5078ed65603a6f03c771242fe182f13cf406a81a0(
     value: typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]],
 ) -> None:
     """Type checking stubs"""
     pass
-
-def _typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2(
-    value: typing.Optional[typing.List[builtins.str]],
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `cost-monitoring-construct-1.2.2/src/cost_monitoring_construct.egg-info/PKG-INFO` & `cost-monitoring-construct-1.2.3/src/cost_monitoring_construct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.2.2
+Version: 1.2.3
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

