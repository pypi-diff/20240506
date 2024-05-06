# Comparing `tmp/FreeTAKServer-UI-2.1.1.2.tar.gz` & `tmp/freetakserver_ui-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTAKServer-UI-2.1.1.2.tar", last modified: Sat Mar 30 17:01:31 2024, max compression
+gzip compressed data, was "freetakserver_ui-2.2.tar", max compression
```

## Comparing `FreeTAKServer-UI-2.1.1.2.tar` & `freetakserver_ui-2.2.tar`

### file list

```diff
@@ -1,291 +1,318 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.757290 FreeTAKServer-UI-2.1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.709291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.709291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.713291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.705291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.709291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.717291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)    34734 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/all.css
--rw-r--r--   0 runner    (1001) docker     (127)   402662 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)   833072 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   357341 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    31396 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/bootstrap-rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/css.css
--rw-r--r--   0 runner    (1001) docker     (127)    23450 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/global.css
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis.css
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_grey.css
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_red.css
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/nucleo-icons.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.717291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.css
--rw-r--r--   0 runner    (1001) docker     (127)    19033 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.717291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.721291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/
--rw-r--r--   0 runner    (1001) docker     (127)  1682267 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/12345.png
--rw-r--r--   0 runner    (1001) docker     (127)   261027 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/FreeTakServer3.png
--rw-r--r--   0 runner    (1001) docker     (127)    37930 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/anime3.png
--rw-r--r--   0 runner    (1001) docker     (127)    39891 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/anime6.png
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/apple-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   213199 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/bg5.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/default-avatar.png
--rw-r--r--   0 runner    (1001) docker     (127)    86218 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/emilyz.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)   670266 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/header.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    38381 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/img_3115.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    74556 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/james.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    76654 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/mike.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/now-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/spinner.svg
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/spinner1.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)   474593 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/charts/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    58031 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/moment/
--rw-r--r--   0 runner    (1001) docker     (127)    58862 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/moment/moment.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    15612 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   157844 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/perfect-scrollbar.jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   184656 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/socket.io-1.4.5.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.725291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/_typography.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.733291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_code.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_jumbotron.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_media.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_print.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    47781 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.737291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_background-variant.scss
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_float.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_nav-divider.scss
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_size.scss
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_text-emphasis.scss
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_text-hide.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_visibility.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.741291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_align.scss
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_background.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_float.scss
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_overflow.scss
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_screenreaders.scss
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_sizing.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_visibility.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.741291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.745291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_alerts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_example-pages.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)    18838 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    30622 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_white-content.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.745291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-map.scss
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-plain.scss
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-task.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-user.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_background-variant.scss
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_badges.scss
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_icon.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_modals.scss
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_page-header.scss
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/opacity.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_floating.scss
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_helper.scss
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_sizing.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_transform.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/base-site-rtl.html
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/base-site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/500.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.749291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/login/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/login/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.753291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/navigation-rtl.html
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/scripts-sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar-rtl.html
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.753291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.753291 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/about.html
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/configure.html
--rw-r--r--   0 runner    (1001) docker     (127)    22322 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/connect.html
--rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    29329 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/mission.html
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-403.html
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-404.html
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-500.html
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-blank.html
--rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-rtl-support.html
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-user.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/qr.html
--rw-r--r--   0 runner    (1001) docker     (127)    26090 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-icons.html
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-maps.html
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-notifications.html
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-tables.html
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-typography.html
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/users.html
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/webmap.html
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/gunicorn-cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.757290 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/test_selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:01:31.757290 FreeTAKServer-UI-2.1.1.2/FreeTAKServer_UI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-30 17:01:31.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer_UI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-03-30 17:01:31.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer_UI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 17:01:31.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer_UI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-30 17:01:31.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer_UI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 17:01:31.000000 FreeTAKServer-UI-2.1.1.2/FreeTAKServer_UI.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-30 17:01:31.757290 FreeTAKServer-UI-2.1.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1646 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-03-30 17:01:31.757290 FreeTAKServer-UI-2.1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-30 17:01:22.000000 FreeTAKServer-UI-2.1.1.2/setup.py
+-rw-r--r--   0        0        0       36 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/Procfile
+-rw-r--r--   0        0        0        0 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/__init__.py
+-rw-r--r--   0        0        0     3594 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/app/__init__.py
+-rw-r--r--   0        0        0      257 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/forms.py
+-rw-r--r--   0        0        0     1280 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/models.py
+-rw-r--r--   0        0        0     3236 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/routes.py
+-rw-r--r--   0        0        0    34734 2024-05-06 11:49:54.616629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/all.css
+-rw-r--r--   0        0        0   402662 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css
+-rw-r--r--   0        0        0   833072 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css.map
+-rw-r--r--   0        0        0   357341 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.min.css
+-rw-r--r--   0        0        0    31396 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/bootstrap-rtl.css
+-rw-r--r--   0        0        0     6078 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/css.css
+-rw-r--r--   0        0        0    23450 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/global.css
+-rw-r--r--   0        0        0     4507 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis.css
+-rw-r--r--   0        0        0     4608 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_grey.css
+-rw-r--r--   0        0        0     4558 2024-05-06 11:49:54.620629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_red.css
+-rw-r--r--   0        0        0     7743 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/nucleo-icons.css
+-rw-r--r--   0        0        0      904 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.css
+-rw-r--r--   0        0        0    19033 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.js
+-rw-r--r--   0        0        0    26524 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.eot
+-rw-r--r--   0        0        0    26364 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0        0        0    15168 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff
+-rw-r--r--   0        0        0    12616 2024-05-06 11:49:54.624629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0        0        0  1682267 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/12345.png
+-rw-r--r--   0        0        0   261027 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/FreeTakServer3.png
+-rw-r--r--   0        0        0    37930 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/anime3.png
+-rw-r--r--   0        0        0    39891 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/anime6.png
+-rw-r--r--   0        0        0     2446 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/apple-icon.png
+-rw-r--r--   0        0        0   213199 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/bg5.jpg
+-rw-r--r--   0        0        0     2864 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/default-avatar.png
+-rw-r--r--   0        0        0    86218 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/emilyz.jpg
+-rw-r--r--   0        0        0     2761 2024-05-06 11:49:54.628629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/favicon.png
+-rw-r--r--   0        0        0   670266 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/header.jpg
+-rw-r--r--   0        0        0    38381 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/img_3115.jpg
+-rw-r--r--   0        0        0    74556 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/james.jpg
+-rw-r--r--   0        0        0    76654 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/mike.jpg
+-rw-r--r--   0        0        0     8172 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/now-logo.png
+-rw-r--r--   0        0        0      671 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/spinner.svg
+-rw-r--r--   0        0        0      671 2024-05-06 11:49:54.632629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/spinner1.svg
+-rw-r--r--   0        0        0   474593 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/apexcharts.js
+-rw-r--r--   0        0        0     7296 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js
+-rw-r--r--   0        0        0     4474 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js.map
+-rw-r--r--   0        0        0     4540 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.min.js
+-rw-r--r--   0        0        0     1420 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/charts/apexcharts.js
+-rw-r--r--   0        0        0       15 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/config.js
+-rw-r--r--   0        0        0    58031 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0        0        0    86659 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/core/jquery.min.js
+-rw-r--r--   0        0        0    18994 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/core/popper.min.js
+-rw-r--r--   0        0        0      682 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/custom.js
+-rw-r--r--   0        0        0    58862 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/moment/moment.min.js
+-rw-r--r--   0        0        0    15612 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0        0        0   157844 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0        0        0    18292 2024-05-06 11:49:54.636629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0        0        0   184656 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/socket.io-1.4.5.js
+-rw-r--r--   0        0        0    48220 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/socket.io.min.js
+-rw-r--r--   0        0        0       30 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/_buttons.scss
+-rw-r--r--   0        0        0       40 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/_typography.scss
+-rw-r--r--   0        0        0     1148 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0        0        0     1119 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0        0        0     1278 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0        0        0     3624 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0        0        0     2547 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0        0        0     5872 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_card.scss
+-rw-r--r--   0        0        0     4756 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0        0        0      956 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_close.scss
+-rw-r--r--   0        0        0     1013 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_code.scss
+-rw-r--r--   0        0        0    14866 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss
+-rw-r--r--   0        0        0     4363 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0        0        0     8816 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0        0        0     2719 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0        0        0     1016 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0        0        0     1153 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_images.scss
+-rw-r--r--   0        0        0     5855 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_input-group.scss
+-rw-r--r--   0        0        0      405 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_jumbotron.scss
+-rw-r--r--   0        0        0     3752 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0        0        0       83 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_media.scss
+-rw-r--r--   0        0        0     1059 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0        0        0     5930 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0        0        0     2069 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0        0        0     6415 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0        0        0     1740 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0        0        0     4797 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0        0        0     3001 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_print.scss
+-rw-r--r--   0        0        0     1068 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0        0        0    11184 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0        0        0      572 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_root.scss
+-rw-r--r--   0        0        0     1051 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0        0        0     3520 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0        0        0      990 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0        0        0     2512 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0        0        0      261 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0        0        0     2244 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_type.scss
+-rw-r--r--   0        0        0      502 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0        0        0    47781 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0        0        0      572 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0        0        0      411 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0        0        0      920 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss
+-rw-r--r--   0        0        0      242 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0        0        0      474 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_background-variant.scss
+-rw-r--r--   0        0        0      318 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_badge.scss
+-rw-r--r--   0        0        0     1340 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0        0        0      532 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0        0        0     4482 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0        0        0     3369 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0        0        0     1406 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0        0        0       93 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0        0        0      613 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0        0        0      386 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_float.scss
+-rw-r--r--   0        0        0     4912 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0        0        0     2050 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0        0        0     1828 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss
+-rw-r--r--   0        0        0     1568 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0        0        0      749 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss
+-rw-r--r--   0        0        0     1159 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0        0        0      431 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0        0        0      168 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0        0        0      261 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_nav-divider.scss
+-rw-r--r--   0        0        0      462 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0        0        0      479 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0        0        0      202 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0        0        0      733 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss
+-rw-r--r--   0        0        0      148 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_size.scss
+-rw-r--r--   0        0        0      792 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss
+-rw-r--r--   0        0        0      364 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_text-emphasis.scss
+-rw-r--r--   0        0        0      326 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_text-hide.scss
+-rw-r--r--   0        0        0      168 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0        0        0      364 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0        0        0      189 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_visibility.scss
+-rw-r--r--   0        0        0      420 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_align.scss
+-rw-r--r--   0        0        0      397 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_background.scss
+-rw-r--r--   0        0        0     1765 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss
+-rw-r--r--   0        0        0       37 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_clearfix.scss
+-rw-r--r--   0        0        0      519 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss
+-rw-r--r--   0        0        0      846 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss
+-rw-r--r--   0        0        0     2769 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss
+-rw-r--r--   0        0        0      376 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_float.scss
+-rw-r--r--   0        0        0      133 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_overflow.scss
+-rw-r--r--   0        0        0      484 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_position.scss
+-rw-r--r--   0        0        0      115 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_screenreaders.scss
+-rw-r--r--   0        0        0      249 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_shadows.scss
+-rw-r--r--   0        0        0      498 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_sizing.scss
+-rw-r--r--   0        0        0     2101 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss
+-rw-r--r--   0        0        0      431 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_stretched-link.scss
+-rw-r--r--   0        0        0     2010 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss
+-rw-r--r--   0        0        0      174 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_visibility.scss
+-rw-r--r--   0        0        0     6473 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss
+-rw-r--r--   0        0        0     1600 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_alerts.scss
+-rw-r--r--   0        0        0     5032 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_buttons.scss
+-rw-r--r--   0        0        0     5098 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_card.scss
+-rw-r--r--   0        0        0     3645 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss
+-rw-r--r--   0        0        0     7600 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_dropdown.scss
+-rw-r--r--   0        0        0     4562 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_example-pages.scss
+-rw-r--r--   0        0        0     6861 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss
+-rw-r--r--   0        0        0     1406 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_footer.scss
+-rw-r--r--   0        0        0     2878 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_forms.scss
+-rw-r--r--   0        0        0      568 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_functions.scss
+-rw-r--r--   0        0        0      117 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_images.scss
+-rw-r--r--   0        0        0     7400 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_input-group.scss
+-rw-r--r--   0        0        0     3573 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_misc.scss
+-rw-r--r--   0        0        0      478 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_mixins.scss
+-rw-r--r--   0        0        0     2818 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_modal.scss
+-rw-r--r--   0        0        0     6140 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_navbar.scss
+-rw-r--r--   0        0        0     3400 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_rtl.scss
+-rw-r--r--   0        0        0    18838 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss
+-rw-r--r--   0        0        0     3458 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_tables.scss
+-rw-r--r--   0        0        0     2446 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_type.scss
+-rw-r--r--   0        0        0      309 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_utilities.scss
+-rw-r--r--   0        0        0    30622 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_variables.scss
+-rw-r--r--   0        0        0     6207 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_white-content.scss
+-rw-r--r--   0        0        0      981 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss
+-rw-r--r--   0        0        0       26 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-map.scss
+-rw-r--r--   0        0        0      270 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-plain.scss
+-rw-r--r--   0        0        0      421 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-task.scss
+-rw-r--r--   0        0        0     1703 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-user.scss
+-rw-r--r--   0        0        0      331 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_alert.scss
+-rw-r--r--   0        0        0      449 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_background-variant.scss
+-rw-r--r--   0        0        0      280 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_badges.scss
+-rw-r--r--   0        0        0     9533 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss
+-rw-r--r--   0        0        0      516 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss
+-rw-r--r--   0        0        0     2678 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_forms.scss
+-rw-r--r--   0        0        0      147 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_icon.scss
+-rw-r--r--   0        0        0     6389 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss
+-rw-r--r--   0        0        0      304 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_modals.scss
+-rw-r--r--   0        0        0      474 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_page-header.scss
+-rw-r--r--   0        0        0      687 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss
+-rw-r--r--   0        0        0     7224 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss
+-rw-r--r--   0        0        0      629 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss
+-rw-r--r--   0        0        0      152 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/opacity.scss
+-rw-r--r--   0        0        0      799 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss
+-rw-r--r--   0        0        0      809 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_floating.scss
+-rw-r--r--   0        0        0      816 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_helper.scss
+-rw-r--r--   0        0        0      242 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_position.scss
+-rw-r--r--   0        0        0      348 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_shadows.scss
+-rw-r--r--   0        0        0       64 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_sizing.scss
+-rw-r--r--   0        0        0     2039 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss
+-rw-r--r--   0        0        0      982 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_text.scss
+-rw-r--r--   0        0        0      276 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_transform.scss
+-rw-r--r--   0        0        0     3315 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss
+-rw-r--r--   0        0        0     2598 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss
+-rw-r--r--   0        0        0     2598 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss
+-rw-r--r--   0        0        0     3578 2024-05-06 11:49:54.640629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard.scss
+-rw-r--r--   0        0        0     2204 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/base-site-rtl.html
+-rw-r--r--   0        0        0     2665 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/base-site.html
+-rw-r--r--   0        0        0      759 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/errors/403.html
+-rw-r--r--   0        0        0      760 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/errors/404.html
+-rw-r--r--   0        0        0      767 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/errors/500.html
+-rw-r--r--   0        0        0     2349 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/login/login.html
+-rw-r--r--   0        0        0     2100 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/login/register.html
+-rw-r--r--   0        0        0     1587 2024-05-06 11:49:54.644629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/fixed-plugin.html
+-rw-r--r--   0        0        0        0 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/footer.html
+-rw-r--r--   0        0        0     4284 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/navigation-rtl.html
+-rw-r--r--   0        0        0     3079 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/navigation.html
+-rw-r--r--   0        0        0     3353 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/scripts-sidebar.html
+-rw-r--r--   0        0        0      976 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/scripts.html
+-rw-r--r--   0        0        0     2226 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar-rtl.html
+-rw-r--r--   0        0        0     1792 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar.html
+-rw-r--r--   0        0        0     1104 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/base/util.py
+-rw-r--r--   0        0        0      257 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/__init__.py
+-rw-r--r--   0        0        0     8074 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/routes.py
+-rw-r--r--   0        0        0     5689 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/about.html
+-rw-r--r--   0        0        0    17264 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/configure.html
+-rw-r--r--   0        0        0    22400 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/connect.html
+-rw-r--r--   0        0        0    25842 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/index.html
+-rw-r--r--   0        0        0    29407 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/mission.html
+-rw-r--r--   0        0        0       32 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-403.html
+-rw-r--r--   0        0        0       32 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-404.html
+-rw-r--r--   0        0        0       32 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-500.html
+-rw-r--r--   0        0        0      769 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-blank.html
+-rw-r--r--   0        0        0    14841 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-rtl-support.html
+-rw-r--r--   0        0        0     3337 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-user.html
+-rw-r--r--   0        0        0      188 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/qr.html
+-rw-r--r--   0        0        0    26090 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-icons.html
+-rw-r--r--   0        0        0      705 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-maps.html
+-rw-r--r--   0        0        0     5857 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-notifications.html
+-rw-r--r--   0        0        0     6793 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-tables.html
+-rw-r--r--   0        0        0     5914 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-typography.html
+-rw-r--r--   0        0        0    14428 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/users.html
+-rw-r--r--   0        0        0      662 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/webmap.html
+-rw-r--r--   0        0        0     2757 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/config.py
+-rw-r--r--   0        0        0      243 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/db.json
+-rw-r--r--   0        0        0      276 2024-05-06 11:49:54.648629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/bin/easy_install
+-rw-r--r--   0        0        0  4526456 2024-05-06 11:49:54.672629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/bin/python3
+-rw-r--r--   0        0        0    22274 2024-05-06 11:49:54.672629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/include/python3.6m/Python-ast.h
+-rw-r--r--   0        0        0     1966 2024-05-06 11:49:54.672629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/include/python3.6m/graminit.h
+-rw-r--r--   0        0        0      513 2024-05-06 11:49:54.672629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/include/python3.6m/intrcheck.h
+-rw-r--r--   0        0        0      291 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/include/python3.6m/osmodule.h
+-rw-r--r--   0        0        0     2036 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/config-3.6m-x86_64-linux-gnu/python-config.py
+-rw-r--r--   0        0        0    13557 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/encodings/iso8859_16.py
+-rw-r--r--   0        0        0    13404 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/encodings/iso8859_2.py
+-rw-r--r--   0        0        0    15170 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/encodings/mac_farsi.py
+-rw-r--r--   0        0        0      946 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/encodings/utf_7.py
+-rw-r--r--   0        0        0        4 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/Flask_Migrate-2.5.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0    30041 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/SQLAlchemy-1.3.16.dist-info/RECORD
+-rw-r--r--   0        0        0     7040 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/Werkzeug-1.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0     5721 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/alembic/autogenerate/rewriter.py
+-rw-r--r--   0        0        0        8 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/alembic-1.4.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0      444 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/dateutil/tz/__init__.py
+-rw-r--r--   0        0        0     3753 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/dns/e164.py
+-rw-r--r--   0        0        0     1319 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/dns/hash.py
+-rw-r--r--   0        0        0      950 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/dns/rdtypes/ANY/NS.py
+-rw-r--r--   0        0        0     4597 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/dns/rdtypes/ANY/SOA.py
+-rw-r--r--   0        0        0      813 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/flask_login/_compat.py
+-rw-r--r--   0        0        0     2223 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/flask_login/signals.py
+-rw-r--r--   0        0        0     2916 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/flask_migrate/templates/flask/env.py
+-rw-r--r--   0        0        0     1390 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/flask_sqlalchemy/utils.py
+-rw-r--r--   0        0        0     6126 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/gunicorn/workers/ggevent.py
+-rw-r--r--   0        0        0     1565 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/idna-2.9.dist-info/LICENSE.rst
+-rw-r--r--   0        0        0      495 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     2774 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0    10766 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    40452 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0     3592 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0        0        0     7476 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0        0        0      744 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0     1138 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0      562 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0     8248 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0   226313 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0        0        0      558 2024-05-06 11:49:54.676629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0     2233 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/python_editor-1.0.4.dist-info/METADATA
+-rw-r--r--   0        0        0    15130 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0      524 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     4659 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3970 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/sqlalchemy/dialects/mysql/zxjdbc.py
+-rw-r--r--   0        0        0     1363 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/sqlalchemy/dialects/sybase/__init__.py
+-rw-r--r--   0        0        0    31820 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/sqlalchemy/ext/mutable.py
+-rw-r--r--   0        0        0    14371 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/werkzeug/local.py
+-rw-r--r--   0        0        0     2240 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/werkzeug/middleware/dispatcher.py
+-rw-r--r--   0        0        0     5714 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/wtforms/locale/et/LC_MESSAGES/wtforms.po
+-rw-r--r--   0        0        0     4389 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/wtforms/locale/wtforms.pot
+-rw-r--r--   0        0        0     3436 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/wtforms/locale/zh/LC_MESSAGES/wtforms.mo
+-rw-r--r--   0        0        0     3231 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/site-packages/wtforms/locale/zh_TW/LC_MESSAGES/wtforms.mo
+-rw-r--r--   0        0        0    29496 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/env1/lib/python3.6/tokenize.py
+-rw-r--r--   0        0        0      218 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/gunicorn-cfg.py
+-rw-r--r--   0        0        0       38 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/README
+-rw-r--r--   0        0        0        0 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/__init__.py
+-rw-r--r--   0        0        0      770 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/alembic.ini
+-rw-r--r--   0        0        0     2979 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/env.py
+-rw-r--r--   0        0        0      494 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/script.py.mako
+-rw-r--r--   0        0        0      920 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/versions/6b6aa97e1b29_.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/migrations/versions/__init__.py
+-rw-r--r--   0        0        0    46235 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/package-lock.json
+-rw-r--r--   0        0        0      576 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/package.json
+-rw-r--r--   0        0        0     4492 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/run.py
+-rw-r--r--   0        0        0        5 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/test
+-rw-r--r--   0        0        0       87 2024-05-06 11:49:54.680629 freetakserver_ui-2.2/FreeTAKServer-UI/tests/__init__.py
+-rw-r--r--   0        0        0  7874704 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/FreeTAKServer-UI/tests/chromedriver
+-rw-r--r--   0        0        0     1910 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/FreeTAKServer-UI/tests/conftest.py
+-rw-r--r--   0        0        0     2770 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/FreeTAKServer-UI/tests/test_base.py
+-rw-r--r--   0        0        0      584 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/FreeTAKServer-UI/tests/test_example.py
+-rw-r--r--   0        0        0      531 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/FreeTAKServer-UI/tests/test_selenium.py
+-rwxr-xr-x   0        0        0     1100 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/LICENSE.md
+-rwxr-xr-x   0        0        0     1646 2024-05-06 11:49:54.720629 freetakserver_ui-2.2/README.md
+-rw-r--r--   0        0        0      988 2024-05-06 11:49:54.724629 freetakserver_ui-2.2/pyproject.toml
+-rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 freetakserver_ui-2.2/PKG-INFO
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/__init__.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 def register_blueprints(app):
     for module_name in ('base', 'home'):
         module = import_module('app.{}.routes'.format(module_name))
         app.register_blueprint(module.blueprint)
 
 def configure_database(app):
 
