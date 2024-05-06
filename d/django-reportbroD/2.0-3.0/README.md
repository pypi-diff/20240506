# Comparing `tmp/django-reportbroD-2.0.tar.gz` & `tmp/django-reportbroD-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reportbroD-2.0.tar", last modified: Wed Apr 24 11:58:57 2024, max compression
+gzip compressed data, was "django-reportbroD-3.0.tar", last modified: Mon May  6 16:19:14 2024, max compression
```

## Comparing `django-reportbroD-2.0.tar` & `django-reportbroD-3.0.tar`

### file list

```diff
@@ -1,163 +1,173 @@
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.418981 django-reportbroD-2.0/
--rw-r--r--   0 rider     (1000) rider     (1000)      111 2024-02-21 17:30:29.000000 django-reportbroD-2.0/MANIFEST.in
--rw-r--r--   0 rider     (1000) rider     (1000)     2628 2024-04-24 11:58:57.418981 django-reportbroD-2.0/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     1686 2024-04-09 19:59:30.000000 django-reportbroD-2.0/README.md
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.338980 django-reportbroD-2.0/django_reportbroD/
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-2.0/django_reportbroD/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-04-22 20:05:48.000000 django-reportbroD-2.0/django_reportbroD/admin.py
--rw-r--r--   0 rider     (1000) rider     (1000)      192 2024-04-24 11:15:09.000000 django-reportbroD-2.0/django_reportbroD/apps.py
--rw-r--r--   0 rider     (1000) rider     (1000)      832 2024-04-22 20:05:48.000000 django-reportbroD-2.0/django_reportbroD/forms.py
--rw-r--r--   0 rider     (1000) rider     (1000)      801 2024-04-22 20:05:48.000000 django-reportbroD-2.0/django_reportbroD/menus.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.338980 django-reportbroD-2.0/django_reportbroD/migrations/
--rw-r--r--   0 rider     (1000) rider     (1000)     1738 2024-04-11 16:32:42.000000 django-reportbroD-2.0/django_reportbroD/migrations/0001_initial.py
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-2.0/django_reportbroD/migrations/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)     1864 2024-04-22 20:05:48.000000 django-reportbroD-2.0/django_reportbroD/models.py
--rw-r--r--   0 rider     (1000) rider     (1000)    14448 2024-04-22 20:05:48.000000 django-reportbroD-2.0/django_reportbroD/reportcore.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.332313 django-reportbroD-2.0/django_reportbroD/static/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.332313 django-reportbroD-2.0/django_reportbroD/static/assets/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.342313 django-reportbroD-2.0/django_reportbroD/static/assets/css/
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-2.0/django_reportbroD/static/assets/css/mCSB_buttons.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-2.0/django_reportbroD/static/assets/css/owl.video.play.html
--rw-r--r--   0 rider     (1000) rider     (1000)   509223 2019-03-30 20:18:10.000000 django-reportbroD-2.0/django_reportbroD/static/assets/css/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)   236692 2019-03-30 20:18:06.000000 django-reportbroD-2.0/django_reportbroD/static/assets/css/vendors.css
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.372314 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    24288 2019-03-30 20:18:20.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   351196 2019-03-30 20:18:20.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    62768 2019-03-30 20:18:20.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    31064 2019-03-30 20:18:20.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16604 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   163862 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    41636 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    20528 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    99368 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    40348 2019-03-30 20:18:22.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    26004 2019-03-30 20:18:24.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:24.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   213926 2019-03-30 20:18:26.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    61920 2019-03-30 20:18:24.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    29500 2019-03-30 20:18:24.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/featherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:26.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    77159 2019-03-30 20:18:26.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.html
--rw-r--r--   0 rider     (1000) rider     (1000)   444379 2019-03-30 20:18:28.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   165548 2019-03-30 20:18:28.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    98024 2019-03-30 20:18:26.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:28.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:28.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    61020 2019-03-30 20:18:28.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   400219 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   143936 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    80356 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    48132 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    21308 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     7936 2019-03-30 20:18:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:32.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:32.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    38383 2019-03-30 20:18:32.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   238287 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    99212 2019-03-30 20:18:32.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    50312 2019-03-30 20:18:32.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16746 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/summernotec360.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16560 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/summernotec360.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    10324 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/summernotec360.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   234269 2019-03-30 20:18:36.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    78584 2019-03-30 20:18:36.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    56108 2019-03-30 20:18:34.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:36.000000 django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.378980 django-reportbroD-2.0/django_reportbroD/static/assets/img/
--rw-r--r--   0 rider     (1000) rider     (1000)    39361 2019-03-30 21:07:44.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/02.jpg
--rw-r--r--   0 rider     (1000) rider     (1000)    59862 2024-03-21 18:14:53.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/base64.png
--rw-r--r--   0 rider     (1000) rider     (1000)    82742 2024-03-21 18:11:05.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/dictionario.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.378980 django-reportbroD-2.0/django_reportbroD/static/assets/img/export/
--rw-r--r--   0 rider     (1000) rider     (1000)     1876 2019-03-30 21:07:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/export/csv.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1348 2019-03-30 21:07:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/export/txt.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     2060 2019-03-30 21:07:30.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/export/xlsx.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-02-21 14:09:26.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.378980 django-reportbroD-2.0/django_reportbroD/static/assets/img/file-icon/
--rw-r--r--   0 rider     (1000) rider     (1000)     6359 2024-04-22 20:10:11.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/file-icon/reporte.png
--rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-03-09 16:12:06.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/lista.png
--rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-02-21 13:55:04.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/logo-icon.png
--rw-r--r--   0 rider     (1000) rider     (1000)     2422 2019-03-30 20:18:36.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/logo-light.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 13:43:58.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/logo.png
--rw-r--r--   0 rider     (1000) rider     (1000)    49844 2024-03-21 17:54:33.000000 django-reportbroD-2.0/django_reportbroD/static/assets/img/parametros.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.382314 django-reportbroD-2.0/django_reportbroD/static/assets/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   576312 2019-03-30 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/assets/js/app.js
--rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2019-03-30 20:19:02.000000 django-reportbroD-2.0/django_reportbroD/static/assets/js/vendors.js
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.402314 django-reportbroD-2.0/django_reportbroD/static/reportlib/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.402314 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.402314 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.402314 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
--rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-02-21 21:05:40.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/css/styles.css
--rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.405648 django-reportbroD-2.0/django_reportbroD/static/reportlib/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
--rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/js/jquery.cookie.js
--rw-r--r--   0 rider     (1000) rider     (1000)   318139 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/js/knockout-3.5.1.js
--rw-r--r--   0 rider     (1000) rider     (1000)    68249 2024-02-14 15:51:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/js/knockout-3.5.1.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.css
--rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.css.map
--rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.js
--rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
--rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.js.map
--rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.min.js.map
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.408981 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/
--rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/ajaxload.gif
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.412314 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.412314 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
--rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 20:18:44.000000 django-reportbroD-2.0/django_reportbroD/static/reportlib/src/rb_logo_white.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.415648 django-reportbroD-2.0/django_reportbroD/templates/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.418981 django-reportbroD-2.0/django_reportbroD/templates/bases/
--rw-r--r--   0 rider     (1000) rider     (1000)     1776 2024-03-06 19:20:14.000000 django-reportbroD-2.0/django_reportbroD/templates/bases/base.html
--rw-r--r--   0 rider     (1000) rider     (1000)      346 2024-02-18 06:01:54.000000 django-reportbroD-2.0/django_reportbroD/templates/bases/footer.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1969 2024-02-21 13:50:22.000000 django-reportbroD-2.0/django_reportbroD/templates/bases/header.html
--rw-r--r--   0 rider     (1000) rider     (1000)      653 2024-03-12 18:36:16.000000 django-reportbroD-2.0/django_reportbroD/templates/bases/navigator.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1890 2024-04-24 10:48:29.000000 django-reportbroD-2.0/django_reportbroD/templates/create.html
--rw-r--r--   0 rider     (1000) rider     (1000)    20741 2024-03-09 15:34:58.000000 django-reportbroD-2.0/django_reportbroD/templates/document.html
--rw-r--r--   0 rider     (1000) rider     (1000)     2116 2024-04-22 20:06:57.000000 django-reportbroD-2.0/django_reportbroD/templates/edit.html
--rw-r--r--   0 rider     (1000) rider     (1000)     6189 2024-03-21 18:27:10.000000 django-reportbroD-2.0/django_reportbroD/templates/especif.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1128 2024-04-22 20:06:57.000000 django-reportbroD-2.0/django_reportbroD/templates/formulario.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3066 2024-04-22 20:06:57.000000 django-reportbroD-2.0/django_reportbroD/templates/import.html
--rw-r--r--   0 rider     (1000) rider     (1000)    10082 2024-04-22 20:06:57.000000 django-reportbroD-2.0/django_reportbroD/templates/index.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3065 2024-04-22 20:06:57.000000 django-reportbroD-2.0/django_reportbroD/templates/report.html
--rw-r--r--   0 rider     (1000) rider     (1000)       63 2024-04-22 20:05:48.000000 django-reportbroD-2.0/django_reportbroD/tests.py
--rw-r--r--   0 rider     (1000) rider     (1000)      743 2024-04-24 10:41:26.000000 django-reportbroD-2.0/django_reportbroD/urls.py
--rw-r--r--   0 rider     (1000) rider     (1000)     2702 2024-04-24 10:48:33.000000 django-reportbroD-2.0/django_reportbroD/utils.py
--rw-r--r--   0 rider     (1000) rider     (1000)     3221 2024-04-24 10:41:58.000000 django-reportbroD-2.0/django_reportbroD/views.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:58:57.338980 django-reportbroD-2.0/django_reportbroD.egg-info/
--rw-r--r--   0 rider     (1000) rider     (1000)     2628 2024-04-24 11:58:57.000000 django-reportbroD-2.0/django_reportbroD.egg-info/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     7144 2024-04-24 11:58:57.000000 django-reportbroD-2.0/django_reportbroD.egg-info/SOURCES.txt
--rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-04-24 11:58:57.000000 django-reportbroD-2.0/django_reportbroD.egg-info/dependency_links.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-04-24 11:58:57.000000 django-reportbroD-2.0/django_reportbroD.egg-info/requires.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-04-24 11:58:57.000000 django-reportbroD-2.0/django_reportbroD.egg-info/top_level.txt
--rw-r--r--   0 rider     (1000) rider     (1000)     1061 2024-04-24 11:58:57.418981 django-reportbroD-2.0/setup.cfg
--rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-2.0/setup.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.829754 django-reportbroD-3.0/
+-rw-r--r--   0 rider     (1000) rider     (1000)      131 2024-05-06 16:14:06.000000 django-reportbroD-3.0/MANIFEST.in
+-rw-r--r--   0 rider     (1000) rider     (1000)     3580 2024-05-06 16:19:14.833087 django-reportbroD-3.0/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     2522 2024-05-06 15:46:26.000000 django-reportbroD-3.0/README.md
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.713086 django-reportbroD-3.0/django_reportbroD/
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-3.0/django_reportbroD/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-02-18 03:27:34.000000 django-reportbroD-3.0/django_reportbroD/admin.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      191 2024-05-06 13:12:04.000000 django-reportbroD-3.0/django_reportbroD/apps.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      803 2024-05-01 16:21:02.000000 django-reportbroD-3.0/django_reportbroD/base.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      832 2024-04-14 18:53:48.000000 django-reportbroD-3.0/django_reportbroD/forms.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      984 2024-05-05 01:43:48.000000 django-reportbroD-3.0/django_reportbroD/menus.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.713086 django-reportbroD-3.0/django_reportbroD/migrations/
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-3.0/django_reportbroD/migrations/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     1864 2024-04-14 17:00:30.000000 django-reportbroD-3.0/django_reportbroD/models.py
+-rw-r--r--   0 rider     (1000) rider     (1000)    13363 2024-05-01 16:25:14.000000 django-reportbroD-3.0/django_reportbroD/reportcore.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.709752 django-reportbroD-3.0/django_reportbroD/static/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.709752 django-reportbroD-3.0/django_reportbroD/static/assets/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.716419 django-reportbroD-3.0/django_reportbroD/static/assets/css/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/mCSB_buttons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/owl.video.play.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   509223 2019-03-30 20:18:10.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/style.css
+-rw-r--r--   0 rider     (1000) rider     (1000)   236692 2024-05-05 16:55:58.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/vendors.css
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.766420 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    24288 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   351196 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    62768 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    31064 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16604 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   163862 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    41636 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    20528 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    99368 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    40348 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    26004 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   213926 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    61920 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    29500 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/featherd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    77159 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   444379 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)   165548 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    98024 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    61020 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   400219 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)   143936 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    80356 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    48132 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    21308 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)     7936 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    38383 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   238287 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    99212 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    50312 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16746 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16560 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    10324 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   234269 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    78584 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    56108 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.769753 django-reportbroD-3.0/django_reportbroD/static/assets/img/
+-rw-r--r--   0 rider     (1000) rider     (1000)    39361 2019-03-30 21:07:44.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/02.jpg
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.769753 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1876 2019-03-30 21:07:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/csv.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     1348 2019-03-30 21:07:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/txt.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     2060 2019-03-30 21:07:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/xlsx.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-02-21 14:09:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/favicon.ico
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.776420 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1182 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/ai.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1380 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/css.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      948 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/dbf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1383 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/doc.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1215 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/dwg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1269 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/exe.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1006 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/html.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1364 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/jpg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1399 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/pdf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1397 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/png.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1430 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/psd.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     6359 2024-04-14 18:02:54.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/reporte.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1005 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/rtf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1421 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/svg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      974 2019-03-30 21:07:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/xls.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1332 2019-03-30 21:07:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/xml.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      997 2019-03-30 21:07:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/zip.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-03-09 16:12:06.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/lista.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-02-21 13:55:04.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-icon.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     2422 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-light.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 13:43:58.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/logo.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.779753 django-reportbroD-3.0/django_reportbroD/static/assets/js/
+-rw-r--r--   0 rider     (1000) rider     (1000)   576312 2019-03-30 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/assets/js/app.js
+-rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2019-03-30 20:19:02.000000 django-reportbroD-3.0/django_reportbroD/static/assets/js/vendors.js
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.813087 django-reportbroD-3.0/django_reportbroD/static/reportlib/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.813087 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.813087 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.816420 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/style.css
+-rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-02-21 21:05:40.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/styles.css
+-rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/favicon.ico
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.819754 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/
+-rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
+-rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
+-rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery.cookie.js
+-rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css
+-rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css.map
+-rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js
+-rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.map
+-rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js
+-rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js.map
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.823087 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/
+-rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/ajaxload.gif
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.826420 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.826420 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_white.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.829754 django-reportbroD-3.0/django_reportbroD/templates/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.829754 django-reportbroD-3.0/django_reportbroD/templates/bases/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1926 2024-05-05 18:22:34.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/base.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      352 2024-04-15 00:52:16.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/footer.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     2825 2024-05-05 18:10:40.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/header.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      654 2024-05-05 01:48:02.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/navigator.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1890 2024-02-21 13:51:56.000000 django-reportbroD-3.0/django_reportbroD/templates/create.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    20738 2024-05-05 02:23:36.000000 django-reportbroD-3.0/django_reportbroD/templates/document.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     2122 2024-04-30 23:35:42.000000 django-reportbroD-3.0/django_reportbroD/templates/edit.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    22882 2024-05-05 16:43:04.000000 django-reportbroD-3.0/django_reportbroD/templates/especif.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1128 2024-02-20 03:51:56.000000 django-reportbroD-3.0/django_reportbroD/templates/formulario.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     3066 2024-04-15 00:38:30.000000 django-reportbroD-3.0/django_reportbroD/templates/import.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    10082 2024-05-05 02:25:04.000000 django-reportbroD-3.0/django_reportbroD/templates/index.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     3065 2024-04-14 18:52:08.000000 django-reportbroD-3.0/django_reportbroD/templates/report.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      743 2024-04-14 18:59:30.000000 django-reportbroD-3.0/django_reportbroD/urls.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     3568 2024-05-01 16:21:34.000000 django-reportbroD-3.0/django_reportbroD/utils.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     3281 2024-04-15 01:49:12.000000 django-reportbroD-3.0/django_reportbroD/views.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.713086 django-reportbroD-3.0/django_reportbroD.egg-info/
+-rw-r--r--   0 rider     (1000) rider     (1000)     3580 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     7696 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/SOURCES.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/dependency_links.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/requires.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/top_level.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)     1177 2024-05-06 16:19:14.833087 django-reportbroD-3.0/setup.cfg
+-rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-3.0/setup.py
```

### Comparing `django-reportbroD-2.0/PKG-INFO` & `django-reportbroD-3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,101 @@
-Metadata-Version: 2.1
-Name: django-reportbroD
-Version: 2.0
-Summary: A Django app to create and use ReportBro reports with a sample admin
-Author: Rider Raul Espinosa Perez
-Author-email: riderraule@gmail.com
-License: MIT
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 5.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # django-reportbroD
 A Django app to create and use ReportBro reports with a sample admin.
 
 Quick start
 -----------
 
 1. Add "reportbroD" to your INSTALLED_APPS setting like this:
