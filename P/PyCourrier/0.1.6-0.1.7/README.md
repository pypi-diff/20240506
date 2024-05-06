# Comparing `tmp/PyCourrier-0.1.6.tar.gz` & `tmp/PyCourrier-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCourrier-0.1.6.tar", last modified: Thu May  2 02:31:56 2024, max compression
+gzip compressed data, was "PyCourrier-0.1.7.tar", last modified: Sun May  5 13:18:28 2024, max compression
```

## Comparing `PyCourrier-0.1.6.tar` & `PyCourrier-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 02:31:56.866898 PyCourrier-0.1.6/
--rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3223 2024-05-02 02:31:56.862077 PyCourrier-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 02:31:56.788350 PyCourrier-0.1.6/PyCourrier/
--rw-rw-rw-   0        0        0     5938 2024-05-02 02:28:17.000000 PyCourrier-0.1.6/PyCourrier/MailSender.py
--rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.6/PyCourrier/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:31:56.859038 PyCourrier-0.1.6/PyCourrier.egg-info/
--rw-rw-rw-   0        0        0     3223 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 02:31:56.000000 PyCourrier-0.1.6/PyCourrier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2783 2024-05-02 02:30:24.000000 PyCourrier-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 02:31:56.868893 PyCourrier-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-05-02 02:28:31.000000 PyCourrier-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:18:28.366984 PyCourrier-0.1.7/
+-rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3223 2024-05-05 13:18:28.363078 PyCourrier-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-05 13:18:28.306472 PyCourrier-0.1.7/PyCourrier/
+-rw-rw-rw-   0        0        0     5984 2024-05-05 13:15:01.000000 PyCourrier-0.1.7/PyCourrier/MailSender.py
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.7/PyCourrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:18:28.356246 PyCourrier-0.1.7/PyCourrier.egg-info/
+-rw-rw-rw-   0        0        0     3223 2024-05-05 13:18:28.000000 PyCourrier-0.1.7/PyCourrier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-05 13:18:28.000000 PyCourrier-0.1.7/PyCourrier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 13:18:28.000000 PyCourrier-0.1.7/PyCourrier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 13:18:28.000000 PyCourrier-0.1.7/PyCourrier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2783 2024-05-02 02:30:24.000000 PyCourrier-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 13:18:28.366984 PyCourrier-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-05-05 13:18:13.000000 PyCourrier-0.1.7/setup.py
```

### Comparing `PyCourrier-0.1.6/LICENSE` & `PyCourrier-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCourrier-0.1.6/PKG-INFO` & `PyCourrier-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyCourrier-0.1.6/PyCourrier/MailSender.py` & `PyCourrier-0.1.7/PyCourrier/MailSender.py`

 * *Files 18% similar despite different names*

```diff
@@ -122,34 +122,31 @@
             logging.error("Not connected to any server. Please connect first.")
             raise ConnectionError("Not connected to any server. Please connect first.")
 
         if not self.msg:
             logging.error("Message not set. Please set the message before sending.")
             raise ValueError("Message not set.")
 
-        try:
-            # Set the 'To' header with all recipients
-            self.msg['To'] = ", ".join(self.recipients)
-
-            tasks = []
-            loop = get_event_loop()
-
-            for recipient in self.recipients:
-                task = loop.create_task(self.send_email(recipient))
-                tasks.append(task)
-
-            await gather(*tasks)
-            logging.info("All messages sent")
-        except smtplib.SMTPException as error:
-            logging.error(f"Failed to send mail: {error}")
-            raise
+        tasks = [self.send_email(recipient) for recipient in self.recipients]
+        await gather(*tasks)
+        logging.info("All messages sent")
 
     async def send_email(self, recipient):
-        """Send the email to a recipient."""
+        """Send the email to a single recipient."""
         try:
             logging.info(f"Sending to {recipient}")
-            
+
+            # Create a new message for each recipient to set the 'To' header individually
+            msg = MIMEMultipart('alternative')
+            msg['Subject'] = self.msg['Subject']
+            msg['From'] = self.msg['From']
+            msg['To'] = recipient  # Set the recipient's email
+
+            # Attach the plain and HTML parts from the original message
+            for part in self.msg.get_payload():
+                msg.attach(part)
+
             # Convert the message to a string and then send it
-            self.smtpserver.sendmail(self.username, recipient, self.msg.as_string())
+            self.smtpserver.sendmail(self.username, recipient, msg.as_string())
         except smtplib.SMTPException as error:
             logging.error(f"Failed to send mail to {recipient}: {error}")
             raise
```

### Comparing `PyCourrier-0.1.6/PyCourrier.egg-info/PKG-INFO` & `PyCourrier-0.1.7/PyCourrier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyCourrier-0.1.6/README.md` & `PyCourrier-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PyCourrier-0.1.6/setup.py` & `PyCourrier-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='PyCourrier',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     description='A simple email sender utility',
     author='Abdelmajid Habouch',
     author_email='Habush1610@gmail.com',
     url='https://github.com/mjiid/PyCourrier',
     license='MIT',
     install_requires=[
```

