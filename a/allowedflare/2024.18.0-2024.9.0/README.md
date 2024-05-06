# Comparing `tmp/allowedflare-2024.18.0.tar.gz` & `tmp/allowedflare-2024.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allowedflare-2024.18.0.tar", last modified: Mon May  6 01:47:42 2024, max compression
+gzip compressed data, was "allowedflare-2024.9.0.tar", last modified: Fri Mar  1 17:00:06 2024, max compression
```

## Comparing `allowedflare-2024.18.0.tar` & `allowedflare-2024.9.0.tar`

### file list

```diff
@@ -1,21 +1,14 @@
-drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-05-06 01:47:42.840820 allowedflare-2024.18.0/
--rw-r--r--   0 jessicacovington   (501) staff       (20)     1508 2023-11-21 12:24:17.000000 allowedflare-2024.18.0/LICENSE
--rw-r--r--   0 jessicacovington   (501) staff       (20)     2874 2024-05-06 01:47:42.840556 allowedflare-2024.18.0/PKG-INFO
--rw-r--r--   0 jessicacovington   (501) staff       (20)     2327 2024-05-03 16:00:33.000000 allowedflare-2024.18.0/README.md
-drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-05-06 01:47:42.837170 allowedflare-2024.18.0/allowedflare-proxy/
--rw-r--r--   0 jessicacovington   (501) staff       (20)      899 2024-05-03 16:00:33.000000 allowedflare-2024.18.0/allowedflare-proxy/index.test.ts
--rw-r--r--   0 jessicacovington   (501) staff       (20)     1154 2024-05-03 16:00:33.000000 allowedflare-2024.18.0/allowedflare-proxy/index.ts
--rw-r--r--   0 jessicacovington   (501) staff       (20)    10947 2024-04-04 16:11:15.000000 allowedflare-2024.18.0/allowedflare-proxy/tsconfig.json
-drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-05-06 01:47:42.840225 allowedflare-2024.18.0/allowedflare.egg-info/
--rw-r--r--   0 jessicacovington   (501) staff       (20)     2874 2024-05-06 01:47:42.000000 allowedflare-2024.18.0/allowedflare.egg-info/PKG-INFO
--rw-r--r--   0 jessicacovington   (501) staff       (20)      404 2024-05-06 01:47:42.000000 allowedflare-2024.18.0/allowedflare.egg-info/SOURCES.txt
--rw-r--r--   0 jessicacovington   (501) staff       (20)        1 2024-05-06 01:47:42.000000 allowedflare-2024.18.0/allowedflare.egg-info/dependency_links.txt
--rw-r--r--   0 jessicacovington   (501) staff       (20)       28 2024-05-06 01:47:42.000000 allowedflare-2024.18.0/allowedflare.egg-info/requires.txt
--rw-r--r--   0 jessicacovington   (501) staff       (20)       20 2024-05-06 01:47:42.000000 allowedflare-2024.18.0/allowedflare.egg-info/top_level.txt
-drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-05-06 01:47:42.839569 allowedflare-2024.18.0/django_allowedflare/
--rw-r--r--   0 jessicacovington   (501) staff       (20)     3939 2024-05-06 01:41:48.000000 allowedflare-2024.18.0/django_allowedflare/__init__.py
--rw-r--r--   0 jessicacovington   (501) staff       (20)      127 2024-03-04 23:49:28.000000 allowedflare-2024.18.0/django_allowedflare/login.html
-drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-05-06 01:47:42.839906 allowedflare-2024.18.0/jupyterhub_allowedflare/
--rw-r--r--   0 jessicacovington   (501) staff       (20)      572 2024-05-06 01:41:48.000000 allowedflare-2024.18.0/jupyterhub_allowedflare/__init__.py
--rw-r--r--   0 jessicacovington   (501) staff       (20)     1190 2024-05-03 16:00:33.000000 allowedflare-2024.18.0/pyproject.toml
--rw-r--r--   0 jessicacovington   (501) staff       (20)       38 2024-05-06 01:47:42.840865 allowedflare-2024.18.0/setup.cfg
+drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-03-01 17:00:06.269369 allowedflare-2024.9.0/
+-rw-r--r--   0 jessicacovington   (501) staff       (20)     1508 2023-11-21 12:24:17.000000 allowedflare-2024.9.0/LICENSE
+-rw-r--r--   0 jessicacovington   (501) staff       (20)     1726 2024-03-01 17:00:06.269164 allowedflare-2024.9.0/PKG-INFO
+-rw-r--r--   0 jessicacovington   (501) staff       (20)     1180 2023-11-21 13:30:41.000000 allowedflare-2024.9.0/README.md
+drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-03-01 17:00:06.268941 allowedflare-2024.9.0/allowedflare.egg-info/
+-rw-r--r--   0 jessicacovington   (501) staff       (20)     1726 2024-03-01 17:00:06.000000 allowedflare-2024.9.0/allowedflare.egg-info/PKG-INFO
+-rw-r--r--   0 jessicacovington   (501) staff       (20)      243 2024-03-01 17:00:06.000000 allowedflare-2024.9.0/allowedflare.egg-info/SOURCES.txt
+-rw-r--r--   0 jessicacovington   (501) staff       (20)        1 2024-03-01 17:00:06.000000 allowedflare-2024.9.0/allowedflare.egg-info/dependency_links.txt
+-rw-r--r--   0 jessicacovington   (501) staff       (20)       28 2024-03-01 17:00:06.000000 allowedflare-2024.9.0/allowedflare.egg-info/requires.txt
+-rw-r--r--   0 jessicacovington   (501) staff       (20)       20 2024-03-01 17:00:06.000000 allowedflare-2024.9.0/allowedflare.egg-info/top_level.txt
+drwxr-xr-x   0 jessicacovington   (501) staff       (20)        0 2024-03-01 17:00:06.268699 allowedflare-2024.9.0/django_allowedflare/
+-rw-r--r--   0 jessicacovington   (501) staff       (20)     3337 2024-03-01 16:47:37.000000 allowedflare-2024.9.0/django_allowedflare/__init__.py
+-rw-r--r--   0 jessicacovington   (501) staff       (20)     1279 2024-03-01 16:47:37.000000 allowedflare-2024.9.0/pyproject.toml
+-rw-r--r--   0 jessicacovington   (501) staff       (20)       38 2024-03-01 17:00:06.269410 allowedflare-2024.9.0/setup.cfg
```

### Comparing `allowedflare-2024.18.0/LICENSE` & `allowedflare-2024.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allowedflare-2024.18.0/pyproject.toml` & `allowedflare-2024.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,31 @@
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Topic :: Internet :: WWW/HTTP :: Session',
 ]
 description = 'Authenticate to Django with JSON Web Tokens (JWTs) signed by Cloudflare Access'
-dependencies = ['cryptography', 'pyjwt', 'requests']
+dependencies = [
+    'cryptography',
+    'pyjwt',
+    'requests',
+]
 dynamic = ['version']
 name = 'allowedflare'
 readme = 'README.md'
 
 [project.urls]
 Homepage = 'https://github.com/covracer/allowedflare'
 
+[tool.black]
+line-length = 100
+skip-magic-trailing-comma = true
+skip-string-normalization = true
+
 [tool.ruff.format]
 quote-style = 'single'
 skip-magic-trailing-comma = true
 
 [tool.ruff.lint.flake8-quotes]
 inline-quotes = 'single'
 
@@ -33,13 +42,13 @@
 
 [tool.ruff.lint]
 ignore = [
     'EM101', # Allow exceptions to use string literals because keeping code as simple as possible is more important than keeping tracebacks as simple as possible.
 ]
 
 [tool.mypy]
-plugins = ['mypy_drf_plugin.main', 'mypy_django_plugin.main']
+plugins = ['mypy_django_plugin.main']
 
 [tool.setuptools]
 packages = ['django_allowedflare']
 
 [tool.setuptools_scm]
```