-
+```
     INSTALLED_APPS = [
    
-...
+                ... ,
    'django_reportbroD.apps.ReportbrodConfig',
 
    ]
 
+```
 2. Add 'django_reportbroD.menus.get_menu_items' to your OPTIONS.context_processors in your TEMPLATES settings. This enables the use of menu for the installed report app. 
-
+ ```
         'OPTIONS': {
    
-            'context_processors': [...,'django_reportbroD.menus.get_menu_items'
+            'context_processors': [...,
+'django_reportbroD.menus.get_menu_items'
    
             ],
             
         }
-
+```
 
 3. Include the reportbroD URLconf in your project urls.py like this:
 
    path("reportbroD/", include("django_reportbroD.urls", namespace="reportbroD")),
 
-4. Run ``python manage.py makemigrations`` and ``python manage.py migrate`` to create the models and to migrating to data base.
+4. Run ``python manage.py migrate reportbroD`` to create the models and to migrating to data base.
 
 5. Start the development server.
 
 6. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
 
 
 Using report
 -----------
 
 1. Create a app to using the view file or other file .py for defining the view function to show/export selected report
-  from django_reportbroD.utils import convert_to_base64, convert_list_to_dict, to_dict
-   from django_reportbroD.reportcore import reportPDF, reportXLSX
-   
+ ```
+  from django_reportbroD.utils import convert_to_base64, convert_list_to_dict, to_dict, export_report_by_code, export_report_by_name, export_report_from_JSON
+  
    def generar_pdf(request):
    
      products=Product.objects.all()
    
      #converting in a dictionary
      productos=[to_dict(p) for p in products]
    
      imagen= convert_to_base64(products.first().imagen.url, 'jpg')
    
      data={
+            "productos":productos,
+            "imagen":imagen
+          }
+   
+     code_report= 12
+
+     return export_report_by_code(template_code=code_report, data=data, extension="pdf")
+
+def generar_xls(request):
+   
+     products=Product.objects.all()
+   
+     #converting in a dictionary
+     productos=[to_dict(p) for p in products]
+   
+     imagen= convert_to_base64(products.first().imagen.url, 'jpg')
+   
+     data={
    "productos":productos,
    "imagen":imagen
     }
    
-     code_report= 12
 
-     return reportPDF(request, code_report, data, file="reporte productos")
- 
+     return export_report_by_name(template_name="Plantilla de obrero" , data=data, extension="xlsx")
+
+
+def generar_reporte(request):
+   
+     products=Product.objects.all()
+   
+     #converting in a dictionary
+     productos=[to_dict(p) for p in products]
    
+     imagen= convert_to_base64(products.first().imagen.url, 'jpg')
+   
+     data={
+   "productos":productos,
+   "imagen":imagen
+    }
+   
+
+     return export_report_from_JSON(path_json="reporte.json", data=data, extension="xlsx")
+ 
+   ```
```

### Comparing `django-reportbroD-2.0/django_reportbroD/forms.py` & `django-reportbroD-3.0/django_reportbroD/forms.py`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/models.py` & `django-reportbroD-3.0/django_reportbroD/models.py`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/reportcore.py` & `django-reportbroD-3.0/django_reportbroD/reportcore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import datetime
 import json
 import uuid
 
 from django.db.models import Sum
