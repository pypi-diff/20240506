# Comparing `tmp/pragmatic_business_rules-0.4.0.tar.gz` & `tmp/pragmatic_business_rules-0.4.1.tar.gz`

## Comparing `pragmatic_business_rules-0.4.0.tar` & `pragmatic_business_rules-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/dev_requirements.txt
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/dprint.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/mypy.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/requirements.txt
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/examples/long.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/__init__.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/action.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/asserts.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/condition.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/main.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/types.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_action.py
--rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_condition.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_main.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_validators.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/LICENSE
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/dev_requirements.txt
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/dprint.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/mypy.ini
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/requirements.txt
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/examples/long.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/__init__.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/action.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/asserts.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/condition.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/main.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/types.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_action.py
+-rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_condition.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_main.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_validators.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/LICENSE
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/PKG-INFO
```

### Comparing `pragmatic_business_rules-0.4.0/examples/long.json` & `pragmatic_business_rules-0.4.1/examples/long.json`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/action.py` & `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/action.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/asserts.py` & `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/asserts.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/condition.py` & `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from .types import Condition, Conditional, number
 from decimal import Decimal
 from typing import TypedDict, cast, Literal, Optional, Union
 
 class ConditionValues(TypedDict):
 	label_1: Optional[str]
 	label_2: Optional[str]
-	value_1: Union[None| number | str]
-	value_2: Union[None| number | str]
+	value_1: Union[None, number, str]
+	value_2: Union[None, number, str]
 
 def __get_condition_values(
 	condition: Condition,
 	constants: dict[str, Union[number, str]],
 	variables: dict[str, Union[number, str]],
 ) -> ConditionValues:
 	categories = list(filter(lambda k: k != "operator", condition.keys()))
@@ -21,15 +21,15 @@
 	elif len(categories) != 2:
 		raise Exception(f'A condition must be composed by two categories of values, {"only " if len(categories) == 1 else ""}"{", ".join(sorted(categories))}" found')
 	
 	values: dict = {}
 	i = 1
 	for category in categories:
 		label: Optional[str] = None
-		value: Union[None | number | str]
+		value: Union[None, number, str]
 
 		if category == "constant":
 			constant_name = cast(str, condition.get(category))
 			if constant_name not in constants:
 				raise Exception(f"Constant '{constant_name}' not defined")
 
 			label = constant_name
```

### Comparing `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/main.py` & `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/main.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/types.py` & `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/types.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/validators.py` & `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/validators.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/tests/test_action.py` & `pragmatic_business_rules-0.4.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/tests/test_condition.py` & `pragmatic_business_rules-0.4.1/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/tests/test_main.py` & `pragmatic_business_rules-0.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/tests/test_validators.py` & `pragmatic_business_rules-0.4.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/LICENSE` & `pragmatic_business_rules-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.0/pyproject.toml` & `pragmatic_business_rules-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pragmatic-business-rules"
-version = "0.4.0"
+version = "0.4.1"
 authors = [{ name = "Soremwar", email = "stephenguerrero43@gmail.com" }]
 description = "Pragmatic business rules"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
```

### Comparing `pragmatic_business_rules-0.4.0/PKG-INFO` & `pragmatic_business_rules-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pragmatic-business-rules
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pragmatic business rules
 Project-URL: Homepage, https://github.com/Soremwar/pragmatic_business_rules
 Project-URL: Issues, https://github.com/Soremwar/pragmatic_business_rules/issues
 Author-email: Soremwar <stephenguerrero43@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

