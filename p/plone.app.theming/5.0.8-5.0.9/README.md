# Comparing `tmp/plone_app_theming-5.0.8.tar.gz` & `tmp/plone_app_theming-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_app_theming-5.0.8.tar", last modified: Mon Apr 22 10:07:07 2024, max compression
+gzip compressed data, was "plone_app_theming-5.0.9.tar", last modified: Mon May  6 12:39:57 2024, max compression
```

## Comparing `plone_app_theming-5.0.8.tar` & `plone_app_theming-5.0.9.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.190099 plone_app_theming-5.0.8/
--rw-r--r--   0 maurits    (501) staff       (20)     1342 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      540 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/.flake8
--rw-r--r--   0 maurits    (501) staff       (20)      663 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      284 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1927 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)    22164 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      674 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      172 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    65122 2024-04-22 10:07:07.189659 plone_app_theming-5.0.8/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      286 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      536 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/TODO.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.152033 plone_app_theming-5.0.8/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    41101 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4191 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/pyproject.toml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.142113 plone_app_theming-5.0.8/resources/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.142228 plone_app_theming-5.0.8/resources/theme/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.153387 plone_app_theming-5.0.8/resources/theme/theme1/
--rw-r--r--   0 maurits    (501) staff       (20)      191 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/manifest.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      153 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/othertheme.html
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.153830 plone_app_theming-5.0.8/resources/theme/theme1/overrides/
--rw-r--r--   0 maurits    (501) staff       (20)      544 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/overrides/plone.app.layout.viewlets.colophon.pt
--rw-r--r--   0 maurits    (501) staff       (20)      885 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/rules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      211 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/theme.html
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.155800 plone_app_theming-5.0.8/resources/theme/theme1/views/
--rw-r--r--   0 maurits    (501) staff       (20)     3947 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/views/class-view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      124 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/views/context-view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      121 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/views/name-view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      127 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/views/permission-view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      121 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/views/test-view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      217 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/resources/theme/theme1/views/views.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-22 10:07:07.190182 plone_app_theming-5.0.8/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2422 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.143007 plone_app_theming-5.0.8/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.156116 plone_app_theming-5.0.8/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.159596 plone_app_theming-5.0.8/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.164809 plone_app_theming-5.0.8/src/plone/app/theming/
--rw-r--r--   0 maurits    (501) staff       (20)      152 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.167593 plone_app_theming-5.0.8/src/plone/app/theming/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1194 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    38831 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    16099 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1074 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/custom_css.py
--rw-r--r--   0 maurits    (501) staff       (20)      470 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/help.py
--rw-r--r--   0 maurits    (501) staff       (20)      939 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/icon.gif
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.168815 plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/
--rw-r--r--   0 maurits    (501) staff       (20)     1644 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/controlpanel.css
--rw-r--r--   0 maurits    (501) staff       (20)     5536 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/defaultPreview.png
--rwxr-xr-x   0 maurits    (501) staff       (20)     1495 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/preview.png
--rw-r--r--   0 maurits    (501) staff       (20)    40897 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/userguide.rst
--rw-r--r--   0 maurits    (501) staff       (20)      488 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/theme-error.pt
--rw-r--r--   0 maurits    (501) staff       (20)      772 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/browser/themefile.py
--rw-r--r--   0 maurits    (501) staff       (20)     2747 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/events.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.169733 plone_app_theming-5.0.8/src/plone/app/theming/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      412 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1832 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/exportimport/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)      381 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/header.py
--rw-r--r--   0 maurits    (501) staff       (20)     9484 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.170930 plone_app_theming-5.0.8/src/plone/app/theming/plugins/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/plugins/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      476 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/plugins/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1391 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/plugins/hooks.py
--rw-r--r--   0 maurits    (501) staff       (20)     2689 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/plugins/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     6244 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/policy.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.144211 plone_app_theming-5.0.8/src/plone/app/theming/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.172126 plone_app_theming-5.0.8/src/plone/app/theming/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      161 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1043 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      187 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      132 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1136 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.179208 plone_app_theming-5.0.8/src/plone/app/theming/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.179789 plone_app_theming-5.0.8/src/plone/app/theming/tests/another-theme/
--rw-r--r--   0 maurits    (501) staff       (20)      608 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/another-theme/manifest.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      213 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/another-theme/rules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      126 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)      890 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      242 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/french.html
--rw-r--r--   0 maurits    (501) staff       (20)      156 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/includes.html
--rw-r--r--   0 maurits    (501) staff       (20)      456 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/includes.xml
--rw-r--r--   0 maurits    (501) staff       (20)      438 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/localrules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      119 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/nonascii.html
--rw-r--r--   0 maurits    (501) staff       (20)      342 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/nonascii.xml
--rw-r--r--   0 maurits    (501) staff       (20)      199 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/notheme.pt
--rw-r--r--   0 maurits    (501) staff       (20)      116 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/one.html
--rw-r--r--   0 maurits    (501) staff       (20)      442 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/otherrules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      153 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/othertheme.html
--rw-r--r--   0 maurits    (501) staff       (20)       53 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/package_theme.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1095 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/paramrules.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.183419 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/
--rw-r--r--   0 maurits    (501) staff       (20)      471 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/css-js.xml
--rw-r--r--   0 maurits    (501) staff       (20)      139 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/manifest.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       46 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/nonascii.html
--rw-r--r--   0 maurits    (501) staff       (20)      340 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/nonascii.xml
--rw-r--r--   0 maurits    (501) staff       (20)      153 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/othertheme.html
--rw-r--r--   0 maurits    (501) staff       (20)      632 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/overridesrules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/overridestheme.html
--rw-r--r--   0 maurits    (501) staff       (20)       17 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/resource.css
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/resource.js
--rw-r--r--   0 maurits    (501) staff       (20)      643 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/rules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      177 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/theme.html
--rw-r--r--   0 maurits    (501) staff       (20)      709 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/rules.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.183990 plone_app_theming-5.0.8/src/plone/app/theming/tests/secondary-theme/
--rw-r--r--   0 maurits    (501) staff       (20)      636 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/secondary-theme/manifest.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      213 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/secondary-theme/rules.xml
--rw-r--r--   0 maurits    (501) staff       (20)     4223 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     4183 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     4937 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/test_policy.py
--rw-r--r--   0 maurits    (501) staff       (20)    29670 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/test_transform.py
--rw-r--r--   0 maurits    (501) staff       (20)    29016 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      177 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/theme.html
--rw-r--r--   0 maurits    (501) staff       (20)      116 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/two.html
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.187039 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/
--rw-r--r--   0 maurits    (501) staff       (20)      752 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/default_rules.zip
--rw-r--r--   0 maurits    (501) staff       (20)     1330 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/ignores_dotfiles_resource_forks.zip
--rw-r--r--   0 maurits    (501) staff       (20)     1029 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_default_rules.zip
--rw-r--r--   0 maurits    (501) staff       (20)     1437 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_default_rules_override.zip
--rw-r--r--   0 maurits    (501) staff       (20)      985 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_prefix.zip
--rw-r--r--   0 maurits    (501) staff       (20)     8584 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_preview.zip
--rw-r--r--   0 maurits    (501) staff       (20)      980 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_rules.zip
--rw-r--r--   0 maurits    (501) staff       (20)      890 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/multiple_dir.zip
--rw-r--r--   0 maurits    (501) staff       (20)      540 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/nodir.zip
--rw-r--r--   0 maurits    (501) staff       (20)     2395 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/subdirectories.zip
--rw-r--r--   0 maurits    (501) staff       (20)     1403 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/theme.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.145300 plone_app_theming-5.0.8/src/plone/app/theming/themes/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.188140 plone_app_theming-5.0.8/src/plone/app/theming/themes/template/
--rw-r--r--   0 maurits    (501) staff       (20)      158 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/themes/template/index.html
--rw-r--r--   0 maurits    (501) staff       (20)       29 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/themes/template/manifest.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1174 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/themes/template/rules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      228 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/themes.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6679 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/transform.py
--rw-r--r--   0 maurits    (501) staff       (20)     1020 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)      524 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/upgrade.py
--rw-r--r--   0 maurits    (501) staff       (20)    25031 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1169 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/src/plone/app/theming/zmi.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:07:07.188549 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    65122 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5179 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      411 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-22 10:07:07.000000 plone_app_theming-5.0.8/src/plone.app.theming.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4616 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/tox.ini
--rw-r--r--   0 maurits    (501) staff       (20)      264 2024-04-22 10:07:06.000000 plone_app_theming-5.0.8/versions.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.695444 plone_app_theming-5.0.9/
+-rw-r--r--   0 maurits    (501) staff       (20)     1342 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/.flake8
+-rw-r--r--   0 maurits    (501) staff       (20)      663 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      284 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1927 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)    22295 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      674 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      172 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    65253 2024-05-06 12:39:57.694785 plone_app_theming-5.0.9/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      286 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      536 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/TODO.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.652122 plone_app_theming-5.0.9/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    41101 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4191 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/pyproject.toml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.640741 plone_app_theming-5.0.9/resources/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.640888 plone_app_theming-5.0.9/resources/theme/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.654123 plone_app_theming-5.0.9/resources/theme/theme1/
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      153 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/othertheme.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.654504 plone_app_theming-5.0.9/resources/theme/theme1/overrides/
+-rw-r--r--   0 maurits    (501) staff       (20)      544 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/overrides/plone.app.layout.viewlets.colophon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      885 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/rules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      211 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/theme.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.656890 plone_app_theming-5.0.9/resources/theme/theme1/views/
+-rw-r--r--   0 maurits    (501) staff       (20)     3947 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/views/class-view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      124 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/views/context-view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/views/name-view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/views/permission-view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/views/test-view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/resources/theme/theme1/views/views.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:39:57.695594 plone_app_theming-5.0.9/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2422 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.642183 plone_app_theming-5.0.9/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.657238 plone_app_theming-5.0.9/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.661424 plone_app_theming-5.0.9/src/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.666619 plone_app_theming-5.0.9/src/plone/app/theming/
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.669830 plone_app_theming-5.0.9/src/plone/app/theming/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1194 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    38831 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    16099 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1074 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/custom_css.py
+-rw-r--r--   0 maurits    (501) staff       (20)      470 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/help.py
+-rw-r--r--   0 maurits    (501) staff       (20)      939 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/icon.gif
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.671077 plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)     1644 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/controlpanel.css
+-rw-r--r--   0 maurits    (501) staff       (20)     5536 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/defaultPreview.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1495 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/preview.png
+-rw-r--r--   0 maurits    (501) staff       (20)    40897 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/userguide.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      488 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/theme-error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      772 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/browser/themefile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2747 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/events.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.672287 plone_app_theming-5.0.9/src/plone/app/theming/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      412 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1832 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/exportimport/handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)      381 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/header.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9484 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.673615 plone_app_theming-5.0.9/src/plone/app/theming/plugins/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/plugins/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      476 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/plugins/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1391 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/plugins/hooks.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2689 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/plugins/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6244 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/policy.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.643915 plone_app_theming-5.0.9/src/plone/app/theming/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.675036 plone_app_theming-5.0.9/src/plone/app/theming/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      161 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1043 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      132 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1136 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.683603 plone_app_theming-5.0.9/src/plone/app/theming/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.684302 plone_app_theming-5.0.9/src/plone/app/theming/tests/another-theme/
+-rw-r--r--   0 maurits    (501) staff       (20)      608 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/another-theme/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      213 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/another-theme/rules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      126 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      242 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/french.html
+-rw-r--r--   0 maurits    (501) staff       (20)      156 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/includes.html
+-rw-r--r--   0 maurits    (501) staff       (20)      456 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/includes.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      438 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/localrules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      119 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/nonascii.html
+-rw-r--r--   0 maurits    (501) staff       (20)      342 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/nonascii.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/notheme.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/one.html
+-rw-r--r--   0 maurits    (501) staff       (20)      442 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/otherrules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      153 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/othertheme.html
+-rw-r--r--   0 maurits    (501) staff       (20)       53 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/package_theme.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1095 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/paramrules.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.687850 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)      471 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/css-js.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       46 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/nonascii.html
+-rw-r--r--   0 maurits    (501) staff       (20)      340 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/nonascii.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      153 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/othertheme.html
+-rw-r--r--   0 maurits    (501) staff       (20)      632 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/overridesrules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/overridestheme.html
+-rw-r--r--   0 maurits    (501) staff       (20)       17 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/resource.css
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/resource.js
+-rw-r--r--   0 maurits    (501) staff       (20)      643 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/rules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      177 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/theme.html
+-rw-r--r--   0 maurits    (501) staff       (20)      709 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/rules.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.688650 plone_app_theming-5.0.9/src/plone/app/theming/tests/secondary-theme/
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/secondary-theme/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      213 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/secondary-theme/rules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     4223 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4183 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4937 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/test_policy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    30487 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/test_transform.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29016 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      177 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/theme.html
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/two.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.692392 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/
+-rw-r--r--   0 maurits    (501) staff       (20)      752 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/default_rules.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1330 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/ignores_dotfiles_resource_forks.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1029 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_default_rules.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1437 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_default_rules_override.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      985 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_prefix.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     8584 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_preview.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_rules.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/multiple_dir.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/nodir.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     2395 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/subdirectories.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1403 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/theme.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.645500 plone_app_theming-5.0.9/src/plone/app/theming/themes/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.693590 plone_app_theming-5.0.9/src/plone/app/theming/themes/template/
+-rw-r--r--   0 maurits    (501) staff       (20)      158 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/themes/template/index.html
+-rw-r--r--   0 maurits    (501) staff       (20)       29 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/themes/template/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1174 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/themes/template/rules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/themes.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6788 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/transform.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)      524 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/upgrade.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25031 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1169 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/src/plone/app/theming/zmi.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:39:57.693984 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    65253 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5179 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      411 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:39:57.000000 plone_app_theming-5.0.9/src/plone.app.theming.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4616 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/tox.ini
+-rw-r--r--   0 maurits    (501) staff       (20)      264 2024-05-06 12:39:56.000000 plone_app_theming-5.0.9/versions.cfg
```

### Comparing `plone_app_theming-5.0.8/.editorconfig` & `plone_app_theming-5.0.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/.flake8` & `plone_app_theming-5.0.9/.flake8`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/.gitignore` & `plone_app_theming-5.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/.pre-commit-config.yaml` & `plone_app_theming-5.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/CHANGES.rst` & `plone_app_theming-5.0.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.9 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Fix an issue with unicode characters happening with lxml 5 [ale-rt] (#238)
+
+
 5.0.8 (2024-04-22)
 ------------------
 
 Bug fixes:
 
 
 - Traverse to theme resources from the navigation root again.
```