-    @app.before_first_request
+    @app.before_request
     def initialize_database():
+        # Only run this once, and then remove the funtion. 
+        app.before_request_funcs[None].remove(initialize_database)
         db.create_all()
 
     @app.teardown_request
     def shutdown_session(exception=None):
         db.session.remove()
 
 def configure_logs(app):
@@ -84,15 +86,15 @@
     CORS(app, origins=[api_uri, webmap_uri])
     
     #if database_exists(app.config['SQLALCHEMY_DATABASE_URI']) == False:
     #    raise Exception("Database does not exist, check your DataBase path and ensure that you've started FTS")
     # UI configuration
     # UI version DO NOT modify it
     
-    app.config['UIVERSION'] = '2.1.1.1'
+    app.config['UIVERSION'] = '2.2'
 
     # number of milliseconds to query FTS for connected Users, health, a System status
     app.config['USERINTERVAL'] = '180000';
     app.config['SERVERHEALTHINTERVAL'] = '180000';
     app.config['SYSSTATUSINTERVAL'] = '600000';
     app.config['DATAPACKAGESIZELIMIT'] = '15360000';
     if selenium:
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/forms.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/forms.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/models.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- encoding: utf-8 -*-
 """
 License: MIT
 Copyright (c) 2019 - present AppSeed.us
 """
 
 from flask_login import UserMixin