-from django.http import HttpResponseBadRequest, HttpResponse, Http404, HttpResponseServerError
+from django.http import HttpResponseBadRequest, HttpResponse, HttpResponseServerError
 from django.shortcuts import render
 from django.utils.safestring import SafeString
 from django.views.decorators.clickjacking import xframe_options_exempt
 from django.views.decorators.csrf import csrf_exempt, ensure_csrf_cookie
 from reportbro import Report, ReportBroError
 from timeit import default_timer as timer
-
 from .models import ReportDefinition, ReportRequest
-from .utils import json_default, create_base_report_template
+from .base import json_default, create_base_report_template
+
+
 
 MAX_CACHE_SIZE = 1000 * 1024 * 1024  # keep max. 1000 MB of generated pdf files in db
 
 
 @ensure_csrf_cookie
 def edit(request, pk):
-    """Shows a page with ReportBro Designer to edit our albums report template.
+    """Shows a page with ReportBro Designer to edit our report template.
 
     The report template is loaded from the db (report_definition table),
     in case no report template exists a hardcoded template is generated in
     *create_album_report_template* for this Demo App. Normally you'd probably
     start with an empty report (empty string, so no report is loaded
     in the Designer) in this case.
     """
@@ -215,83 +216,55 @@
         ReportDefinition.objects.create(
             name=str(pk)+" reporte",
             report_definition=report_definition, 
             last_modified_at=now)
     return HttpResponse('ok')
 
 
-def reportPDF(request, code, data, file="reporte" ):
-    """Prints a pdf file with the available data. 
 
