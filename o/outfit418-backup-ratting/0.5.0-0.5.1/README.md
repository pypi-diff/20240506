# Comparing `tmp/outfit418_backup_ratting-0.5.0.tar.gz` & `tmp/outfit418_backup_ratting-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outfit418_backup_ratting-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "outfit418_backup_ratting-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `outfit418_backup_ratting-0.5.0.tar` & `outfit418_backup_ratting-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     1539 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/LICENSE
--rwxr-xr-x   0        0        0      536 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/README.md
--rwxr-xr-x   0        0        0      143 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/__init__.py
--rwxr-xr-x   0        0        0      248 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/apps.py
--rwxr-xr-x   0        0        0     1206 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/auth_hooks.py
--rwxr-xr-x   0        0        0      108 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/forms.py
--rw-r--r--   0        0        0      361 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/management/commands/418_login_update.py
--rw-r--r--   0        0        0     1061 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/management/commands/418_ts_update.py
--rwxr-xr-x   0        0        0     1409 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/0001_initial.py
--rw-r--r--   0        0        0      660 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/0002_general.py
--rw-r--r--   0        0        0      900 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/0003_characterauditlogindata.py
--rwxr-xr-x   0        0        0        0 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/__init__.py
--rwxr-xr-x   0        0        0     1099 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/models.py
--rwxr-xr-x   0        0        0      152 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/provider.py
--rw-r--r--   0        0        0      374 2024-05-06 07:57:16.814092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/signals.py
--rwxr-xr-x   0        0        0     5456 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/tasks.py
--rw-r--r--   0        0        0     2377 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html
--rwxr-xr-x   0        0        0      486 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/index.html
--rw-r--r--   0        0        0        0 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/templatetags/__init__.py
--rw-r--r--   0        0        0      269 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/templatetags/outfit_tags.py
--rwxr-xr-x   0        0        0      247 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/urls.py
--rwxr-xr-x   0        0        0      851 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/utils.py
--rwxr-xr-x   0        0        0     3983 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/views.py
--rwxr-xr-x   0        0        0      868 2024-05-06 07:57:16.818092 outfit418_backup_ratting-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 outfit418_backup_ratting-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1539 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0      536 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/README.md
+-rwxr-xr-x   0        0        0      143 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/__init__.py
+-rwxr-xr-x   0        0        0      248 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/apps.py
+-rwxr-xr-x   0        0        0     1206 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/auth_hooks.py
+-rwxr-xr-x   0        0        0      108 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/forms.py
+-rw-r--r--   0        0        0      361 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/management/commands/418_login_update.py
+-rw-r--r--   0        0        0     1061 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/management/commands/418_ts_update.py
+-rwxr-xr-x   0        0        0     1409 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/0001_initial.py
+-rw-r--r--   0        0        0      660 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/0002_general.py
+-rw-r--r--   0        0        0      900 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/0003_characterauditlogindata.py
+-rwxr-xr-x   0        0        0        0 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/__init__.py
+-rwxr-xr-x   0        0        0     1099 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/models.py
+-rwxr-xr-x   0        0        0      152 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/provider.py
+-rw-r--r--   0        0        0      374 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/signals.py
+-rwxr-xr-x   0        0        0     5456 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/tasks.py
+-rw-r--r--   0        0        0     2377 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html
+-rwxr-xr-x   0        0        0      486 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/templates/outfit418_backup_ratting/index.html
+-rw-r--r--   0        0        0        0 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/templatetags/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/templatetags/outfit_tags.py
+-rwxr-xr-x   0        0        0      247 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/urls.py
+-rwxr-xr-x   0        0        0      851 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/utils.py
+-rwxr-xr-x   0        0        0     3983 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/views.py
+-rwxr-xr-x   0        0        0      868 2024-05-06 08:11:56.337505 outfit418_backup_ratting-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 outfit418_backup_ratting-0.5.1/PKG-INFO
```

### Comparing `outfit418_backup_ratting-0.5.0/LICENSE` & `outfit418_backup_ratting-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/README.md` & `outfit418_backup_ratting-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/auth_hooks.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/management/commands/418_ts_update.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/management/commands/418_ts_update.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/0001_initial.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/0002_general.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/0002_general.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/migrations/0003_characterauditlogindata.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/migrations/0003_characterauditlogindata.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/models.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/models.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/tasks.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/tasks.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     {% include "bundles/datatables-js-bs5.html" %}
     <script src="{% allianceauth_pve_static 'allianceauth_pve/js/spop.js' %}"></script>
     <script src="{% allianceauth_pve_static 'allianceauth_pve/js/copy_text.js' %}"></script>
 {% endblock extra_javascript %}
 
 {% block extra_script %}
     $(document).ready(function() {
+        $('[data-bs-toggle="tooltip"]').tooltip();
         $('.table').DataTable({
             "pageLength": 50
         });
-        $('[data-bs-toggle="tooltip"]').tooltip();
     });
 {% endblock extra_script %}
```

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/utils.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/utils.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/outfit418_backup_ratting/views.py` & `outfit418_backup_ratting-0.5.1/outfit418_backup_ratting/views.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/pyproject.toml` & `outfit418_backup_ratting-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.5.0/PKG-INFO` & `outfit418_backup_ratting-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outfit418_backup_ratting
-Version: 0.5.0
+Version: 0.5.1
 Summary: Backup for Outfit418 data
 Keywords: allianceauth,allianceauth_pve,outfit418,eveonline
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: allianceauth~=4.0
 Requires-Dist: allianceauth_pve~=1.10
```