### Comparing `plone_app_theming-5.0.8/LICENSE` & `plone_app_theming-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/PKG-INFO` & `plone_app_theming-5.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.theming
-Version: 5.0.8
+Version: 5.0.9
 Summary: Integrates the Diazo theming engine with Plone
 Home-page: https://pypi.org/project/plone.app.theming
 Author: Martin Aspeli and Laurence Rowe
 Author-email: optilude@gmail.com
 License: GPL
 Keywords: plone diazo xdv deliverance theme transform xslt
 Classifier: Development Status :: 5 - Production/Stable
@@ -1093,14 +1093,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.9 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Fix an issue with unicode characters happening with lxml 5 [ale-rt] (#238)
+
+
 5.0.8 (2024-04-22)
 ------------------
 
 Bug fixes:
 
 
 - Traverse to theme resources from the navigation root again.
```

### Comparing `plone_app_theming-5.0.8/TODO.txt` & `plone_app_theming-5.0.9/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/docs/index.rst` & `plone_app_theming-5.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/pyproject.toml` & `plone_app_theming-5.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/resources/theme/theme1/overrides/plone.app.layout.viewlets.colophon.pt` & `plone_app_theming-5.0.9/resources/theme/theme1/overrides/plone.app.layout.viewlets.colophon.pt`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/resources/theme/theme1/rules.xml` & `plone_app_theming-5.0.9/resources/theme/theme1/rules.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/resources/theme/theme1/views/class-view.pt` & `plone_app_theming-5.0.9/resources/theme/theme1/views/class-view.pt`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/setup.py` & `plone_app_theming-5.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.0.8"
+version = "5.0.9"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n"
     f"{(Path('src') / 'plone' / 'app' / 'theming' / 'browser' / 'resources' / 'userguide.rst').read_text()}\n"
     f"{Path('CHANGES.rst').read_text()}"
 )
