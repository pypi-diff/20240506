# Comparing `tmp/django_oscar_odin-0.1.0b2.tar.gz` & `tmp/django_oscar_odin-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oscar_odin-0.1.0b2.tar", max compression
+gzip compressed data, was "django_oscar_odin-0.1.0b4.tar", max compression
```

## Comparing `django_oscar_odin-0.1.0b2.tar` & `django_oscar_odin-0.1.0b4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      547 2024-01-09 14:34:20.479673 django_oscar_odin-0.1.0b2/README.md
--rw-r--r--   0        0        0       65 2024-01-04 10:53:08.121289 django_oscar_odin-0.1.0b2/oscar_odin/__init__.py
--rw-r--r--   0        0        0      567 2024-03-12 09:26:15.033293 django_oscar_odin-0.1.0b2/oscar_odin/apps.py
--rw-r--r--   0        0        0      732 2024-03-12 09:26:33.551476 django_oscar_odin-0.1.0b2/oscar_odin/django_resolver.py
--rw-r--r--   0        0        0       46 2024-01-09 14:34:20.481029 django_oscar_odin-0.1.0b2/oscar_odin/exceptions.py
--rw-r--r--   0        0        0     1169 2024-03-12 09:26:33.552050 django_oscar_odin-0.1.0b2/oscar_odin/fields.py
--rw-r--r--   0        0        0     1081 2023-11-22 08:00:39.259519 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/address.json
--rw-r--r--   0        0        0      523 2023-11-22 08:00:39.259579 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/auth.json
--rw-r--r--   0        0        0   232255 2023-11-22 08:00:39.260362 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/catalogue.json
--rw-r--r--   0        0        0    18340 2024-01-09 14:34:20.481385 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/csv/products.csv
--rw-r--r--   0        0        0     1625 2023-11-22 08:00:39.260441 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/offer.json
--rw-r--r--   0        0        0     4165 2023-11-22 08:00:39.260506 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/order.json
--rw-r--r--   0        0        0      556 2023-11-22 08:00:39.260568 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/partner.json
--rw-r--r--   0        0        0    72609 2024-03-12 08:43:00.328897 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/address.json
--rw-r--r--   0        0        0      515 2024-03-12 08:43:00.329014 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/auth.json
--rw-r--r--   0        0        0     6315 2024-03-12 08:43:00.329125 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/catalogue.json
--rw-r--r--   0        0        0    12582 2024-03-12 08:43:00.329241 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/order.json
--rw-r--r--   0        0        0     2422 2024-03-12 08:43:00.329342 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/partner.json
--rw-r--r--   0        0        0      102 2023-11-22 08:00:39.260655 django_oscar_odin-0.1.0b2/oscar_odin/mappings/__init__.py
--rw-r--r--   0        0        0     1071 2024-03-12 09:26:33.552999 django_oscar_odin-0.1.0b2/oscar_odin/mappings/_common.py
--rw-r--r--   0        0        0     4115 2024-03-12 09:26:33.553628 django_oscar_odin-0.1.0b2/oscar_odin/mappings/_model_mapper.py
--rw-r--r--   0        0        0     1295 2024-03-12 09:26:33.554478 django_oscar_odin-0.1.0b2/oscar_odin/mappings/address.py
--rw-r--r--   0        0        0      375 2024-03-12 09:26:33.555000 django_oscar_odin-0.1.0b2/oscar_odin/mappings/auth.py
--rw-r--r--   0        0        0    14370 2024-05-02 11:37:32.133629 django_oscar_odin-0.1.0b2/oscar_odin/mappings/catalogue.py
--rw-r--r--   0        0        0     3106 2024-02-23 13:21:29.278952 django_oscar_odin-0.1.0b2/oscar_odin/mappings/constants.py
--rw-r--r--   0        0        0    20905 2024-05-02 11:37:32.133916 django_oscar_odin-0.1.0b2/oscar_odin/mappings/context.py
--rw-r--r--   0        0        0     8199 2024-03-12 09:26:33.555693 django_oscar_odin-0.1.0b2/oscar_odin/mappings/order.py
--rw-r--r--   0        0        0      182 2024-01-09 14:34:20.482517 django_oscar_odin-0.1.0b2/oscar_odin/resources/__init__.py
--rw-r--r--   0        0        0      250 2024-05-02 11:37:32.134160 django_oscar_odin-0.1.0b2/oscar_odin/resources/_base.py
--rw-r--r--   0        0        0     2942 2024-05-02 11:37:32.134385 django_oscar_odin-0.1.0b2/oscar_odin/resources/address.py
--rw-r--r--   0        0        0      368 2024-05-02 11:37:32.134571 django_oscar_odin-0.1.0b2/oscar_odin/resources/auth.py
--rw-r--r--   0        0        0     3145 2024-05-02 11:37:32.134767 django_oscar_odin-0.1.0b2/oscar_odin/resources/catalogue.py
--rw-r--r--   0        0        0     6630 2024-05-02 11:37:32.134990 django_oscar_odin-0.1.0b2/oscar_odin/resources/order.py
--rw-r--r--   0        0        0     2647 2024-05-02 11:37:32.135194 django_oscar_odin-0.1.0b2/oscar_odin/utils.py
--rw-r--r--   0        0        0     2284 2024-05-02 15:07:49.004932 django_oscar_odin-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 django_oscar_odin-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      547 2024-01-09 14:34:20.479673 django_oscar_odin-0.1.0b4/README.md
+-rw-r--r--   0        0        0       65 2024-01-04 10:53:08.121289 django_oscar_odin-0.1.0b4/oscar_odin/__init__.py
+-rw-r--r--   0        0        0      567 2024-03-12 09:26:15.033293 django_oscar_odin-0.1.0b4/oscar_odin/apps.py
+-rw-r--r--   0        0        0      732 2024-03-12 09:26:33.551476 django_oscar_odin-0.1.0b4/oscar_odin/django_resolver.py
+-rw-r--r--   0        0        0       46 2024-01-09 14:34:20.481029 django_oscar_odin-0.1.0b4/oscar_odin/exceptions.py
+-rw-r--r--   0        0        0     1169 2024-03-12 09:26:33.552050 django_oscar_odin-0.1.0b4/oscar_odin/fields.py
+-rw-r--r--   0        0        0     1081 2023-11-22 08:00:39.259519 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/address.json
+-rw-r--r--   0        0        0      523 2023-11-22 08:00:39.259579 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/auth.json
+-rw-r--r--   0        0        0   232255 2023-11-22 08:00:39.260362 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/catalogue.json
+-rw-r--r--   0        0        0    18340 2024-01-09 14:34:20.481385 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/csv/products.csv
+-rw-r--r--   0        0        0     1625 2023-11-22 08:00:39.260441 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/offer.json
+-rw-r--r--   0        0        0     4165 2023-11-22 08:00:39.260506 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/order.json
+-rw-r--r--   0        0        0      556 2023-11-22 08:00:39.260568 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/partner.json
+-rw-r--r--   0        0        0    72609 2024-03-12 08:43:00.328897 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/address.json
+-rw-r--r--   0        0        0      515 2024-03-12 08:43:00.329014 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/auth.json
+-rw-r--r--   0        0        0     6315 2024-03-12 08:43:00.329125 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/catalogue.json
+-rw-r--r--   0        0        0    12582 2024-03-12 08:43:00.329241 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/order.json
+-rw-r--r--   0        0        0     2422 2024-03-12 08:43:00.329342 django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/partner.json
+-rw-r--r--   0        0        0      102 2023-11-22 08:00:39.260655 django_oscar_odin-0.1.0b4/oscar_odin/mappings/__init__.py
+-rw-r--r--   0        0        0     1071 2024-03-12 09:26:33.552999 django_oscar_odin-0.1.0b4/oscar_odin/mappings/_common.py
+-rw-r--r--   0        0        0     4115 2024-03-12 09:26:33.553628 django_oscar_odin-0.1.0b4/oscar_odin/mappings/_model_mapper.py
+-rw-r--r--   0        0        0     1295 2024-03-12 09:26:33.554478 django_oscar_odin-0.1.0b4/oscar_odin/mappings/address.py
+-rw-r--r--   0        0        0      375 2024-03-12 09:26:33.555000 django_oscar_odin-0.1.0b4/oscar_odin/mappings/auth.py
+-rw-r--r--   0        0        0    14516 2024-05-05 13:55:25.464438 django_oscar_odin-0.1.0b4/oscar_odin/mappings/catalogue.py
+-rw-r--r--   0        0        0     3106 2024-02-23 13:21:29.278952 django_oscar_odin-0.1.0b4/oscar_odin/mappings/constants.py
+-rw-r--r--   0        0        0    20905 2024-05-02 11:37:32.133916 django_oscar_odin-0.1.0b4/oscar_odin/mappings/context.py
+-rw-r--r--   0        0        0     8199 2024-03-12 09:26:33.555693 django_oscar_odin-0.1.0b4/oscar_odin/mappings/order.py
+-rw-r--r--   0        0        0      182 2024-01-09 14:34:20.482517 django_oscar_odin-0.1.0b4/oscar_odin/resources/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-02 11:37:32.134160 django_oscar_odin-0.1.0b4/oscar_odin/resources/_base.py
+-rw-r--r--   0        0        0     2942 2024-05-02 11:37:32.134385 django_oscar_odin-0.1.0b4/oscar_odin/resources/address.py
+-rw-r--r--   0        0        0      368 2024-05-02 11:37:32.134571 django_oscar_odin-0.1.0b4/oscar_odin/resources/auth.py
+-rw-r--r--   0        0        0     3145 2024-05-02 11:37:32.134767 django_oscar_odin-0.1.0b4/oscar_odin/resources/catalogue.py
+-rw-r--r--   0        0        0     6630 2024-05-02 11:37:32.134990 django_oscar_odin-0.1.0b4/oscar_odin/resources/order.py
+-rw-r--r--   0        0        0     2647 2024-05-02 11:37:32.135194 django_oscar_odin-0.1.0b4/oscar_odin/utils.py
+-rw-r--r--   0        0        0     2284 2024-05-06 08:33:31.947108 django_oscar_odin-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 django_oscar_odin-0.1.0b4/PKG-INFO
```

### Comparing `django_oscar_odin-0.1.0b2/README.md` & `django_oscar_odin-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/apps.py` & `django_oscar_odin-0.1.0b4/oscar_odin/apps.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/django_resolver.py` & `django_oscar_odin-0.1.0b4/oscar_odin/django_resolver.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fields.py` & `django_oscar_odin-0.1.0b4/oscar_odin/fields.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/address.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/address.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/auth.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/auth.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/catalogue.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/catalogue.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/csv/products.csv` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/csv/products.csv`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/offer.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/offer.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/order.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/order.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/partner.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/partner.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/address.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/address.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/auth.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/auth.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/catalogue.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/catalogue.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/order.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/order.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/partner.json` & `django_oscar_odin-0.1.0b4/oscar_odin/fixtures/oscar_odin/test_discount/partner.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/_common.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/_common.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/_model_mapper.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/_model_mapper.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/address.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/address.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/catalogue.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/catalogue.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,35 +170,38 @@
         """Map product class."""
         item = self.source.get_product_class()
         return ProductClassToResource.apply(item, context=self.context)
 
     @staticmethod
     def _attribute_value_to_native_type(item):
         """Handle ProductAttributeValue to native type conversion."""
