# Comparing `tmp/python_criteria-0.6.1.tar.gz` & `tmp/python_criteria-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_criteria-0.6.1.tar", last modified: Tue Apr 30 23:37:24 2024, max compression
+gzip compressed data, was "python_criteria-0.7.0.tar", last modified: Mon May  6 00:48:05 2024, max compression
```

## Comparing `python_criteria-0.6.1.tar` & `python_criteria-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.579294 python_criteria-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.575293 python_criteria-0.6.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.575293 python_criteria-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.575293 python_criteria-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.575293 python_criteria-0.6.1/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.579294 python_criteria-0.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 23:37:20.000000 python_criteria-0.6.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 23:37:20.000000 python_criteria-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 23:37:24.579294 python_criteria-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 23:37:20.000000 python_criteria-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-30 23:37:20.000000 python_criteria-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.579294 python_criteria-0.6.1/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-30 23:37:20.000000 python_criteria-0.6.1/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:37:24.579294 python_criteria-0.6.1/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 23:37:24.000000 python_criteria-0.6.1/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-30 23:37:24.000000 python_criteria-0.6.1/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:37:24.000000 python_criteria-0.6.1/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 23:37:24.000000 python_criteria-0.6.1/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:37:24.579294 python_criteria-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.296601 python_criteria-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 00:48:01.000000 python_criteria-0.7.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 00:48:01.000000 python_criteria-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 00:48:05.292601 python_criteria-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 00:48:01.000000 python_criteria-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 00:48:01.000000 python_criteria-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-06 00:48:01.000000 python_criteria-0.7.0/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:48:05.292601 python_criteria-0.7.0/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 00:48:05.000000 python_criteria-0.7.0/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 00:48:05.000000 python_criteria-0.7.0/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 00:48:05.000000 python_criteria-0.7.0/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 00:48:05.000000 python_criteria-0.7.0/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 00:48:05.296601 python_criteria-0.7.0/setup.cfg
```

### Comparing `python_criteria-0.6.1/.devcontainer/devcontainer.json` & `python_criteria-0.7.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/.devcontainer/docker-compose.yml` & `python_criteria-0.7.0/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/.github/workflows/python-publish.yml` & `python_criteria-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/.gitignore` & `python_criteria-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/.pylintrc` & `python_criteria-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/.vscode/tasks.json` & `python_criteria-0.7.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/LICENSE` & `python_criteria-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/pyproject.toml` & `python_criteria-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/python_criteria/clauses.py` & `python_criteria-0.7.0/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/python_criteria/entity.py` & `python_criteria-0.7.0/python_criteria/entity.py`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/python_criteria/filter.py` & `python_criteria-0.7.0/python_criteria/filter.py`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/python_criteria/label.py` & `python_criteria-0.7.0/python_criteria/label.py`

 * *Files identical despite different names*

### Comparing `python_criteria-0.6.1/python_criteria/sqlalchemy.py` & `python_criteria-0.7.0/python_criteria/sqlalchemy.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,58 +3,60 @@
 type SQLAlchemyTable = Any
 
 from .clauses import BooleanClause
 from .visitor import BaseVisitor
 
 
 class SQLAlchemyVisitor(BaseVisitor):
-    def visit_eq(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field) == comparison.value
+    def visit_eq(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field) == comparison.value
 
-    def visit_ne(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field) != comparison.value
+    def visit_ne(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field) != comparison.value
 
-    def visit_lt(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field) < comparison.value
+    def visit_lt(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field) < comparison.value
 
-    def visit_le(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field) <= comparison.value
+    def visit_le(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field) <= comparison.value
 
-    def visit_gt(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field) > comparison.value
+    def visit_gt(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field) > comparison.value
 
-    def visit_ge(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field) >= comparison.value
+    def visit_ge(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field) >= comparison.value
 
-    def visit_in(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field).in_(comparison.value)
+    def visit_in(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field).in_(comparison.value)
 
