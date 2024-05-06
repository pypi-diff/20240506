# Comparing `tmp/flake8-pydantic-0.3.0.tar.gz` & `tmp/flake8_pydantic-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-pydantic-0.3.0.tar", last modified: Thu Mar 14 20:24:35 2024, max compression
+gzip compressed data, was "flake8_pydantic-0.3.1.tar", last modified: Mon May  6 16:40:30 2024, max compression
```

## Comparing `flake8-pydantic-0.3.0.tar` & `flake8_pydantic-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-14 20:24:35.870698 flake8-pydantic-0.3.0/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1066 2024-02-22 19:15:11.000000 flake8-pydantic-0.3.0/LICENSE
--rw-r--r--   0 victorien  (1000) victorien  (1000)     7420 2024-03-14 20:24:35.870698 flake8-pydantic-0.3.0/PKG-INFO
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     4865 2024-02-24 17:10:21.000000 flake8-pydantic-0.3.0/README.md
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2069 2024-03-14 20:23:37.000000 flake8-pydantic-0.3.0/pyproject.toml
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       38 2024-03-14 20:24:35.870698 flake8-pydantic-0.3.0/setup.cfg
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-14 20:24:35.866698 flake8-pydantic-0.3.0/src/
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-14 20:24:35.866698 flake8-pydantic-0.3.0/src/flake8_pydantic/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       50 2024-02-21 19:47:48.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      172 2024-02-24 15:23:26.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/_compat.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     5437 2024-02-24 17:10:21.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/_utils.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1270 2024-03-14 20:23:37.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/errors.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      542 2024-02-24 17:10:21.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/plugin.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-02-21 19:39:46.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/py.typed
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     5407 2024-03-14 20:17:55.000000 flake8-pydantic-0.3.0/src/flake8_pydantic/visitor.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-14 20:24:35.870698 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/
--rw-r--r--   0 victorien  (1000) victorien  (1000)     7420 2024-03-14 20:24:35.000000 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      564 2024-03-14 20:24:35.000000 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        1 2024-03-14 20:24:35.000000 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       48 2024-03-14 20:24:35.000000 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/entry_points.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       60 2024-03-14 20:24:35.000000 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/requires.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       16 2024-03-14 20:24:35.000000 flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-14 20:24:35.870698 flake8-pydantic-0.3.0/tests/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      785 2024-02-23 18:24:47.000000 flake8-pydantic-0.3.0/tests/test_is_dataclass.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2425 2024-02-23 18:24:52.000000 flake8-pydantic-0.3.0/tests/test_is_pydantic_model.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-06 16:40:30.897005 flake8_pydantic-0.3.1/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1066 2024-02-22 19:15:11.000000 flake8_pydantic-0.3.1/LICENSE
+-rw-r--r--   0 victorien  (1000) victorien  (1000)     7420 2024-05-06 16:40:30.897005 flake8_pydantic-0.3.1/PKG-INFO
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4865 2024-02-24 17:10:21.000000 flake8_pydantic-0.3.1/README.md
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2069 2024-05-06 16:39:34.000000 flake8_pydantic-0.3.1/pyproject.toml
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       38 2024-05-06 16:40:30.897005 flake8_pydantic-0.3.1/setup.cfg
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-06 16:40:30.893005 flake8_pydantic-0.3.1/src/
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-06 16:40:30.893005 flake8_pydantic-0.3.1/src/flake8_pydantic/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       50 2024-02-21 19:47:48.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      172 2024-02-24 15:23:26.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/_compat.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     6486 2024-05-06 16:33:58.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/_utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1270 2024-03-14 20:23:37.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/errors.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      542 2024-02-24 17:10:21.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/plugin.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-02-21 19:39:46.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/py.typed
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     5471 2024-05-06 16:31:38.000000 flake8_pydantic-0.3.1/src/flake8_pydantic/visitor.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-06 16:40:30.897005 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/
+-rw-r--r--   0 victorien  (1000) victorien  (1000)     7420 2024-05-06 16:40:30.000000 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      564 2024-05-06 16:40:30.000000 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        1 2024-05-06 16:40:30.000000 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       48 2024-05-06 16:40:30.000000 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/entry_points.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       60 2024-05-06 16:40:30.000000 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       16 2024-05-06 16:40:30.000000 flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-06 16:40:30.897005 flake8_pydantic-0.3.1/tests/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      785 2024-02-23 18:24:47.000000 flake8_pydantic-0.3.1/tests/test_is_dataclass.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3130 2024-05-06 16:33:58.000000 flake8_pydantic-0.3.1/tests/test_is_pydantic_model.py
```

### Comparing `flake8-pydantic-0.3.0/LICENSE` & `flake8_pydantic-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-0.3.0/PKG-INFO` & `flake8_pydantic-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pydantic
-Version: 0.3.0
+Version: 0.3.1
 Summary: A flake8 plugin to check Pydantic related code.
 Author-email: Victorien <contact@vctrn.dev>
 License: MIT License
         
         Copyright (c) 2023 Victorien
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `flake8-pydantic-0.3.0/README.md` & `flake8_pydantic-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-0.3.0/pyproject.toml` & `flake8_pydantic-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flake8-pydantic"
-version = "0.3.0"
+version = "0.3.1"
 description = "A flake8 plugin to check Pydantic related code."
 readme = "README.md"
 authors = [
     {name = "Victorien", email = "contact@vctrn.dev"}
 ]
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `flake8-pydantic-0.3.0/src/flake8_pydantic/_utils.py` & `flake8_pydantic-0.3.1/src/flake8_pydantic/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             names.add(dec.id)
         elif isinstance(dec, ast.Attribute):
             names.add(dec.attr)
 
     return names
 
 