```

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/configure.zcml` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/controlpanel.pt` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/controlpanel.py` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/custom_css.py` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/custom_css.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/icon.gif` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/icon.gif`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/controlpanel.css` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/controlpanel.css`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/defaultPreview.png` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/defaultPreview.png`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/preview.png` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/preview.png`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/resources/userguide.rst` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/resources/userguide.rst`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/browser/themefile.py` & `plone_app_theming-5.0.9/src/plone/app/theming/browser/themefile.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/configure.zcml` & `plone_app_theming-5.0.9/src/plone/app/theming/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/exportimport/handler.py` & `plone_app_theming-5.0.9/src/plone/app/theming/exportimport/handler.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/interfaces.py` & `plone_app_theming-5.0.9/src/plone/app/theming/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/plugins/hooks.py` & `plone_app_theming-5.0.9/src/plone/app/theming/plugins/hooks.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/plugins/utils.py` & `plone_app_theming-5.0.9/src/plone/app/theming/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/policy.py` & `plone_app_theming-5.0.9/src/plone/app/theming/policy.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/profiles/default/controlpanel.xml` & `plone_app_theming-5.0.9/src/plone/app/theming/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/testing.py` & `plone_app_theming-5.0.9/src/plone/app/theming/testing.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/another-theme/manifest.cfg` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/another-theme/manifest.cfg`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/configure.zcml` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/paramrules.xml` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/paramrules.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/overridesrules.xml` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/overridesrules.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/resources/rules.xml` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/resources/rules.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/rules.xml` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/rules.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/secondary-theme/manifest.cfg` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/secondary-theme/manifest.cfg`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/test_controlpanel.py` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/test_exportimport.py` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/test_policy.py` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/test_transform.py` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from App.config import getConfiguration
 from diazo.compiler import compile_theme
