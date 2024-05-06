# Comparing `tmp/trex-mail-0.1.8.tar.gz` & `tmp/trex-mail-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-mail-0.1.8.tar", last modified: Tue Aug 15 14:08:44 2023, max compression
+gzip compressed data, was "trex-mail-0.1.9.tar", last modified: Tue Aug 15 14:29:41 2023, max compression
```

## Comparing `trex-mail-0.1.8.tar` & `trex-mail-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-15 14:08:44.261973 trex-mail-0.1.8/
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-mail-0.1.8/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      456 2023-08-15 14:08:44.262112 trex-mail-0.1.8/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       26 2020-09-13 13:01:59.000000 trex-mail-0.1.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-15 14:08:44.262709 trex-mail-0.1.8/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      753 2023-08-15 14:08:34.000000 trex-mail-0.1.8/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-15 14:08:44.256994 trex-mail-0.1.8/trex_mail.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      456 2023-08-15 14:08:44.000000 trex-mail-0.1.8/trex_mail.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2023-08-15 14:08:44.000000 trex-mail-0.1.8/trex_mail.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-15 14:08:44.000000 trex-mail-0.1.8/trex_mail.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       11 2023-08-15 14:08:44.000000 trex-mail-0.1.8/trex_mail.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       15 2023-08-15 14:08:44.000000 trex-mail-0.1.8/trex_mail.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-15 14:08:44.261083 trex-mail-0.1.8/trexmail/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-13 13:01:40.000000 trex-mail-0.1.8/trexmail/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      928 2022-08-22 02:44:07.000000 trex-mail-0.1.8/trexmail/conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2510 2023-08-15 13:51:48.000000 trex-mail-0.1.8/trexmail/email_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)      732 2023-08-15 13:17:55.000000 trex-mail-0.1.8/trexmail/flask_mail.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2732 2022-08-22 02:44:45.000000 trex-mail-0.1.8/trexmail/mailjet.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1715 2022-08-22 02:44:30.000000 trex-mail-0.1.8/trexmail/sendgrid.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-15 14:29:41.961866 trex-mail-0.1.9/
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-mail-0.1.9/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      456 2023-08-15 14:29:41.962030 trex-mail-0.1.9/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       26 2020-09-13 13:01:59.000000 trex-mail-0.1.9/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-15 14:29:41.962694 trex-mail-0.1.9/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      753 2023-08-15 14:29:34.000000 trex-mail-0.1.9/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-15 14:29:41.959486 trex-mail-0.1.9/trex_mail.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      456 2023-08-15 14:29:41.000000 trex-mail-0.1.9/trex_mail.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2023-08-15 14:29:41.000000 trex-mail-0.1.9/trex_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-15 14:29:41.000000 trex-mail-0.1.9/trex_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       11 2023-08-15 14:29:41.000000 trex-mail-0.1.9/trex_mail.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       15 2023-08-15 14:29:41.000000 trex-mail-0.1.9/trex_mail.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-15 14:29:41.961587 trex-mail-0.1.9/trexmail/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-13 13:01:40.000000 trex-mail-0.1.9/trexmail/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      928 2022-08-22 02:44:07.000000 trex-mail-0.1.9/trexmail/conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2513 2023-08-15 14:25:52.000000 trex-mail-0.1.9/trexmail/email_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      732 2023-08-15 13:17:55.000000 trex-mail-0.1.9/trexmail/flask_mail.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2732 2022-08-22 02:44:45.000000 trex-mail-0.1.9/trexmail/mailjet.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1715 2022-08-22 02:44:30.000000 trex-mail-0.1.9/trexmail/sendgrid.py
```

### Comparing `trex-mail-0.1.8/setup.py` & `trex-mail-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-mail',  
-     version='0.1.8',
+     version='0.1.9',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-mail",
      packages=setuptools.find_packages(),
```

### Comparing `trex-mail-0.1.8/trexmail/conf.py` & `trex-mail-0.1.9/trexmail/conf.py`

 * *Files identical despite different names*

### Comparing `trex-mail-0.1.8/trexmail/email_helper.py` & `trex-mail-0.1.9/trexmail/email_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 logger = logging.getLogger('helper')
 #logger = logging.getLogger('debug')
 
 def trigger_send_email(sender_address=DEFAULT_SENDER, recipient_address=None, subject=None, message=None, cc_address=None):
     
     logger.debug('sender_address=%s', sender_address)
     logger.debug('recipient_address=%s', recipient_address)
-    
+    '''
     send_email(sender           = sender_address, 
                    to_address   = [recipient_address], 
                    subject      = subject, 
                    body         = message,
                    app          = current_app
                    )
-    #if DEPLOYMENT_MODE == LOCAL_MODE:
+    
     '''
+    #if DEPLOYMENT_MODE == LOCAL_MODE:
     if False:
         logger.info('send email directly')
         send_email(sender           = sender_address, 
                    to_address   = [recipient_address], 
                    subject      = subject, 
                    body         = message,
                    app          = current_app
@@ -52,9 +53,9 @@
                         in_seconds      = 1, 
                         http_method     = 'POST',
                         credential_path = SYSTEM_TASK_SERVICE_CREDENTIAL_PATH, 
                         project_id      = SYSTEM_TASK_GCLOUD_PROJECT_ID,
                         location        = SYSTEM_TASK_GCLOUD_LOCATION,
                         service_email   = SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL
                         )
-    '''   
+     
     return True
```

### Comparing `trex-mail-0.1.8/trexmail/flask_mail.py` & `trex-mail-0.1.9/trexmail/flask_mail.py`

 * *Files identical despite different names*

### Comparing `trex-mail-0.1.8/trexmail/mailjet.py` & `trex-mail-0.1.9/trexmail/mailjet.py`

 * *Files identical despite different names*

### Comparing `trex-mail-0.1.8/trexmail/sendgrid.py` & `trex-mail-0.1.9/trexmail/sendgrid.py`

 * *Files identical despite different names*

