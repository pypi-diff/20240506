# Comparing `tmp/django-command-2.1.0.tar.gz` & `tmp/django_command-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-command-2.1.0.tar", last modified: Tue Dec 12 10:37:36 2023, max compression
+gzip compressed data, was "django_command-2.2.0.tar", last modified: Mon May  6 13:40:33 2024, max compression
```

## Comparing `django-command-2.1.0.tar` & `django_command-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:37:36.034683 django-command-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-12 10:37:28.000000 django-command-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2023-12-12 10:37:36.034683 django-command-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-12-12 10:37:28.000000 django-command-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:37:36.034683 django-command-2.1.0/django_command/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 10:37:28.000000 django-command-2.1.0/django_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2023-12-12 10:37:28.000000 django-command-2.1.0/django_command/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 10:37:36.034683 django-command-2.1.0/django_command.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2023-12-12 10:37:36.000000 django-command-2.1.0/django_command.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-12 10:37:36.000000 django-command-2.1.0/django_command.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 10:37:36.000000 django-command-2.1.0/django_command.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-12 10:37:36.000000 django-command-2.1.0/django_command.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-12 10:37:36.000000 django-command-2.1.0/django_command.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-12 10:37:36.000000 django-command-2.1.0/django_command.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-12 10:37:28.000000 django-command-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 10:37:36.034683 django-command-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:40:33.769863 django_command-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-06 13:40:29.000000 django_command-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-06 13:40:33.769863 django_command-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-06 13:40:29.000000 django_command-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:40:33.765863 django_command-2.2.0/django_command/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:40:29.000000 django_command-2.2.0/django_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-06 13:40:29.000000 django_command-2.2.0/django_command/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:40:33.769863 django_command-2.2.0/django_command.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-06 13:40:33.000000 django_command-2.2.0/django_command.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 13:40:33.000000 django_command-2.2.0/django_command.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:40:33.000000 django_command-2.2.0/django_command.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 13:40:33.000000 django_command-2.2.0/django_command.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 13:40:33.000000 django_command-2.2.0/django_command.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 13:40:33.000000 django_command-2.2.0/django_command.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 13:40:29.000000 django_command-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:40:33.769863 django_command-2.2.0/setup.cfg
```

### Comparing `django-command-2.1.0/LICENSE` & `django_command-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-command-2.1.0/PKG-INFO` & `django_command-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-command
-Version: 2.1.0
+Version: 2.2.0
 Summary: Django-command is a command line tool that allows you to run commonly used commands in development Django projects.
 Maintainer-email: Isaev Abbas <abbas.isaev@gmail.com>
 License: Copyright (c) 2023 Abbas Isaev.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -63,15 +63,15 @@
       [ ] collect_static                 [3] Assembling static files in the STATIC_ROOT folder
       [ ] make_migrations                [4] Creating migrations
       [ ] make_migrations_app            [5] Creating the first migration for the application
       [ ] make_empty_migrations_app      [6] Create a blank migration for the application. Used to add default data to the database table
       [ ] migrate                        [7] Applying migrations [--db_label default]
       [ ] create_superuser               [8] Creating a user with superuser rights
       [ ] create_app                     [9] Creating an application
-      [ ] run_server                     [10] Running a project on a port (default "8000") [--port 8000]
+      [ ] run_server                     [10] Running a project on a port number, or ipaddr:port (default "127.0.0.1:8000") [--port 127.0.0.1:8000]
       [ ] install_requirements           [11] Install all dependencies for a project from a file (default "requirements.txt")
       [ ] print_requirements             [12] Automatically generates all the necessary dependencies for the project, and also allows you to save this list to a file (default "requirements.txt") [--save_in_file requirements.txt]
    ```
 
 2. Commands can be executed by their name or number.
     ```shell
     django-command make_migrations migrate
@@ -96,10 +96,10 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -db DB_LABEL, --db_label DB_LABEL
                         database label for "migrate" command
   -s SAVE_IN_FILE, --save_in_file SAVE_IN_FILE
                         save to file for "print_requirements" command