-from sqlalchemy import Binary, Column, Integer, String
+from sqlalchemy import Column, Integer, String
 
 from app import db, login_manager
 
 from app.base.util import hash_pass
 
 class User(db.Model, UserMixin):
     __tablename__ = 'user'
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/routes.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from app import db, login_manager
 from app.base import blueprint
 from app.base.forms import LoginForm, CreateAccountForm
 from app.base.models import User
 from flask import current_app as app
 from app.base.util import verify_pass
+from requests.exceptions import ConnectionError
 
 @blueprint.route('/')
 def route_default():
     return redirect(url_for('base_blueprint.login'))
 
 @blueprint.route('/error-<error>')
 def route_errors(error):
@@ -35,15 +36,18 @@
     if 'login' in request.form:
         import requests
         # read form data
         username = request.form['username']
         password = request.form['password']
 
         # Locate user
-        user = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/AuthenticateUser", params={"username": username, "password": password}, headers={"Authorization": f"{app.config['APIKEY']}"})
+        try:
+            user = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/AuthenticateUser", params={"username": username, "password": password}, headers={"Authorization": f"{app.config['APIKEY']}"})
+        except ConnectionError:
+            return render_template('login/login.html', msg=f'FTS Server is not reachable at {app.config.get("IP", "IP NOT SET!")}', form=login_form)
         try:
             user = user.json()
         except:
             return render_template('login/login.html', msg='Wrong user or password', form=login_form)
         
         # Check the password
         if user:
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/all.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/all.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css.map` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.min.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/black-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/bootstrap-rtl.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/bootstrap-rtl.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/css.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/css.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/global.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/global.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_grey.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_grey.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_red.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/jarvis_red.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/css/nucleo-icons.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.css` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.css`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/demo/demo.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.eot` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.ttf` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff2` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/12345.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/12345.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/FreeTakServer3.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/FreeTakServer3.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/anime3.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/anime3.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/anime6.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/anime6.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/apple-icon.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/apple-icon.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/bg5.jpg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/bg5.jpg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/default-avatar.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/default-avatar.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/emilyz.jpg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/emilyz.jpg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/favicon.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/favicon.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/header.jpg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/header.jpg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/img_3115.jpg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/img_3115.jpg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/james.jpg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/james.jpg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/mike.jpg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/mike.jpg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/now-logo.png` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/now-logo.png`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/spinner.svg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/spinner.svg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/img/spinner1.svg` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/img/spinner1.svg`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/apexcharts.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js.map` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/black-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/charts/apexcharts.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/charts/apexcharts.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/bootstrap.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/jquery.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/core/popper.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/custom.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/custom.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/moment/moment.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/bootstrap-notify.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/chartjs.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/perfect-scrollbar.jquery.min.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/plugins/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/js/socket.io-1.4.5.js` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/js/socket.io-1.4.5.js`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_alert.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_badge.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_button-group.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_buttons.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_card.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_carousel.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_close.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_code.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_code.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_forms.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_forms.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_functions.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_grid.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_images.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_input-group.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_input-group.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_list-group.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_mixins.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_modal.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_nav.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_navbar.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_pagination.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_popover.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_print.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_print.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_progress.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_reboot.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_root.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_spinners.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tables.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_toasts.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_type.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_variables.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_box-shadow.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_alerts.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_alerts.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_buttons.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_buttons.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_card.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_card.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_checkboxes-radio.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_dropdown.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_example-pages.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_example-pages.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_footer.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_footer.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_forms.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_forms.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_functions.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_functions.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_input-group.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_input-group.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_misc.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_misc.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_modal.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_modal.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_navbar.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_navbar.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_rtl.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_rtl.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_sidebar-and-main-panel.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_tables.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_tables.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_type.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_type.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_variables.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_variables.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_white-content.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/_white-content.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-chart.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-user.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/cards/_card-user.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_forms.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_inputs.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_popovers.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_vendor-prefixes.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/mixins/_wizard.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_backgrounds.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_floating.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_floating.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_helper.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_helper.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_text.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-animate-bootstrap-notify.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/custom/vendor/_plugin-perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard/plugins/_plugin-perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard.scss` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/static/assets/scss/black-dashboard.scss`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/base-site-rtl.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/base-site-rtl.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/base-site.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/base-site.html`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 		<!--     Fonts and icons     -->
 		<link href="/static/assets/css/css.css" rel="stylesheet" />
 		<link href="/static/assets/css/all.css" rel="stylesheet" />
 		<!-- Nucleo Icons -->
 		<link href="/static/assets/css/nucleo-icons.css" rel="stylesheet" />
 		<!-- CSS Files -->
 		<link href="/static/assets/css/black-dashboard.css?v=1.0.10" rel="stylesheet" />
