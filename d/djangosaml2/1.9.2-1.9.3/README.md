# Comparing `tmp/djangosaml2-1.9.2.tar.gz` & `tmp/djangosaml2-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml2-1.9.2.tar", last modified: Thu Feb 15 17:42:35 2024, max compression
+gzip compressed data, was "djangosaml2-1.9.3.tar", last modified: Mon May  6 13:49:52 2024, max compression
```

## Comparing `djangosaml2-1.9.2.tar` & `djangosaml2-1.9.3.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/CHANGES
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.094365 djangosaml2-1.9.2/djangosaml2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.090365 djangosaml2-1.9.2/djangosaml2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.098364 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/auth_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/login_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/logout_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/wayf.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.098364 djangosaml2-1.9.2/djangosaml2/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/templatetags/idplist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/djangosaml2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    43948 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/djangosaml2/tests/attribute-maps/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/attribute-maps/django_saml_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    11106 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/attribute-maps/saml_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/idpcert.csr
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/idpcert.key
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/idpcert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/mycert.csr
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/mycert.key
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/mycert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/remote_metadata.xml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/sp_metadata.xml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/spcert.csr
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/spcert.key
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/spcert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35400 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/djangosaml2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/djangosaml2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-02-15 17:42:35.000000 djangosaml2-1.9.2/djangosaml2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-15 17:42:35.000000 djangosaml2-1.9.2/djangosaml2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 17:42:35.000000 djangosaml2-1.9.2/djangosaml2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 17:42:34.000000 djangosaml2-1.9.2/djangosaml2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-15 17:42:35.000000 djangosaml2-1.9.2/djangosaml2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-15 17:42:35.000000 djangosaml2-1.9.2/djangosaml2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.090365 djangosaml2-1.9.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.094365 djangosaml2-1.9.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.094365 djangosaml2-1.9.2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/docs/source/_templates/pplnx_template/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/docs/source/_templates/pplnx_template/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/docs/source/_templates/pplnx_template/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-15 17:42:35.102364 djangosaml2-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-15 17:42:26.000000 djangosaml2-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.429602 djangosaml2-1.9.3/djangosaml2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.425602 djangosaml2-1.9.3/djangosaml2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.433602 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/login_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/post_binding_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/wayf.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.433602 djangosaml2-1.9.3/djangosaml2/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/templatetags/idplist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/djangosaml2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    43948 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/djangosaml2/tests/attribute-maps/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/attribute-maps/django_saml_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11106 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/attribute-maps/saml_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/idpcert.csr
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/idpcert.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/idpcert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/mycert.csr
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/mycert.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/mycert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/remote_metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/sp_metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/spcert.csr
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/spcert.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/spcert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34821 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/djangosaml2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/djangosaml2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-06 13:49:52.000000 djangosaml2-1.9.3/djangosaml2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-06 13:49:52.000000 djangosaml2-1.9.3/djangosaml2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:49:52.000000 djangosaml2-1.9.3/djangosaml2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:49:52.000000 djangosaml2-1.9.3/djangosaml2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 13:49:52.000000 djangosaml2-1.9.3/djangosaml2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 13:49:52.000000 djangosaml2-1.9.3/djangosaml2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.425602 djangosaml2-1.9.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.425602 djangosaml2-1.9.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.425602 djangosaml2-1.9.3/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/docs/source/_templates/pplnx_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/docs/source/_templates/pplnx_template/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/docs/source/_templates/pplnx_template/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 13:49:52.437602 djangosaml2-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-06 13:49:46.000000 djangosaml2-1.9.3/setup.py
```

### Comparing `djangosaml2-1.9.2/CHANGES` & `djangosaml2-1.9.3/CHANGES`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/COPYING` & `djangosaml2-1.9.3/COPYING`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/PKG-INFO` & `djangosaml2-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.9.2
+Version: 1.9.3
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.9.2/README.md` & `djangosaml2-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/backends.py` & `djangosaml2-1.9.3/djangosaml2/backends.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/cache.py` & `djangosaml2-1.9.3/djangosaml2/cache.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/conf.py` & `djangosaml2-1.9.3/djangosaml2/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/middleware.py` & `djangosaml2-1.9.3/djangosaml2/middleware.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/overrides.py` & `djangosaml2-1.9.3/djangosaml2/overrides.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/signals.py` & `djangosaml2-1.9.3/djangosaml2/signals.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.9.3/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/templatetags/idplist.py` & `djangosaml2-1.9.3/djangosaml2/templatetags/idplist.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/__init__.py` & `djangosaml2-1.9.3/djangosaml2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/attribute-maps/django_saml_uri.py` & `djangosaml2-1.9.3/djangosaml2/tests/attribute-maps/django_saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/attribute-maps/saml_uri.py` & `djangosaml2-1.9.3/djangosaml2/tests/attribute-maps/saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/auth_response.py` & `djangosaml2-1.9.3/djangosaml2/tests/auth_response.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/conf.py` & `djangosaml2-1.9.3/djangosaml2/tests/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.9.3/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/idpcert.key` & `djangosaml2-1.9.3/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.9.3/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/mycert.csr` & `djangosaml2-1.9.3/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/mycert.key` & `djangosaml2-1.9.3/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/mycert.pem` & `djangosaml2-1.9.3/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.9.3/djangosaml2/tests/remote_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.9.3/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.9.3/djangosaml2/tests/sp_metadata.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/spcert.csr` & `djangosaml2-1.9.3/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/spcert.key` & `djangosaml2-1.9.3/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/tests/spcert.pem` & `djangosaml2-1.9.3/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/urls.py` & `djangosaml2-1.9.3/djangosaml2/urls.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/djangosaml2/utils.py` & `djangosaml2-1.9.3/djangosaml2/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import base64
 import logging
 import re
 import urllib
 import zlib
