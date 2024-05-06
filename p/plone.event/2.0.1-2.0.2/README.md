# Comparing `tmp/plone.event-2.0.1.tar.gz` & `tmp/plone_event-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.event-2.0.1.tar", last modified: Fri Oct  6 22:09:06 2023, max compression
+gzip compressed data, was "plone_event-2.0.2.tar", last modified: Mon May  6 12:53:26 2024, max compression
```

## Comparing `plone.event-2.0.1.tar` & `plone_event-2.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:06.598961 plone.event-2.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     5108 2023-10-06 22:09:05.000000 plone.event-2.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-10-06 22:09:05.000000 plone.event-2.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-10-06 22:09:05.000000 plone.event-2.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     6466 2023-10-06 22:09:06.598383 plone.event-2.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      254 2023-10-06 22:09:05.000000 plone.event-2.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:06.586409 plone.event-2.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1181 2023-10-06 22:09:05.000000 plone.event-2.0.1/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-10-06 22:09:05.000000 plone.event-2.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      743 2023-10-06 22:09:05.000000 plone.event-2.0.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      726 2023-10-06 22:09:05.000000 plone.event-2.0.1/docs/contributors.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:06.586852 plone.event-2.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:06.594211 plone.event-2.0.1/plone/event/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      836 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)      154 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5624 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     7936 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)    20975 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/recurrence.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6553 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/recurrence_dateutil.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:06.597295 plone.event-2.0.1/plone/event/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1796 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/test_adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)      851 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/test_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)      426 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/test_recurrence_int_sequence.py
--rw-r--r--   0 maurits    (501) staff       (20)     7321 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/test_recurrence_sequence_ical.py
--rw-r--r--   0 maurits    (501) staff       (20)     2508 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/test_recurrence_sequence_timedelta.py
--rw-r--r--   0 maurits    (501) staff       (20)     2836 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    20393 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     3187 2023-10-06 22:09:05.000000 plone.event-2.0.1/plone/event/utils.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:09:06.590007 plone.event-2.0.1/plone.event.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     6466 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      939 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       98 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-10-06 22:09:06.000000 plone.event-2.0.1/plone.event.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4191 2023-10-06 22:09:05.000000 plone.event-2.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-10-06 22:09:06.599082 plone.event-2.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1618 2023-10-06 22:09:05.000000 plone.event-2.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:26.152235 plone_event-2.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     5541 2024-05-06 12:53:25.000000 plone_event-2.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:53:25.000000 plone_event-2.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2024-05-06 12:53:25.000000 plone_event-2.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     6899 2024-05-06 12:53:26.151708 plone_event-2.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      254 2024-05-06 12:53:25.000000 plone_event-2.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:26.139356 plone_event-2.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1181 2024-05-06 12:53:25.000000 plone_event-2.0.2/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2024-05-06 12:53:25.000000 plone_event-2.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      743 2024-05-06 12:53:25.000000 plone_event-2.0.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2024-05-06 12:53:25.000000 plone_event-2.0.2/docs/contributors.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:26.139822 plone_event-2.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:26.146705 plone_event-2.0.2/plone/event/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      836 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5624 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7489 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20975 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/recurrence.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6553 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/recurrence_dateutil.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:26.149874 plone_event-2.0.2/plone/event/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1796 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/test_adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      851 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/test_doctest.py
+-rw-r--r--   0 maurits    (501) staff       (20)      426 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/test_recurrence_int_sequence.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8149 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/test_recurrence_sequence_ical.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2508 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/test_recurrence_sequence_timedelta.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2836 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20393 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3187 2024-05-06 12:53:25.000000 plone_event-2.0.2/plone/event/utils.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:26.150446 plone_event-2.0.2/plone.event.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     6899 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      939 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       98 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:53:26.000000 plone_event-2.0.2/plone.event.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4191 2024-05-06 12:53:25.000000 plone_event-2.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:53:26.152310 plone_event-2.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1618 2024-05-06 12:53:25.000000 plone_event-2.0.2/setup.py
```

### Comparing `plone.event-2.0.1/CHANGES.rst` & `plone_event-2.0.2/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Keep the rrule UNTIL property UTC specifier, if defined.
+  [mamico] (30-2)
+- Set the rrule's EXDATE to the same time as the event's start time.
+  In our implementation we want the rrule's EXDATE property to have the same time as the event's start time.
+  Otherwise recurrence dates might be included where they should not due to an user-undefined EXDATE time.
+  [mamico] (#30)
+
+
 2.0.1 (2023-10-07)
 ------------------
 
 Bug fixes:
 
 
 - Ignore dtstart and until time in rrule in recurrence_sequence_ical [mamico] (#23)
```

### Comparing `plone.event-2.0.1/PKG-INFO` & `plone_event-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.event
-Version: 2.0.1
+Version: 2.0.2
 Summary: Event and calendaring related tools not bound to Plone
 Home-page: https://github.com/plone/plone.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Plone calendar calendaring event recurring
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Keep the rrule UNTIL property UTC specifier, if defined.
+  [mamico] (30-2)
+- Set the rrule's EXDATE to the same time as the event's start time.
+  In our implementation we want the rrule's EXDATE property to have the same time as the event's start time.
+  Otherwise recurrence dates might be included where they should not due to an user-undefined EXDATE time.
+  [mamico] (#30)
+
+
 2.0.1 (2023-10-07)
 ------------------
 
 Bug fixes:
 
 
 - Ignore dtstart and until time in rrule in recurrence_sequence_ical [mamico] (#23)
```

### Comparing `plone.event-2.0.1/docs/INSTALL.txt` & `plone_event-2.0.2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/docs/LICENSE.GPL` & `plone_event-2.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/docs/LICENSE.txt` & `plone_event-2.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/docs/contributors.rst` & `plone_event-2.0.2/docs/contributors.rst`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/adapters.py` & `plone_event-2.0.2/plone/event/adapters.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/interfaces.py` & `plone_event-2.0.2/plone/event/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/recurrence.py` & `plone_event-2.0.2/plone/event/recurrence.py`

 * *Files 26% similar despite different names*

```diff
@@ -68,47 +68,48 @@
     _until = tzdel(until)
     if duration:
         assert isinstance(duration, datetime.timedelta)
     else:
         duration = datetime.timedelta(0)
 
     if recrule:
-        # We want the recurrence be calculated ignoring the DTSTART,
-        # which is defined by the event's own start.
-        # ‌ Also set the UNTIL time to the end of the day to include the last
-        # occurrence for sure.
-        #
-        # start is a mandatory parameter for this function, remove DTSTART
-        # from recrule
-        recrule = re.sub(r"DTSTART:[^;\n]*[;\n]", "", recrule, re.MULTILINE)
-        # TODO BUGFIX WRONG TIME DEFINITIONS
-        # THIS HACK ensures, that UNTIL, RDATE and EXDATE definitions with
-        # incorrect time (currently always set to 0:00 by the recurrence
-        # widget) are handled correctly.
-        #
-        # Following fixes are made:
-        # - The UNTIL date should be included in the recurrence set, as defined
-        #   by RFC5545 (fix sets it to the end of the day)
-        # - RDATE definitions should have the same time as the start date.
-        # - EXDATE definitions should exclude occurrences on the specific date
-        #   only the same time as the start date.
-        # In the long term ,the recurrence widget should be able to set the
-        # time for UNTIL, RDATE and EXDATE.
-        t0 = start.time()  # set initial time information.
-        # First, replace all times in the recurring rule with starttime
+        # The event's start time.
+        t0 = start.time()
+        # The event's start time as RFC8601 string
         t0str = f"T{t0.hour:02d}{t0.minute:02d}{t0.second:02d}"
-        # Replace any times set to 000000 with start time, not all
-        # rrules are set by a specific broken widget.  Don't waste time
-        # subbing if the start time is already 000000.
+
+        # 1) Remove DTSTART from the recurrence rule
+        # The start date is always included and therefore removed from the
+        # recurrence rule.
+        recrule = re.sub(r"DTSTART:[^;\n]*[;\n]", "", recrule, re.MULTILINE)
+
+        # 2) Set all RDATE (actually any) time definitions to the start date of
+        # the event, except for those explicitly set to 00:00:00 which might
+        # come from recurrence rule widgets which explicitly set it to that
+        # time.
         if t0str != "T000000":
             recrule = re.sub(r"T000000", t0str, recrule)
-        # Then, replace each until times with the end of the day
+
+        # 3) Set the UNTIL times to the end of the day to make sure to include
+        # any possible occurrence on that date.
+        recrule = re.sub(
+            r"(UNTIL[^T]*[0-9]{8})T([0-9]{6})(Z?)",
+            r"\1T235959\3",
+            recrule,
+        )
+
+        # 4) Set the EXDATE properties to the same start time as the event's
+        # start time to make sure to really exclude those occurrences.
         recrule = re.sub(
-            r"(UNTIL[^T]*[0-9]{8})T([0-9]{6}Z?)",
-            r"\1T235959",
+            r"EXDATE:([^\n\s]+)",
+            lambda m: re.sub(
+                r"T[0-9]{6}(Z?)",
+                rf"{t0str}\1",
+                m.group(0),
+            ),
             recrule,
         )
 
         # RFC2445 string
         # forceset: always return a rruleset
         # dtstart: optional used when no dtstart is in RFC2445 string
         #          dtstart is given as timezone naive time. timezones are
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plone.event-2.0.1/plone/event/recurrence.rst` & `plone_event-2.0.2/plone/event/recurrence.rst`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/recurrence_dateutil.rst` & `plone_event-2.0.2/plone/event/recurrence_dateutil.rst`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/tests/test_adapters.py` & `plone_event-2.0.2/plone/event/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/tests/test_doctest.py` & `plone_event-2.0.2/plone/event/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/tests/test_recurrence_sequence_ical.py` & `plone_event-2.0.2/plone/event/tests/test_recurrence_sequence_ical.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,7 +191,29 @@
         start = at.localize(datetime(2023, 9, 4, 1, 0))
         # DTSTART is ignored, because start is ever explicitly given
         recrule = "DTSTART:20230903T180000Z\nRRULE:FREQ=DAILY;UNTIL=20230905T230000Z"
         seq = list(recurrence_sequence_ical(start, recrule=recrule))
         self.assertEqual(len(seq), 2)
         self.assertEqual(seq[0], at.localize(datetime(2023, 9, 4, 1, 0)))
         self.assertEqual(seq[1], at.localize(datetime(2023, 9, 5, 1, 0)))
+
+    def test_recrule_with_exclude(self):
+        from datetime import datetime
+        from plone.event.recurrence import recurrence_sequence_ical
+
+        import pytz
+
+        at = pytz.timezone("UTC")
+        recrule = (
+            "RRULE:FREQ=DAILY;INTERVAL=1;UNTIL=20240428T100000Z\n"
+            "EXDATE:20240423T100000Z,20240425T100000Z"
+        )
+
+        # EXDATE with same time as start date should be excluded
+        start = at.localize(datetime(2024, 4, 22, 10, 0))
+        seq = list(recurrence_sequence_ical(start, recrule=recrule))
+        self.assertEqual(len(seq), 5)
+
+        # even EXDATE with different time as start date should be excluded
+        start = at.localize(datetime(2024, 4, 22, 14, 0))
+        seq = list(recurrence_sequence_ical(start, recrule=recrule))
+        self.assertEqual(len(seq), 5)
```

### Comparing `plone.event-2.0.1/plone/event/tests/test_recurrence_sequence_timedelta.py` & `plone_event-2.0.2/plone/event/tests/test_recurrence_sequence_timedelta.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/tests/test_utils.py` & `plone_event-2.0.2/plone/event/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/utils.py` & `plone_event-2.0.2/plone/event/utils.py`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone/event/utils.rst` & `plone_event-2.0.2/plone/event/utils.rst`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/plone.event.egg-info/PKG-INFO` & `plone_event-2.0.2/plone.event.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.event
-Version: 2.0.1
+Version: 2.0.2
 Summary: Event and calendaring related tools not bound to Plone
 Home-page: https://github.com/plone/plone.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: Plone calendar calendaring event recurring
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Keep the rrule UNTIL property UTC specifier, if defined.
+  [mamico] (30-2)
+- Set the rrule's EXDATE to the same time as the event's start time.
+  In our implementation we want the rrule's EXDATE property to have the same time as the event's start time.
+  Otherwise recurrence dates might be included where they should not due to an user-undefined EXDATE time.
+  [mamico] (#30)
+
+
 2.0.1 (2023-10-07)
 ------------------
 
 Bug fixes:
 
 
 - Ignore dtstart and until time in rrule in recurrence_sequence_ical [mamico] (#23)
```

### Comparing `plone.event-2.0.1/plone.event.egg-info/SOURCES.txt` & `plone_event-2.0.2/plone.event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/pyproject.toml` & `plone_event-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.event-2.0.1/setup.py` & `plone_event-2.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.1"
+version = "2.0.2"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="plone.event",
```