-		<script src="/static/assets/js/socket.io-1.4.5.js"></script>
+		<script src="/static/assets/js/socket.io.min.js"></script>
 		<script>
 			document.write('<link href="/static/assets/css/jarvis.css?r=' + Math.floor(Math.random() * 100) + '" rel="stylesheet" type="text/css" />');
 			document.write('<link href="/static/assets/css/jarvis_red.css?r=' + Math.floor(Math.random() * 100) + '" rel="stylesheet" type="text/css" />');
 			document.write('<link href="/static/assets/css/jarvis_grey.css?r=' + Math.floor(Math.random() * 100) + '" rel="stylesheet" type="text/css" />');
 			document.write('<link href="/static/assets/css/global.css?r=' + Math.floor(Math.random() * 100) + '" rel="stylesheet" type="text/css" />');
 		</script>
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/403.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/404.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/errors/500.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/errors/500.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/login/login.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/login/login.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/login/register.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/login/register.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/fixed-plugin.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/fixed-plugin.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/navigation-rtl.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/navigation-rtl.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/navigation.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/navigation.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/scripts-sidebar.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/scripts-sidebar.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/scripts.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/scripts.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar-rtl.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar-rtl.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/templates/site_template/sidebar.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/base/util.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/base/util.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/routes.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from app import login_manager
 from jinja2 import TemplateNotFound
 import requests
 from flask import current_app as app
 from app.base.forms import UpdateAccountForm
 from app.base.models import User
 from app import db