-        obj_type = item.attribute.type
-        if obj_type == item.attribute.OPTION:
-            return item.value.option
-
-        elif obj_type == item.attribute.MULTI_OPTION:
-            return item.value.values_list("option", flat=True)
-
-        elif obj_type == item.attribute.FILE:
-            return item.value.url
-
-        elif obj_type == item.attribute.IMAGE:
-            return item.value.url
-
-        elif obj_type == item.attribute.ENTITY:
-            if hasattr(item.value, "json"):
-                return item.value.json()
-            else:
-                return f"{repr(item.value)} has no json method, can not convert to json"
-
-        # return the value as stored on ProductAttributeValue in the correct type
-        return item.value
+        try:
+            obj_type = item.attribute.type
+            if obj_type == item.attribute.OPTION:
+                return item.value.option
+
+            elif obj_type == item.attribute.MULTI_OPTION:
+                return item.value.values_list("option", flat=True)
+
+            elif obj_type == item.attribute.FILE:
+                return item.value.url
+
+            elif obj_type == item.attribute.IMAGE:
+                return item.value.url
+
+            elif obj_type == item.attribute.ENTITY:
+                if hasattr(item.value, "json"):
+                    return item.value.json()
+                else:
+                    return f"{repr(item.value)} has no json method, can not convert to json"
+
+            # return the value as stored on ProductAttributeValue in the correct type
+            return item.value
+        except AttributeError:
+            return item.value_as_text
 
     @odin.assign_field
     def attributes(self) -> Dict[str, Any]:
         """Map attributes."""
         attribute_value_to_native_type = self._attribute_value_to_native_type
         return {
             item.attribute.code: attribute_value_to_native_type(item)
```

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/constants.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/constants.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/context.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/context.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/mappings/order.py` & `django_oscar_odin-0.1.0b4/oscar_odin/mappings/order.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/resources/address.py` & `django_oscar_odin-0.1.0b4/oscar_odin/resources/address.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/resources/catalogue.py` & `django_oscar_odin-0.1.0b4/oscar_odin/resources/catalogue.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/resources/order.py` & `django_oscar_odin-0.1.0b4/oscar_odin/resources/order.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/oscar_odin/utils.py` & `django_oscar_odin-0.1.0b4/oscar_odin/utils.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b2/pyproject.toml` & `django_oscar_odin-0.1.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-oscar-odin"
-version = "0.1.0b2"
+version = "0.1.0b4"
 description = "Odin Resources and mappings to Oscar models"
 authors = ["Tim Savage <tim@savage.company>"]
 maintainers = [
     "Viggo de Vries <viggo@highbiza.nl>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `django_oscar_odin-0.1.0b2/PKG-INFO` & `django_oscar_odin-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-odin
-Version: 0.1.0b2
+Version: 0.1.0b4
 Summary: Odin Resources and mappings to Oscar models
 Home-page: https://github.com/django-oscar/oscar-odin
 License: BSD-3-Clause
 Keywords: data-structure,validation,data-mapping
 Author: Tim Savage
 Author-email: tim@savage.company
 Maintainer: Viggo de Vries
```