+from html import unescape
 from lxml import etree
 from os import environ
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.theming.interfaces import IThemeSettings
 from plone.app.theming.testing import THEMING_FUNCTIONAL_TESTING
+from plone.app.theming.testing import THEMING_INTEGRATION_TESTING
 from plone.app.theming.transform import ThemeTransform
 from plone.app.theming.utils import applyTheme
 from plone.app.theming.utils import getTheme
 from plone.app.theming.utils import PythonResolver
 from plone.app.theming.utils import resolvePythonURL
 from plone.registry.interfaces import IRegistry
 from plone.testing.zope import Browser
@@ -21,15 +23,38 @@
 
 import os.path
 import re
 import transaction
 import unittest
 
 
-class TestCase(unittest.TestCase):
+class IntegrationTestCase(unittest.TestCase):
+
+    layer = THEMING_INTEGRATION_TESTING
+
+    def test_transform_parseTree_with_unicode(self):
+        request = self.layer["request"]
+        request.response.setHeader("Content-Type", "text/html; charset=utf-8")
+        transform = ThemeTransform(None, request)
+        snippet = "\n".join(
+            (
+                "<!DOCTYPE html>",
+                "<html>",
+                "<body>",
+                "<div>à</div>",
+                "</body>",
+                "</html>",
+            )
+        )
+        parsed = transform.parseTree([snippet.encode()])
+        serialized = unescape(parsed.serialize().decode())
+        self.assertEqual(snippet, serialized)
+
+
+class FunctionalTestCase(unittest.TestCase):
     layer = THEMING_FUNCTIONAL_TESTING
 
     def setUp(self):
         # Enable debug mode always to ensure cache is disabled by default
         getConfiguration().debug_mode = True
 
         self.settings = getUtility(IRegistry).forInterface(IThemeSettings)