+from functools import lru_cache, wraps
 from typing import Optional
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import resolve_url
 from django.urls import NoReverseMatch
 from django.utils.http import url_has_allowed_host_and_scheme
+from django.utils.module_loading import import_string
 
 from saml2.config import SPConfig
 from saml2.mdstore import MetaDataMDX
 from saml2.s_utils import UnknownSystemEntity
 
 logger = logging.getLogger(__name__)
 
@@ -202,7 +204,59 @@
         return HttpResponse(content)
 
     else:
         logger.warning(
             f"Idp hinting: cannot detect request type [{http_response.status_code}]"
         )
     return False
+
+
+@lru_cache()
+def get_csp_handler():
+    """Returns a view decorator for CSP."""
+
+    def empty_view_decorator(view):
+        return view
+
+    csp_handler_string = get_custom_setting("SAML_CSP_HANDLER", None)
+
+    if csp_handler_string is None:
+        # No CSP handler configured, attempt to use django-csp
+        return _django_csp_update_decorator() or empty_view_decorator
+
+    if csp_handler_string.strip() != "":
+        # Non empty string is configured, attempt to import it
+        csp_handler = import_string(csp_handler_string)
+
+        def custom_csp_updater(f):
+            @wraps(f)
+            def wrapper(*args, **kwargs):
+                return csp_handler(f(*args, **kwargs))
+
+            return wrapper
+
+        return custom_csp_updater
+
+    # Fall back to empty decorator when csp_handler_string is empty
+    return empty_view_decorator
+
+
+def _django_csp_update_decorator():
+    """Returns a view CSP decorator if django-csp is available, otherwise None."""
+    try:
+        from csp.decorators import csp_update
+    except ModuleNotFoundError:
+        # If csp is not installed, do not update fields as Content-Security-Policy
+        # is not used
+        logger.warning(
+            "django-csp could not be found, not updating Content-Security-Policy. Please "
+            "make sure CSP is configured. This can be done by your reverse proxy, "
+            "django-csp or a custom CSP handler via SAML_CSP_HANDLER. See "
+            "https://djangosaml2.readthedocs.io/contents/security.html#content-security-policy"
+            " for more information. "
+            "This warning can be disabled by setting `SAML_CSP_HANDLER=''` in your settings."
+        )
+        return
+    else:
+        # autosubmit of forms uses nonce per default
+        # form-action https: to send data to IdPs
+        return csp_update(FORM_ACTION=["https:"])
```

### Comparing `djangosaml2-1.9.2/djangosaml2/views.py` & `djangosaml2-1.9.3/djangosaml2/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import base64
 import logging