+from requests.exceptions import ConnectionError
 
 @login_manager.user_loader
 def load_user(user_id):
     return User.query.filter_by(uid=user_id).first()
 
 @blueprint.route('/index')
 @login_required
@@ -59,14 +60,24 @@
 
     try:
         outgoing_federation_json_data = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/FederationTable", headers= headers).json()
     except Exception as e:
         print(e)
         outgoing_federation_json_data = {'federations': []}
    
+    try:
+        requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}", headers= headers)
+    except ConnectionError:
+        return render_template('mission.html', msg=f'FTS Server is not reachable at {app.config.get("IP", "IP NOT SET!")}', segment="mission", 
+                                json_data = {},
+                                mission_json_data = {'data': []},
+                                excheck_json_data = {},
+                                outgoing_federation_json_data = {'federations': []},
+                                websocketkey=app.config['WEBSOCKETKEY'], apikey=app.config['APIKEY'], port=app.config['PORT'], protocol=app.config['PROTOCOL'], ip=app.config['IP'])
+
     return render_template('mission.html', json_data = json_data['json_list'], 
     mission_json_data = mission_json_data['data'],
     excheck_json_data = excheck_json_data['data'][0]['contents'],
     outgoing_federation_json_data = outgoing_federation_json_data['federations'],
     segment = "mission",
     websocketkey=app.config['WEBSOCKETKEY'], apikey=app.config['APIKEY'], port=app.config['PORT'], protocol=app.config['PROTOCOL'], ip=app.config['IP'],
     datapackagesizelimit=app.config['DATAPACKAGESIZELIMIT']
@@ -77,26 +88,36 @@
 
 
 
 @blueprint.route('/connect')
 @login_required
 def connectApi():
     headers = {'Authorization': app.config['APIKEY']}
-    json_data = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/ManageEmergency/getEmergency", headers= headers)
+    try:
+        json_data = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/ManageEmergency/getEmergency", headers= headers)
+    except ConnectionError:
+        return render_template('connect.html', msg=f'FTS Server is not reachable at {app.config.get("IP", "IP NOT SET!")}', segment="connect", 
+                                json_data = {'json_list': []},
+                                websocketkey=app.config['WEBSOCKETKEY'], apikey=app.config['APIKEY'], port=app.config['PORT'], protocol=app.config['PROTOCOL'], ip=app.config['IP'])
     json_data = json_data.json()
     
     return render_template('connect.html', json_data = json_data['json_list'], segment="connect",
     websocketkey=app.config['WEBSOCKETKEY'], apikey=app.config['APIKEY'], port=app.config['PORT'], protocol=app.config['PROTOCOL'], ip=app.config['IP'])     
 
 
 @blueprint.route('/configure')
 @login_required
 def configureApi():
     headers = {'Authorization': app.config['APIKEY']}
-    outgoing_federation_json_data = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/FederationTable", headers= headers).json()
+    try:
+        outgoing_federation_json_data = requests.get(f"{app.config['PROTOCOL']}://{app.config['IP']}:{app.config['PORT']}/FederationTable", headers= headers).json()
+    except ConnectionError:
+        return render_template('configure.html', msg=f'FTS Server is not reachable at {app.config.get("IP", "IP NOT SET!")}', segment="configure", 
+                                outgoing_federation_json_data = {'federations': []},
+                                websocketkey=app.config['WEBSOCKETKEY'], apikey=app.config['APIKEY'], port=app.config['PORT'], protocol=app.config['PROTOCOL'], ip=app.config['IP'])
 
     return render_template('configure.html', segment="configure", 
     outgoing_federation_json_data = outgoing_federation_json_data['federations'],
     websocketkey=app.config['WEBSOCKETKEY'], apikey=app.config['APIKEY'], port=app.config['PORT'], protocol=app.config['PROTOCOL'], ip=app.config['IP'])
 
 @blueprint.route('/users')
 @login_required
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/about.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/about.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/configure.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/configure.html`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 	
 </div>
 
 
 
 
 </div>
-<div id="snackbar">&nbsp;</div>
+<div id="snackbar" {{'class=show' if msg is defined else ''}}>{{ msg if msg is defined else '&nbsp;' }}</div>
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
 
 
 <script>
```

#### html2text {}

```diff
@@ -34,10 +34,10 @@
 Fallback
 {% for items in outgoing_federation_json_data %}
 {{items['name']}}
 {% endfor %}
 [One of: Enabled/Disabled]
  
 Apply
- 
+{'class=show' if msg is defined else ''}}>{{ msg if msg is defined else ' ' }}
 {% endblock content %} {% block javascripts %}
 {% endblock javascripts %}
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/connect.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/connect.html`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 						</div>
 					</div>
 				</div>
 			</div>
 		</div>
 	</div>
 </div>
-<div id="snackbar">&nbsp;</div>
+<div id="snackbar" {{'class=show' if msg is defined else ''}}>{{ msg if msg is defined else '&nbsp;' }}</div>
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/index.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/index.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/mission.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/mission.html`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 			<button class="btn btn-simple btn-twitter" onclick="addOF()" style="color: #278aed; border-color: #278aed">Submit</button>
 		</div>
 	</div>
 
 
 </div>
 
-<div id="snackbar">&nbsp;</div>
+<div id="snackbar" {{'class=show' if msg is defined else ''}}>{{ msg if msg is defined else '&nbsp;' }}</div>
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
 
 <script>
```

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-blank.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-blank.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-rtl-support.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-rtl-support.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/page-user.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/page-user.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-icons.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-icons.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-maps.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-maps.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-notifications.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-notifications.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-tables.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-tables.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/ui-typography.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/ui-typography.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/users.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/users.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/app/home/templates/webmap.html` & `freetakserver_ui-2.2/FreeTAKServer-UI/app/home/templates/webmap.html`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/config.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/config.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/run.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/run.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/conftest.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/test_base.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/test_example.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/FreeTAKServer-UI/tests/test_selenium.py` & `freetakserver_ui-2.2/FreeTAKServer-UI/tests/test_selenium.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/LICENSE.md` & `freetakserver_ui-2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-UI-2.1.1.2/README.md` & `freetakserver_ui-2.2/README.md`

 * *Files identical despite different names*

