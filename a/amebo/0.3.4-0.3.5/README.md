# Comparing `tmp/amebo-0.3.4.tar.gz` & `tmp/amebo-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amebo-0.3.4.tar", max compression
+gzip compressed data, was "amebo-0.3.5.tar", max compression
```

## Comparing `amebo-0.3.4.tar` & `amebo-0.3.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     7394 2024-05-05 03:08:04.783226 amebo-0.3.4/README.md
--rw-r--r--   0        0        0      283 2024-05-05 15:52:56.734898 amebo-0.3.4/amebo/.env
--rw-r--r--   0        0        0       31 2024-05-06 12:13:57.406339 amebo-0.3.4/amebo/__init__.py
--rwxr-xr-x   0        0        0       43 2024-05-06 12:14:43.168051 amebo-0.3.4/amebo/amebo.sh
--rw-r--r--   0        0        0      773 2024-04-23 13:58:53.898443 amebo-0.3.4/amebo/amebo_readers.py
--rw-r--r--   0        0        0      844 2023-09-06 17:31:38.136649 amebo-0.3.4/amebo/amebo_writers.py
--rw-r--r--   0        0        0     2571 2024-05-06 11:49:29.177002 amebo-0.3.4/amebo/aproko.py
--rw-r--r--   0        0        0        0 2024-05-06 11:40:37.932901 amebo-0.3.4/amebo/constants/__init__.py
--rw-r--r--   0        0        0      129 2024-04-23 10:53:18.032385 amebo-0.3.4/amebo/constants/literals.py
--rw-r--r--   0        0        0     1955 2023-09-06 17:31:38.141358 amebo-0.3.4/amebo/constants/scripts.py
--rw-r--r--   0        0        0        0 2024-05-06 11:40:46.525615 amebo-0.3.4/amebo/controllers/__init__.py
--rw-r--r--   0        0        0     2796 2024-05-06 11:48:00.171264 amebo-0.3.4/amebo/controllers/actions.py
--rw-r--r--   0        0        0      412 2024-04-23 14:07:10.599429 amebo-0.3.4/amebo/controllers/app.py
--rw-r--r--   0        0        0     3895 2024-05-06 11:48:58.620551 amebo-0.3.4/amebo/controllers/events.py
--rw-r--r--   0        0        0     4558 2024-05-06 11:48:56.511645 amebo-0.3.4/amebo/controllers/gists.py
--rw-r--r--   0        0        0     4971 2024-05-06 11:50:14.065121 amebo-0.3.4/amebo/controllers/microservices.py
--rw-r--r--   0        0        0     2874 2024-05-06 11:50:26.656940 amebo-0.3.4/amebo/controllers/subscribers.py
--rw-r--r--   0        0        0        0 2024-05-06 11:40:52.710933 amebo-0.3.4/amebo/decorators/__init__.py
--rw-r--r--   0        0        0     1634 2024-05-06 11:50:33.529261 amebo-0.3.4/amebo/decorators/formatters.py
--rw-r--r--   0        0        0     1899 2024-05-06 11:49:06.630283 amebo-0.3.4/amebo/decorators/providers.py
--rw-r--r--   0        0        0      593 2024-04-23 10:39:57.541079 amebo-0.3.4/amebo/decorators/security.py
--rw-r--r--   0        0        0     4196 2023-09-06 17:31:38.137961 amebo-0.3.4/amebo/dist/amebo-0.1.1-py3-none-any.whl
--rw-r--r--   0        0        0     4013 2023-09-06 17:31:38.138160 amebo-0.3.4/amebo/dist/amebo-0.1.1.tar.gz
--rw-r--r--   0        0        0     4258 2023-09-06 17:31:38.138307 amebo-0.3.4/amebo/dist/amebo-0.1.2-py3-none-any.whl
--rw-r--r--   0        0        0     4068 2023-09-06 17:31:38.138496 amebo-0.3.4/amebo/dist/amebo-0.1.2.tar.gz
--rw-r--r--   0        0        0     4931 2024-05-06 10:43:40.490726 amebo-0.3.4/amebo/dist/amebo-0.2.0-py3-none-any.whl
--rw-r--r--   0        0        0     4509 2024-05-06 10:43:40.425293 amebo-0.3.4/amebo/dist/amebo-0.2.0.tar.gz
--rw-r--r--   0        0        0     4936 2024-05-06 11:26:51.191205 amebo-0.3.4/amebo/dist/amebo-0.3.0-py3-none-any.whl
--rw-r--r--   0        0        0     4514 2024-05-06 11:26:51.126554 amebo-0.3.4/amebo/dist/amebo-0.3.0.tar.gz
--rw-r--r--   0        0        0     1316 2024-05-06 09:35:11.528350 amebo-0.3.4/amebo/engines.py
--rw-r--r--   0        0        0      735 2023-08-28 08:37:12.552639 amebo-0.3.4/amebo/entities.py
--rw-r--r--   0        0        0     1326 2023-09-06 17:31:38.138962 amebo-0.3.4/amebo/handlers.py
--rw-r--r--   0        0        0      244 2024-05-06 12:27:58.988598 amebo-0.3.4/amebo/main.py
--rw-r--r--   0        0        0        0 2024-04-23 10:24:36.287481 amebo-0.3.4/amebo/middleware.py
--rw-r--r--   0        0        0        0 2024-05-06 11:41:02.497626 amebo-0.3.4/amebo/middlewares/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-06 12:33:27.089773 amebo-0.3.4/amebo/middlewares/database.py
--rw-r--r--   0        0        0      604 2024-04-23 13:28:24.231735 amebo-0.3.4/amebo/middlewares/security.py
--rw-r--r--   0        0        0      465 2024-04-23 13:24:59.563293 amebo-0.3.4/amebo/middlewares/setup.py
--rw-r--r--   0        0        0      704 2024-04-23 10:51:13.107504 amebo-0.3.4/amebo/models/actions.py
--rw-r--r--   0        0        0      726 2024-05-05 19:28:21.684796 amebo-0.3.4/amebo/models/events.py
--rw-r--r--   0        0        0      793 2024-05-05 16:53:56.861747 amebo-0.3.4/amebo/models/microservices.py
--rw-r--r--   0        0        0      553 2024-05-06 11:51:13.036509 amebo-0.3.4/amebo/models/subscribers.py
--rw-r--r--   0        0        0     1727 2023-08-28 08:37:12.553078 amebo-0.3.4/amebo/public/all.css
--rw-r--r--   0        0        0    41352 2023-08-28 08:37:12.553310 amebo-0.3.4/amebo/public/alpine.min.js
--rw-r--r--   0        0        0   353976 2024-05-05 20:04:17.923681 amebo-0.3.4/amebo/public/amebo.webp
--rw-r--r--   0        0        0   207302 2023-08-28 08:37:12.553825 amebo-0.3.4/amebo/public/bulma.min.css
--rw-r--r--   0        0        0     1436 2024-05-06 01:03:14.589179 amebo-0.3.4/amebo/public/heaven.css
--rw-r--r--   0        0        0      219 2023-08-28 08:37:12.553994 amebo-0.3.4/amebo/public/icons/add.svg
--rw-r--r--   0        0        0      697 2023-08-28 08:37:12.554083 amebo-0.3.4/amebo/public/icons/bulb.svg
--rw-r--r--   0        0        0      732 2023-08-28 08:37:12.554165 amebo-0.3.4/amebo/public/icons/ear.svg
--rw-r--r--   0        0        0      354 2023-08-28 08:37:12.554249 amebo-0.3.4/amebo/public/icons/flash-outline.svg
--rw-r--r--   0        0        0      842 2023-08-28 08:37:12.554329 amebo-0.3.4/amebo/public/icons/hardware-chip.svg
--rw-r--r--   0        0        0      356 2023-08-28 08:37:12.554396 amebo-0.3.4/amebo/public/icons/leaf-outline.svg
--rw-r--r--   0        0        0      936 2023-08-28 08:37:12.554476 amebo-0.3.4/amebo/public/icons/megaphone.svg
--rw-r--r--   0        0        0      370 2023-08-28 08:37:12.554547 amebo-0.3.4/amebo/public/icons/search.svg
--rw-r--r--   0        0        0      390 2023-08-28 08:37:12.554629 amebo-0.3.4/amebo/public/icons/send.svg
--rw-r--r--   0        0        0    15633 2023-08-28 08:37:12.554736 amebo-0.3.4/amebo/public/toastify.js
--rw-r--r--   0        0        0     1096 2023-08-28 08:37:12.554827 amebo-0.3.4/amebo/public/toastify.min.css
--rw-r--r--   0        0        0     2300 2024-05-06 12:30:52.996148 amebo-0.3.4/amebo/router.py
--rw-r--r--   0        0        0       23 2024-04-23 12:52:10.324095 amebo-0.3.4/amebo/templates/404.html
--rw-r--r--   0        0        0     5713 2024-05-05 20:37:01.462002 amebo-0.3.4/amebo/templates/abase.axml
--rw-r--r--   0        0        0     2778 2024-05-05 20:28:32.119659 amebo-0.3.4/amebo/templates/actions.axml
--rw-r--r--   0        0        0     9310 2024-05-06 01:09:36.957047 amebo-0.3.4/amebo/templates/actions.html
--rw-r--r--   0        0        0     6923 2024-05-05 20:29:00.671201 amebo-0.3.4/amebo/templates/events.html
--rw-r--r--   0        0        0     9424 2024-05-05 16:50:34.675416 amebo-0.3.4/amebo/templates/functions.axml
--rw-r--r--   0        0        0     6502 2023-08-28 08:37:12.555959 amebo-0.3.4/amebo/templates/gists.html
--rw-r--r--   0        0        0     4851 2023-09-06 17:31:38.143027 amebo-0.3.4/amebo/templates/login.html
--rw-r--r--   0        0        0     1017 2023-08-28 08:37:12.556082 amebo-0.3.4/amebo/templates/logs.html
--rw-r--r--   0        0        0     5432 2024-05-05 16:41:53.599815 amebo-0.3.4/amebo/templates/microservices.html
--rw-r--r--   0        0        0     1875 2024-05-05 16:59:06.725863 amebo-0.3.4/amebo/templates/scripts.axml
--rw-r--r--   0        0        0     4888 2023-08-28 08:37:12.556334 amebo-0.3.4/amebo/templates/subscribers.html
--rw-r--r--   0        0        0     1261 2024-05-06 11:52:36.970476 amebo-0.3.4/amebo/utils/helpers.py
--rw-r--r--   0        0        0     1161 2024-04-23 10:52:26.352293 amebo-0.3.4/amebo/utils/structs.py
--rw-r--r--   0        0        0      558 2024-05-06 12:33:37.605795 amebo-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     8142 1970-01-01 00:00:00.000000 amebo-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     7394 2024-05-05 03:08:04.783226 amebo-0.3.5/README.md
+-rw-r--r--   0        0        0      283 2024-05-05 15:52:56.734898 amebo-0.3.5/amebo/.env
+-rw-r--r--   0        0        0       31 2024-05-06 12:13:57.406339 amebo-0.3.5/amebo/__init__.py
+-rwxr-xr-x   0        0        0       43 2024-05-06 12:14:43.168051 amebo-0.3.5/amebo/amebo.sh
+-rw-r--r--   0        0        0      773 2024-04-23 13:58:53.898443 amebo-0.3.5/amebo/amebo_readers.py
+-rw-r--r--   0        0        0      844 2023-09-06 17:31:38.136649 amebo-0.3.5/amebo/amebo_writers.py
+-rw-r--r--   0        0        0     2571 2024-05-06 11:49:29.177002 amebo-0.3.5/amebo/aproko.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:40:37.932901 amebo-0.3.5/amebo/constants/__init__.py
+-rw-r--r--   0        0        0      129 2024-04-23 10:53:18.032385 amebo-0.3.5/amebo/constants/literals.py
+-rw-r--r--   0        0        0     1955 2023-09-06 17:31:38.141358 amebo-0.3.5/amebo/constants/scripts.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:40:46.525615 amebo-0.3.5/amebo/controllers/__init__.py
+-rw-r--r--   0        0        0     2796 2024-05-06 11:48:00.171264 amebo-0.3.5/amebo/controllers/actions.py
+-rw-r--r--   0        0        0      412 2024-04-23 14:07:10.599429 amebo-0.3.5/amebo/controllers/app.py
+-rw-r--r--   0        0        0     3895 2024-05-06 11:48:58.620551 amebo-0.3.5/amebo/controllers/events.py
+-rw-r--r--   0        0        0     4558 2024-05-06 11:48:56.511645 amebo-0.3.5/amebo/controllers/gists.py
+-rw-r--r--   0        0        0     4971 2024-05-06 11:50:14.065121 amebo-0.3.5/amebo/controllers/microservices.py
+-rw-r--r--   0        0        0     2874 2024-05-06 11:50:26.656940 amebo-0.3.5/amebo/controllers/subscribers.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:40:52.710933 amebo-0.3.5/amebo/decorators/__init__.py
+-rw-r--r--   0        0        0     1634 2024-05-06 11:50:33.529261 amebo-0.3.5/amebo/decorators/formatters.py
+-rw-r--r--   0        0        0     1899 2024-05-06 11:49:06.630283 amebo-0.3.5/amebo/decorators/providers.py
+-rw-r--r--   0        0        0      593 2024-04-23 10:39:57.541079 amebo-0.3.5/amebo/decorators/security.py
+-rw-r--r--   0        0        0     4196 2023-09-06 17:31:38.137961 amebo-0.3.5/amebo/dist/amebo-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0     4013 2023-09-06 17:31:38.138160 amebo-0.3.5/amebo/dist/amebo-0.1.1.tar.gz
+-rw-r--r--   0        0        0     4258 2023-09-06 17:31:38.138307 amebo-0.3.5/amebo/dist/amebo-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0     4068 2023-09-06 17:31:38.138496 amebo-0.3.5/amebo/dist/amebo-0.1.2.tar.gz
+-rw-r--r--   0        0        0     4931 2024-05-06 10:43:40.490726 amebo-0.3.5/amebo/dist/amebo-0.2.0-py3-none-any.whl
+-rw-r--r--   0        0        0     4509 2024-05-06 10:43:40.425293 amebo-0.3.5/amebo/dist/amebo-0.2.0.tar.gz
+-rw-r--r--   0        0        0     4936 2024-05-06 11:26:51.191205 amebo-0.3.5/amebo/dist/amebo-0.3.0-py3-none-any.whl
+-rw-r--r--   0        0        0     4514 2024-05-06 11:26:51.126554 amebo-0.3.5/amebo/dist/amebo-0.3.0.tar.gz
+-rw-r--r--   0        0        0     1316 2024-05-06 09:35:11.528350 amebo-0.3.5/amebo/engines.py
+-rw-r--r--   0        0        0      735 2023-08-28 08:37:12.552639 amebo-0.3.5/amebo/entities.py
+-rw-r--r--   0        0        0     1326 2023-09-06 17:31:38.138962 amebo-0.3.5/amebo/handlers.py
+-rw-r--r--   0        0        0      244 2024-05-06 12:27:58.988598 amebo-0.3.5/amebo/main.py
+-rw-r--r--   0        0        0        0 2024-04-23 10:24:36.287481 amebo-0.3.5/amebo/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:02.497626 amebo-0.3.5/amebo/middlewares/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-06 12:33:27.089773 amebo-0.3.5/amebo/middlewares/database.py
+-rw-r--r--   0        0        0      604 2024-04-23 13:28:24.231735 amebo-0.3.5/amebo/middlewares/security.py
+-rw-r--r--   0        0        0      465 2024-04-23 13:24:59.563293 amebo-0.3.5/amebo/middlewares/setup.py
+-rw-r--r--   0        0        0      704 2024-04-23 10:51:13.107504 amebo-0.3.5/amebo/models/actions.py
+-rw-r--r--   0        0        0      726 2024-05-05 19:28:21.684796 amebo-0.3.5/amebo/models/events.py
+-rw-r--r--   0        0        0      793 2024-05-05 16:53:56.861747 amebo-0.3.5/amebo/models/microservices.py
+-rw-r--r--   0        0        0      553 2024-05-06 11:51:13.036509 amebo-0.3.5/amebo/models/subscribers.py
+-rw-r--r--   0        0        0     1727 2023-08-28 08:37:12.553078 amebo-0.3.5/amebo/public/all.css
+-rw-r--r--   0        0        0    41352 2023-08-28 08:37:12.553310 amebo-0.3.5/amebo/public/alpine.min.js
+-rw-r--r--   0        0        0   353976 2024-05-05 20:04:17.923681 amebo-0.3.5/amebo/public/amebo.webp
+-rw-r--r--   0        0        0   207302 2023-08-28 08:37:12.553825 amebo-0.3.5/amebo/public/bulma.min.css
+-rw-r--r--   0        0        0     1436 2024-05-06 01:03:14.589179 amebo-0.3.5/amebo/public/heaven.css
+-rw-r--r--   0        0        0      219 2023-08-28 08:37:12.553994 amebo-0.3.5/amebo/public/icons/add.svg
+-rw-r--r--   0        0        0      697 2023-08-28 08:37:12.554083 amebo-0.3.5/amebo/public/icons/bulb.svg
+-rw-r--r--   0        0        0      732 2023-08-28 08:37:12.554165 amebo-0.3.5/amebo/public/icons/ear.svg
+-rw-r--r--   0        0        0      354 2023-08-28 08:37:12.554249 amebo-0.3.5/amebo/public/icons/flash-outline.svg
+-rw-r--r--   0        0        0      842 2023-08-28 08:37:12.554329 amebo-0.3.5/amebo/public/icons/hardware-chip.svg
+-rw-r--r--   0        0        0      356 2023-08-28 08:37:12.554396 amebo-0.3.5/amebo/public/icons/leaf-outline.svg
+-rw-r--r--   0        0        0      936 2023-08-28 08:37:12.554476 amebo-0.3.5/amebo/public/icons/megaphone.svg
+-rw-r--r--   0        0        0      370 2023-08-28 08:37:12.554547 amebo-0.3.5/amebo/public/icons/search.svg
+-rw-r--r--   0        0        0      390 2023-08-28 08:37:12.554629 amebo-0.3.5/amebo/public/icons/send.svg
+-rw-r--r--   0        0        0    15633 2023-08-28 08:37:12.554736 amebo-0.3.5/amebo/public/toastify.js
+-rw-r--r--   0        0        0     1096 2023-08-28 08:37:12.554827 amebo-0.3.5/amebo/public/toastify.min.css
+-rw-r--r--   0        0        0     2300 2024-05-06 12:30:52.996148 amebo-0.3.5/amebo/router.py
+-rw-r--r--   0        0        0       23 2024-04-23 12:52:10.324095 amebo-0.3.5/amebo/templates/404.html
+-rw-r--r--   0        0        0     5713 2024-05-05 20:37:01.462002 amebo-0.3.5/amebo/templates/abase.axml
+-rw-r--r--   0        0        0     2778 2024-05-05 20:28:32.119659 amebo-0.3.5/amebo/templates/actions.axml
+-rw-r--r--   0        0        0     9310 2024-05-06 01:09:36.957047 amebo-0.3.5/amebo/templates/actions.html
+-rw-r--r--   0        0        0     6923 2024-05-05 20:29:00.671201 amebo-0.3.5/amebo/templates/events.html
+-rw-r--r--   0        0        0     9424 2024-05-05 16:50:34.675416 amebo-0.3.5/amebo/templates/functions.axml
+-rw-r--r--   0        0        0     6502 2023-08-28 08:37:12.555959 amebo-0.3.5/amebo/templates/gists.html
+-rw-r--r--   0        0        0     4851 2023-09-06 17:31:38.143027 amebo-0.3.5/amebo/templates/login.html
+-rw-r--r--   0        0        0     1017 2023-08-28 08:37:12.556082 amebo-0.3.5/amebo/templates/logs.html
+-rw-r--r--   0        0        0     5432 2024-05-05 16:41:53.599815 amebo-0.3.5/amebo/templates/microservices.html
+-rw-r--r--   0        0        0     1875 2024-05-05 16:59:06.725863 amebo-0.3.5/amebo/templates/scripts.axml
+-rw-r--r--   0        0        0     4888 2023-08-28 08:37:12.556334 amebo-0.3.5/amebo/templates/subscribers.html
+-rw-r--r--   0        0        0     1261 2024-05-06 11:52:36.970476 amebo-0.3.5/amebo/utils/helpers.py
+-rw-r--r--   0        0        0     1161 2024-04-23 10:52:26.352293 amebo-0.3.5/amebo/utils/structs.py
+-rw-r--r--   0        0        0      557 2024-05-06 12:34:33.585734 amebo-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8141 1970-01-01 00:00:00.000000 amebo-0.3.5/PKG-INFO
```

### Comparing `amebo-0.3.4/README.md` & `amebo-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/amebo_readers.py` & `amebo-0.3.5/amebo/amebo_readers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/amebo_writers.py` & `amebo-0.3.5/amebo/amebo_writers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/aproko.py` & `amebo-0.3.5/amebo/aproko.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/constants/scripts.py` & `amebo-0.3.5/amebo/constants/scripts.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/controllers/actions.py` & `amebo-0.3.5/amebo/controllers/actions.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/controllers/events.py` & `amebo-0.3.5/amebo/controllers/events.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/controllers/gists.py` & `amebo-0.3.5/amebo/controllers/gists.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/controllers/microservices.py` & `amebo-0.3.5/amebo/controllers/microservices.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/controllers/subscribers.py` & `amebo-0.3.5/amebo/controllers/subscribers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/decorators/formatters.py` & `amebo-0.3.5/amebo/decorators/formatters.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/decorators/providers.py` & `amebo-0.3.5/amebo/decorators/providers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/decorators/security.py` & `amebo-0.3.5/amebo/decorators/security.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.1.1-py3-none-any.whl` & `amebo-0.3.5/amebo/dist/amebo-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.1.1.tar.gz` & `amebo-0.3.5/amebo/dist/amebo-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.1.2-py3-none-any.whl` & `amebo-0.3.5/amebo/dist/amebo-0.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.1.2.tar.gz` & `amebo-0.3.5/amebo/dist/amebo-0.1.2.tar.gz`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.2.0-py3-none-any.whl` & `amebo-0.3.5/amebo/dist/amebo-0.2.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.2.0.tar.gz` & `amebo-0.3.5/amebo/dist/amebo-0.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.3.0-py3-none-any.whl` & `amebo-0.3.5/amebo/dist/amebo-0.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/dist/amebo-0.3.0.tar.gz` & `amebo-0.3.5/amebo/dist/amebo-0.3.0.tar.gz`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/engines.py` & `amebo-0.3.5/amebo/engines.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/entities.py` & `amebo-0.3.5/amebo/entities.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/handlers.py` & `amebo-0.3.5/amebo/handlers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/middlewares/database.py` & `amebo-0.3.5/amebo/middlewares/database.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/middlewares/security.py` & `amebo-0.3.5/amebo/middlewares/security.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/models/actions.py` & `amebo-0.3.5/amebo/models/actions.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/models/events.py` & `amebo-0.3.5/amebo/models/events.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/models/microservices.py` & `amebo-0.3.5/amebo/models/microservices.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/models/subscribers.py` & `amebo-0.3.5/amebo/models/subscribers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/all.css` & `amebo-0.3.5/amebo/public/all.css`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/alpine.min.js` & `amebo-0.3.5/amebo/public/alpine.min.js`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/amebo.webp` & `amebo-0.3.5/amebo/public/amebo.webp`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/bulma.min.css` & `amebo-0.3.5/amebo/public/bulma.min.css`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/heaven.css` & `amebo-0.3.5/amebo/public/heaven.css`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/icons/bulb.svg` & `amebo-0.3.5/amebo/public/icons/bulb.svg`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/icons/ear.svg` & `amebo-0.3.5/amebo/public/icons/ear.svg`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/icons/hardware-chip.svg` & `amebo-0.3.5/amebo/public/icons/hardware-chip.svg`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/icons/megaphone.svg` & `amebo-0.3.5/amebo/public/icons/megaphone.svg`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/toastify.js` & `amebo-0.3.5/amebo/public/toastify.js`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/public/toastify.min.css` & `amebo-0.3.5/amebo/public/toastify.min.css`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/router.py` & `amebo-0.3.5/amebo/router.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/abase.axml` & `amebo-0.3.5/amebo/templates/abase.axml`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/actions.axml` & `amebo-0.3.5/amebo/templates/actions.axml`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/actions.html` & `amebo-0.3.5/amebo/templates/actions.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/events.html` & `amebo-0.3.5/amebo/templates/events.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/functions.axml` & `amebo-0.3.5/amebo/templates/functions.axml`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/gists.html` & `amebo-0.3.5/amebo/templates/gists.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/login.html` & `amebo-0.3.5/amebo/templates/login.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/logs.html` & `amebo-0.3.5/amebo/templates/logs.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/microservices.html` & `amebo-0.3.5/amebo/templates/microservices.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/scripts.axml` & `amebo-0.3.5/amebo/templates/scripts.axml`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/templates/subscribers.html` & `amebo-0.3.5/amebo/templates/subscribers.html`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/utils/helpers.py` & `amebo-0.3.5/amebo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/amebo/utils/structs.py` & `amebo-0.3.5/amebo/utils/structs.py`

 * *Files identical despite different names*

### Comparing `amebo-0.3.4/pyproject.toml` & `amebo-0.3.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "amebo"
-version = "0.3.4"
+version = "0.3.5"
 description = "HTTP Event Notifications Server - Asynchronous Communication Engine"
 authors = ["Tersoo"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "amebo"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "0.23.3"
 jinja2 = "3.1.2"
 fastjsonschema = "2.19.1"
 orjson = "3.8.9"
-pydantic = "1.10.7"
+pydantic = "2.7.1"
 pyjwt = "2.7.0"
 uvicorn = "0.14.0"
 routerling = "0.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `amebo-0.3.4/PKG-INFO` & `amebo-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: amebo
-Version: 0.3.4
+Version: 0.3.5
 Summary: HTTP Event Notifications Server - Asynchronous Communication Engine
 License: MIT
 Author: Tersoo
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastjsonschema (==2.19.1)
 Requires-Dist: httpx (==0.23.3)
 Requires-Dist: jinja2 (==3.1.2)
 Requires-Dist: orjson (==3.8.9)
-Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: pyjwt (==2.7.0)
 Requires-Dist: routerling (==0.5.1)
 Requires-Dist: uvicorn (==0.14.0)
 Description-Content-Type: text/markdown
 
 # AMEBO
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: amebo Version: 0.3.4 Summary: HTTP Event
+Metadata-Version: 2.1 Name: amebo Version: 0.3.5 Summary: HTTP Event
 Notifications Server - Asynchronous Communication Engine License: MIT Author:
 Tersoo Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 fastjsonschema (==2.19.1) Requires-Dist: httpx (==0.23.3) Requires-Dist: jinja2
-(==3.1.2) Requires-Dist: orjson (==3.8.9) Requires-Dist: pydantic (==1.10.7)
+(==3.1.2) Requires-Dist: orjson (==3.8.9) Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: pyjwt (==2.7.0) Requires-Dist: routerling (==0.5.1) Requires-
 Dist: uvicorn (==0.14.0) Description-Content-Type: text/markdown # AMEBO Amebo
 is the simplest pubsub server to use, deploy, understand or maintain. It was
 built to enable communication between applications i.e. microservices or
 modules (if you are using monoliths), and hopes to be able to serve as a small
 but capable and simpler alternative to Kafka, RabbitMQ, SQS/SNS. 1.
 Availability: Amebo runs on battle tested open source tools i.e. Redis,
```