+from functools import wraps
 from typing import Optional
 from urllib.parse import quote
 
 from django.conf import settings
 from django.core.exceptions import PermissionDenied, SuspiciousOperation
 from django.http import (
     HttpRequest,
@@ -65,42 +66,33 @@
 from .cache import IdentityCache, OutstandingQueriesCache, StateCache
 from .conf import get_config
 from .exceptions import IdPConfigurationMissing
 from .overrides import Saml2Client
 from .utils import (
     add_idp_hinting,
     available_idps,
+    get_csp_handler,
     get_custom_setting,
     get_fallback_login_redirect_url,
     get_idp_sso_supported_bindings,
     get_location,
     validate_referral_url,
 )
 
 logger = logging.getLogger("djangosaml2")
 
-# Update Content-Security-Policy headers for POST-Bindings
-try:
-    from csp.decorators import csp_update
-except ModuleNotFoundError:
-    # If csp is not installed, do not update fields as Content-Security-Policy
-    # is not used
-    def saml2_csp_update(view):
-        return view
-
-    logger.warning("django-csp could not be found, not updating Content-Security-Policy. Please "
-                   "make sure CSP is configured at least by httpd or setup django-csp. See "
-                   "https://djangosaml2.readthedocs.io/contents/security.html#content-security-policy"
-                   " for more information")
-else:
-    # script-src 'unsafe-inline' to autosubmit forms,
-    # form-action https: to send data to IdPs
-    saml2_csp_update = csp_update(
-        SCRIPT_SRC=["'unsafe-inline'"], FORM_ACTION=["https:"]
-    )
+
+def saml2_csp_update(view):
+    csp_handler = get_csp_handler()
+
+    @wraps(view)
+    def wrapper(*args, **kwargs):
+        return csp_handler(view)(*args, **kwargs)
+
+    return wrapper
 
 
 def _set_subject_id(session, subject_id):
     session["_saml2_subject_id"] = code(subject_id)
 
 
 def _get_subject_id(session):
@@ -792,15 +784,15 @@
         )
 
     def post(self, request, *args, **kwargs):
         return self.do_logout_service(
             request, request.POST, saml2.BINDING_HTTP_POST, *args, **kwargs
         )
 
-    def do_logout_service(self, request, data, binding):
+    def do_logout_service(self, request, data, binding, *args, **kwargs):
         logger.debug("Logout service started")
 
         state, client = self.get_state_client(request)
 
         if "SAMLResponse" in data:  # we started the logout
             logger.debug("Receiving a logout response from the IdP")
             try:
```

### Comparing `djangosaml2-1.9.2/djangosaml2.egg-info/PKG-INFO` & `djangosaml2-1.9.3/djangosaml2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.9.2
+Version: 1.9.3
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.9.2/djangosaml2.egg-info/SOURCES.txt` & `djangosaml2-1.9.3/djangosaml2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 djangosaml2.egg-info/requires.txt
 djangosaml2.egg-info/top_level.txt
 djangosaml2/templates/djangosaml2/auth_error.html
 djangosaml2/templates/djangosaml2/echo_attributes.html
 djangosaml2/templates/djangosaml2/example_post_binding_form.html
 djangosaml2/templates/djangosaml2/login_error.html
 djangosaml2/templates/djangosaml2/logout_error.html
+djangosaml2/templates/djangosaml2/post_binding_form.html
 djangosaml2/templates/djangosaml2/wayf.html
 djangosaml2/templatetags/__init__.py
 djangosaml2/templatetags/idplist.py
 djangosaml2/tests/__init__.py
 djangosaml2/tests/auth_response.py
 djangosaml2/tests/conf.py
 djangosaml2/tests/idpcert.csr
```

### Comparing `djangosaml2-1.9.2/docs/source/_templates/pplnx_template/footer.html` & `djangosaml2-1.9.3/docs/source/_templates/pplnx_template/footer.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/docs/source/_templates/pplnx_template/layout.html` & `djangosaml2-1.9.3/docs/source/_templates/pplnx_template/layout.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.9.2/setup.py` & `djangosaml2-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return codecs.open(
         os.path.join(os.path.dirname(__file__), *rnames), encoding="utf-8"
     ).read()
 
 
 setup(
     name="djangosaml2",
-    version="1.9.2",
+    version="1.9.3",
     description="pysaml2 integration for Django",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
```