-    """
-   
 
-    # NOTE: these params must match exactly with the parameters defined in the
-    # report definition in ReportBro Designer, check the name and type (Number, Date, List, ...)
-    # of those parameters in the Designer.
-    #params = dict(year=year, albums=list(get_albums(year)), current_date=datetime.datetime.now())
-    params=data
+def reportPDF(report_definition, data, file="reporte"):
+    """Prints a pdf file with the available data. 
 
-    if ReportDefinition.objects.filter(pk=code)== None:
-        create_base_report_template(code)
+    """
+    # if ReportDefinition.objects.filter(pk=code)== None:
+    #     create_base_report_template(code)
     
 
-    report_definition = ReportDefinition.objects.get(pk=code)
-    
-    if not report_definition:
-        return HttpResponseServerError('no report_definition available')
-    
     
-
     try:
-        report_inst = Report(json.loads(report_definition.report_definition), params)
+        report_inst = Report(json.loads(report_definition), data)
         
         if report_inst.errors:
             # report definition should never contain any errors,
             # unless you saved an invalid report and didn't test in ReportBro Designer
             raise ReportBroError(report_inst.errors[0])
         
         pdf_report = report_inst.generate_pdf()
-        
-        
+
         response = HttpResponse(bytes(pdf_report), content_type='application/pdf')
         response['Content-Disposition'] = 'inline; filename="{filename}"'.format(filename=f"{file}.pdf")
+        
         return response
     except ReportBroError as ex:
         return HttpResponseServerError('report error: ' + str(ex.error))
     except Exception as ex:
         return HttpResponseServerError('report exception: ' + str(ex))
     
 
 
-def reportXLSX(request, code, data, file="reporte" ):
+def reportXLSX(report_definition, data, file="reporte" ):
     """Prints a xlsx file with the available data. 
 
     """
-   
-
-    # NOTE: these params must match exactly with the parameters defined in the
-    # report definition in ReportBro Designer, check the name and type (Number, Date, List, ...)
-    # of those parameters in the Designer.
-    #params = dict(year=year, albums=list(get_albums(year)), current_date=datetime.datetime.now())
-    params=data
-
-    if ReportDefinition.objects.filter(pk=code)== None:
-        create_base_report_template(code)
+    # if ReportDefinition.objects.filter(pk=code)== None:
+    #     create_base_report_template(code)
     
-
-    report_definition = ReportDefinition.objects.get(pk=code)
-    
-    if not report_definition:
-        return HttpResponseServerError('no report_definition available')
-    
-    
-
     try:
-        report_inst = Report(json.loads(report_definition.report_definition), params)
+        report_inst = Report(json.loads(report_definition), data)
         
         if report_inst.errors:
             # report definition should never contain any errors,
             # unless you saved an invalid report and didn't test in ReportBro Designer
             raise ReportBroError(report_inst.errors[0])
         
         pdf_report = report_inst.generate_xlsx()
```

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/css/mCSB_buttons.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/css/mCSB_buttons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/css/owl.video.play.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/css/owl.video.play.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/css/style.css` & `django-reportbroD-3.0/django_reportbroD/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/css/vendors.css` & `django-reportbroD-3.0/django_reportbroD/static/assets/css/vendors.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashicons.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripicons.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/feather.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/featherd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/featherd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesome.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ionicons.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weather.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.html` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-icons.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/summernotec360.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/summernotec360.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/summernotec360.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.ttf` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-icons.woff` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot` & `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/02.jpg` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/02.jpg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/export/csv.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/export/csv.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/export/txt.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/export/txt.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/export/xlsx.svg` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/export/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/favicon.ico` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/file-icon/reporte.png` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/reporte.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/lista.png` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/lista.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/logo-icon.png` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-icon.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/logo-light.png` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-light.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/img/logo.png` & `django-reportbroD-3.0/django_reportbroD/static/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/js/app.js` & `django-reportbroD-3.0/django_reportbroD/static/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/assets/js/vendors.js` & `django-reportbroD-3.0/django_reportbroD/static/assets/js/vendors.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/css/iconfonts/style.css` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/style.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/css/styles.css` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/favicon.ico` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/js/jquery.cookie.js` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.css` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.css.map` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.js` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.js.map` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.min.js` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/reportbro.min.js.map` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/ajaxload.gif` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/ajaxload.gif`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/static/reportlib/src/rb_logo_white.png` & `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_white.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/bases/base.html` & `django-reportbroD-3.0/django_reportbroD/templates/bases/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,29 @@
 	<!-- google fonts 
 	<link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700" rel="stylesheet">
 	-->
 	<!-- plugin stylesheets -->
 	<link rel="stylesheet" type="text/css" href="{% static 'assets/css/vendors.css' %}" />
 	<!-- app style -->
 	<link rel="stylesheet" type="text/css" href="{% static 'assets/css/style.css' %}" />
+	<style>
+
+	.menuhidden{
+display:None;
+		}
+
+	@media screen and (max-width:790px)
+	{
+.menuhidden{
+	display:inline-flex;
+}
+
+	}
+
+	</style>
 
 	{% endblock %}
 
 	{% block configr%}
 
 	{% endblock %}
 </head>
```

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/bases/header.html` & `django-reportbroD-3.0/django_reportbroD/templates/bases/header.html`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <header class="app-header top-bar">
     <!-- begin navbar -->
     <nav class="navbar navbar-expand-md">
 
         <!-- begin navbar-header -->
         <div class="navbar-header d-flex align-items-center">
             <a href="javascript:void:(0)" class="mobile-toggle"><i class="ti ti-align-right"></i></a>
-            <a class="navbar-brand" href="/" >
+            <a class="navbar-brand" href="{% url 'reportbroD:list' %}" >
                 <img src="{% static 'assets/img/logo.png' %}" class="img-fluid logo-desktop" alt="logo" />
                 <img src="{% static 'assets/img/logo-icon.png' %}" class="img-fluid logo-mobile" alt="logo" />
             </a>
         </div>
         <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
             <i class="ti ti-align-left"></i>
         </button>
@@ -32,13 +32,35 @@
                           
                         </a>
                     </li>
                     
                     
                 </ul>
 
+                <ul class="navbar-nav nav-right ml-auto menuhidden">
+                    
+                    {% for elem in menu %}
+                    <li class="nav-item dropdown">
+                        <a class="nav-link " href="{{elem.url}}" id="navbarDropdown2" role="button"  aria-haspopup="true" aria-expanded="false" title="{{elem.label}}">
+                            <i class="{{elem.icon}}"></i>
+
+                            {% if active_page == elem.id %}
+                        <span class="notify">
+                            <span class="blink"></span>
+                <span class="dot"></span>
+                </span>
+                {% endif %}
+                        </a>
+                        
+                    </li>
+
+
+                    {% endfor %}
+                </ul>
+
             </div>
         </div>
         <!-- end navigation -->
     </nav>
     <!-- end navbar -->
-</header>
+</header>
+
```

#### html2text {}

```diff
@@ -1,3 +1,6 @@
 {% load static %}
 _[_l_o_g_o_]_[_l_o_g_o_]
     * _A_d_m_i_n_i_s_t_r_a_c_i_Ã_³_n_ _d_e_ _R_e_p_o_r_t_e_s
+    * {% for elem in menu %}
+    * _{_%_ _i_f_ _a_c_t_i_v_e___p_a_g_e_ _=_=_ _e_l_e_m_._i_d_ _%_}_ _{_%_ _e_n_d_i_f_ _%_}
+    * {% endfor %}
```

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/bases/navigator.html` & `django-reportbroD-3.0/django_reportbroD/templates/bases/navigator.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {% if active_page == elem.id %}
     class="active"
   
     {% endif %}
 
     >
 
-    <a class=" has-arrow "  href="{{elem.url}}" aria-expanded="false">
+    <a class=" has-arrow "  href="{{elem.url}}" aria-expanded="false" >
 
     <i class="{{elem.icon}}"></i>
         <span class="nav-title">{{elem.label}}</span>
 
     </a>
 
 </li>
```

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/create.html` & `django-reportbroD-3.0/django_reportbroD/templates/create.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/document.html` & `django-reportbroD-3.0/django_reportbroD/templates/document.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                                     </div>
                                     <div class="ml-auto d-flex align-items-center">
                                         <nav>
                                             <ol class="breadcrumb p-0 m-b-0">
                                                 <li class="breadcrumb-item">
                                                     <a href="/"><i class="ti ti-home"></i></a>
                                                 </li>
-                                                <li class="breadcrumb-item active text-primary" aria-current="page">Documentación de ReportBro Designer</li>
+                                                <li class="breadcrumb-item active text-primary" aria-current="page">Documentación de ReportBro Admin</li>
                                             </ol>
                                         </nav>
                                     </div>
                                 </div>
                                 <!-- end page title -->
                             </div>
                         </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'bases/base.html'%} {% load static %} {% block content %}
 ************ DDooccuummeennttaaccii?Ã?³nn ************
-   1. DocumentaciÃ³n de ReportBro Designer
+   1. DocumentaciÃ³n de ReportBro Admin
     * _Q_u_Ã_©_ _e_s_ _R_e_p_o_r_t_b_r_o
     * _C_o_m_p_a_t_i_b_i_l_i_d_a_d
     * _E_s_p_e_c_i_f_i_c_a_c_i_o_n_e_s
 **** _11_.._ _LL_ii_bb_rr_ee_rr_ii_aa_ _RR_ee_pp_oo_rr_tt_BB_rr_oo_ _DD_ee_ss_ii_gg_nn_ee_rr ****
 RReeppoorrttBBrroo Designer es un plugin JavaScript que se puede integrar en su
 aplicaciÃ³n web. Aunque esto requiere un poco mÃ¡s de trabajo al principio,
 tener una herramienta de diseÃ±o de plantillas integrada tiene bastantes
```

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/edit.html` & `django-reportbroD-3.0/django_reportbroD/templates/edit.html`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                     </div>
      {% include 'formulario.html' %}
 
     </div>
 </div>
 
 
+    
 </div>
                  
         <!-- end row -->
     </div>
     <!-- end container-fluid -->
 </div>
```

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/formulario.html` & `django-reportbroD-3.0/django_reportbroD/templates/formulario.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/import.html` & `django-reportbroD-3.0/django_reportbroD/templates/import.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/index.html` & `django-reportbroD-3.0/django_reportbroD/templates/index.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/templates/report.html` & `django-reportbroD-3.0/django_reportbroD/templates/report.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-2.0/django_reportbroD/urls.py` & `django-reportbroD-3.0/django_reportbroD/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from .views import *
 from  .reportcore import *
 
 app_name="reportbroD"
 urlpatterns = [
     path("", ReportList.as_view(), name="list"),
     path("create/", CreateReport.as_view(), name="create"),
-    path("import/", importreport, name="import"),
-    path("edit/<int:pk>", EditReport.as_view(), name="edit"),
+     path("import/", importreport, name="import"),
+ path("edit/<int:pk>", EditReport.as_view(), name="edit"),
     path("delete/<int:id>", deletereport, name="delete"),
-    path("duplicate/<int:id>", duplicatereport, name="duplicate"),
-    path("export/<int:id>", exportreport, name="exportation"),
+     path("duplicate/<int:id>", duplicatereport, name="duplicate"),
+     path("export/<int:id>", exportreport, name="exportation"),
     path("docs/", docs_view, name="docs"),
     path("template/<int:pk>/", edit, name="template"),
     path("run/", run, name="report_run"),
     path("save/<int:pk>/", save, name="report_save"),
 
 
 ]
```

### Comparing `django-reportbroD-2.0/django_reportbroD/views.py` & `django-reportbroD-3.0/django_reportbroD/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any
 from django.shortcuts import render, get_object_or_404, redirect
 from .models import ReportDefinition
 from django.views.generic import ListView, CreateView, UpdateView
 from .forms import ReportForm, ReportImpForm
 from django.urls import reverse_lazy
 from datetime import datetime
+from django.core.serializers import serialize
 from django.http import HttpResponse
 import json
 
 
 
 # Create your views here.
 
@@ -78,14 +79,15 @@
 
 def importreport(request):
     
     if request.method=="POST":
         form=ReportImpForm(request.POST, request.FILES)
 
         if form.is_valid():
+           
             cd = request.FILES ['template']
             actual=datetime.now()
             
             try:
                 file=json.load(cd)
                 namereport= file["name"] if ReportDefinition.objects.filter(name=file["name"]).first() is None else file["name"]+" "+actual.isoformat()
                 ReportDefinition.objects.create(
```

### Comparing `django-reportbroD-2.0/django_reportbroD.egg-info/SOURCES.txt` & `django-reportbroD-3.0/django_reportbroD.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 django_reportbroD/__init__.py
 django_reportbroD/admin.py
 django_reportbroD/apps.py
+django_reportbroD/base.py
 django_reportbroD/forms.py
 django_reportbroD/menus.py
 django_reportbroD/models.py
 django_reportbroD/reportcore.py
-django_reportbroD/tests.py
 django_reportbroD/urls.py
 django_reportbroD/utils.py
 django_reportbroD/views.py
 django_reportbroD.egg-info/PKG-INFO
 django_reportbroD.egg-info/SOURCES.txt
 django_reportbroD.egg-info/dependency_links.txt
 django_reportbroD.egg-info/requires.txt
 django_reportbroD.egg-info/top_level.txt
-django_reportbroD/migrations/0001_initial.py
 django_reportbroD/migrations/__init__.py
 django_reportbroD/static/assets/css/mCSB_buttons.html
 django_reportbroD/static/assets/css/owl.video.play.html
 django_reportbroD/static/assets/css/style.css
 django_reportbroD/static/assets/css/vendors.css
 django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
 django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
@@ -74,26 +73,39 @@
 django_reportbroD/static/assets/fonts/summernotec360.woff
 django_reportbroD/static/assets/fonts/themify-icons.eot
 django_reportbroD/static/assets/fonts/themify-icons.svg
 django_reportbroD/static/assets/fonts/themify-icons.ttf
 django_reportbroD/static/assets/fonts/themify-icons.woff
 django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
 django_reportbroD/static/assets/img/02.jpg
-django_reportbroD/static/assets/img/base64.png
-django_reportbroD/static/assets/img/dictionario.png
 django_reportbroD/static/assets/img/favicon.ico
 django_reportbroD/static/assets/img/lista.png
 django_reportbroD/static/assets/img/logo-icon.png
 django_reportbroD/static/assets/img/logo-light.png
 django_reportbroD/static/assets/img/logo.png
-django_reportbroD/static/assets/img/parametros.png
 django_reportbroD/static/assets/img/export/csv.svg
 django_reportbroD/static/assets/img/export/txt.svg
 django_reportbroD/static/assets/img/export/xlsx.svg
+django_reportbroD/static/assets/img/file-icon/ai.png
+django_reportbroD/static/assets/img/file-icon/css.png
+django_reportbroD/static/assets/img/file-icon/dbf.png
+django_reportbroD/static/assets/img/file-icon/doc.png
+django_reportbroD/static/assets/img/file-icon/dwg.png
+django_reportbroD/static/assets/img/file-icon/exe.png
+django_reportbroD/static/assets/img/file-icon/html.png
+django_reportbroD/static/assets/img/file-icon/jpg.png
+django_reportbroD/static/assets/img/file-icon/pdf.png
+django_reportbroD/static/assets/img/file-icon/png.png
+django_reportbroD/static/assets/img/file-icon/psd.png
 django_reportbroD/static/assets/img/file-icon/reporte.png
+django_reportbroD/static/assets/img/file-icon/rtf.png
+django_reportbroD/static/assets/img/file-icon/svg.png
+django_reportbroD/static/assets/img/file-icon/xls.png
+django_reportbroD/static/assets/img/file-icon/xml.png
+django_reportbroD/static/assets/img/file-icon/zip.png
 django_reportbroD/static/assets/js/app.js
 django_reportbroD/static/assets/js/vendors.js
 django_reportbroD/static/reportlib/favicon.ico
 django_reportbroD/static/reportlib/reportbro.css
 django_reportbroD/static/reportlib/reportbro.css.map
 django_reportbroD/static/reportlib/reportbro.js
 django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
@@ -105,16 +117,14 @@
 django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
 django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
 django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
 django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
 django_reportbroD/static/reportlib/js/jquery-3.6.0.js
 django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
 django_reportbroD/static/reportlib/js/jquery.cookie.js
-django_reportbroD/static/reportlib/js/knockout-3.5.1.js
-django_reportbroD/static/reportlib/js/knockout-3.5.1.min.js
 django_reportbroD/static/reportlib/src/ajaxload.gif
 django_reportbroD/static/reportlib/src/rb_logo_dark.png
 django_reportbroD/static/reportlib/src/rb_logo_white.png
 django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
 django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
 django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
 django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
```

### Comparing `django-reportbroD-2.0/setup.cfg` & `django-reportbroD-3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = django-reportbroD
-version = 2.0
-description = A Django app to create and use ReportBro reports with a sample admin
+version = 3.0
+description = A Django app to create and use ReportBro reports with a sample admin. This allows you to generate yours reports using three options: by its code or name from database or JSON template.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Rider Raul Espinosa Perez
 author_email = riderraule@gmail.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
```