-def _has_pydantic_model_base(node: ast.ClassDef, include_root_model: bool) -> bool:
+def _has_pydantic_model_base(node: ast.ClassDef, *, include_root_model: bool) -> bool:
     model_class_names = {"BaseModel"}
     if include_root_model:
         model_class_names.add("RootModel")
 
     for base in node.bases:
         if isinstance(base, ast.Name) and base.id in model_class_names:
             return True
@@ -38,23 +38,63 @@
             t.id == "model_config" for t in stmt.targets if isinstance(t, ast.Name)
         ):
             # model_config = ...
             return True
     return False
 
 
+PYDANTIC_FIELD_ARGUMENTS = {
+    "default",
+    "default_factory",
+    "alias",
+    "alias_priority",
+    "validation_alias",
+    "title",
+    "description",
+    "examples",
+    "exclude",
+    "discriminator",
+    "json_schema_extra",
+    "frozen",
+    "validate_default",
+    "repr",
+    "init",
+    "init_var",
+    "kw_only",
+    "pattern",
+    "strict",
+    "gt",
+    "ge",
+    "lt",
+    "le",
+    "multiple_of",
+    "allow_inf_nan",
+    "max_digits",
+    "decimal_places",
+    "min_length",
+    "max_length",
+    "union_mode",
+}
+
+
 def _has_field_function(node: ast.ClassDef) -> bool:
     for stmt in node.body:
-        if isinstance(stmt, (ast.Assign, ast.AnnAssign)) and isinstance(stmt.value, ast.Call):
-            if isinstance(stmt.value.func, ast.Name) and stmt.value.func.id == "Field":
-                # f = Field(...)
-                return True
-            if isinstance(stmt.value.func, ast.Attribute) and stmt.value.func.attr == "Field":
-                # f = pydantic.Field(...)
-                return True
+        if (
+            isinstance(stmt, (ast.Assign, ast.AnnAssign))
+            and isinstance(stmt.value, ast.Call)
+            and (
+                (isinstance(stmt.value.func, ast.Name) and stmt.value.func.id == "Field")  # f = Field(...)
+                or (
+                    isinstance(stmt.value.func, ast.Attribute) and stmt.value.func.attr == "Field"
+                )  # f = pydantic.Field(...)
+            )
+            and all(kw.arg in PYDANTIC_FIELD_ARGUMENTS for kw in stmt.value.keywords if kw.arg is not None)
+        ):
+            return True
+
     return False
 
 
 def _has_annotated_field(node: ast.ClassDef) -> bool:
     for stmt in node.body:
         if isinstance(stmt, ast.AnnAssign) and isinstance(stmt.annotation, ast.Subscript):
             if isinstance(stmt.annotation.value, ast.Name) and stmt.annotation.value.id == "Annotated":
