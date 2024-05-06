# Comparing `tmp/ipyslides-3.7.6.tar.gz` & `tmp/ipyslides-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.7.6.tar", last modified: Sat May  4 02:36:45 2024, max compression
+gzip compressed data, was "ipyslides-3.8.0.tar", last modified: Mon May  6 20:08:00 2024, max compression
```

## Comparing `ipyslides-3.7.6.tar` & `ipyslides-3.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 02:36:45.641422 ipyslides-3.7.6/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.7.6/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-04 02:36:45.641422 ipyslides-3.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 02:36:45.602952 ipyslides-3.7.6/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.7.6/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-04 02:36:08.000000 ipyslides-3.7.6/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 02:36:45.641422 ipyslides-3.7.6/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.7.6/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    41331 2024-05-04 02:34:37.000000 ipyslides-3.7.6/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.7.6/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    32956 2024-05-02 18:42:52.000000 ipyslides-3.7.6/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.7.6/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.7.6/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-03 23:26:00.000000 ipyslides-3.7.6/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.7.6/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-04 02:36:45.641422 ipyslides-3.7.6/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.7.6/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.7.6/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.7.6/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.7.6/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.7.6/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    21960 2024-05-04 00:50:24.000000 ipyslides-3.7.6/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28848 2024-05-02 18:42:52.000000 ipyslides-3.7.6/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28254 2024-03-06 23:50:13.000000 ipyslides-3.7.6/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15593 2024-05-03 23:26:48.000000 ipyslides-3.7.6/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.7.6/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    49231 2024-05-04 02:08:48.000000 ipyslides-3.7.6/ipyslides/core.py
--rw-rw-rw-   0        0        0    17494 2024-02-24 17:41:41.000000 ipyslides-3.7.6/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.7.6/ipyslides/source.py
--rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.7.6/ipyslides/utils.py
--rw-rw-rw-   0        0        0    13884 2024-03-09 15:23:53.000000 ipyslides-3.7.6/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.7.6/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-04 02:36:45.625259 ipyslides-3.7.6/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-04 02:36:45.000000 ipyslides-3.7.6/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-04 02:36:45.000000 ipyslides-3.7.6/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 02:36:45.000000 ipyslides-3.7.6/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-04 02:36:45.000000 ipyslides-3.7.6/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 02:36:45.000000 ipyslides-3.7.6/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 02:36:45.641422 ipyslides-3.7.6/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.052967 ipyslides-3.8.0/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.0/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-06 20:08:00.052967 ipyslides-3.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.018868 ipyslides-3.8.0/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.0/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-06 20:00:02.000000 ipyslides-3.8.0/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.052967 ipyslides-3.8.0/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.0/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41405 2024-05-06 16:18:36.000000 ipyslides-3.8.0/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.8.0/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33097 2024-05-06 19:59:42.000000 ipyslides-3.8.0/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.8.0/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.8.0/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-03 23:26:00.000000 ipyslides-3.8.0/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.8.0/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.052967 ipyslides-3.8.0/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.8.0/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.0/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.0/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.0/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.0/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    21960 2024-05-04 00:50:24.000000 ipyslides-3.8.0/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28848 2024-05-02 18:42:52.000000 ipyslides-3.8.0/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28513 2024-05-06 19:55:40.000000 ipyslides-3.8.0/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15593 2024-05-06 16:29:40.000000 ipyslides-3.8.0/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.0/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    49425 2024-05-06 16:22:38.000000 ipyslides-3.8.0/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18477 2024-05-06 18:06:44.000000 ipyslides-3.8.0/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.0/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.8.0/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.0/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.0/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.034422 ipyslides-3.8.0/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 20:08:00.052967 ipyslides-3.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.0/setup.py
```

### Comparing `ipyslides-3.7.6/LICENSE` & `ipyslides-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/PKG-INFO` & `ipyslides-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.7.6
+Version: 3.8.0
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.7.6/README.md` & `ipyslides-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/_layout_css.py` & `ipyslides-3.8.0/ipyslides/_base/_layout_css.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,14 +682,15 @@
                 ).css,
             },
             "<.Scroll-Btn": { # top level
                 "color": "var(--jp-brand-color1,skyblue) !important",
                 "background": "transparent !important",
                 "font-size": "0.8em !important",
                 "opacity": "0 !important",
+                "height": "auto !important", # for show when slide shown
                 "transition": "all 400ms ease-in-out !important",
                 "^:hover": {"font-weight": "bold !important","font-size": "0.9em !important",},
                 "^:hover, ^:focus, ^:active, ^.mod-active" : {
                     "box-shadow": "none !important",
                     "opacity": "1 !important",
                     "outline": "none !important",
                 },
```

### Comparing `ipyslides-3.7.6/ipyslides/_base/_widgets.py` & `ipyslides-3.8.0/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/base.py` & `ipyslides-3.8.0/ipyslides/_base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,17 @@
         @slides.on_refresh
         def update_time():
             print('Local Time: {3}:{4}:{5}'.format(*time.localtime())) # Print time in HH:MM:SS format
         # Updates on update_display or refresh button click
         ```
         ::: note-warning
             Do not use this to change global state of slides, because that will affect all slides.
+        
+        ::: note-info
+            Use `ipywidgets.interact/interactive` if you need extra control widgets beyond just a refresh.
         """
         return self._dynamic_private(func, tag = '_has_widgets', hide_refresher = False)
     
     def _dynamic_private(self, func, tag = None, hide_refresher = False):
         "Not for user use, internal function for other dynamic content decorators with their own tags."
         self.verify_running('Dynamic content can only be used inside slide constructor!')
         return self.running._dynamic_private(func, tag = tag, hide_refresher = hide_refresher)
```

### Comparing `ipyslides-3.7.6/ipyslides/_base/export_html.py` & `ipyslides-3.8.0/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/export_template.py` & `ipyslides-3.8.0/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/icons.py` & `ipyslides-3.8.0/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/intro.py` & `ipyslides-3.8.0/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/js/interaction.js` & `ipyslides-3.8.0/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/js/notes.js` & `ipyslides-3.8.0/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/navigation.py` & `ipyslides-3.8.0/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/notes.py` & `ipyslides-3.8.0/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/screenshot.py` & `ipyslides-3.8.0/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/settings.py` & `ipyslides-3.8.0/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/slide.py` & `ipyslides-3.8.0/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_base/styles.py` & `ipyslides-3.8.0/ipyslides/_base/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,15 +343,14 @@
                 }, 
                 '^.next': {'opacity':'0.5',},
             },
             '.FirstTOC .toc-item.next' : {'opacity':'1',}, # In start, see full as same opacity
             'ul li::marker, ol li::marker': {'color':'var(--accent-color)',},
             '.raw-text': { # Should follow theme under slides 
                 'font-family': f'{code_font!r}, "Cascadia Code","Ubuntu Mono", "SimSun-ExtB", "Courier New" !important', # Should be same in notebook cell
-                'background':'var(--secondary-bg) !important',
                 'color':'var(--primary-fg) !important',
                 'max-height':'400px',
                 'white-space':'pre !important',
             },
             '.text-box': { # general text box for writing inline refrences etc. 
                 'font-size':'0.85em !important', 
                 'line-height':'0.99em !important',
@@ -472,14 +471,22 @@
                 },
                 '^.code-no-focus': {'opacity':'0.3 !important'},
                 '^.code-focus':{'text-shadow':'0 0 1px var(--primary-bg)'},
             },
             '^::-webkit-scrollbar': {'background':'var(--secondary-bg) !important',},
             '^::-webkit-scrollbar-corner': {'display': 'none',},
         },