-    def visit_like(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field).ilike(
+    def visit_like(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
+        return self._attr(_object_mapping, comparison.field).ilike(
             comparison.value, escape="\\"
         )
 
-    def visit_not_like(self, _object: Any, comparison: BooleanClause):
-        return self._attr(_object, comparison.field).not_ilike(
+    def visit_not_like(
+        self, _object_mapping: dict[Any, Any], comparison: BooleanClause
+    ):
+        return self._attr(_object_mapping, comparison.field).not_ilike(
             comparison.value, escape="\\"
         )
 
-    def visit_or(self, _object: Any, comparisons: list[Any]):
+    def visit_or(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         _op = comparisons[0]
         for comp in comparisons[1:]:
             _op = _op | comp  #! <--- Caution: do not modify bitwise operator
 
         return _op
 
-    def visit_and(self, _object: Any, comparisons: list[Any]):
+    def visit_and(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         _op = comparisons[0]
         for comp in comparisons[1:]:
             _op = _op & comp  #! <--- Caution: do not modify bitwise operator
         return _op
 
-    def visit_xor(self, _object: Any, comparisons: list[Any]):
+    def visit_xor(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         return (
             comparisons[0] ^ comparisons[1]
         )  #! <--- Caution: do not modify bitwise operator
 
-    def visit_not(self, _object: Any, comparisons: list[Any]):
+    def visit_not(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         return ~comparisons[0]  #! <--- Caution: do not modify bitwise operator
```

### Comparing `python_criteria-0.6.1/python_criteria/visitor.py` & `python_criteria-0.7.0/python_criteria/visitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,25 +34,31 @@
             and hasattr(subclass, "visit_xor")
             and callable(subclass.visit_xor)
             and hasattr(subclass, "visit_not")
             and callable(subclass.visit_not)
             or NotImplemented
         )
 
-    def _attr(self, _object: Any, field: FilterableAttribute):
+    def _attr(self, _object_mapping: dict[Any, Any], field: FilterableAttribute):
+        _object = _object_mapping.get(field.parent_class)
+        if _object is None:
+            raise RuntimeError(
+                f"Invalid _object_mapping. Missing class '{field.parent_class.__name__}'."
+            )
+
         if not hasattr(_object, field.name):
             raise ValueError(
                 f"'{field.name}' is not a valid attribute of '{field.parent_class.__name__}'"
             )
 
         return getattr(_object, field.name)
 
     def visit(
         self,
-        _object: Any,
+        _object_mapping: dict[Any, Any],
         _filter: Filter,
     ):
         if not isinstance(_filter, Filter):
             raise ValueError("_filter argument should be an instance of Filter.")
 
         clause = _filter.clause
         if clause is None:
@@ -60,64 +66,66 @@
 
         name = clause.__class__.__name__.lower()
         method = getattr(self, "visit_" + name)
 
         if isinstance(clause, BooleanClauseList):
             comparisons = []
             for item in clause.clause_list:
-                comparisons.append(self.visit(_object, Filter(item)))
+                comparisons.append(self.visit(_object_mapping, Filter(item)))
 
-            return method(_object, comparisons)
+            return method(_object_mapping, comparisons)
 
-        return method(_object, clause)
+        return method(_object_mapping, clause)
 
     @abc.abstractmethod
-    def visit_eq(self, _object: Any, comparison: BooleanClause):
+    def visit_eq(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_ne(self, _object: Any, comparison: BooleanClause):
+    def visit_ne(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_lt(self, _object: Any, comparison: BooleanClause):
+    def visit_lt(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_le(self, _object: Any, comparison: BooleanClause):
+    def visit_le(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_gt(self, _object: Any, comparison: BooleanClause):
+    def visit_gt(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_ge(self, _object: Any, comparison: BooleanClause):
+    def visit_ge(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_in(self, _object: Any, comparison: BooleanClause):
+    def visit_in(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_like(self, _object: Any, comparison: BooleanClause):
+    def visit_like(self, _object_mapping: dict[Any, Any], comparison: BooleanClause):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_not_like(self, _object: Any, comparison: BooleanClause):
+    def visit_not_like(
+        self, _object_mapping: dict[Any, Any], comparison: BooleanClause
+    ):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_or(self, _object: Any, comparisons: list[Any]):
+    def visit_or(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_and(self, _object: Any, comparisons: list[Any]):
+    def visit_and(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_xor(self, _object: Any, comparisons: list[Any]):
+    def visit_xor(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def visit_not(self, _object: Any, comparisons: list[Any]):
+    def visit_not(self, _object_mapping: dict[Any, Any], comparisons: list[Any]):
         raise NotImplementedError
```

### Comparing `python_criteria-0.6.1/python_criteria.egg-info/SOURCES.txt` & `python_criteria-0.7.0/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

