# Comparing `tmp/drf_redesign-0.3.5.tar.gz` & `tmp/drf_redesign-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_redesign-0.3.5.tar", max compression
+gzip compressed data, was "drf_redesign-0.3.6.tar", max compression
```

## Comparing `drf_redesign-0.3.5.tar` & `drf_redesign-0.3.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-05-04 07:27:50.221553 drf_redesign-0.3.5/LICENSE
--rw-r--r--   0        0        0     3571 2024-05-04 07:27:50.221553 drf_redesign-0.3.5/README.md
--rw-r--r--   0        0        0       91 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/__init__.py
--rw-r--r--   0        0        0      235 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/apps.py
--rw-r--r--   0        0        0    27873 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1056 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      585 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1398 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1433 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0     1006 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-05-04 07:27:50.225553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1487 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1054 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     5226 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     2065 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      296 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1461 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1474 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templatetags/__init__.py
--rw-r--r--   0        0        0     1682 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/drf_redesign/templatetags/rest_framework_redesign.py
--rw-r--r--   0        0        0      576 2024-05-04 07:27:50.229553 drf_redesign-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 drf_redesign-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3571 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/README.md
+-rw-r--r--   0        0        0       91 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/apps.py
+-rw-r--r--   0        0        0    27876 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1056 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      585 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1398 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1433 2024-05-06 10:14:47.801159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0     1006 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1487 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1054 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     5226 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     2051 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      296 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1461 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1474 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templatetags/__init__.py
+-rw-r--r--   0        0        0     1682 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/drf_redesign/templatetags/rest_framework_redesign.py
+-rw-r--r--   0        0        0      576 2024-05-06 10:14:47.805159 drf_redesign-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 drf_redesign-0.3.6/PKG-INFO
```

### Comparing `drf_redesign-0.3.5/LICENSE` & `drf_redesign-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/README.md` & `drf_redesign-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/api.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
               </div>
             </div>
           </div>
         {% endif %}
 
         {% if extra_actions %}
           <div class="dropdown">
-            <button class="btn btn-info w-100 shadow-sm" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
+            <button class="btn btn-warning w-100 shadow-sm" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
               <span class="d-flex align-items-center justify-content-center gap-4">
                 {% translate "Extra Actions" %}
                 <i class="bi bi-chevron-down"></i>
               </span>
             </button>
             <ul class="dropdown-menu rounded-4 shadow-sm pb-3 w-100" aria-labelledby="extra-actions-menu">
```

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/filters/base.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/filters/ordering.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/filters/search.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/checkbox.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/input.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/radio.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/select.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/select_multiple.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/horizontal/textarea.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/checkbox.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/input.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/radio.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/select.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/select_multiple.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/inline/textarea.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/login.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/pagination/numbers.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 {% load i18n %}
 
 <nav aria-label="Pagination" class="d-flex align-items-center">
-  <ol class="pagination pagination-lg flex-wrap gap-4 mb-0">
+  <ol class="pagination flex-wrap gap-4 mb-0">
     {% if previous_url %}
       <li class="page-item">
-        <a class="page-link rounded-4 shadow-sm d-flex align-item-center gap-4" href="{{ previous_url }}" aria-label="Previous">
+        <a class="page-link rounded-3 shadow-sm d-flex align-item-center gap-4" href="{{ previous_url }}" aria-label="Previous">
           <i class="bi bi-chevron-left"></i>
           {% translate 'Prev' %}
         </a>
       </li>
     {% else %}
       <li class="page-item disabled">
-        <a class="page-link rounded-4 shadow-sm d-flex align-item-center gap-4" href="#" aria-label="Previous">
+        <a class="page-link rounded-3 shadow-sm d-flex align-item-center gap-4" href="#" aria-label="Previous">
           <i class="bi bi-chevron-left"></i>
           {% translate 'Prev' %}
         </a>
       </li>
     {% endif %}
 
     {% for page_link in page_links %}
       {% if page_link.is_break %}
         <li class="page-item disabled">
-          <a class="page-link rounded-4 shadow-sm" href="#">
+          <a class="page-link rounded-3 shadow-sm" href="#">
             <span aria-hidden="true">&hellip;</span>
           </a>
         </li>
       {% else %}
         {% if page_link.is_active %}
           <li class="page-item active" aria-current="page">
-            <a class="page-link rounded-4 shadow-sm" href="{{ page_link.url }}">
+            <a class="page-link rounded-3 shadow-sm" href="{{ page_link.url }}">
               {{ page_link.number }}
             </a>
           </li>
         {% else %}
           <li class="page-item">
-            <a class="page-link rounded-4 shadow-sm" href="{{ page_link.url }}">
+            <a class="page-link rounded-3 shadow-sm" href="{{ page_link.url }}">
               {{ page_link.number }}
             </a>
           </li>
         {% endif %}
       {% endif %}
     {% endfor %}
 
     {% if next_url %}
       <li class="page-item">
-        <a class="page-link rounded-4 shadow-sm d-flex align-item-center gap-4" href="{{ next_url }}" aria-label="Next">
+        <a class="page-link rounded-3 shadow-sm d-flex align-item-center gap-4" href="{{ next_url }}" aria-label="Next">
           {% translate 'Next' %}
           <i class="bi bi-chevron-right"></i>
         </a>
       </li>
     {% else %}
       <li class="page-item disabled">
-        <a class="page-link rounded-4 shadow-sm d-flex align-item-center gap-4" href="#" aria-label="Next">
+        <a class="page-link rounded-3 shadow-sm d-flex align-item-center gap-4" href="#" aria-label="Next">
           {% translate 'Next' %}
           <i class="bi bi-chevron-right"></i>
         </a>
       </li>
     {% endif %}
   </ol>
 </nav>
```

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/pagination/previous_and_next.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/checkbox.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/input.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/radio.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/select.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/select_multiple.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templates/rest_framework/vertical/textarea.html` & `drf_redesign-0.3.6/drf_redesign/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/drf_redesign/templatetags/rest_framework_redesign.py` & `drf_redesign-0.3.6/drf_redesign/templatetags/rest_framework_redesign.py`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.5/pyproject.toml` & `drf_redesign-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-redesign"
-version = "0.3.5"
+version = "0.3.6"
 description = "Redesign of the browse-able api of Django REST Framework with Bootstrap 5"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_redesign"}]
 homepage = "https://github.com/youzarsiph/drf-redesign/"
 repository = "https://github.com/youzarsiph/drf-redesign/"
```

### Comparing `drf_redesign-0.3.5/PKG-INFO` & `drf_redesign-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-redesign
-Version: 0.3.5
+Version: 0.3.6
 Summary: Redesign of the browse-able api of Django REST Framework with Bootstrap 5
 Home-page: https://github.com/youzarsiph/drf-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