@@ -80,37 +120,53 @@
         if isinstance(stmt, ast.FunctionDef):
             decorator_names = get_decorator_names(stmt.decorator_list)
             if PYDANTIC_DECORATORS & decorator_names:
                 return True
     return False
 
 
+PYDANTIC_METHODS = {
+    "model_construct",
+    "model_copy",
+    "model_dump",
+    "model_dump_json",
+    "model_json_schema",
+    "model_parametrized_name",
+    "model_rebuild",
+    "model_validate",
+    "model_validate_json",
+    "model_validate_strings",
+}
+
+
 def _has_pydantic_method(node: ast.ClassDef) -> bool:
     for stmt in node.body:
-        if isinstance(stmt, ast.FunctionDef) and stmt.name.startswith(("model_", "__pydantic_")):
+        if isinstance(stmt, ast.FunctionDef) and (
+            stmt.name.startswith(("__pydantic_", "__get_pydantic_")) or stmt.name in PYDANTIC_METHODS
+        ):
             return True
     return False
 
 
-def is_pydantic_model(node: ast.ClassDef, include_root_model: bool = True) -> bool:
+def is_pydantic_model(node: ast.ClassDef, *, include_root_model: bool = True) -> bool:
     """Determine if a class definition is a Pydantic model.
 
     Multiple heuristics are use to determine if this is the case:
     - The class inherits from `BaseModel` (or `RootModel` if `include_root_model` is `True`).
     - The class has a `model_config` attribute set.
     - The class has a field defined with the `Field` function.
     - The class has a field making use of `Annotated`.
     - The class makes use of Pydantic decorators, such as `computed_field` or `model_validator`.
     - The class overrides any of the Pydantic methods, such as `model_dump`.
     """
     if not node.bases:
         return False
 
     return (
-        _has_pydantic_model_base(node, include_root_model)
+        _has_pydantic_model_base(node, include_root_model=include_root_model)
         or _has_model_config(node)
         or _has_field_function(node)
         or _has_annotated_field(node)
         or _has_pydantic_decorator(node)
         or _has_pydantic_method(node)
     )
```

### Comparing `flake8-pydantic-0.3.0/src/flake8_pydantic/errors.py` & `flake8_pydantic-0.3.1/src/flake8_pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-0.3.0/src/flake8_pydantic/plugin.py` & `flake8_pydantic-0.3.1/src/flake8_pydantic/plugin.py`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-0.3.0/src/flake8_pydantic/visitor.py` & `flake8_pydantic-0.3.1/src/flake8_pydantic/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,17 @@
         else:
             self.class_stack.append("other_class")
 
     def leave_class(self) -> None:
         self.class_stack.pop()
 
     @property
-    def current_class(self) -> ClassType:
+    def current_class(self) -> ClassType | None:
+        if not self.class_stack:
+            return None
         return self.class_stack[-1]
 
     def _check_pyd_001(self, node: ast.AnnAssign) -> None:
         if (
             self.current_class in {"pydantic_model", "dataclass"}
             and isinstance(node.value, ast.Call)
             and is_function(node.value, "Field")
```

### Comparing `flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/PKG-INFO` & `flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pydantic
-Version: 0.3.0
+Version: 0.3.1
 Summary: A flake8 plugin to check Pydantic related code.
 Author-email: Victorien <contact@vctrn.dev>
 License: MIT License
         
         Copyright (c) 2023 Victorien
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `flake8-pydantic-0.3.0/src/flake8_pydantic.egg-info/SOURCES.txt` & `flake8_pydantic-0.3.1/src/flake8_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-0.3.0/tests/test_is_dataclass.py` & `flake8_pydantic-0.3.1/tests/test_is_dataclass.py`

 * *Files identical despite different names*

