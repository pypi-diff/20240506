# Comparing `tmp/saraapi-0.0.0.1.tar.gz` & `tmp/saraapi-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saraapi-0.0.0.1.tar", last modified: Mon May  6 00:10:17 2024, max compression
+gzip compressed data, was "saraapi-0.0.0.2.tar", last modified: Mon May  6 02:05:52 2024, max compression
```

## Comparing `saraapi-0.0.0.1.tar` & `saraapi-0.0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 00:10:17.294105 saraapi-0.0.0.1/
--rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0      737 2024-05-06 00:10:17.291684 saraapi-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-05-05 22:38:47.000000 saraapi-0.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 00:10:17.268794 saraapi-0.0.0.1/sara/
--rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.1/sara/__init__.py
--rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.1/sara/ext.py
--rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.1/sara/nsfw.py
--rw-rw-rw-   0        0        0      630 2024-05-05 21:25:49.000000 saraapi-0.0.0.1/sara/req.py
--rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.1/sara/sfw.py
-drwxrwxrwx   0        0        0        0 2024-05-06 00:10:17.290526 saraapi-0.0.0.1/saraApi.egg-info/
--rw-rw-rw-   0        0        0      737 2024-05-06 00:10:17.000000 saraapi-0.0.0.1/saraApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-06 00:10:17.000000 saraapi-0.0.0.1/saraApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 00:10:17.000000 saraapi-0.0.0.1/saraApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 00:10:17.000000 saraapi-0.0.0.1/saraApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 00:10:17.000000 saraapi-0.0.0.1/saraApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 00:10:17.294105 saraapi-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-05 23:32:15.000000 saraapi-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:05:52.787742 saraapi-0.0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4799 2024-05-06 02:05:52.785210 saraapi-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4066 2024-05-06 01:36:18.000000 saraapi-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 02:05:52.759827 saraapi-0.0.0.2/sara/
+-rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.2/sara/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.2/sara/ext.py
+-rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.2/sara/nsfw.py
+-rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.2/sara/req.py
+-rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.2/sara/sfw.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:05:52.784207 saraapi-0.0.0.2/saraApi.egg-info/
+-rw-rw-rw-   0        0        0     4799 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 02:05:52.787742 saraapi-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-06 01:59:13.000000 saraapi-0.0.0.2/setup.py
```

### Comparing `saraapi-0.0.0.1/sara/ext.py` & `saraapi-0.0.0.2/sara/ext.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.1/sara/nsfw.py` & `saraapi-0.0.0.2/sara/nsfw.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.1/sara/req.py` & `saraapi-0.0.0.2/sara/req.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,13 +4,13 @@
     """
     @param  Request Parameter
     @return String
     """
     try:
         r = requests.get(f"https://sara-funciones-api.vercel.app/api/category?category={param}").json()
     except Exception as e:
-        raise Exception(f"ERROR: > {e}\n\n\nPlease Contact Raphiel#8922 or Open a Issue in https://github.com/RaphielHS/akaneko-wrapper/issues/")
+        raise Exception(f"ERROR: > {e}\n\n\nPlease Contact evergaster or Open a Issue in https://github.com/RaphielHS/akaneko-wrapper/issues/")
     else:
         try:
             return r['url']
         except Exception as e:
-            raise Exception(f"ERROR: > {e}\n\n\nPlease Contact Raphiel#8922 or Open a Issue in https://github.com/RaphielHS/akaneko-wrapper/issues/")
+            raise Exception(f"ERROR: > {e}\n\n\nPlease Contact evergaster or Open a Issue in https://github.com/RaphielHS/akaneko-wrapper/issues/")
```

### Comparing `saraapi-0.0.0.1/setup.py` & `saraapi-0.0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md','r', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 install_requires = [
 	'requests'
 ]
 
-version = '0.0.0.1'
+version = '0.0.0.2'
 
 setup(
     author='evergaster',
     version=version,
     description='sara api public based akanekopy',
     install_package_data=True,
     install_requires=install_requires,
```

