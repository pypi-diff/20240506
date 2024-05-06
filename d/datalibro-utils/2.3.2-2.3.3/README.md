# Comparing `tmp/datalibro_utils-2.3.2.tar.gz` & `tmp/datalibro_utils-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_utils-2.3.2.tar", last modified: Fri Apr 26 10:19:15 2024, max compression
+gzip compressed data, was "datalibro_utils-2.3.3.tar", last modified: Mon May  6 05:57:36 2024, max compression
```

## Comparing `datalibro_utils-2.3.2.tar` & `datalibro_utils-2.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 10:19:15.424294 datalibro_utils-2.3.2/
--rw-rw-rw-   0        0        0      301 2024-04-26 10:19:15.424294 datalibro_utils-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1145 2023-11-01 08:51:17.000000 datalibro_utils-2.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 10:19:15.418261 datalibro_utils-2.3.2/datalibro_utils/
--rw-rw-rw-   0        0        0      180 2023-12-08 10:02:45.000000 datalibro_utils-2.3.2/datalibro_utils/__init__.py
--rw-rw-rw-   0        0        0     7743 2023-11-01 08:48:50.000000 datalibro_utils-2.3.2/datalibro_utils/datalibro_auth.py
--rw-rw-rw-   0        0        0     6590 2024-04-26 10:08:14.000000 datalibro_utils-2.3.2/datalibro_utils/dlbi.py
--rw-rw-rw-   0        0        0     1404 2023-11-01 08:51:17.000000 datalibro_utils-2.3.2/datalibro_utils/email.py
--rw-rw-rw-   0        0        0    13183 2024-04-07 05:56:09.000000 datalibro_utils-2.3.2/datalibro_utils/mapping.py
--rw-rw-rw-   0        0        0      866 2023-11-06 04:16:52.000000 datalibro_utils-2.3.2/datalibro_utils/openai.py
--rw-rw-rw-   0        0        0     2316 2023-10-27 10:47:34.000000 datalibro_utils-2.3.2/datalibro_utils/pet_sys.py
--rw-rw-rw-   0        0        0       80 2023-06-28 06:14:01.000000 datalibro_utils-2.3.2/datalibro_utils/test.py
-drwxrwxrwx   0        0        0        0 2024-04-26 10:19:15.422908 datalibro_utils-2.3.2/datalibro_utils.egg-info/
--rw-rw-rw-   0        0        0      301 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-26 10:19:15.000000 datalibro_utils-2.3.2/datalibro_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 10:19:15.424800 datalibro_utils-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0      399 2024-04-26 10:19:06.000000 datalibro_utils-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 05:57:36.881088 datalibro_utils-2.3.3/
+-rw-rw-rw-   0        0        0      301 2024-05-06 05:57:36.881088 datalibro_utils-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2023-11-01 08:51:17.000000 datalibro_utils-2.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 05:57:36.874733 datalibro_utils-2.3.3/datalibro_utils/
+-rw-rw-rw-   0        0        0      180 2023-12-08 10:02:45.000000 datalibro_utils-2.3.3/datalibro_utils/__init__.py
+-rw-rw-rw-   0        0        0     7743 2023-11-01 08:48:50.000000 datalibro_utils-2.3.3/datalibro_utils/datalibro_auth.py
+-rw-rw-rw-   0        0        0     6708 2024-05-06 05:54:47.000000 datalibro_utils-2.3.3/datalibro_utils/dlbi.py
+-rw-rw-rw-   0        0        0     1404 2023-11-01 08:51:17.000000 datalibro_utils-2.3.3/datalibro_utils/email.py
+-rw-rw-rw-   0        0        0    13183 2024-04-07 05:56:09.000000 datalibro_utils-2.3.3/datalibro_utils/mapping.py
+-rw-rw-rw-   0        0        0      866 2023-11-06 04:16:52.000000 datalibro_utils-2.3.3/datalibro_utils/openai.py
+-rw-rw-rw-   0        0        0     2316 2023-10-27 10:47:34.000000 datalibro_utils-2.3.3/datalibro_utils/pet_sys.py
+-rw-rw-rw-   0        0        0       80 2023-06-28 06:14:01.000000 datalibro_utils-2.3.3/datalibro_utils/test.py
+drwxrwxrwx   0        0        0        0 2024-05-06 05:57:36.880090 datalibro_utils-2.3.3/datalibro_utils.egg-info/
+-rw-rw-rw-   0        0        0      301 2024-05-06 05:57:36.000000 datalibro_utils-2.3.3/datalibro_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-05-06 05:57:36.000000 datalibro_utils-2.3.3/datalibro_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 05:57:36.000000 datalibro_utils-2.3.3/datalibro_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-06 05:57:36.000000 datalibro_utils-2.3.3/datalibro_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 05:57:36.000000 datalibro_utils-2.3.3/datalibro_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 05:57:36.882193 datalibro_utils-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-05-06 05:57:23.000000 datalibro_utils-2.3.3/setup.py
```

### Comparing `datalibro_utils-2.3.2/README.md` & `datalibro_utils-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.2/datalibro_utils/datalibro_auth.py` & `datalibro_utils-2.3.3/datalibro_utils/datalibro_auth.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.2/datalibro_utils/dlbi.py` & `datalibro_utils-2.3.3/datalibro_utils/dlbi.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
             label_visibility="hidden",
             key=col_name
         )
     if "(ALL)" in selection:
         selection = unique_values
     return selection
 
-def time_range_filter(s_date, relative_date=date.today() + relativedelta(months=-1)):
+def time_range_filter(s_date, relative_date=None):
+    if relative_date is None:
+        relative_date = date.today() + relativedelta(months=-1)
     date_range = st.date_input('**Date Range**', (relative_date, date.today()))
     st.caption(f"*Date range from {min(s_date)} to {max(s_date)}")
     return date_range
 
 def cols_filter(df, filter_cols):
     return {col: add_multiselect(col, df) for col in filter_cols}
 
@@ -90,15 +92,17 @@
     list_ani_val = [int(value/10), int(value/4), int(value/3*2)]
     with st.empty():
         for val in list_ani_val:
             st.metric(':rainbow['+label+']', f'{val:,}')
             time.sleep(0.08)
         st.metric(label, f'{value:,}')
 
-def side_control(df, date_col, view_size_cols, relative_date=date.today() + relativedelta(months=-1), start_time_size=0, multi_pages=None):
+def side_control(df, date_col, view_size_cols, relative_date=None, start_time_size=0, multi_pages=None):
+    if relative_date is None:
+        relative_date = date.today() + relativedelta(months=-1)
     with st.sidebar:
         data_labels = get_data_labels()
         page_selection = None
         if multi_pages:
             page_selection = st.radio(
                 "**Page**",
                 multi_pages
```

### Comparing `datalibro_utils-2.3.2/datalibro_utils/email.py` & `datalibro_utils-2.3.3/datalibro_utils/email.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.2/datalibro_utils/mapping.py` & `datalibro_utils-2.3.3/datalibro_utils/mapping.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.2/datalibro_utils/openai.py` & `datalibro_utils-2.3.3/datalibro_utils/openai.py`

 * *Files identical despite different names*

### Comparing `datalibro_utils-2.3.2/datalibro_utils/pet_sys.py` & `datalibro_utils-2.3.3/datalibro_utils/pet_sys.py`

 * *Files identical despite different names*