### Comparing `flake8-pydantic-0.3.0/tests/test_is_pydantic_model.py` & `flake8_pydantic-0.3.1/tests/test_is_pydantic_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,32 +31,42 @@
 HAS_MODEL_CONFIG = """
 class SubModel(ParentModel):
     model_config = {}
 """
 
 HAS_FIELD_FUNCTION_1 = """
 class SubModel(ParentModel):
-    a = Field()
+    a = Field(title="A")
 """
 
 HAS_FIELD_FUNCTION_2 = """
 class SubModel(ParentModel):
-    a: int = Field()
+    a: int = Field(gt=1)
 """
 
 HAS_FIELD_FUNCTION_3 = """
 class SubModel(ParentModel):
-    a = pydantic.Field()
+    a = pydantic.Field(alias="b")
 """
 
 HAS_FIELD_FUNCTION_4 = """
 class SubModel(ParentModel):
+    a: int = pydantic.Field(repr=True)
+"""
+
+HAS_FIELD_FUNCTION_5 = """
+class SubModel(ParentModel):
     a: int = pydantic.Field()
 """
 
+HAS_FIELD_FUNCTION_6 = """
+class SubModel(ParentModel):
+    a: int = pydantic.Field(1)
+"""
+
 USES_ANNOTATED_1 = """
 class SubModel(ParentModel):
     a: Annotated[int, ""]
 """
 
 USES_ANNOTATED_2 = """
 class SubModel(ParentModel):
@@ -82,38 +92,58 @@
 """
 
 HAS_PYDANTIC_METHOD_2 = """
 class SubModel(ParentModel):
     def __pydantic_some_method__(self): pass
 """
 
+HAS_PYDANTIC_METHOD_3 = """
+class SubModel(ParentModel):
+    def __get_pydantic_core_schema__(self): pass
+"""
+
 # Negative cases:
 NO_BASES = """
 class Model:
     a = Field()
 """
 
+UNRELATED_FIELD_ARG = """
+class SubModel(ParentModel):
+    a: int = Field(some_arg=1)
+"""
+
+UNRELATED_MODEL_METHOD = """
+class SubModel(ParentModel):
+    def model_unrelated(): pass
+"""
+
 
 @pytest.mark.parametrize(
     ["source", "expected"],
     [
         (SUBCLASSES_BASE_MODEL_1, True),
         (SUBCLASSES_BASE_MODEL_2, True),
         (SUBCLASSES_ROOT_MODEL, True),
         (HAS_ANNOTATED_MODEL_CONFIG, True),
         (HAS_MODEL_CONFIG, True),
         (HAS_FIELD_FUNCTION_1, True),
         (HAS_FIELD_FUNCTION_2, True),
         (HAS_FIELD_FUNCTION_3, True),
         (HAS_FIELD_FUNCTION_4, True),
+        (HAS_FIELD_FUNCTION_5, True),
+        (HAS_FIELD_FUNCTION_6, True),
         (USES_ANNOTATED_1, True),
         (USES_ANNOTATED_2, True),
         (HAS_PYDANTIC_DECORATOR_1, True),
         (HAS_PYDANTIC_DECORATOR_2, True),
         (HAS_PYDANTIC_METHOD_1, True),
         (HAS_PYDANTIC_METHOD_2, True),
+        (HAS_PYDANTIC_METHOD_3, True),
         (NO_BASES, False),
+        (UNRELATED_FIELD_ARG, False),
+        (UNRELATED_MODEL_METHOD, False),
     ],
 )
 def test_is_pydantic_model(source: str, expected: bool) -> None:
     class_def = cast(ast.ClassDef, ast.parse(source).body[0])
     assert is_pydantic_model(class_def) == expected
```

