# Comparing `tmp/etm-dgraham-6.2.1.tar.gz` & `tmp/etm-dgraham-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.2.1.tar", last modified: Mon May  6 10:36:54 2024, max compression
+gzip compressed data, was "etm-dgraham-6.2.2.tar", last modified: Mon May  6 14:20:42 2024, max compression
```

## Comparing `etm-dgraham-6.2.1.tar` & `etm-dgraham-6.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.397990 etm-dgraham-6.2.1/
--rw-r--r--   0 dag        (501) staff       (20)     6418 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   145616 2024-05-06 10:36:54.397757 etm-dgraham-6.2.1/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   144047 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.1/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.1/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.390507 etm-dgraham-6.2.1/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.393399 etm-dgraham-6.2.1/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-05 16:45:06.000000 etm-dgraham-6.2.1/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.1/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.1/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   329909 2024-05-06 10:36:50.000000 etm-dgraham-6.2.1/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38891 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126266 2024-05-04 14:12:33.000000 etm-dgraham-6.2.1/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.395795 etm-dgraham-6.2.1/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   145616 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-06 10:36:54.000000 etm-dgraham-6.2.1/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.1/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.1/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.1/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-06 10:36:54.398036 etm-dgraham-6.2.1/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.1/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.395910 etm-dgraham-6.2.1/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.1/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 10:36:54.397211 etm-dgraham-6.2.1/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.1/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.1/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.1/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.1/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 14:20:42.865033 etm-dgraham-6.2.2/
+-rw-r--r--   0 dag        (501) staff       (20)     6003 2024-05-06 14:20:40.000000 etm-dgraham-6.2.2/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.2/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   145677 2024-05-06 14:20:42.864777 etm-dgraham-6.2.2/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   144108 2024-05-06 14:19:59.000000 etm-dgraham-6.2.2/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.2/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.2/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 14:20:42.854755 etm-dgraham-6.2.2/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.2/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.2/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.2/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 14:20:42.860028 etm-dgraham-6.2.2/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.2/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.2/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-06 14:20:40.000000 etm-dgraham-6.2.2/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-05 16:45:06.000000 etm-dgraham-6.2.2/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.2/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.2/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   330976 2024-05-06 14:19:59.000000 etm-dgraham-6.2.2/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.2/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.2/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126266 2024-05-04 14:12:33.000000 etm-dgraham-6.2.2/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 14:20:42.862580 etm-dgraham-6.2.2/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   145677 2024-05-06 14:20:42.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-06 14:20:42.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-06 14:20:42.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-06 14:20:42.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-06 14:20:42.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-06 14:20:42.000000 etm-dgraham-6.2.2/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.2/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.2/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.2/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.2/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.2.2/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.2/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-06 14:20:42.865074 etm-dgraham-6.2.2/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.2/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 14:20:42.862702 etm-dgraham-6.2.2/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.2/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-06 14:20:42.864189 etm-dgraham-6.2.2/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.2/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.2/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.2/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.2/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.2.1/CHANGES.txt` & `etm-dgraham-6.2.2/CHANGES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-2024-05-06 9c3ccea Daniel Graham
+2024-05-06 002cbec Daniel Graham
+    Tagged version 6.2.2.
+
+2024-05-06 e802430 Daniel Graham
+    Added goals.txt to the output associated with keep_current
+
+2024-05-06 c3d0360 Daniel Graham
+    Show average as 0 instead of 0.0 in goals view
+
+2024-05-06 4caaed7 Daniel Graham
     Tagged version 6.2.1.
 
 2024-05-06 272ef22 Daniel Graham
     Fixed sorting bug in do next view
 
 2024-05-05 bd65af8 Daniel Graham
     README tweaks
@@ -192,22 +201,7 @@
 
 2024-03-05 95e00a7 Daniel Graham
     Treat allday tasks as due at midnight and thus finished ahead of
     time if finished anytime during the due date.
 
 2024-03-04 3e1bb78 Daniel Graham
     Tagged version 6.1.16.
