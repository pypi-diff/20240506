# Comparing `tmp/trex-conf-0.0.2.tar.gz` & `tmp/trex-conf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-conf-0.0.2.tar", last modified: Mon Apr 29 06:50:05 2024, max compression
+gzip compressed data, was "trex-conf-1.0.0.tar", last modified: Mon May  6 07:49:46 2024, max compression
```

## Comparing `trex-conf-0.0.2.tar` & `trex-conf-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 06:50:05.402234 trex-conf-0.0.2/
--rw-r--r--   0 jacklok    (501) staff       (20)      405 2024-04-29 06:50:05.402127 trex-conf-0.0.2/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       30 2024-04-29 04:10:38.000000 trex-conf-0.0.2/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-29 06:50:05.402853 trex-conf-0.0.2/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      989 2024-04-29 06:49:53.000000 trex-conf-0.0.2/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 06:50:05.401590 trex-conf-0.0.2/trex_conf.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      405 2024-04-29 06:50:05.000000 trex-conf-0.0.2/trex_conf.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)      222 2024-04-29 06:50:05.000000 trex-conf-0.0.2/trex_conf.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-29 06:50:05.000000 trex-conf-0.0.2/trex_conf.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        9 2024-04-29 06:50:05.000000 trex-conf-0.0.2/trex_conf.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 06:50:05.400132 trex-conf-0.0.2/trexconf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 04:02:50.000000 trex-conf-0.0.2/trexconf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16151 2024-04-29 04:32:06.000000 trex-conf-0.0.2/trexconf/conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-conf-0.0.2/trexconf/config_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:49:46.203161 trex-conf-1.0.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)      405 2024-05-06 07:49:46.202978 trex-conf-1.0.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       30 2024-04-29 04:10:38.000000 trex-conf-1.0.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 07:49:46.203630 trex-conf-1.0.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      989 2024-05-06 07:49:43.000000 trex-conf-1.0.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:49:46.202593 trex-conf-1.0.0/trex_conf.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      405 2024-05-06 07:49:46.000000 trex-conf-1.0.0/trex_conf.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)      247 2024-05-06 07:49:46.000000 trex-conf-1.0.0/trex_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 07:49:46.000000 trex-conf-1.0.0/trex_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        9 2024-05-06 07:49:46.000000 trex-conf-1.0.0/trex_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:49:46.202151 trex-conf-1.0.0/trexconf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 04:02:50.000000 trex-conf-1.0.0/trexconf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16588 2024-05-05 09:45:11.000000 trex-conf-1.0.0/trexconf/conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-conf-1.0.0/trexconf/config_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32678 2024-05-04 13:55:38.000000 trex-conf-1.0.0/trexconf/program_conf.py
```

### Comparing `trex-conf-0.0.2/setup.py` & `trex-conf-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 setuptools.setup(
     #Application name and details
      name='trex-conf',
      description="TRex Configuration package",
      long_description=long_description,
      long_description_content_type="text/markdown",  
      url="https://bitbucket.org/lokjac/trex-conf",
-     version='0.0.2',
+     version='1.0.0',
      
      #Author details
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      
      #packages=setuptools.find_packages(),
      packages=setuptools.find_packages(),
```

### Comparing `trex-conf-0.0.2/trexconf/conf.py` & `trex-conf-1.0.0/trexconf/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,30 @@
 @author: jacklok
 '''
 import logging, os, config_path
 from trexconf.config_util import read_config
 
 logger = logging.getLogger('debug')
 
+APPLICATION_NAME                                    = os.environ.get('APPLICATION_NAME')
+MOBILE_APP_NAME                                     = os.environ.get('MOBILE_APP_NAME')
+
+API_VERSION                                         = '0.0.1'
 
 PRODUCTION_MODE                                     = "PROD"
 DEMO_MODE                                           = "DEMO"
 LOCAL_MODE                                          = "LOCAL"
 
 DEPLOYMENT_MODE                                     = os.environ.get('DEPLOYMENT_MODE')
 
 SECRET_KEY                                          = os.environ.get('SECRET_KEY')
 MAX_PASSWORD_LENGTH                                 = os.environ.get('MAX_PASSWORD_LENGTH')
 
+API_TOKEN_EXPIRY_LENGTH_IN_MINUTE                   = os.environ.get('API_TOKEN_EXPIRY_LENGTH_IN_MINUTE')
+
 SYSTEM_TASK_GCLOUD_PROJECT_ID                       = os.environ.get('SYSTEM_TASK_GCLOUD_PROJECT_ID')
 SYSTEM_TASK_GCLOUD_LOCATION                         = os.environ.get('SYSTEM_TASK_GCLOUD_LOCATION')
 SYSTEM_TASK_SERVICE_ACCOUNT_KEY                     = os.environ.get('SYSTEM_TASK_SERVICE_ACCOUNT_KEY')
 SYSTEM_TASK_SERVICE_CREDENTIAL_PATH                 = os.path.abspath(os.path.dirname(config_path.__file__)) + '/' + SYSTEM_TASK_SERVICE_ACCOUNT_KEY
 SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL                   = os.environ.get('SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL')
 
 SYSTEM_BASE_URL                                     = os.environ.get('SYSTEM_BASE_URL')
@@ -68,14 +74,16 @@
 EMAIL_EXPIRY_LENGTH_IN_MINUTE               = os.environ.get('EMAIL_EXPIRY_LENGTH_IN_MINUTE')
 MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE        = os.environ.get('MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE')
 
 INSTANT_REWARD_CUSTOM_URL                   = os.environ.get('INSTANT_REWARD_CUSTOM_URL')
 
 REFER_A_FRIEND_CUSTOM_URL                   = os.environ.get('REFER_A_FRIEND_CUSTOM_URL')
 
+REFER_A_FRIEND_DEEP_LINK                    = os.environ.get('REFER_A_FRIEND_DEEP_LINK')
+
 TASK_BASE_URL                               = os.environ.get('TASK_BASE_URL')
 
 DEBUG_MODE                                  = os.environ.get('DEBUG_MODE')
 
 APPLICATION_SHOW_DASHBOARD_MESSAGE          = False
 APPLICATION_SHOW_DASHBOARD_NOTIFICATION     = False
```

### Comparing `trex-conf-0.0.2/trexconf/config_util.py` & `trex-conf-1.0.0/trexconf/config_util.py`

 * *Files identical despite different names*