```

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/test_utils.py` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/default_rules.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/default_rules.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/ignores_dotfiles_resource_forks.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/ignores_dotfiles_resource_forks.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_default_rules.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_default_rules.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_default_rules_override.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_default_rules_override.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_prefix.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_prefix.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_preview.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_preview.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/manifest_rules.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/manifest_rules.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/multiple_dir.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/multiple_dir.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/nodir.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/nodir.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/tests/zipfiles/subdirectories.zip` & `plone_app_theming-5.0.9/src/plone/app/theming/tests/zipfiles/subdirectories.zip`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/theme.py` & `plone_app_theming-5.0.9/src/plone/app/theming/theme.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/themes/template/rules.xml` & `plone_app_theming-5.0.9/src/plone/app/theming/themes/template/rules.xml`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/transform.py` & `plone_app_theming-5.0.9/src/plone/app/theming/transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from plone.app.theming.utils import theming_policy
 from plone.app.theming.zmi import patch_zmi
 from plone.transformchain.interfaces import ITransform
 from repoze.xmliter.utils import getHTMLSerializer
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
+from ZPublisher.HTTPRequest import default_encoding
 
 import logging
 
 
 # Disable theming of ZMI
 patch_zmi()
 
@@ -116,15 +117,17 @@
             "zip",
             "deflate",
             "compress",
         ):
             return None
 
         try:
-            return getHTMLSerializer(result, pretty_print=False)
+            return getHTMLSerializer(
+                result, pretty_print=False, encoding=default_encoding
+            )
         except (AttributeError, TypeError, etree.ParseError):
             return None
 
     def transformBytes(self, result, encoding):
         try:
             result = result.decode(encoding)
         except UnicodeDecodeError:
```

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/traversal.py` & `plone_app_theming-5.0.9/src/plone/app/theming/traversal.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/upgrade.py` & `plone_app_theming-5.0.9/src/plone/app/theming/upgrade.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/utils.py` & `plone_app_theming-5.0.9/src/plone/app/theming/utils.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone/app/theming/zmi.py` & `plone_app_theming-5.0.9/src/plone/app/theming/zmi.py`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/src/plone.app.theming.egg-info/PKG-INFO` & `plone_app_theming-5.0.9/src/plone.app.theming.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.theming
-Version: 5.0.8
+Version: 5.0.9
 Summary: Integrates the Diazo theming engine with Plone
 Home-page: https://pypi.org/project/plone.app.theming
 Author: Martin Aspeli and Laurence Rowe
 Author-email: optilude@gmail.com
 License: GPL
 Keywords: plone diazo xdv deliverance theme transform xslt
 Classifier: Development Status :: 5 - Production/Stable
@@ -1093,14 +1093,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.9 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Fix an issue with unicode characters happening with lxml 5 [ale-rt] (#238)
+
+
 5.0.8 (2024-04-22)
 ------------------
 
 Bug fixes:
 
 
 - Traverse to theme resources from the navigation root again.
```

### Comparing `plone_app_theming-5.0.8/src/plone.app.theming.egg-info/SOURCES.txt` & `plone_app_theming-5.0.9/src/plone.app.theming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone_app_theming-5.0.8/tox.ini` & `plone_app_theming-5.0.9/tox.ini`

 * *Files identical despite different names*