-  -p PORT, --port PORT  port for "run_server" command
+  -p PORT, --port PORT  port number, or ipaddr:port for "run_server" command
   -v, --version         show program's version number and exit
 ```
```

### Comparing `django-command-2.1.0/README.md` & `django_command-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       [ ] collect_static                 [3] Assembling static files in the STATIC_ROOT folder
       [ ] make_migrations                [4] Creating migrations
       [ ] make_migrations_app            [5] Creating the first migration for the application
       [ ] make_empty_migrations_app      [6] Create a blank migration for the application. Used to add default data to the database table
       [ ] migrate                        [7] Applying migrations [--db_label default]
       [ ] create_superuser               [8] Creating a user with superuser rights
       [ ] create_app                     [9] Creating an application
-      [ ] run_server                     [10] Running a project on a port (default "8000") [--port 8000]
+      [ ] run_server                     [10] Running a project on a port number, or ipaddr:port (default "127.0.0.1:8000") [--port 127.0.0.1:8000]
       [ ] install_requirements           [11] Install all dependencies for a project from a file (default "requirements.txt")
       [ ] print_requirements             [12] Automatically generates all the necessary dependencies for the project, and also allows you to save this list to a file (default "requirements.txt") [--save_in_file requirements.txt]
    ```
 
 2. Commands can be executed by their name or number.
     ```shell
     django-command make_migrations migrate
@@ -57,10 +57,10 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -db DB_LABEL, --db_label DB_LABEL
                         database label for "migrate" command
   -s SAVE_IN_FILE, --save_in_file SAVE_IN_FILE
                         save to file for "print_requirements" command
-  -p PORT, --port PORT  port for "run_server" command
+  -p PORT, --port PORT  port number, or ipaddr:port for "run_server" command
   -v, --version         show program's version number and exit
 ```
```

### Comparing `django-command-2.1.0/django_command/command.py` & `django_command-2.2.0/django_command/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import argparse
 import os
 import sys
 
 import inquirer
 
-__version__ = '2.1.0'
+__version__ = '2.2.0'
 
 # Имя этого файла
 CURRENT_SCRIPT_NAME = os.path.basename(__file__)
 # Список локалей
 LOCALES = ['ru', 'en']
 DEFAULT_REQUIREMENTS = 'requirements.txt'
-DEFAULT_PORT = '8000'
+DEFAULT_ADDR_PORT = '127.0.0.1:8000'
 DEFAULT_DB_LABEL = 'default'
 
 # Список команд
 COMMANDS = {
     'create_local': f'Creating locales ({", ".join(LOCALES)})',
     'update_local': 'Updating and compiling locales',
     'collect_static': 'Assembling static files in the STATIC_ROOT folder',
     'make_migrations': 'Creating migrations',
     'make_migrations_app': 'Creating the first migration for the application',
     'make_empty_migrations_app': 'Create a blank migration for the application. '
                                  'Used to add default data to the database table',
     'migrate': f'Applying migrations [--db_label {DEFAULT_DB_LABEL}]',
     'create_superuser': 'Creating a user with superuser rights',
     'create_app': 'Creating an application',
-    'run_server': f'Running a project on a port (default "{DEFAULT_PORT}") [--port {DEFAULT_PORT}]',
+    'run_server': f'Running a project on a port number, or ipaddr:port '
+                  f'(default "{DEFAULT_ADDR_PORT}") [--port {DEFAULT_ADDR_PORT}]',
     'install_requirements': f'Install all dependencies for a project from a file (default "{DEFAULT_REQUIREMENTS}")',
     'print_requirements': 'Automatically generates all the necessary dependencies for the project, '
                           f'and also allows you to save this list to a file (default "{DEFAULT_REQUIREMENTS}") '
                           f'[--save_in_file {DEFAULT_REQUIREMENTS}]'
 }
 
 