-
-2024-03-04 34a9181 Daniel Graham
-    Fixed bug in processing job summaries for tasks.
-
-2024-03-03 3cfa34e Daniel Graham
-    Tagged version 6.1.15.
-
-2024-03-03 c3d4615 Daniel Graham
-    Refactored timer_report and show_timers into get_timers. Added
-    round_to_minutes to ensure that the total reported in timer view
-    is consistent with the items listed. In reporting the moment a
-    timer status last changed use the datetime if the change occurred
-    on the current date and the timedelta between the current moment
-    and the datetime otherwise. Added 'inactive' to type_colors.
-    Changed default 'light' type_colors for 'paused' and 'running'.
```

### Comparing `etm-dgraham-6.2.1/PKG-INFO` & `etm-dgraham-6.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.1
+Version: 6.2.2
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -1239,19 +1239,17 @@
 
 [↺ contents](#contents)
 
 ## Mobile access to your reminders {#mobile}
 
 The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
 
-* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary. A width of 46, for example, works well for an iPhone in portrait mode.
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will written to `current.txt` and updated whenever necessary. Similarly, the 'do next' view will be written to "next.txt" and 'goals' view will be written to "goals.txt". In all cases, the output will be wrapped to fit `width`. A width of 46, for example, works well for an iPhone in portrait mode.
 
-* `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
-
-By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
+By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule, tasks and goals on your mobile device.
 
 Here is a screen shot from an iPhone of an illustrative `current.txt`:
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/current_on_iphone.png" alt="new" title="current view" width="300px" hspace="20px"/>
 
 
 [↺ contents](#contents)
@@ -1274,14 +1272,15 @@
     view
         a) agenda
         b) busy
         c) completed
         d) do next
         e) effort
         f) forthcoming
+        g) goals
         h) history
         i) index
         j) journal
         k) konnected
         l) location
         m) timers
         o) occurrences
@@ -1319,15 +1318,17 @@
         E) edit
         C) edit copy
         D) delete
         F) finish
         P) toggle pin
         R) reschedule
         S) schedule new
-        g) open goto link
+        G) open goto link
+        ^a) toggle goal active/inactive
+        ^e) end goal 
         ^h) show completion history
         ^r) show repetitions
         ^u) update last modified
         ^x) toggle archived status
         --- konnected view
         k) toggle showing konnections
     timers
```

### Comparing `etm-dgraham-6.2.1/README.md` & `etm-dgraham-6.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1196,19 +1196,17 @@
 
 [↺ contents](#contents)
 
 ## Mobile access to your reminders {#mobile}
 
 The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
 
-* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary. A width of 46, for example, works well for an iPhone in portrait mode.
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will written to `current.txt` and updated whenever necessary. Similarly, the 'do next' view will be written to "next.txt" and 'goals' view will be written to "goals.txt". In all cases, the output will be wrapped to fit `width`. A width of 46, for example, works well for an iPhone in portrait mode.
 
-* `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
-
-By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
+By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule, tasks and goals on your mobile device.
 
 Here is a screen shot from an iPhone of an illustrative `current.txt`:
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/current_on_iphone.png" alt="new" title="current view" width="300px" hspace="20px"/>
 
 
 [↺ contents](#contents)
@@ -1231,14 +1229,15 @@
     view
         a) agenda
         b) busy
         c) completed
         d) do next
         e) effort
         f) forthcoming
+        g) goals
         h) history
         i) index
         j) journal
         k) konnected
         l) location
         m) timers
         o) occurrences
@@ -1276,15 +1275,17 @@
         E) edit
         C) edit copy
         D) delete
         F) finish
         P) toggle pin
         R) reschedule
         S) schedule new
-        g) open goto link
+        G) open goto link
+        ^a) toggle goal active/inactive
+        ^e) end goal 
         ^h) show completion history
         ^r) show repetitions
         ^u) update last modified
         ^x) toggle archived status
         --- konnected view
         k) toggle showing konnections
     timers
```

### Comparing `etm-dgraham-6.2.1/bump.py` & `etm-dgraham-6.2.2/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/docs/index_konnections.md` & `etm-dgraham-6.2.2/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/docs/index_usedtime.md` & `etm-dgraham-6.2.2/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/docs/multiple_timers.md` & `etm-dgraham-6.2.2/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm/__main__.py` & `etm-dgraham-6.2.2/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm/common.py` & `etm-dgraham-6.2.2/etm/common.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm/data.py` & `etm-dgraham-6.2.2/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm/make_examples.py` & `etm-dgraham-6.2.2/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm/model.py` & `etm-dgraham-6.2.2/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3054,21 +3054,24 @@
         if (
             'keep_current' in self.settings
             and self.settings['keep_current'][0]
         ):
             # weeks is not zero
             self.mk_current = True
             self.mk_next = True
+            self.mk_goals = True
             self.currfile = os.path.normpath(
                 os.path.join(etmdir, 'current.txt')
             )
             self.nextfile = os.path.normpath(os.path.join(etmdir, 'next.txt'))
+            self.goalsfile = os.path.normpath(os.path.join(etmdir, 'goals.txt'))
         else:
             self.mk_current = False
             self.mk_next = False
+            self.mk_goals = False
             self.currfile = None
             self.nextfile = None
 
         if 'locale' in self.settings:
             locale_str = settings['locale']
             # locale_str should have the format "en_US"
             if locale_str:
@@ -3960,14 +3963,29 @@
             )
             next_view = current_hsh['next'] if 'next' in current_hsh else None
             if next_txt:
                 with open(self.nextfile, 'w', encoding='utf-8') as fo:
                     fo.write(re.sub(EtmChar.LINEDOT, '   ', next_txt))
                 logger.info(f'saved do next to {self.nextfile}')
 
+        if self.mk_goals:
+            goals_view, row2id, goals_txt = show_goals(
+                self.db,
+                self.repeat_list,
+                self.pinned_list,
+                self.link_list,
+                self.konnected,
+                self.timers,
+            )
+            goals_view = current_hsh['goals'] if 'goals' in current_hsh else None
+            if goals_txt:
+                with open(self.goalsfile, 'w', encoding='utf-8') as fo:
+                    fo.write(re.sub(EtmChar.LINEDOT, '   ', goals_txt))
+                logger.info(f'saved goals to {self.goalsfile}')
+
     def show_query(self):
         self.is_showing_query = True
 
     def hide_query(self):
         self.is_showing_query = False
 
 
@@ -7921,25 +7939,24 @@
         flags = get_flags(
             doc_id, repeat_list, link_list, konnected, pinned_list, timers
         )
         if 'j' in item:
             task_location = item.get('l', '~')
             priority = int(item.get('p', 0))
             sort_priority = str(4 - int(priority))
-            show_priority = str(priority) if priority > 0 else ''
+            # show_priority = str(priority) if priority > 0 else ''
             for job in item['j']:
                 if job.get('f', None) is not None:
                     # show completed jobs only in completed view
                     continue
                 location = job.get('l', task_location)
                 extent = job.get('e', '')
                 extent = format_duration(extent) if extent else ''
-                status = '0' if job.get('status') == '-' else '1'
                 # status 1 -> waiting, status 0 -> available
-                # rhc = ' '.join([show_priority, extent])
+                status = '0' if job.get('status') == '-' else '1'
                 rhc = extent
                 summary = job.get('summary')
                 job_id = job.get('i', None)
                 job_sort = str(job_id)
                 rows.append(
                     {
                         'id': doc_id,
@@ -7964,16 +7981,15 @@
                 )
         else:
             location = item.get('l', '~')
             priority = int(item.get('p', 0))
             extent = item.get('e', '')
             extent = format_duration(extent) if extent else ''
             sort_priority = str(4 - int(priority))
-            show_priority = str(priority) if priority > 0 else ''
-            # rhc = ' '.join([show_priority, extent])
+            # show_priority = str(priority) if priority > 0 else ''
             rhc = extent
             summary = item['summary']
             rows.append(
                 {
                     'id': doc_id,
                     'job': None,
                     'instance': None,
@@ -7984,15 +8000,15 @@
                         summary,
                         flags,
                         rhc,
                         (doc_id, None, None),
                     ],
                 }
             )
-    logger.debug(f"{[x['sort'] for x in rows] = }")
+    # logger.debug(f"{[x['sort'] for x in rows] = }")
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         if using_groups:
             groups = location2groups.get(row['location'], ['OTHER'])
             for group in groups:
                 path = f"{group}/{row['location']}"
@@ -8015,15 +8031,15 @@
                     path = f"{group}/{row['location']}"
                     values = row['columns']
                     cdict.add(path, values)
             else:
                 path = row['location']
                 values = row['columns']
                 cdict.add(path, values)
-        ctree, crow2id = cdict.as_tree(cdict)
+        ctree, _ = cdict.as_tree(cdict)
         current_hsh['next'] = ctree
 
     return tree, row2id, ctree
 
 
 def show_journal(
     db,
@@ -8103,14 +8119,17 @@
     link_list=[],
     konnected=[],
     timers={},
 ):
     """
     goals grouped by current, paused, ended
     """
+    global current_hsh
+    mk_goals = settings['keep_current'][0] > 0
+    goals_width = settings['keep_current'][1] - 1
     rows = []
     path2sort = {
         'Active': 1,
         'Inactive': 2,
         'Ended': 3,
     }
     # goal_hsh = {} 
@@ -8127,15 +8146,15 @@
         summary = item.get('summary').strip()
         s = item.get('s', None)
         q = item.get('q', [])
         h = item.get('h', {})
         for k, v in h.items():
             count += 1
             total += int(v)
-        average = f"{total/count:.2}" if count else 0
+        average = f"{total/count:.2}" if count and total else 0
         logger.debug(f"{summary = }; {total = }; {count = }; {average = }")
         path = None
         # status: current, paused, ended, bad
         
         quota = q[0] if len(q) > 0 else None
         if not s or q is None:
             logger.error(f"bad goal: {item = }")
@@ -8197,15 +8216,26 @@
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict)
-    return tree, row2id
+
+    ctree = None
+    if mk_goals:
+        cdict = NDict(compact=True, width=goals_width)
+        for row in rows:
+            path = row['path']
+            values = row['values']
+            cdict.add(path, values)
+        ctree, _ = cdict.as_tree(cdict)
+        current_hsh['goals'] = ctree
+
+    return tree, row2id, ctree
 
 
 def show_tags(
     db,
     id2relevant,
     repeat_list=[],
     pinned_list=[],
```

### Comparing `etm-dgraham-6.2.1/etm/options.py` & `etm-dgraham-6.2.2/etm/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,21 +384,21 @@
 # list will only have their starting times displayed in agenda view
 # and will neither appear nor cause conflicts in busy view.
 
 keep_current: {keep_current}
 # A list of two, non-negative integers for "weeks" and "width". If
 # weeks is positive, the agenda for that integer number of weeks
 # starting with the current week will be written to "current.txt" in
-# your etm home directory and updated when necessary. Similarly, the
-# 'do next' view will be written to "next.txt". In both cases, the
-# format will be scaled to fit "width". A width of 46, e.g, fits an
-# iPhone display in portrait mode. You could, for example, create a
-# link to these files in a pCloud or GoogleDrive folder and always
-# have access to your agenda and do next on your mobile device.
-
+# your etm home directory and updated when necessary. Similarly, 'do
+# next' view will be written to "next.txt" and 'goals' view to
+# "goals.txt". In all cases, the output will be scaled to fit "width".
+# A width of 46, e.g, fits an iPhone display in portrait mode. You
+# could, for example, create a link to these files in a pCloud or
+# GoogleDrive folder and always have access to your agenda, tasks and
+# goals on your mobile device.
 
 archive_after: {archive_after}
 # non-negative integer. If zero, do not archive items. If positive,
 # finished tasks and events with last datetimes falling more than this
 # number of years before the current date will automatically be
 # archived on a daily basis.  Archived items are moved from the
 # "items" table in the database to the "archive" table and will no
```

### Comparing `etm-dgraham-6.2.1/etm/report.py` & `etm-dgraham-6.2.2/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm/view.py` & `etm-dgraham-6.2.2/etm/view.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.2.2/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.1
+Version: 6.2.2
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -1239,19 +1239,17 @@
 
 [↺ contents](#contents)
 
 ## Mobile access to your reminders {#mobile}
 
 The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
 
-* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary. A width of 46, for example, works well for an iPhone in portrait mode.
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will written to `current.txt` and updated whenever necessary. Similarly, the 'do next' view will be written to "next.txt" and 'goals' view will be written to "goals.txt". In all cases, the output will be wrapped to fit `width`. A width of 46, for example, works well for an iPhone in portrait mode.
 
-* `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
-
-By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
+By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule, tasks and goals on your mobile device.
 
 Here is a screen shot from an iPhone of an illustrative `current.txt`:
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/current_on_iphone.png" alt="new" title="current view" width="300px" hspace="20px"/>
 
 
 [↺ contents](#contents)
@@ -1274,14 +1272,15 @@
     view
         a) agenda
         b) busy
         c) completed
         d) do next
         e) effort
         f) forthcoming
+        g) goals
         h) history
         i) index
         j) journal
         k) konnected
         l) location
         m) timers
         o) occurrences
@@ -1319,15 +1318,17 @@
         E) edit
         C) edit copy
         D) delete
         F) finish
         P) toggle pin
         R) reschedule
         S) schedule new
-        g) open goto link
+        G) open goto link
+        ^a) toggle goal active/inactive
+        ^e) end goal 
         ^h) show completion history
         ^r) show repetitions
         ^u) update last modified
         ^x) toggle archived status
         --- konnected view
         k) toggle showing konnections
     timers
```

### Comparing `etm-dgraham-6.2.1/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.2.2/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.2.2/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etmlogo.png` & `etm-dgraham-6.2.2/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etmlogo_small.png` & `etm-dgraham-6.2.2/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/etmview_agenda.png` & `etm-dgraham-6.2.2/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/namedcolors.py` & `etm-dgraham-6.2.2/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/new.png` & `etm-dgraham-6.2.2/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/setup.py` & `etm-dgraham-6.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/test/test_parser.py` & `etm-dgraham-6.2.2/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/utilities/colons_to_slashes.py` & `etm-dgraham-6.2.2/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/utilities/etm_in` & `etm-dgraham-6.2.2/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/utilities/inbasket` & `etm-dgraham-6.2.2/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.1/utilities/open_in_mutt` & `etm-dgraham-6.2.2/utilities/open_in_mutt`

 * *Files identical despite different names*

