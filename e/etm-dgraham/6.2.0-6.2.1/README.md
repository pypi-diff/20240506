# Comparing `tmp/etm-dgraham-6.2.0.tar.gz` & `tmp/etm-dgraham-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.2.0.tar", last modified: Sat May  4 10:40:25 2024, max compression
+gzip compressed data, was "etm-dgraham-6.2.1.tar", last modified: Mon May  6 10:36:54 2024, max compression
```

## Comparing `etm-dgraham-6.2.0.tar` & `etm-dgraham-6.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-04 10:40:25.937248 etm-dgraham-6.2.0/
--rw-r--r--   0 dag        (501) staff       (20)     7159 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.0/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   140777 2024-05-04 10:40:25.937004 etm-dgraham-6.2.0/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   139208 2024-04-24 18:26:45.000000 etm-dgraham-6.2.0/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.0/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.0/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-04 10:40:25.931427 etm-dgraham-6.2.0/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.0/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.0/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.0/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-04 10:40:25.933198 etm-dgraham-6.2.0/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.0/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    26465 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.0/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.0/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   329580 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38891 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126266 2024-05-04 10:40:20.000000 etm-dgraham-6.2.0/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-04 10:40:25.935560 etm-dgraham-6.2.0/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   140777 2024-05-04 10:40:25.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-04 10:40:25.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-04 10:40:25.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-04 10:40:25.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-04 10:40:25.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-04 10:40:25.000000 etm-dgraham-6.2.0/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.0/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.0/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.0/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.0/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.2.0/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.0/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-04 10:40:25.937290 etm-dgraham-6.2.0/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.0/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-04 10:40:25.935690 etm-dgraham-6.2.0/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.0/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-04 10:40:25.936486 etm-dgraham-6.2.0/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.0/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.0/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.0/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.0/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.397990 etm-dgraham-6.2.1/
+-rw-r--r--   0 dag        (501) staff       (20)     6418 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   145616 2024-05-06 10:36:54.397757 etm-dgraham-6.2.1/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   144047 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.1/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.1/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.390507 etm-dgraham-6.2.1/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.393399 etm-dgraham-6.2.1/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-05 16:45:06.000000 etm-dgraham-6.2.1/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.1/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.1/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   329909 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38891 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126266 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.395795 etm-dgraham-6.2.1/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   145616 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.1/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.1/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-06 10:36:54.398036 etm-dgraham-6.2.1/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.1/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.395910 etm-dgraham-6.2.1/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.1/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.397211 etm-dgraham-6.2.1/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.1/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.1/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.1/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.2.0/CHANGES.txt` & `etm-dgraham-6.2.1/CHANGES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,44 @@
-2024-05-04 8132171 Daniel Graham
+2024-05-06 9c3ccea Daniel Graham
+    Tagged version 6.2.1.
+
+2024-05-06 272ef22 Daniel Graham
+    Fixed sorting bug in do next view
+
+2024-05-05 bd65af8 Daniel Graham
+    README tweaks
+
+2024-05-05 e337b72 Daniel Graham
+    README tweaks
+
+2024-05-05 68b9823 Daniel Graham
+    README tweaks
+
+2024-05-05 1789fb5 Daniel Graham
+    Merge branch 'working'
+
+2024-05-05 abf7a33 Daniel Graham
+    First pass at adding goals to README
+
+2024-05-05 a58c62f Daniel Graham
+    Merge branch 'working'
+
+2024-05-05 92a4a5b Daniel Graham
+    Updated implementing_goals
+
+2024-05-05 f71fd6c Daniel Graham
+    Updates for implementing_goals
+
+2024-05-04 65f93a4 Daniel Graham
+    Updated docs/implementing_goals.md
+
+2024-05-04 8601216 Daniel Graham
+    Updated docs/implementing_goals.md
+
+2024-05-04 6ffaa2f Daniel Graham
     Tagged version 6.2.0. Added a new item type, goal, and a
     corresponding goal view.
 
 2024-05-04 bd93aab Daniel Graham
     Merge branch 'working' into goals
 
 2024-05-04 9aa9c5f Daniel Graham