+        '.highlight, pre, .raw-text': {
+            '^:hover::-webkit-scrollbar': {
+                    'background':'var(--secondary-bg) !important'
+                },
+                '^:hover::-webkit-scrollbar-thumb': {
+                    'background':'var(--hover-bg) !important'
+                },
+        },
         'span.lang-name': {
             'color':'var(--accent-color)',
             'font-size':'0.8em',
         },
         '.docs': { # docs have Python code only, so no need to have fancy things there
             'margin-bottom':'1em !important',
             '.highlight': {'border':'none !important',},
```

### Comparing `ipyslides-3.7.6/ipyslides/_base/widgets.py` & `ipyslides-3.8.0/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/_demo.py` & `ipyslides-3.8.0/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/core.py` & `ipyslides-3.8.0/ipyslides/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys, os, json, re, textwrap, math
 from contextlib import contextmanager, suppress
 from collections import namedtuple
 
 from IPython import get_ipython
-from IPython.display import display
+from IPython.display import display, clear_output
 
 
 from .xmd import fmt, parse, capture_content, xtr, extender as _extender
 from .source import Code
 from .writer import GotoButton, write
 from .formatters import XTML, HtmlWidget, bokeh2html, plt2html, highlight, htmlize, serializer
 from . import utils
@@ -166,15 +166,15 @@
         return output
     
     def _post_run_cell(self, result):
         self._unregister_postrun_cell() # it will be initialized from next building slides
         if result.error_before_exec or result.error_in_exec:
             return  # Do not display if there is an error
 
-        scroll_btn = ipw.Button(description= 'Go to Slides', icon= 'scroll').add_class('Scroll-Btn')
+        scroll_btn = ipw.Button(description= 'Go to Slides', icon= 'scroll', layout={'height':'0px'}).add_class('Scroll-Btn') # height later handled by hover
         
         if self._slides_per_cell:
             self.navigate_to(self._slides_per_cell[0].index) # more logical to go in start slide rather end
 
         for slide in self._slides_per_cell:
             slide._scroll_btn = scroll_btn
         
@@ -535,14 +535,15 @@
         return self._ipython_display_()
 
     def _ipython_display_(self):
         "Auto display when self is on last line of a cell"
         if not self.is_jupyter_session():
             raise Exception("Python/IPython REPL cannot show slides. Use IPython notebook instead.")
 
+        clear_output(wait = True) # Avoids jump buttons and other things in same cell created by scripts producing slides
         self._unregister_postrun_cell() # no need to scroll button where showing itself
         self._update_toc()  # Update toc before displaying app to include all sections
         self._update_dynamic_content()  # Update dynamic content before displaying app
         self.close_view()  # Close previous views
         self.__reset_navbox()  # Important to add inview button for each new view
         self._display_box = ipw.VBox(children=[self._box]).add_class(
             "DisplayBox"
```

### Comparing `ipyslides-3.7.6/ipyslides/formatters.py` & `ipyslides-3.8.0/ipyslides/formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,15 +246,17 @@
     
     def get_func(self, obj_type):
         "Get serializer function for a type. Returns None if not found."
         if type(obj_type) in serializer.types: # Do not check instance here, need specific information
             for item in serializer.available:
                 if type(obj_type) == item['obj']:
                     return item['func']
-        # Check instance for ipywidgets.HTML after user defined types
+        # Check instance for ipywidgets.HTML/Output after user defined types
+        elif isinstance(obj_type, ipw.Output):
+            return self._alt_output
         elif isinstance(obj_type, (ipw.HTML, ipw.HTMLMath, HtmlWidget)): # Instance here is fine to include subclasses as they will behave same
             return self._alt_html
         return None
     
     def get_metadata(self, obj_type):
         "Get metadata for a type to use in `display(obj, metadata)` for export purpose. This take precedence over object's own html representation. Returns None if not found."
         if (func := self.get_func(obj_type)):
@@ -272,14 +274,34 @@
         """Convert ipywidgets.HTML object to HTML string."""
         if not isinstance(html_widget,(ipw.HTML,ipw.HTMLMath,HtmlWidget)):
             raise TypeError(f"Expects ipywidgets.(HTML/HTMLMath) or ipyslides's HtmlWidget, got {type(html_widget)}")
 
         className = ' '.join(html_widget._dom_classes) # To keep style of HTML widget, latest as well
         return f'<div class="{className}">{html_widget.value}</div>' 
     
+    def _alt_output(self, output_widget):
+        "Convert objects in ipywidgets.Output to HTML string."
+        if not isinstance(output_widget, ipw.Output):
+            raise TypeError(f"Expects Output widget instnace, got {type(output_widget)}")
+        
+        from .xmd import raw # avoid circular import
+        
+        className = ' '.join(output_widget._dom_classes) # To keep style of Output widget, latest as well
+        content = ''
+        for d in output_widget.outputs:
+            if 'text' in d:
+                content += raw(d['text']).value
+            elif 'data' in d:
+                if 'text/html' in d['data']:
+                    content += d['data']['text/html']  
+                elif 'text/latex' in d['data']:
+                    content += d['data']['text/latex']
+        
+        return f'<div class="{className}">{content}</div>' 
+    
 
     def unregister(self, obj_type):
         "Unregister all serializer handlers for a type."
         for item in self._libs:
             if obj_type is item['obj']:
                 self._libs.remove(item)
```

### Comparing `ipyslides-3.7.6/ipyslides/source.py` & `ipyslides-3.8.0/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/utils.py` & `ipyslides-3.8.0/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides/writer.py` & `ipyslides-3.8.0/ipyslides/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         
     def display(self):
         slides = get_slides_instance()
         if slides and (context := (slides.in_proxy or slides.running)):
             display(context._exp4widget(self._widget, self._func))
         else:
             display(self._widget, metadata = {'DOMWidget': '---'}) # Display widget under slides/notebook anywhere
-
+        
 def _fmt_html(output):
     "Format captured rich output and others to html if possible. Used in other modules too."
     if hasattr(output, 'fmt_html'): # Columns
         return output.fmt_html()
     # Metadat text.html Should take precedence over data if given
     elif hasattr(output, 'metadata') and isinstance(output.metadata, dict) and 'text/html' in output.metadata: 
         return output.metadata['text/html']
@@ -247,7 +247,26 @@
         - A single string passed to `write` is equivalent to `parse` command.
         - You can add mini columns inside a column by markdown syntax or `Slides.cols`, but content type is limited in that case.
     """
     wr = Writer(*objs,widths = widths)
     if not any([(wr._slides and wr._slides.running), wr._in_proxy, len(objs) == 1]):
         return wr.update_display() # Update in usual cell to have widgets working, but not single object which displays outside of box
 
+# Patch for interact/interactive patching to show in output
+
+def _interact_ipython_display(self):
+    def fmt_output_html(w):
+        return serializer.get_func(w.out)(w.out)
+    
+    klass = type(self)
+    ip_disp = getattr(klass, '_ipython_display_',None)
+
+    if ip_disp:
+        delattr(klass, '_ipython_display_') # avoids looping of display
+    
+    AltForWidget(self, fmt_output_html).display() # display internally 
+    
+    if ip_disp:
+        klass._ipython_display_ = ip_disp # reset back
+
+
+ipw.interaction.interactive._ipython_display_ = _interact_ipython_display
```

### Comparing `ipyslides-3.7.6/ipyslides/xmd.py` & `ipyslides-3.8.0/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.8.0/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.7.6
+Version: 3.8.0
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.7.6/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.8.0/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.6/setup.py` & `ipyslides-3.8.0/setup.py`

 * *Files identical despite different names*