@@ -51,15 +52,16 @@
         # answers['commands'] = sys.argv[1:]
         parser = argparse.ArgumentParser(prog='django-command',
                                          description=f'CLI tool that allows you to run commonly used commands '
                                                      f'when developing Django projects.')
         parser.add_argument('commands', nargs='+', type=str, help=f'commands to run: {", ".join(COMMANDS.keys())}')
         parser.add_argument('-db', '--db_label', help='database label for "migrate" command')
         parser.add_argument('-s', '--save_in_file', help='save to file for "print_requirements" command')
-        parser.add_argument('-p', '--port', default=DEFAULT_PORT, help='port for "run_server" command')
+        parser.add_argument('-p', '--port', default=DEFAULT_ADDR_PORT,
+                            help='port number, or ipaddr:port for "run_server" command')
         parser.add_argument('-v', '--version', action='version', version=__version__)
         args = parser.parse_args()
 
         answers['commands'] = args.commands
     else:
         choices_commands = [
             ("{:<30} [{}] {}".format(key, index + 1, value), key) for index, (key, value) in enumerate(COMMANDS.items())
@@ -154,27 +156,27 @@
 
             if app_name != '':
                 os.system(f'python manage.py startapp {app_name}')
             else:
                 print('You must enter the name of the application!')
         elif com == 'run_server':
             if args and args.port:
-                port = args.port
+                addr_port = args.port
             else:
                 question = [
                     inquirer.Text(
-                        'port',
-                        message='Enter port',
-                        default=DEFAULT_PORT
+                        'addr_port',
+                        message='Enter port number, or ipaddr:port',
+                        default=DEFAULT_ADDR_PORT
                     )
                 ]
                 answer = inquirer.prompt(question)
-                port = answer['port']
+                addr_port = answer['addr_port']
 
-            os.system(f'python manage.py runserver {port}')
+            os.system(f'python manage.py runserver {addr_port}')
         elif com == 'install_requirements':
             question = [
                 inquirer.Text(
                     'fileName',
                     message='Install dependencies from file',
                     default=DEFAULT_REQUIREMENTS
                 )
```

### Comparing `django-command-2.1.0/django_command.egg-info/PKG-INFO` & `django_command-2.2.0/django_command.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-command
-Version: 2.1.0
+Version: 2.2.0
 Summary: Django-command is a command line tool that allows you to run commonly used commands in development Django projects.
 Maintainer-email: Isaev Abbas <abbas.isaev@gmail.com>
 License: Copyright (c) 2023 Abbas Isaev.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -63,15 +63,15 @@
       [ ] collect_static                 [3] Assembling static files in the STATIC_ROOT folder
       [ ] make_migrations                [4] Creating migrations
       [ ] make_migrations_app            [5] Creating the first migration for the application
       [ ] make_empty_migrations_app      [6] Create a blank migration for the application. Used to add default data to the database table
       [ ] migrate                        [7] Applying migrations [--db_label default]
       [ ] create_superuser               [8] Creating a user with superuser rights
       [ ] create_app                     [9] Creating an application
-      [ ] run_server                     [10] Running a project on a port (default "8000") [--port 8000]
+      [ ] run_server                     [10] Running a project on a port number, or ipaddr:port (default "127.0.0.1:8000") [--port 127.0.0.1:8000]
       [ ] install_requirements           [11] Install all dependencies for a project from a file (default "requirements.txt")
       [ ] print_requirements             [12] Automatically generates all the necessary dependencies for the project, and also allows you to save this list to a file (default "requirements.txt") [--save_in_file requirements.txt]
    ```
 
 2. Commands can be executed by their name or number.
     ```shell
     django-command make_migrations migrate
@@ -96,10 +96,10 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -db DB_LABEL, --db_label DB_LABEL
                         database label for "migrate" command
   -s SAVE_IN_FILE, --save_in_file SAVE_IN_FILE
                         save to file for "print_requirements" command
-  -p PORT, --port PORT  port for "run_server" command
+  -p PORT, --port PORT  port number, or ipaddr:port for "run_server" command
   -v, --version         show program's version number and exit
 ```
```

### Comparing `django-command-2.1.0/pyproject.toml` & `django_command-2.2.0/pyproject.toml`

 * *Files identical despite different names*