@@ -171,55 +207,7 @@
     Refactored timer_report and show_timers into get_timers. Added
     round_to_minutes to ensure that the total reported in timer view
     is consistent with the items listed. In reporting the moment a
     timer status last changed use the datetime if the change occurred
     on the current date and the timedelta between the current moment
     and the datetime otherwise. Added 'inactive' to type_colors.
     Changed default 'light' type_colors for 'paused' and 'running'.
-
-2024-02-29 0a6134f Daniel Graham
-    Tagged version 6.1.14.
-
-2024-02-29 465af5b Daniel Graham
-    Removed extraneous 'level=0
-    '
-
-2024-02-29 1b565b0 Daniel Graham
-    Tagged version 6.1.13. Conditionally show active timer in
-    statusbar 2nd line
-
-2024-02-29 fbe470f Daniel Graham
-    Fixed leap year bug in archiving items. Refactored fitting strings
-    into available terminal width using 'truncate_string'. Added
-    'conditional' status bar second line to show active timer when one
-    exists. Removed unused 'level' argument from NDict as_tree.
-    Reformated timer report to show total time for item, the current
-    status and the moment the status last changed.
-
-2024-02-24 f71dfcd Daniel Graham
-    Tagged version 6.1.12.
-
-2024-02-24 d0f5f18 Daniel Graham
-    Added 'show occurrences' bound to 'o' to display a list of fields
-    such as @i, @l, ..., with the distince occurrences of each and the
-    number of times used.
-
-2024-02-16 878447b Daniel Graham
-    Tagged version 6.1.11.
-
-2024-02-16 53022e3 Daniel Graham
-    Corrected wording in README regarding tab completion for @k
-    entries.
-
-2024-02-16 2f48d58 Daniel Graham
-    Jinja template tweaks for wrapping @d entries. Bind N (along with
-    +) to create new item but only if is_not_searching.
-
-2024-02-13 f99e118 Daniel Graham
-    Tagged version 6.1.10.
-
-2024-02-13 f4ac9a4 Daniel Graham
-    Fixed bug in processing do_reschedule when an empty string is
-    returned.
-
-2024-02-12 1c2f8be Daniel Graham
-    Tagged version 6.1.9.
```

### Comparing `etm-dgraham-6.2.0/PKG-INFO` & `etm-dgraham-6.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.0
+Version: 6.2.1
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -55,14 +55,15 @@
             -   [just in time entry prompts and feedback](#just-in-time-entry-prompts-and-feedback)
             -   [fuzzy parsing of datetimes](#fuzzy-parsing-of-datetimes)
             -   [relative datetimes](#relative-datetimes)
             -   [tab completion](#tab-completion)
     -   [Views](#views)
         -   [Weekly Views](#weekly-views)
         -   [Do Next View](#do-next-view)
+        -   [Goals View](#goals-view)
         -   [Timer View](#timer-view)
         -   [Review View](#review-view)
         -   [Pinned View](#pinned-view)
         -   [Konnected View](#konnected-view)
         -   [Used Time Views](#used-time-views)
         -   [Query View](#query-view)
             -   [Simple queries](#simple-queries)
@@ -93,14 +94,15 @@
         -   [From a virtual environment](#from-a-virtual-environment)
         -   [From a system wide installation](#from-a-system-wide-installation)
 -   [Details](#details)
     -   [Item Types](#item-types)
         -   [event](#event)
         -   [task](#task)
         -   [journal](#journal)
+        -   [goal](#goal)
         -   [inbox](#inbox)
         -   [status](#status)
             -   [beginning soon](#beginning-soon)
             -   [past due](#past-due)
             -   [waiting](#waiting)
             -   [finished](#finished)
     -   [Options](#options)
@@ -524,14 +526,15 @@
 
   * a: Agenda: dated unfinished tasks and other reminders by year-week and week day
   * b: Busy: a graphical illustration of busy and conflicted times by year-week
   * c: Completed: finished tasks and jobs and used time entries by year-week and week day
   * d: Do Next: undated tasks grouped by location/context and ordered by priority (highest first) and extent (least first)
   * e: Effort: instances of reminders with used time entries with daily totals displayed graphically
   * f: Forthcoming: unfinished dated tasks and other dated reminders by next occurrence
+  * g: Goals: the status of all *goal* reminders as of the current year and week
   * h: History: all items by the latter of the modified or created datetimes in descending order, i.e., most recent first. Datetimes are displayed using a 5 character format where, e.g., 1:15pm today would be displayed as 13:15, November 7 of the current year as 11/17 and January 15 of 2012 as 12.01.
   * i: Index: all items grouped hierarchically by index entry
   * j: Journal: journal entries grouped hierarchically by index entry
   * k: Konnection: items with @k konnection links either to or from the selected item.
   * l: Location: items grouped hierarchically by location entry
   * m: Timers: items with timers.
   * p: Pinned: items whose pin status is on.
@@ -603,14 +606,44 @@
         'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
         '{', '|', '}', '~'
 
 Context is useful for more than just the sorting order. Suppose you have a task that you want to deal with the next time you’re at the lake house. Just add `@l at/lake house` and all you have to remember is to check the subgroup 'lake house ' under the 'at' group in *do next view* when you’re next there. Many such contexts come to mind - `at/grocery store`, `at/office`, ...
 
 One final useful context is 'waiting for'. E.g., completing a task might depend upon getting something from Joe. Add `@l waiting for/Joe` to the task and it will be listed in the subgroup 'Joe' under 'waiting for'.
 
+[↺ contents](#contents)
+
+### Goals View {#goals-view}
+
+This is a dedicated view *only for goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current week*. 
+
+This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
+
+Consider this illustrative screenshot from *Goals View*:
+
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/walk_the_dog.png" alt="new" title="goals view" width="600px" hspace="20px"/>
+
+Notice first that there is no heading displaying a date or week since *goal view* displays the status of *all* goals at the *current time*. 
+
+In this screen shot "walk the dog" is selected and its details panel is displayed. The leading "3/7+2 (4.8)" in the main window indicates that 3 instances of the goal of 7 have been completed in the current week, that 2 more completions today are needed to get back on schedule for the week and that 4.8 is the current average number of the entire history completions per week for this goal. This history is displayed in the details panel.
+
+In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
+- walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
+- wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
+- interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
+
+This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
+- F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*.
+- ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
+
+A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
+
+[↺ contents](#contents)
+
 ### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and the elapsed time and *state* of the associated timer.
 
 The sort order assures that the reminder with the active timer will always be at the top of the list and followed by the reminders with the most recently modified timers. This makes it easy to switch back and forth between recent timers.
 
 [↺ contents](#contents)
@@ -1747,14 +1780,35 @@
 - Journal entries with @s entries associate the entry with the datetime given by @s. A vacation log entry, for example, might record the highlights of the day given by @s. They are displayed in *Agenda* view as well as *Journal* view.
 - While Journal entries do not support repetition using `@r` entries, they do support the use of `@+` entries to add additional dates or datetimes to that provided by the `@s` entry.
 
 Corresponds to VJOURNAL in the vcalendar specification.
 
 [↺ contents](#contents)
 
+### goal {#goal}
+
+Type character: **~**
+
+The goal itemtype is intended to support pursuing S.M.A.R.T. goals (Specific, Measurable, Achievable, Relevant, Timed) in *etm*. Here is an example of a *goal* as it would be entered:
+
+```
+    ~ interval training @s 2024/4/22 @q 3
+```
+- It is a *goal* because of the `~` type character. 
+- Because I have a custom interval setting on my exercise bike, "interval training" is *specific* and *measurable*. It is also *achievable* and *relevant* for me.
+- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically converted to the Monday of the corresponding week.
+- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3, 5`  then the goal would have been 3 times per week repeated for 5 weeks.
+- If this goal were selected in *etm* on, say, Wednesday, April 24 and "F" were pressed, then *etm* would add an `@h 2024:17 1` (history of completions) entry to indicate 1 completion of the goal for the week of *2024:17*. Pressing "F" again in the same week with this goal selected would change this entry to `@h 2024:17 2`.  As one last example, pressing "F" with the goal selected sometime during the week of *2024:18* would leave the recorded entry as
+
+    ```
+    ~ interval training @s 2024/4/29 @q 3 @h 2024:17 2, 2024:18 1
+    ```
+
+[↺ contents](#contents)
+
 ### inbox {#inbox}
 
 Type character: **!**
 
 An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the scheduled time.
 
 Inbox items are also useful when you have an idea but not enough time to think about it. Create an inbox entry with just enough information in the summary to remind you of the idea. Make a habit at the end of the day of checking inbox items. The idea is not necessarily to complete them but to change those that can’t be finished quickly to, say, undated tasks with appropriate `@l` entries and enough detail in the summaries and the `@d` descriptions so that you will have all the information you need to act on them when the time comes.
```

### Comparing `etm-dgraham-6.2.0/README.md` & `etm-dgraham-6.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
             -   [just in time entry prompts and feedback](#just-in-time-entry-prompts-and-feedback)
             -   [fuzzy parsing of datetimes](#fuzzy-parsing-of-datetimes)
             -   [relative datetimes](#relative-datetimes)
             -   [tab completion](#tab-completion)
     -   [Views](#views)
         -   [Weekly Views](#weekly-views)
         -   [Do Next View](#do-next-view)
+        -   [Goals View](#goals-view)
         -   [Timer View](#timer-view)
         -   [Review View](#review-view)
         -   [Pinned View](#pinned-view)
         -   [Konnected View](#konnected-view)
         -   [Used Time Views](#used-time-views)
         -   [Query View](#query-view)
             -   [Simple queries](#simple-queries)
@@ -50,14 +51,15 @@
         -   [From a virtual environment](#from-a-virtual-environment)
         -   [From a system wide installation](#from-a-system-wide-installation)
 -   [Details](#details)
     -   [Item Types](#item-types)
         -   [event](#event)
         -   [task](#task)
         -   [journal](#journal)
+        -   [goal](#goal)
         -   [inbox](#inbox)
         -   [status](#status)
             -   [beginning soon](#beginning-soon)
             -   [past due](#past-due)
             -   [waiting](#waiting)
             -   [finished](#finished)
     -   [Options](#options)
@@ -481,14 +483,15 @@
 
   * a: Agenda: dated unfinished tasks and other reminders by year-week and week day
   * b: Busy: a graphical illustration of busy and conflicted times by year-week
   * c: Completed: finished tasks and jobs and used time entries by year-week and week day
   * d: Do Next: undated tasks grouped by location/context and ordered by priority (highest first) and extent (least first)
   * e: Effort: instances of reminders with used time entries with daily totals displayed graphically
   * f: Forthcoming: unfinished dated tasks and other dated reminders by next occurrence
+  * g: Goals: the status of all *goal* reminders as of the current year and week
   * h: History: all items by the latter of the modified or created datetimes in descending order, i.e., most recent first. Datetimes are displayed using a 5 character format where, e.g., 1:15pm today would be displayed as 13:15, November 7 of the current year as 11/17 and January 15 of 2012 as 12.01.
   * i: Index: all items grouped hierarchically by index entry
   * j: Journal: journal entries grouped hierarchically by index entry
   * k: Konnection: items with @k konnection links either to or from the selected item.
   * l: Location: items grouped hierarchically by location entry
   * m: Timers: items with timers.
   * p: Pinned: items whose pin status is on.
@@ -560,14 +563,44 @@
         'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
         '{', '|', '}', '~'
 
 Context is useful for more than just the sorting order. Suppose you have a task that you want to deal with the next time you’re at the lake house. Just add `@l at/lake house` and all you have to remember is to check the subgroup 'lake house ' under the 'at' group in *do next view* when you’re next there. Many such contexts come to mind - `at/grocery store`, `at/office`, ...
 
 One final useful context is 'waiting for'. E.g., completing a task might depend upon getting something from Joe. Add `@l waiting for/Joe` to the task and it will be listed in the subgroup 'Joe' under 'waiting for'.
 
+[↺ contents](#contents)
+
+### Goals View {#goals-view}
+
+This is a dedicated view *only for goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current week*. 
+
+This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
+
+Consider this illustrative screenshot from *Goals View*:
+
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/walk_the_dog.png" alt="new" title="goals view" width="600px" hspace="20px"/>
+
+Notice first that there is no heading displaying a date or week since *goal view* displays the status of *all* goals at the *current time*. 
+
+In this screen shot "walk the dog" is selected and its details panel is displayed. The leading "3/7+2 (4.8)" in the main window indicates that 3 instances of the goal of 7 have been completed in the current week, that 2 more completions today are needed to get back on schedule for the week and that 4.8 is the current average number of the entire history completions per week for this goal. This history is displayed in the details panel.
+
+In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
+- walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
+- wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
+- interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
+
+This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
+- F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*.
+- ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
+
+A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
+
+[↺ contents](#contents)
+
 ### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and the elapsed time and *state* of the associated timer.
 
 The sort order assures that the reminder with the active timer will always be at the top of the list and followed by the reminders with the most recently modified timers. This makes it easy to switch back and forth between recent timers.
 
 [↺ contents](#contents)
@@ -1704,14 +1737,35 @@
 - Journal entries with @s entries associate the entry with the datetime given by @s. A vacation log entry, for example, might record the highlights of the day given by @s. They are displayed in *Agenda* view as well as *Journal* view.
 - While Journal entries do not support repetition using `@r` entries, they do support the use of `@+` entries to add additional dates or datetimes to that provided by the `@s` entry.
 
 Corresponds to VJOURNAL in the vcalendar specification.
 
 [↺ contents](#contents)
 
+### goal {#goal}
+
+Type character: **~**
+
+The goal itemtype is intended to support pursuing S.M.A.R.T. goals (Specific, Measurable, Achievable, Relevant, Timed) in *etm*. Here is an example of a *goal* as it would be entered:
+
+```
+    ~ interval training @s 2024/4/22 @q 3
+```
+- It is a *goal* because of the `~` type character. 
+- Because I have a custom interval setting on my exercise bike, "interval training" is *specific* and *measurable*. It is also *achievable* and *relevant* for me.
+- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically converted to the Monday of the corresponding week.
+- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3, 5`  then the goal would have been 3 times per week repeated for 5 weeks.
+- If this goal were selected in *etm* on, say, Wednesday, April 24 and "F" were pressed, then *etm* would add an `@h 2024:17 1` (history of completions) entry to indicate 1 completion of the goal for the week of *2024:17*. Pressing "F" again in the same week with this goal selected would change this entry to `@h 2024:17 2`.  As one last example, pressing "F" with the goal selected sometime during the week of *2024:18* would leave the recorded entry as
+
+    ```
+    ~ interval training @s 2024/4/29 @q 3 @h 2024:17 2, 2024:18 1
+    ```
+
+[↺ contents](#contents)
+
 ### inbox {#inbox}
 
 Type character: **!**
 
 An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the scheduled time.
 
 Inbox items are also useful when you have an idea but not enough time to think about it. Create an inbox entry with just enough information in the summary to remind you of the idea. Make a habit at the end of the day of checking inbox items. The idea is not necessarily to complete them but to change those that can’t be finished quickly to, say, undated tasks with appropriate `@l` entries and enough detail in the summaries and the `@d` descriptions so that you will have all the information you need to act on them when the time comes.
```

### Comparing `etm-dgraham-6.2.0/bump.py` & `etm-dgraham-6.2.1/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/docs/index_konnections.md` & `etm-dgraham-6.2.1/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/docs/index_usedtime.md` & `etm-dgraham-6.2.1/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/docs/multiple_timers.md` & `etm-dgraham-6.2.1/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm/__main__.py` & `etm-dgraham-6.2.1/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm/common.py` & `etm-dgraham-6.2.1/etm/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,33 @@
  prompt_toolkit:     {prompt_toolkit_version}
  tinydb:             {tinydb_version}
  jinja2:             {jinja2_version}
  ruamel.yaml:        {ruamel_version}
  platform:           {system_platform}\
 """
 
+def check_output(cmd):
+    if not cmd:
+        return
+    res = ''
+    try:
+        res = subprocess.check_output(
+            cmd,
+            stderr=subprocess.STDOUT,
+            shell=True,
+            universal_newlines=True,
+            encoding='UTF-8',
+        )
+        return True, res
+    except subprocess.CalledProcessError as e:
+        logger.warning(f"Error running {cmd}\n'{e.output}'")
+        lines = e.output.strip().split('\n')
+        msg = lines[-1]
+        return False, msg
+
 def db_replace(new):
     """
     Used with update to replace the original doc with new.
     """
 
     def transform(doc):
         # update doc to include key/values from new
```

### Comparing `etm-dgraham-6.2.0/etm/data.py` & `etm-dgraham-6.2.1/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm/make_examples.py` & `etm-dgraham-6.2.1/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm/model.py` & `etm-dgraham-6.2.1/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     update_db,
     db_replace,
     # write_back,
     # settings,
     WA,
     timers_file,
     etmhome,
+    check_output,
 )
 
 # beginbusy = settings.beginbusy
 # usedtime_hours = settings.usedtime_hours
 
 from tinydb.table import Document 
 from etm.common import TimeIt 
@@ -7919,38 +7920,39 @@
         doc_id = item.doc_id
         flags = get_flags(
             doc_id, repeat_list, link_list, konnected, pinned_list, timers
         )
         if 'j' in item:
             task_location = item.get('l', '~')
             priority = int(item.get('p', 0))
-            sort_priority = 4 - int(priority)
+            sort_priority = str(4 - int(priority))
             show_priority = str(priority) if priority > 0 else ''
             for job in item['j']:
                 if job.get('f', None) is not None:
                     # show completed jobs only in completed view
                     continue
                 location = job.get('l', task_location)
                 extent = job.get('e', '')
                 extent = format_duration(extent) if extent else ''
-                status = 0 if job.get('status') == '-' else 1
+                status = '0' if job.get('status') == '-' else '1'
                 # status 1 -> waiting, status 0 -> available
-                rhc = ' '.join([show_priority, extent]).center(7, ' ')
+                # rhc = ' '.join([show_priority, extent])
+                rhc = extent
                 summary = job.get('summary')
                 job_id = job.get('i', None)
                 job_sort = str(job_id)
                 rows.append(
                     {
                         'id': doc_id,
                         'job': job_id,
                         'instance': None,
                         'sort': (
                             location,
-                            status,
                             sort_priority,
+                            status,
                             job_sort,
                             job.get('summary', ''),
                         ),
                         'location': location,
                         'columns': [
                             job.get('status', ''),
                             summary,
@@ -7961,17 +7963,18 @@
                     }
                 )
         else:
             location = item.get('l', '~')
             priority = int(item.get('p', 0))
             extent = item.get('e', '')
             extent = format_duration(extent) if extent else ''
-            sort_priority = 4 - int(priority)
+            sort_priority = str(4 - int(priority))
             show_priority = str(priority) if priority > 0 else ''
-            rhc = ' '.join([show_priority, extent]).center(7, ' ')
+            # rhc = ' '.join([show_priority, extent])
+            rhc = extent
             summary = item['summary']
             rows.append(
                 {
                     'id': doc_id,
                     'job': None,
                     'instance': None,
                     'sort': (location, sort_priority, extent, item['summary']),
@@ -7981,14 +7984,15 @@
                         summary,
                         flags,
                         rhc,
                         (doc_id, None, None),
                     ],
                 }
             )
+    logger.debug(f"{[x['sort'] for x in rows] = }")
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         if using_groups:
             groups = location2groups.get(row['location'], ['OTHER'])
             for group in groups:
                 path = f"{group}/{row['location']}"
@@ -9479,18 +9483,24 @@
 Documentation:  dagraham.github.io/etm-dgraham
 PyPi:           pypi.org/project/etm-dgraham
 GitHub:         github.com/dagraham/etm-dgraham
 Developer:      dnlgrhm@gmail.com
 
 {copyright}\
 """
+    which_etm = "?"
+    ok, msg = check_output('which etm')
+    if ok:
+        userhome = os.path.expanduser('~')
+        which_etm = os.path.join('~', os.path.relpath(msg, userhome))
 
     ret2 = f"""\
+ etm home:           {etmhome}
+ path to etm:        {which_etm}\
 {VERSION_INFO}
- etm directory:      {etmhome}\
 """
     return ret1, ret2
 
 
 dataview = None
 item = None
```

### Comparing `etm-dgraham-6.2.0/etm/options.py` & `etm-dgraham-6.2.1/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm/report.py` & `etm-dgraham-6.2.1/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm/view.py` & `etm-dgraham-6.2.1/etm/view.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.0
+Version: 6.2.1
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -55,14 +55,15 @@
             -   [just in time entry prompts and feedback](#just-in-time-entry-prompts-and-feedback)
             -   [fuzzy parsing of datetimes](#fuzzy-parsing-of-datetimes)
             -   [relative datetimes](#relative-datetimes)
             -   [tab completion](#tab-completion)
     -   [Views](#views)
         -   [Weekly Views](#weekly-views)
         -   [Do Next View](#do-next-view)
+        -   [Goals View](#goals-view)
         -   [Timer View](#timer-view)
         -   [Review View](#review-view)
         -   [Pinned View](#pinned-view)
         -   [Konnected View](#konnected-view)
         -   [Used Time Views](#used-time-views)
         -   [Query View](#query-view)
             -   [Simple queries](#simple-queries)
@@ -93,14 +94,15 @@
         -   [From a virtual environment](#from-a-virtual-environment)
         -   [From a system wide installation](#from-a-system-wide-installation)
 -   [Details](#details)
     -   [Item Types](#item-types)
         -   [event](#event)
         -   [task](#task)
         -   [journal](#journal)
+        -   [goal](#goal)
         -   [inbox](#inbox)
         -   [status](#status)
             -   [beginning soon](#beginning-soon)
             -   [past due](#past-due)
             -   [waiting](#waiting)
             -   [finished](#finished)
     -   [Options](#options)
@@ -524,14 +526,15 @@
 
   * a: Agenda: dated unfinished tasks and other reminders by year-week and week day
   * b: Busy: a graphical illustration of busy and conflicted times by year-week
   * c: Completed: finished tasks and jobs and used time entries by year-week and week day
   * d: Do Next: undated tasks grouped by location/context and ordered by priority (highest first) and extent (least first)
   * e: Effort: instances of reminders with used time entries with daily totals displayed graphically
   * f: Forthcoming: unfinished dated tasks and other dated reminders by next occurrence
+  * g: Goals: the status of all *goal* reminders as of the current year and week
   * h: History: all items by the latter of the modified or created datetimes in descending order, i.e., most recent first. Datetimes are displayed using a 5 character format where, e.g., 1:15pm today would be displayed as 13:15, November 7 of the current year as 11/17 and January 15 of 2012 as 12.01.
   * i: Index: all items grouped hierarchically by index entry
   * j: Journal: journal entries grouped hierarchically by index entry
   * k: Konnection: items with @k konnection links either to or from the selected item.
   * l: Location: items grouped hierarchically by location entry
   * m: Timers: items with timers.
   * p: Pinned: items whose pin status is on.
@@ -603,14 +606,44 @@
         'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
         '{', '|', '}', '~'
 
 Context is useful for more than just the sorting order. Suppose you have a task that you want to deal with the next time you’re at the lake house. Just add `@l at/lake house` and all you have to remember is to check the subgroup 'lake house ' under the 'at' group in *do next view* when you’re next there. Many such contexts come to mind - `at/grocery store`, `at/office`, ...
 
 One final useful context is 'waiting for'. E.g., completing a task might depend upon getting something from Joe. Add `@l waiting for/Joe` to the task and it will be listed in the subgroup 'Joe' under 'waiting for'.
 
+[↺ contents](#contents)
+
+### Goals View {#goals-view}
+
+This is a dedicated view *only for goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current week*. 
+
+This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
+
+Consider this illustrative screenshot from *Goals View*:
+
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/walk_the_dog.png" alt="new" title="goals view" width="600px" hspace="20px"/>
+
+Notice first that there is no heading displaying a date or week since *goal view* displays the status of *all* goals at the *current time*. 
+
+In this screen shot "walk the dog" is selected and its details panel is displayed. The leading "3/7+2 (4.8)" in the main window indicates that 3 instances of the goal of 7 have been completed in the current week, that 2 more completions today are needed to get back on schedule for the week and that 4.8 is the current average number of the entire history completions per week for this goal. This history is displayed in the details panel.
+
+In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
+- walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
+- wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
+- interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
+
+This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
+- F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*.
+- ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
+
+A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
+
+[↺ contents](#contents)
+
 ### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and the elapsed time and *state* of the associated timer.
 
 The sort order assures that the reminder with the active timer will always be at the top of the list and followed by the reminders with the most recently modified timers. This makes it easy to switch back and forth between recent timers.
 
 [↺ contents](#contents)
@@ -1747,14 +1780,35 @@
 - Journal entries with @s entries associate the entry with the datetime given by @s. A vacation log entry, for example, might record the highlights of the day given by @s. They are displayed in *Agenda* view as well as *Journal* view.
 - While Journal entries do not support repetition using `@r` entries, they do support the use of `@+` entries to add additional dates or datetimes to that provided by the `@s` entry.
 
 Corresponds to VJOURNAL in the vcalendar specification.
 
 [↺ contents](#contents)
 
+### goal {#goal}
+
+Type character: **~**
+
+The goal itemtype is intended to support pursuing S.M.A.R.T. goals (Specific, Measurable, Achievable, Relevant, Timed) in *etm*. Here is an example of a *goal* as it would be entered:
+
+```
+    ~ interval training @s 2024/4/22 @q 3
+```
+- It is a *goal* because of the `~` type character. 
+- Because I have a custom interval setting on my exercise bike, "interval training" is *specific* and *measurable*. It is also *achievable* and *relevant* for me.
+- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically converted to the Monday of the corresponding week.
+- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3, 5`  then the goal would have been 3 times per week repeated for 5 weeks.
+- If this goal were selected in *etm* on, say, Wednesday, April 24 and "F" were pressed, then *etm* would add an `@h 2024:17 1` (history of completions) entry to indicate 1 completion of the goal for the week of *2024:17*. Pressing "F" again in the same week with this goal selected would change this entry to `@h 2024:17 2`.  As one last example, pressing "F" with the goal selected sometime during the week of *2024:18* would leave the recorded entry as
+
+    ```
+    ~ interval training @s 2024/4/29 @q 3 @h 2024:17 2, 2024:18 1
+    ```
+
+[↺ contents](#contents)
+
 ### inbox {#inbox}
 
 Type character: **!**
 
 An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the scheduled time.
 
 Inbox items are also useful when you have an idea but not enough time to think about it. Create an inbox entry with just enough information in the summary to remind you of the idea. Make a habit at the end of the day of checking inbox items. The idea is not necessarily to complete them but to change those that can’t be finished quickly to, say, undated tasks with appropriate `@l` entries and enough detail in the summaries and the `@d` descriptions so that you will have all the information you need to act on them when the time comes.
```

### Comparing `etm-dgraham-6.2.0/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.2.1/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etmlogo.png` & `etm-dgraham-6.2.1/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etmlogo_small.png` & `etm-dgraham-6.2.1/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/etmview_agenda.png` & `etm-dgraham-6.2.1/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/namedcolors.py` & `etm-dgraham-6.2.1/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/new.png` & `etm-dgraham-6.2.1/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/setup.py` & `etm-dgraham-6.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/test/test_parser.py` & `etm-dgraham-6.2.1/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/utilities/colons_to_slashes.py` & `etm-dgraham-6.2.1/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/utilities/etm_in` & `etm-dgraham-6.2.1/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/utilities/inbasket` & `etm-dgraham-6.2.1/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.0/utilities/open_in_mutt` & `etm-dgraham-6.2.1/utilities/open_in_mutt`

 * *Files identical despite different names*

