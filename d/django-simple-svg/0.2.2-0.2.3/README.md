# Comparing `tmp/django-simple-svg-0.2.2.tar.gz` & `tmp/django_simple_svg-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-svg-0.2.2.tar", last modified: Sun Dec  4 07:16:31 2022, max compression
+gzip compressed data, was "django_simple_svg-0.2.3.tar", last modified: Mon May  6 14:51:38 2024, max compression
```

## Comparing `django-simple-svg-0.2.2.tar` & `django_simple_svg-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2022-12-04 07:16:31.712753 django-simple-svg-0.2.2/
--rw-r--r--   0 maxshapira   (501) staff       (20)     1078 2022-07-11 17:56:41.000000 django-simple-svg-0.2.2/LICENSE
--rw-r--r--   0 maxshapira   (501) staff       (20)     3208 2022-12-04 07:16:31.713062 django-simple-svg-0.2.2/PKG-INFO
--rw-r--r--   0 maxshapira   (501) staff       (20)     1786 2022-12-04 07:07:35.000000 django-simple-svg-0.2.2/README.md
-drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2022-12-04 07:16:31.706706 django-simple-svg-0.2.2/django_simple_svg.egg-info/
--rw-r--r--   0 maxshapira   (501) staff       (20)     3208 2022-12-04 07:16:31.000000 django-simple-svg-0.2.2/django_simple_svg.egg-info/PKG-INFO
--rw-r--r--   0 maxshapira   (501) staff       (20)      375 2022-12-04 07:16:31.000000 django-simple-svg-0.2.2/django_simple_svg.egg-info/SOURCES.txt
--rw-r--r--   0 maxshapira   (501) staff       (20)        1 2022-12-04 07:16:31.000000 django-simple-svg-0.2.2/django_simple_svg.egg-info/dependency_links.txt
--rw-r--r--   0 maxshapira   (501) staff       (20)       12 2022-12-04 07:16:31.000000 django-simple-svg-0.2.2/django_simple_svg.egg-info/requires.txt
--rw-r--r--   0 maxshapira   (501) staff       (20)       11 2022-12-04 07:16:31.000000 django-simple-svg-0.2.2/django_simple_svg.egg-info/top_level.txt
--rw-r--r--   0 maxshapira   (501) staff       (20)      127 2022-12-04 07:16:31.713945 django-simple-svg-0.2.2/setup.cfg
--rw-r--r--   0 maxshapira   (501) staff       (20)     1958 2022-12-04 06:20:22.000000 django-simple-svg-0.2.2/setup.py
-drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2022-12-04 07:16:31.710058 django-simple-svg-0.2.2/simple_svg/
--rw-r--r--   0 maxshapira   (501) staff       (20)       94 2022-12-04 07:15:46.000000 django-simple-svg-0.2.2/simple_svg/__init__.py
--rw-r--r--   0 maxshapira   (501) staff       (20)       41 2021-09-13 06:40:11.000000 django-simple-svg-0.2.2/simple_svg/exceptions.py
-drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2022-12-04 07:16:31.711251 django-simple-svg-0.2.2/simple_svg/templatetags/
--rw-r--r--   0 maxshapira   (501) staff       (20)        0 2021-09-13 06:40:11.000000 django-simple-svg-0.2.2/simple_svg/templatetags/__init__.py
--rw-r--r--   0 maxshapira   (501) staff       (20)     1705 2021-09-15 08:41:07.000000 django-simple-svg-0.2.2/simple_svg/templatetags/svg.py
--rw-r--r--   0 maxshapira   (501) staff       (20)     2647 2021-09-15 08:41:07.000000 django-simple-svg-0.2.2/simple_svg/tests.py
+drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2024-05-06 14:51:38.039819 django_simple_svg-0.2.3/
+-rw-r--r--   0 maxshapira   (501) staff       (20)     1078 2022-07-11 17:56:41.000000 django_simple_svg-0.2.3/LICENSE
+-rw-r--r--   0 maxshapira   (501) staff       (20)     1586 2024-05-06 14:51:38.039588 django_simple_svg-0.2.3/PKG-INFO
+-rw-r--r--   0 maxshapira   (501) staff       (20)      157 2024-05-06 06:48:37.000000 django_simple_svg-0.2.3/README.md
+drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2024-05-06 14:51:38.038698 django_simple_svg-0.2.3/django_simple_svg.egg-info/
+-rw-r--r--   0 maxshapira   (501) staff       (20)     1586 2024-05-06 14:51:37.000000 django_simple_svg-0.2.3/django_simple_svg.egg-info/PKG-INFO
+-rw-r--r--   0 maxshapira   (501) staff       (20)      375 2024-05-06 14:51:37.000000 django_simple_svg-0.2.3/django_simple_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 maxshapira   (501) staff       (20)        1 2024-05-06 14:51:37.000000 django_simple_svg-0.2.3/django_simple_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 maxshapira   (501) staff       (20)       12 2024-05-06 14:51:37.000000 django_simple_svg-0.2.3/django_simple_svg.egg-info/requires.txt
+-rw-r--r--   0 maxshapira   (501) staff       (20)       11 2024-05-06 14:51:37.000000 django_simple_svg-0.2.3/django_simple_svg.egg-info/top_level.txt
+-rw-r--r--   0 maxshapira   (501) staff       (20)      127 2024-05-06 14:51:38.040810 django_simple_svg-0.2.3/setup.cfg
+-rw-r--r--   0 maxshapira   (501) staff       (20)     1958 2022-12-04 06:20:22.000000 django_simple_svg-0.2.3/setup.py
+drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2024-05-06 14:51:38.036623 django_simple_svg-0.2.3/simple_svg/
+-rw-r--r--   0 maxshapira   (501) staff       (20)       94 2024-05-06 14:50:51.000000 django_simple_svg-0.2.3/simple_svg/__init__.py
+-rw-r--r--   0 maxshapira   (501) staff       (20)       41 2021-09-13 06:40:11.000000 django_simple_svg-0.2.3/simple_svg/exceptions.py
+drwxr-xr-x   0 maxshapira   (501) staff       (20)        0 2024-05-06 14:51:38.037849 django_simple_svg-0.2.3/simple_svg/templatetags/
+-rw-r--r--   0 maxshapira   (501) staff       (20)        0 2021-09-13 06:40:11.000000 django_simple_svg-0.2.3/simple_svg/templatetags/__init__.py
+-rw-r--r--   0 maxshapira   (501) staff       (20)     1705 2021-09-15 08:41:07.000000 django_simple_svg-0.2.3/simple_svg/templatetags/svg.py
+-rw-r--r--   0 maxshapira   (501) staff       (20)     2647 2021-09-15 08:41:07.000000 django_simple_svg-0.2.3/simple_svg/tests.py
```

### Comparing `django-simple-svg-0.2.2/LICENSE` & `django_simple_svg-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-svg-0.2.2/setup.py` & `django_simple_svg-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-simple-svg-0.2.2/simple_svg/templatetags/svg.py` & `django_simple_svg-0.2.3/simple_svg/templatetags/svg.py`

 * *Files identical despite different names*

### Comparing `django-simple-svg-0.2.2/simple_svg/tests.py` & `django_simple_svg-0.2.3/simple_svg/tests.py`

 * *Files identical despite different names*

