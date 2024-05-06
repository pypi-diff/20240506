# Comparing `tmp/frozendict-2.4.3.tar.gz` & `tmp/frozendict-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frozendict-2.4.3.tar", last modified: Sun May  5 14:08:51 2024, max compression
+gzip compressed data, was "frozendict-2.4.4.tar", last modified: Mon May  6 19:32:35 2024, max compression
```

## Comparing `frozendict-2.4.3.tar` & `frozendict-2.4.4.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.206916 frozendict-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-05 14:08:44.000000 frozendict-2.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 14:08:44.000000 frozendict-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-05 14:08:51.206916 frozendict-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22190 2024-05-05 14:08:44.000000 frozendict-2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 14:08:44.000000 frozendict-2.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 14:08:51.206916 frozendict-2.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6265 2024-05-05 14:08:44.000000 frozendict-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.186916 frozendict-2.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.194916 frozendict-2.4.3/src/frozendict/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/_frozendict_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.190916 frozendict-2.4.3/src/frozendict/c_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.194916 frozendict-2.4.3/src/frozendict/c_src/3_10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.194916 frozendict-2.4.3/src/frozendict/c_src/3_10/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.194916 frozendict-2.4.3/src/frozendict/c_src/3_10/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.194916 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.194916 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    57234 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   152447 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    60336 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_10/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    63009 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   135061 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    58155 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_6/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    61834 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   132228 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.198916 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    58478 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_7/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    58062 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   141374 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    60418 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_8/frozendictobject.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/Include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/Include/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/Include/frozendictobject.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
--rw-r--r--   0 runner    (1001) docker     (127)    58099 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)   145558 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.202916 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/other.c
--rw-r--r--   0 runner    (1001) docker     (127)    60489 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/c_src/3_9/frozendictobject.c
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/cool.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 14:08:44.000000 frozendict-2.4.3/src/frozendict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.206916 frozendict-2.4.3/src/frozendict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-05 14:08:51.000000 frozendict-2.4.3/src/frozendict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-05 14:08:51.000000 frozendict-2.4.3/src/frozendict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 14:08:51.000000 frozendict-2.4.3/src/frozendict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 14:08:51.000000 frozendict-2.4.3/src/frozendict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:51.206916 frozendict-2.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7607 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    14954 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14534 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/frozendict_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/subclass_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/test_frozendict.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/test_frozendict_subclass.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1888 2024-05-05 14:08:44.000000 frozendict-2.4.3/test/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.955710 frozendict-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-06 19:32:31.000000 frozendict-2.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 19:32:31.000000 frozendict-2.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-06 19:32:35.955710 frozendict-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22190 2024-05-06 19:32:31.000000 frozendict-2.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 19:32:31.000000 frozendict-2.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:32:35.955710 frozendict-2.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6265 2024-05-06 19:32:31.000000 frozendict-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.935710 frozendict-2.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.939710 frozendict-2.4.4/src/frozendict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/_frozendict_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.939710 frozendict-2.4.4/src/frozendict/c_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57234 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   152447 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    60336 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_10/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_6/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_6/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.943710 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63009 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   135061 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    58155 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_6/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61834 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   132228 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    58478 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_7/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_8/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_8/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.947710 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58062 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   141374 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    60418 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_8/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/Include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58099 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)   145558 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.951710 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (127)    60489 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/c_src/3_9/frozendictobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:32:31.000000 frozendict-2.4.4/src/frozendict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.955710 frozendict-2.4.4/src/frozendict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-06 19:32:35.000000 frozendict-2.4.4/src/frozendict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-06 19:32:35.000000 frozendict-2.4.4/src/frozendict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:32:35.000000 frozendict-2.4.4/src/frozendict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 19:32:35.000000 frozendict-2.4.4/src/frozendict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:35.955710 frozendict-2.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7607 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14954 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14534 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/frozendict_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/subclass_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/test_frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/test_frozendict_subclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1888 2024-05-06 19:32:31.000000 frozendict-2.4.4/test/typed.py
```

### Comparing `frozendict-2.4.3/LICENSE.txt` & `frozendict-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/PKG-INFO` & `frozendict-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.4.3
+Version: 2.4.4
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.4.3/README.md` & `frozendict-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/setup.py` & `frozendict-2.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/__init__.py` & `frozendict-2.4.4/src/frozendict/__init__.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/__init__.pyi` & `frozendict-2.4.4/src/frozendict/__init__.pyi`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/_frozendict_py.py` & `frozendict-2.4.4/src/frozendict/_frozendict_py.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/Include/frozendictobject.h` & `frozendict-2.4.4/src/frozendict/c_src/3_10/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h` & `frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/cpython_src/other.c` & `frozendict-2.4.4/src/frozendict/c_src/3_10/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_10/frozendictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_10/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/Include/frozendictobject.h` & `frozendict-2.4.4/src/frozendict/c_src/3_6/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h` & `frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/cpython_src/other.c` & `frozendict-2.4.4/src/frozendict/c_src/3_6/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_6/frozendictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_6/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/Include/frozendictobject.h` & `frozendict-2.4.4/src/frozendict/c_src/3_7/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h` & `frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.4/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_7/frozendictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_7/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/Include/frozendictobject.h` & `frozendict-2.4.4/src/frozendict/c_src/3_8/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h` & `frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/cpython_src/other.c` & `frozendict-2.4.4/src/frozendict/c_src/3_8/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_8/frozendictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_8/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/Include/frozendictobject.h` & `frozendict-2.4.4/src/frozendict/c_src/3_9/Include/frozendictobject.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h` & `frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h` & `frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c` & `frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h` & `frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/cpython_src/other.c` & `frozendict-2.4.4/src/frozendict/c_src/3_9/cpython_src/other.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/c_src/3_9/frozendictobject.c` & `frozendict-2.4.4/src/frozendict/c_src/3_9/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/cool.py` & `frozendict-2.4.4/src/frozendict/cool.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict/monkeypatch.py` & `frozendict-2.4.4/src/frozendict/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/src/frozendict.egg-info/PKG-INFO` & `frozendict-2.4.4/src/frozendict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.4.3
+Version: 2.4.4
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.4.3/src/frozendict.egg-info/SOURCES.txt` & `frozendict-2.4.4/src/frozendict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/base.py` & `frozendict-2.4.4/test/base.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/bench.py` & `frozendict-2.4.4/test/bench.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/common.py` & `frozendict-2.4.4/test/common.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/debug.py` & `frozendict-2.4.4/test/debug.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/frozendict_only.py` & `frozendict-2.4.4/test/frozendict_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/subclass_only.py` & `frozendict-2.4.4/test/subclass_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/test_freeze.py` & `frozendict-2.4.4/test/test_freeze.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/test_frozendict_subclass.py` & `frozendict-2.4.4/test/test_frozendict_subclass.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.4.3/test/typed.py` & `frozendict-2.4.4/test/typed.py`

 * *Files identical despite different names*

