# Comparing `tmp/plone.api-2.1.0.tar.gz` & `tmp/plone_api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.api-2.1.0.tar", last modified: Thu Feb 22 22:02:10 2024, max compression
+gzip compressed data, was "plone_api-2.2.0.tar", last modified: Mon May  6 12:56:07 2024, max compression
```

## Comparing `plone.api-2.1.0.tar` & `plone_api-2.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.311781 plone.api-2.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)    23298 2024-02-22 22:02:08.000000 plone.api-2.1.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       73 2024-02-22 22:02:08.000000 plone.api-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      679 2024-02-22 22:02:08.000000 plone.api-2.1.0/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      357 2024-02-22 22:02:08.000000 plone.api-2.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    27517 2024-02-22 22:02:10.311438 plone.api-2.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1936 2024-02-22 22:02:08.000000 plone.api-2.1.0/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.283130 plone.api-2.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    14247 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/group.md
--rw-r--r--   0 maurits    (501) staff       (20)     2295 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/index.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2024-02-22 22:02:08.000000 plone.api-2.1.0/docs/user.md
--rw-r--r--   0 maurits    (501) staff       (20)      578 2024-02-22 22:02:08.000000 plone.api-2.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      654 2024-02-22 22:02:10.313134 plone.api-2.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2004 2024-02-22 22:02:08.000000 plone.api-2.1.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.272549 plone.api-2.1.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.284028 plone.api-2.1.0/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.293894 plone.api-2.1.0/src/plone/api/
--rw-r--r--   0 maurits    (501) staff       (20)      193 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       98 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    22829 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     8042 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/env.py
--rw-r--r--   0 maurits    (501) staff       (20)     1051 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/exc.py
--rw-r--r--   0 maurits    (501) staff       (20)    11142 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/group.py
--rw-r--r--   0 maurits    (501) staff       (20)    14164 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.273246 plone.api-2.1.0/src/plone/api/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.294865 plone.api-2.1.0/src/plone/api/profiles/testfixture/
--rw-r--r--   0 maurits    (501) staff       (20)      229 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/profiles/testfixture/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.295844 plone.api-2.1.0/src/plone/api/profiles/testfixture/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1734 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      210 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/profiles/testfixture/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)    11554 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/relation.py
--rw-r--r--   0 maurits    (501) staff       (20)      578 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.301975 plone.api-2.1.0/src/plone/api/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      106 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      106 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1658 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.307661 plone.api-2.1.0/src/plone/api/tests/doctests/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    14247 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/group.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/doctests/user.md
--rw-r--r--   0 maurits    (501) staff       (20)    49253 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)     3318 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    17617 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_env.py
--rw-r--r--   0 maurits    (501) staff       (20)    26958 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_group.py
--rw-r--r--   0 maurits    (501) staff       (20)    31336 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)    18992 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_relation.py
--rw-r--r--   0 maurits    (501) staff       (20)    35670 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_user.py
--rw-r--r--   0 maurits    (501) staff       (20)     9812 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/tests/test_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)    14825 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/user.py
--rw-r--r--   0 maurits    (501) staff       (20)     4862 2024-02-22 22:02:08.000000 plone.api-2.1.0/src/plone/api/validation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:02:10.309234 plone.api-2.1.0/src/plone.api.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    27517 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      272 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-22 22:02:10.000000 plone.api-2.1.0/src/plone.api.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3563 2024-02-22 22:02:08.000000 plone.api-2.1.0/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.500844 plone_api-2.2.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    23640 2024-05-06 12:56:06.000000 plone_api-2.2.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2024-05-06 12:56:06.000000 plone_api-2.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2024-05-06 12:56:06.000000 plone_api-2.2.0/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2024-05-06 12:56:06.000000 plone_api-2.2.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    28235 2024-05-06 12:56:07.500311 plone_api-2.2.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1936 2024-05-06 12:56:06.000000 plone_api-2.2.0/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.481537 plone_api-2.2.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    14247 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2295 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2024-05-06 12:56:06.000000 plone_api-2.2.0/docs/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)     4672 2024-05-06 12:56:06.000000 plone_api-2.2.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2024-05-06 12:56:07.501303 plone_api-2.2.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2383 2024-05-06 12:56:06.000000 plone_api-2.2.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.473945 plone_api-2.2.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.481953 plone_api-2.2.0/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.489096 plone_api-2.2.0/src/plone/api/
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      103 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    22805 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8041 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/env.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1051 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/exc.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11142 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14137 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.474452 plone_api-2.2.0/src/plone/api/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.489876 plone_api-2.2.0/src/plone/api/profiles/testfixture/
+-rw-r--r--   0 maurits    (501) staff       (20)      246 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/profiles/testfixture/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.490561 plone_api-2.2.0/src/plone/api/profiles/testfixture/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1939 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1927 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      264 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/profiles/testfixture/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    11490 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.495290 plone_api-2.2.0/src/plone/api/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1658 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.498665 plone_api-2.2.0/src/plone/api/tests/doctests/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    14247 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/doctests/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)    49245 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3301 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17620 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_env.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26959 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    31336 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18992 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35671 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9812 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/tests/test_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15308 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4862 2024-05-06 12:56:06.000000 plone_api-2.2.0/src/plone/api/validation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:56:07.499068 plone_api-2.2.0/src/plone.api.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    28235 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1682 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      450 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:56:07.000000 plone_api-2.2.0/src/plone.api.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     7162 2024-05-06 12:56:06.000000 plone_api-2.2.0/tox.ini
```

### Comparing `plone.api-2.1.0/CHANGES.rst` & `plone_api-2.2.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.2.0 (2024-05-06)
+------------------
+
+New features:
+
+
+- Report if a permission does not exist
+  when calling `api.user.has_permission`.
+  [gforcada] (#515)
+
+
+Bug fixes:
+
+
+- In relation.create: Fix edge case where existing RelationList value is None. @davisagli (#535)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 2.1.0 (2024-02-22)
 ------------------
 
 New features:
 
 
 - Implemented unrestricted find of content types. @gogobd (#312)
@@ -80,16 +104,16 @@
 2.0.4 (2023-07-14)
 ------------------
 
 Bug fixes:
 
 
 - Do not run GitHub Actions tests twice.
-  Only run GitHub Actions tests when commiting directly against master or main or
-  opening a pull request agains master or main. This avoids to run the same test
+  Only run GitHub Actions tests when committing directly against master or main or
+  opening a pull request against master or main. This avoids to run the same test
   suite for the same environment twice.
   [thet] (#0)
 - Mockup TinyMCE settings: Remove unused AtD related views.
 
   Fix a test which was checking for "checkDocument" among other available views.
   "checkDocument" was a TinyMCE endpoint for unmaintained "After the Deadline"
   plugin, which is now removed. (#504)
@@ -470,15 +494,15 @@
   [MrTango]
 
 Bug fixes:
 
 - Simplify the ``plone.api.content.delete`` method.
   [thet]
 
-- content.copy with safe_id=False should raise it's own exeception. Fixes #340
+- content.copy with safe_id=False should raise it's own exception. Fixes #340
   [jaroel]
 
 
 1.6.1 (2017-03-31)
 ------------------
 
 Bug fixes:
```

### Comparing `plone.api-2.1.0/LICENSE` & `plone_api-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/PKG-INFO` & `plone_api-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -18,32 +18,45 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Products.statusmessages
+Requires-Dist: Products.PlonePAS
+Requires-Dist: Products.CMFPlone
 Requires-Dist: decorator
 Requires-Dist: plone.app.uuid
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.intid
+Requires-Dist: plone.app.layout
 Requires-Dist: plone.app.linkintegrity
+Requires-Dist: plone.dexterity
+Requires-Dist: plone.i18n
+Requires-Dist: plone.registry
 Requires-Dist: plone.uuid
 Requires-Dist: setuptools
 Requires-Dist: zope.globalrequest
+Requires-Dist: Products.CMFCore
+Requires-Dist: z3c.relationfield
+Requires-Dist: zc.relation
+Requires-Dist: Zope
+Requires-Dist: zope.intid
 Provides-Extra: test
-Requires-Dist: Products.CMFPlone; extra == "test"
+Requires-Dist: borg.localrole; extra == "test"
 Requires-Dist: manuel>=1.11.2; extra == "test"
-Requires-Dist: plone.app.dexterity; extra == "test"
-Requires-Dist: plone.app.intid; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.textfield; extra == "test"
 Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
 Requires-Dist: plone.indexer; extra == "test"
 Requires-Dist: plone.registry; extra == "test"
-Requires-Dist: z3c.relationfield; extra == "test"
-Requires-Dist: zope.testrunner; extra == "test"
 
 # plone.api
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/plone.api.svg "Latest PyPI version")](https://pypi.python.org/pypi/plone.api/)
 
 
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/plone.api.svg "Number of PyPI downloads")](https://pypi.python.org/pypi/plone.api/)
@@ -84,25 +97,48 @@
 Continuous Integration
     tested on [GitHub Actions](https://github.com/plone/plone.api/actions).
 
 Code Coverage
     is measured at [Coveralls.io](https://coveralls.io/github/plone/plone.api).
 
 
-
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.2.0 (2024-05-06)
+------------------
+
+New features:
+
+
+- Report if a permission does not exist
+  when calling `api.user.has_permission`.
+  [gforcada] (#515)
+
+
+Bug fixes:
+
+
+- In relation.create: Fix edge case where existing RelationList value is None. @davisagli (#535)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 2.1.0 (2024-02-22)
 ------------------
 
 New features:
 
 
 - Implemented unrestricted find of content types. @gogobd (#312)
@@ -171,16 +207,16 @@
 2.0.4 (2023-07-14)
 ------------------
 
 Bug fixes:
 
 
 - Do not run GitHub Actions tests twice.
-  Only run GitHub Actions tests when commiting directly against master or main or
-  opening a pull request agains master or main. This avoids to run the same test
+  Only run GitHub Actions tests when committing directly against master or main or
+  opening a pull request against master or main. This avoids to run the same test
   suite for the same environment twice.
   [thet] (#0)
 - Mockup TinyMCE settings: Remove unused AtD related views.
 
   Fix a test which was checking for "checkDocument" among other available views.
   "checkDocument" was a TinyMCE endpoint for unmaintained "After the Deadline"
   plugin, which is now removed. (#504)
@@ -561,15 +597,15 @@
   [MrTango]
 
 Bug fixes:
 
 - Simplify the ``plone.api.content.delete`` method.
   [thet]
 
-- content.copy with safe_id=False should raise it's own exeception. Fixes #340
+- content.copy with safe_id=False should raise it's own exception. Fixes #340
   [jaroel]
 
 
 1.6.1 (2017-03-31)
 ------------------
 
 Bug fixes:
@@ -1153,15 +1189,14 @@
 0.1a1 (2012-07-13)
 ------------------
 
 - Initial release.
   [davisagli, fulv, iElectric, jcerjak, jonstahl, kcleong, mauritsvanrees,
   wamdam, witsch, zupo]
 
-
 License
 =======
 
 Copyright (C) 2012-2013 Plone Foundation
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License version 2
```

### Comparing `plone.api-2.1.0/README.md` & `plone_api-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/about.md` & `plone_api-2.2.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/content.md` & `plone_api-2.2.0/docs/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/env.md` & `plone_api-2.2.0/docs/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/group.md` & `plone_api-2.2.0/docs/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/index.md` & `plone_api-2.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/portal.md` & `plone_api-2.2.0/docs/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/relation.md` & `plone_api-2.2.0/docs/relation.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/docs/user.md` & `plone_api-2.2.0/docs/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/setup.py` & `plone_api-2.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,73 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
-import os
-
-
-def read(*rnames):
-    return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
+version = "2.2.0"
 
 long_description = (
-    read("README.md") + "\n\n" + read("CHANGES.rst") + "\n\n" + read("LICENSE")
+    f"{Path('README.md').read_text()}\n"
+    f"{Path('CHANGES.rst').read_text()}\n"
+    f"{Path('LICENSE').read_text()}"
 )
 
-version = "2.1.0"
-
 setup(
     name="plone.api",
     version=version,
     description="A Plone API.",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
     author="Plone Foundation",
     author_email="plone-developers@lists.sourceforge.net",
     license="GPL version 2",
     packages=find_packages("src"),
     package_dir={"": "src"},
     namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
     url="https://github.com/plone/plone.api",
     keywords="plone api",
     python_requires=">=3.8",
     install_requires=[
         "Products.statusmessages",
+        "Products.PlonePAS",
+        "Products.CMFPlone",
         "decorator",
         "plone.app.uuid",
+        "plone.app.dexterity",
+        "plone.app.intid",
+        "plone.app.layout",
         "plone.app.linkintegrity",
+        "plone.dexterity",
+        "plone.i18n",
+        "plone.registry",
         "plone.uuid",
         "setuptools",
         "zope.globalrequest",
+        "Products.CMFCore",
+        "z3c.relationfield",
+        "zc.relation",
+        "Zope",
+        "zope.intid",
     ],
     extras_require={
         "test": [
-            "Products.CMFPlone",
+            "borg.localrole",
             "manuel>=1.11.2",
-            "plone.app.dexterity",
-            "plone.app.intid",
+            "plone.app.contenttypes",
+            "plone.app.textfield",
             "plone.app.testing",
+            "plone.testing",
             "plone.indexer",
             "plone.registry",
-            "z3c.relationfield",
-            "zope.testrunner",
         ],
     },
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Intended Audience :: Developers",
```

### Comparing `plone.api-2.1.0/src/plone/api/content.py` & `plone_api-2.2.0/src/plone/api/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 @at_least_one_of("id", "title")
 def create(
     container=None,
     type=None,
     id=None,
     title=None,
     safe_id=False,
-    **kwargs  # NOQA: C816, S101
+    **kwargs,  # NOQA: C816, S101
 ):
     """Create a new content item.
 
     :param container: [required] Container object in which to create the new
         object.
     :type container: Folderish content object
     :param type: [required] Type of the object.
@@ -123,15 +123,15 @@
     :raises:
         ValueError,
     :Example: :ref:`content-get-example`
     """
     if path:
         site = portal.get()
         site_absolute_path = "/".join(site.getPhysicalPath())
-        if not path.startswith("{path}".format(path=site_absolute_path)):
+        if not path.startswith(f"{site_absolute_path}"):
             path = "{site_path}{relative_path}".format(
                 site_path=site_absolute_path,
                 relative_path=path,
             )
         try:
             content = site.restrictedTraverse(path)
         except (KeyError, AttributeError):
@@ -293,15 +293,15 @@
             context=site,
             request=site.REQUEST,
         )
         # look for breaches and manually raise a exception
         breaches = linkintegrity_view.get_breaches(objects)
         if breaches:
             raise LinkIntegrityNotificationException(
-                "Linkintegrity-breaches: {}".format(breaches),
+                f"Linkintegrity-breaches: {breaches}",
             )
 
     for obj_ in objects:
         obj_.aq_parent.manage_delObjects([obj_.getId()])
 
 
 @required_parameters("obj")
```

### Comparing `plone.api-2.1.0/src/plone/api/env.py` & `plone_api-2.2.0/src/plone/api/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,8 +227,8 @@
 
 def zope_version():
     """Return Zope 2 version number.
 
     :returns: string denoting what release of Zope2 this distribution contains
     :Example: :ref:`env-zope-version-example`
     """
-    return get_distribution("Zope2").version
+    return get_distribution("Zope").version
```

### Comparing `plone.api-2.1.0/src/plone/api/exc.py` & `plone_api-2.2.0/src/plone/api/exc.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/group.py` & `plone_api-2.2.0/src/plone/api/group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/portal.py` & `plone_api-2.2.0/src/plone/api/portal.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
 
     registry = getUtility(IRegistry)
 
     if interface is not None:
         records = registry.forInterface(interface, check=False)
         _marker = object()
         if getattr(records, name, _marker) != _marker:
-            return registry["{}.{}".format(interface.__identifier__, name)]
+            return registry[f"{interface.__identifier__}.{name}"]
 
         if default is not MISSING:
             return default
 
         # Show all records on the interface.
         records = [key for key in interface.names()]
         msg = (
@@ -303,15 +303,15 @@
         return registry[name]
 
     if default is not MISSING:
         return default
 
     # Show all records that 'look like' name.
     # We don't dump the whole list, because it 1500+ items.
-    msg = "Cannot find a record with name '{name}'".format(name=name)
+    msg = f"Cannot find a record with name '{name}'"
     records = [key for key in registry.records.keys() if name in key]
     if records:
         msg = (
             "{message}\n"
             "Did you mean?:\n"
             "{records}".format(message=msg, records="\n".join(records))
         )
```

### Comparing `plone.api-2.1.0/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml` & `plone_api-2.2.0/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml`

 * *Files 20% similar despite different names*

#### Comparing `plone.api-2.1.0/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml` & `plone_api-2.2.0/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Dexterity Folder" meta_type="Dexterity FTI">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Dexterity Folder">
   <property name="title">Dexterity Folder</property>
   <property name="description"/>
   <property name="content_icon"/>
   <property name="link_target"/>
   <property name="immediate_view">view</property>
   <property name="global_allow">True</property>
   <property name="filter_content_types">False</property>
@@ -22,14 +22,14 @@
   <property name="schema"/>
   <property name="model_source"/>
   <property name="model_file">plone.api.tests:Dexterity_Folder.xml</property>
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="" link_target="" title="View" url_expr="string:${object_url}" visible="True">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.api-2.1.0/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml` & `plone_api-2.2.0/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml`

 * *Files 18% similar despite different names*

#### Comparing `plone.api-2.1.0/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml` & `plone_api-2.2.0/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Dexterity Item" meta_type="Dexterity FTI">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Dexterity Item">
   <property name="title">Dexterity Item</property>
   <property name="description"/>
   <property name="content_icon"/>
   <property name="link_target"/>
   <property name="immediate_view">view</property>
   <property name="global_allow">True</property>
   <property name="filter_content_types">True</property>
@@ -22,14 +22,14 @@
   <property name="schema"/>
   <property name="model_source"/>
   <property name="model_file">plone.api.tests:Dexterity_Item.xml</property>
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="" link_target="" title="View" url_expr="string:${object_url}" visible="True">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.api-2.1.0/src/plone/api/relation.py` & `plone_api-2.2.0/src/plone/api/relation.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,24 +72,24 @@
     :type id: bool
     :returns: A list of relations
     :rtype: List of RelationValue objects
 
     :Example: :ref:`relation-get-example`
     """
     if source is not None and not base_hasattr(source, "portal_type"):
-        raise InvalidParameterError("{} has no portal_type".format(source))
+        raise InvalidParameterError(f"{source} has no portal_type")
 
     if target is not None and not base_hasattr(target, "portal_type"):
-        raise InvalidParameterError("{} has no portal_type".format(target))
+        raise InvalidParameterError(f"{target} has no portal_type")
 
     if relationship is not None and not isinstance(
         relationship,
         str,
     ):
-        raise InvalidParameterError("{} is no string".format(relationship))
+        raise InvalidParameterError(f"{relationship} is no string")
 
     intids = getUtility(IIntIds)
     relation_catalog = getUtility(ICatalog)
     query = {}
     results = []
 
     if as_dict:
@@ -146,21 +146,21 @@
         If that name is the same as a field name and this field
         is a RelationChoice / RelationList
         we will update the field-value accordingly.
     :type id: string
     :Example: :ref:`relation-create-example`
     """
     if source is not None and not base_hasattr(source, "portal_type"):
-        raise InvalidParameterError("{} has no portal_type".format(source))
+        raise InvalidParameterError(f"{source} has no portal_type")
 
     if target is not None and not base_hasattr(target, "portal_type"):
-        raise InvalidParameterError("{} has no portal_type".format(target))
+        raise InvalidParameterError(f"{target} has no portal_type")
 
     if not isinstance(relationship, str):
-        raise InvalidParameterError("{} is no string".format(relationship))
+        raise InvalidParameterError(f"{relationship} is no string")
 
     relation_catalog = getUtility(ICatalog)
     intids = getUtility(IIntIds)
     to_id = intids.getId(target)
     from_id = intids.getId(source)
     from_attribute = relationship
 
@@ -213,15 +213,15 @@
         logger.info(
             "Add relation to relationlist %s from %s to %s",
             from_attribute,
             source.absolute_url(),
             target.absolute_url(),
         )
         if not has_relation:
-            existing_relations = getattr(source, from_attribute, [])
+            existing_relations = getattr(source, from_attribute, None) or []
             existing_relations.append(RelationValue(to_id))
             setattr(source, from_attribute, existing_relations)
             modified(source)
         return
 
     elif isinstance(field, (Relation, RelationChoice)):
         logger.info(
@@ -263,24 +263,24 @@
         If that name is the same as a field name
         and this field is a RelationChoice/RelationList
         we will delete/update the field-value accordingly.
     :type id: string
     :Example: :ref:`relation-delete-example`
     """
     if source is not None and not base_hasattr(source, "portal_type"):
-        raise InvalidParameterError("{} has no portal_type".format(source))
+        raise InvalidParameterError(f"{source} has no portal_type")
 
     if target is not None and not base_hasattr(target, "portal_type"):
-        raise InvalidParameterError("{} has no portal_type".format(target))
+        raise InvalidParameterError(f"{target} has no portal_type")
 
     if relationship is not None and not isinstance(
         relationship,
         str,
     ):
-        raise InvalidParameterError("{} is no string".format(relationship))
+        raise InvalidParameterError(f"{relationship} is no string")
 
     query = {}
     relation_catalog = getUtility(ICatalog)
     intids = getUtility(IIntIds)
     if source is not None:
         query["from_id"] = intids.getId(source)
     if target is not None:
```

### Comparing `plone.api-2.1.0/src/plone/api/testing.zcml` & `plone_api-2.2.0/src/plone/api/testing.zcml`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="plone.api">
+    i18n_domain="plone.api"
+    >
 
-    <include package="Products.GenericSetup" file="meta.zcml"/>
+  <include
+      package="Products.GenericSetup"
+      file="meta.zcml"
+      />
 
-    <genericsetup:registerProfile
-        name="testfixture"
-        title="plone.api: Test fixture"
-        directory="profiles/testfixture"
-        description="Extension profile to configure a test fixture"
-        for="Products.CMFPlone.interfaces.ITestCasePloneSiteRoot"
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        />
+  <genericsetup:registerProfile
+      name="testfixture"
+      title="plone.api: Test fixture"
+      description="Extension profile to configure a test fixture"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="Products.CMFPlone.interfaces.ITestCasePloneSiteRoot"
+      directory="profiles/testfixture"
+      />
 
 </configure>
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/base.py` & `plone_api-2.2.0/src/plone/api/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/about.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/content.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/env.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/group.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/portal.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/relation.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/relation.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/doctests/user.md` & `plone_api-2.2.0/src/plone/api/tests/doctests/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_content.py` & `plone_api-2.2.0/src/plone/api/tests/test_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
         team_by_path = api.content.get("/about/team")
         team_by_uid = api.content.get(UID=self.team.UID())
         self.assertEqual(self.team, team_by_path)
         self.assertEqual(self.team, team_by_uid)
 
         # Test getting the team document by path that has portal id included
         team_by_path = api.content.get(
-            "/{}/about/team".format(self.portal.getId()),
+            f"/{self.portal.getId()}/about/team",
         )
         self.assertEqual(self.team, team_by_path)
 
         # Test getting an non-existing item by path and UID
         self.assertFalse(api.content.get("/spam/ham"))
         self.assertFalse(api.content.get(UID="bacon"))
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_doctests.py` & `plone_api-2.2.0/src/plone/api/tests/test_doctests.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,11 +121,11 @@
     docs_path = os.path.join(os.path.dirname(__file__), path)
 
     for filename in os.listdir(docs_path):
         try:
             doctests.append(DocFileSuite(os.path.join(path, filename)))
         except OSError:
             logger.warning(
-                "test_doctest.py skipping {file}".format(file=filename),
+                f"test_doctest.py skipping {filename}",
             )
 
     return unittest.TestSuite(doctests)
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_env.py` & `plone_api-2.2.0/src/plone/api/tests/test_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,15 +482,15 @@
         """Tests that missing arguments don't go unnoticed."""
         from plone.api.exc import MissingParameterError
 
         with self.assertRaises(MissingParameterError):
             api.env.adopt_roles()
 
     def test_debug_mode(self):
-        """Tests that the retured value is the same as
+        """Tests that the returned value is the same as
         getConfiguration.debug_mode."""
         from App.config import getConfiguration
         from plone.api.env import debug_mode
 
         getConfiguration().debug_mode = True
         self.assertEqual(debug_mode(), True)
         getConfiguration().debug_mode = False
@@ -526,22 +526,23 @@
     def test_adopt_user_different_username(self):
         user = api.user.get(userid=TEST_USER_ID)
         with api.env.adopt_user(user=user):
             self.assertEqual(api.user.get_current().getId(), TEST_USER_ID)
 
     def test_roles_restored_after_exception(self):
         """Tests that roles are restored after an exception."""
-        self.assertFalse(api.user.has_permission("Manage portal content"))
+        permission = "Manage properties"
+        self.assertFalse(api.user.has_permission(permission))
         try:
             with api.env.adopt_roles(["Manager"]):
-                self.assertTrue(api.user.has_permission("Manage portal content"))
+                self.assertTrue(api.user.has_permission(permission))
                 raise TestException("Test exception")
         except TestException:
             pass
-        self.assertFalse(api.user.has_permission("Manage portal content"))
+        self.assertFalse(api.user.has_permission(permission))
 
     def test_user_restored_after_exception(self):
         """Tests that roles are restored after an exception."""
         self.assertEqual(api.user.get_current().getUserId(), "boss")
         try:
             with api.env.adopt_user(username="superhuman"):
                 self.assertEqual(api.user.get_current().getUserId(), "superhuman")
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_group.py` & `plone_api-2.2.0/src/plone/api/tests/test_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         )
         group = self.group_tool.getGroupById("ham")
         self.assertEqual(ham_group, group)
         self.assertIn("Editor", ham_group.getRoles())
         self.assertIn("Reviewer", ham_group.getMemberIds())
 
     def test_get_constraints(self):
-        """Test the constraints for geting a group."""
+        """Test the constraints for getting a group."""
         from plone.api.exc import MissingParameterError
 
         with self.assertRaises(MissingParameterError):
             api.group.get()
 
     def test_get_no_groupname(self):
         """Test getting a group without passing a groupname."""
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_portal.py` & `plone_api-2.2.0/src/plone/api/tests/test_portal.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
         from plone.api.exc import InvalidParameterError
 
         with self.assertRaises(InvalidParameterError):
             portal.get_registry_record(name=dict({"foo": "bar"}))
 
     def test_get_invalid_registry_record_msg(self):
         """Test that the error message from trying to get a
-        nonexistant registry record produces an error message which
+        nonexistent registry record produces an error message which
         lists suggested registry records.
         """
         from plone.api.exc import InvalidParameterError
 
         with self.assertRaises(InvalidParameterError) as cm:
             portal.get_registry_record(name="nonexistent.sharepoint.power")
         exc_str = str(cm.exception)
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_relation.py` & `plone_api-2.2.0/src/plone/api/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_user.py` & `plone_api-2.2.0/src/plone/api/tests/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         )
         self.assertCountEqual(
             api.user.get_roles(user=user),
             ["Authenticated"],
         )
 
     def test_get_constraints(self):
-        """Test on raised exeption if no username is given when getting the user."""
+        """Test on raised exception if no username is given when getting the user."""
         from plone.api.exc import MissingParameterError
 
         with self.assertRaises(MissingParameterError):
             api.user.get()
 
     def test_get(self):
         """Test getting the user."""
```

### Comparing `plone.api-2.1.0/src/plone/api/tests/test_validation.py` & `plone_api-2.2.0/src/plone/api/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.1.0/src/plone/api/user.py` & `plone_api-2.2.0/src/plone/api/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     :param email: [required] Email for the new user.
     :type email: string
     :param username: Username for the new user. This is required if email
         is not used as a username.
     :type username: string
     :param password: Password for the new user. If it's not set we generate
-        a random 8-char alpha-numeric one.
+        a random 8-char alphanumeric one.
     :type password: string
     :param properties: User properties to assign to the new user. The list of
         available properties is available in ``portal_memberdata`` through ZMI.
     :type properties: dict
     :returns: Newly created user
     :rtype: MemberData object
     :raises:
@@ -323,15 +323,26 @@
 
     if username is None and user is None:
         context = _nop_context_manager()
     else:
         context = env.adopt_user(username, user)
 
     with context:
-        return bool(getSecurityManager().checkPermission(permission, obj))
+        return_value = bool(getSecurityManager().checkPermission(permission, obj))
+        if not return_value:
+            names = [x[0] for x in getPermissions()]
+            if permission not in names:
+                raise InvalidParameterError(
+                    "Cannot find a permission with name '{permission}'\n"
+                    "Available permissions are:\n"
+                    "{names}".format(
+                        permission=permission, names="\n".join(sorted(names))
+                    )
+                )
+        return return_value
 
 
 @required_parameters("roles")
 @mutually_exclusive_parameters("username", "user")
 def grant_roles(username=None, user=None, obj=None, roles=None):
     """Grant roles to a user.
```

### Comparing `plone.api-2.1.0/src/plone/api/validation.py` & `plone_api-2.2.0/src/plone/api/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import inspect
 
 
 def _get_arg_spec(func, validator_args):
     """Get the arguments specified in the function spec.
 
-    and check that the decorator doesn't refer to non-existant args.
+    and check that the decorator doesn't refer to non-existent args.
     """
     signature_args = inspect.getfullargspec(func).args
     extra_args = set(validator_args) - set(signature_args)
     if extra_args:
         raise ValueError(
             "Validator for {name} refers to parameters "
             "that are not part of the function signature: {signature}".format(
```

### Comparing `plone.api-2.1.0/src/plone.api.egg-info/PKG-INFO` & `plone_api-2.2.0/src/plone.api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -18,32 +18,45 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Products.statusmessages
+Requires-Dist: Products.PlonePAS
+Requires-Dist: Products.CMFPlone
 Requires-Dist: decorator
 Requires-Dist: plone.app.uuid
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.intid
+Requires-Dist: plone.app.layout
 Requires-Dist: plone.app.linkintegrity
+Requires-Dist: plone.dexterity
+Requires-Dist: plone.i18n
+Requires-Dist: plone.registry
 Requires-Dist: plone.uuid
 Requires-Dist: setuptools
 Requires-Dist: zope.globalrequest
+Requires-Dist: Products.CMFCore
+Requires-Dist: z3c.relationfield
+Requires-Dist: zc.relation
+Requires-Dist: Zope
+Requires-Dist: zope.intid
 Provides-Extra: test
-Requires-Dist: Products.CMFPlone; extra == "test"
+Requires-Dist: borg.localrole; extra == "test"
 Requires-Dist: manuel>=1.11.2; extra == "test"
-Requires-Dist: plone.app.dexterity; extra == "test"
-Requires-Dist: plone.app.intid; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.textfield; extra == "test"
 Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
 Requires-Dist: plone.indexer; extra == "test"
 Requires-Dist: plone.registry; extra == "test"
-Requires-Dist: z3c.relationfield; extra == "test"
-Requires-Dist: zope.testrunner; extra == "test"
 
 # plone.api
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/plone.api.svg "Latest PyPI version")](https://pypi.python.org/pypi/plone.api/)
 
 
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/plone.api.svg "Number of PyPI downloads")](https://pypi.python.org/pypi/plone.api/)
@@ -84,25 +97,48 @@
 Continuous Integration
     tested on [GitHub Actions](https://github.com/plone/plone.api/actions).
 
 Code Coverage
     is measured at [Coveralls.io](https://coveralls.io/github/plone/plone.api).
 
 
-
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.2.0 (2024-05-06)
+------------------
+
+New features:
+
+
+- Report if a permission does not exist
+  when calling `api.user.has_permission`.
+  [gforcada] (#515)
+
+
+Bug fixes:
+
+
+- In relation.create: Fix edge case where existing RelationList value is None. @davisagli (#535)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 2.1.0 (2024-02-22)
 ------------------
 
 New features:
 
 
 - Implemented unrestricted find of content types. @gogobd (#312)
@@ -171,16 +207,16 @@
 2.0.4 (2023-07-14)
 ------------------
 
 Bug fixes:
 
 
 - Do not run GitHub Actions tests twice.
-  Only run GitHub Actions tests when commiting directly against master or main or
-  opening a pull request agains master or main. This avoids to run the same test
+  Only run GitHub Actions tests when committing directly against master or main or
+  opening a pull request against master or main. This avoids to run the same test
   suite for the same environment twice.
   [thet] (#0)
 - Mockup TinyMCE settings: Remove unused AtD related views.
 
   Fix a test which was checking for "checkDocument" among other available views.
   "checkDocument" was a TinyMCE endpoint for unmaintained "After the Deadline"
   plugin, which is now removed. (#504)
@@ -561,15 +597,15 @@
   [MrTango]
 
 Bug fixes:
 
 - Simplify the ``plone.api.content.delete`` method.
   [thet]
 
-- content.copy with safe_id=False should raise it's own exeception. Fixes #340
+- content.copy with safe_id=False should raise it's own exception. Fixes #340
   [jaroel]
 
 
 1.6.1 (2017-03-31)
 ------------------
 
 Bug fixes:
@@ -1153,15 +1189,14 @@
 0.1a1 (2012-07-13)
 ------------------
 
 - Initial release.
   [davisagli, fulv, iElectric, jcerjak, jonstahl, kcleong, mauritsvanrees,
   wamdam, witsch, zupo]
 
-
 License
 =======
 
 Copyright (C) 2012-2013 Plone Foundation
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License version 2
```

### Comparing `plone.api-2.1.0/src/plone.api.egg-info/SOURCES.txt` & `plone_api-2.2.0/src/plone.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

