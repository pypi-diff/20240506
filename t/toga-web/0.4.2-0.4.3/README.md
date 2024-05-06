# Comparing `tmp/toga-web-0.4.2.tar.gz` & `tmp/toga_web-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-web-0.4.2.tar", last modified: Tue Feb  6 05:55:16 2024, max compression
+gzip compressed data, was "toga_web-0.4.3.tar", last modified: Mon May  6 06:43:36 2024, max compression
```

## Comparing `toga-web-0.4.2.tar` & `toga_web-0.4.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.259053 toga-web-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-06 05:54:28.000000 toga-web-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:54:28.000000 toga-web-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-02-06 05:55:16.259053 toga-web-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-06 05:54:28.000000 toga-web-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-06 05:54:28.000000 toga-web-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:55:16.259053 toga-web-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.251053 toga-web-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.255053 toga-web-0.4.2/src/toga_web/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/libs.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.255053 toga-web-0.4.2/src/toga_web/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/resources/toga.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.255053 toga-web-0.4.2/src/toga_web/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/static/toga.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.259053 toga-web-0.4.2/src/toga_web/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-06 05:54:28.000000 toga-web-0.4.2/src/toga_web/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:55:16.259053 toga-web-0.4.2/src/toga_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-02-06 05:55:16.000000 toga-web-0.4.2/src/toga_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-06 05:55:16.000000 toga-web-0.4.2/src/toga_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:55:16.000000 toga-web-0.4.2/src/toga_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 05:55:16.000000 toga-web-0.4.2/src/toga_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 05:55:16.000000 toga-web-0.4.2/src/toga_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-06 05:55:16.000000 toga-web-0.4.2/src/toga_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.014005 toga_web-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:01.000000 toga_web-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:01.000000 toga_web-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 06:43:36.010005 toga_web-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 06:43:01.000000 toga_web-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-06 06:43:01.000000 toga_web-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:36.014005 toga_web-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.006005 toga_web-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.006005 toga_web-0.4.3/src/toga_web/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/static/toga.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-06 06:43:36.000000 toga_web-0.4.3/src/toga_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/top_level.txt
```

### Comparing `toga-web-0.4.2/LICENSE` & `toga_web-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/PKG-INFO` & `toga_web-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: toga-web
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Web backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
-Project-URL: Documentation, https://toga.readthedocs.io/en/latest/
+Project-URL: Documentation, https://toga.readthedocs.io/
 Project-URL: Tracker, https://github.com/beeware/toga/issues
 Project-URL: Source, https://github.com/beeware/toga
+Project-URL: Changelog, https://toga.readthedocs.io/en/stable/background/project/releases.html
 Keywords: gui,widget,cross-platform,toga,web,pyscript,pyodide,wasm
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-web
 ========
 
 A backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `Web platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/web.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/web.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-web-0.4.2/README.rst` & `toga_web-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ========
 
 A backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `Web platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/web.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/web.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-web-0.4.2/pyproject.toml` & `toga_web-0.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools==69.0.0",
+    "setuptools==69.5.1",
     "setuptools_scm==8.0.4",
     "setuptools_dynamic_dependencies @ git+https://github.com/beeware/setuptools_dynamic_dependencies",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version", "dependencies"]
@@ -36,26 +36,28 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 [project.urls]
 Homepage = "https://beeware.org/project/projects/libraries/toga/"
 Funding = "https://beeware.org/contributing/membership/"
-Documentation = "https://toga.readthedocs.io/en/latest/"
+Documentation = "https://toga.readthedocs.io/"
 Tracker = "https://github.com/beeware/toga/issues"
 Source = "https://github.com/beeware/toga"
+Changelog = "https://toga.readthedocs.io/en/stable/background/project/releases.html"
 
 [project.entry-points."toga.backends"]
 web = "toga_web"
 
 [tool.setuptools_scm]
 root = ".."
```

### Comparing `toga-web-0.4.2/src/toga_web/app.py` & `toga_web-0.4.3/src/toga_web/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import toga
 from toga.command import Separator
 from toga_web.libs import create_element, js
 from toga_web.window import Window
 
+from .screens import Screen as ScreenImpl
+
 
 class MainWindow(Window):
     def on_close(self, *args):
         pass
 
 
 class App:
@@ -38,14 +40,18 @@
         # the <header> for the menubar is inserted before the <main> for the
         # main window.
         self.create_menus()
 
         # Call user code to populate the main window
         self.interface._startup()
 
+    ######################################################################
+    # Commands and menus
+    ######################################################################
+
     def _create_submenu(self, group, items):
         submenu = create_element(
             "sl-dropdown",
             children=[
                 create_element(
                     "span",
                     id=f"menu-{id(group)}",
@@ -57,14 +63,17 @@
                     "sl-menu",
                     children=items,
                 ),
             ],
         )
         return submenu
 
+    def _menu_about(self, command, **kwargs):
+        self.interface.about()
+
     def create_menus(self):
         self._menu_groups = {}
         submenu = None
 
         for cmd in self.interface.commands:
             if isinstance(cmd, Separator):
                 # TODO - add a section break
@@ -129,23 +138,44 @@
         # If there's an existing menubar, replace it.
         old_menubar = js.document.getElementById(menubar_id)
         if old_menubar:
             old_menubar.replaceWith(self.menubar)
         else:
             self.native.append(self.menubar)
 
-    def _menu_about(self, command, **kwargs):
-        self.interface.about()
+    ######################################################################
+    # App lifecycle
+    ######################################################################
+
+    def exit(self):
+        pass
 
     def main_loop(self):
         self.create()
 
+    def set_icon(self, icon):
+        pass
+
     def set_main_window(self, window):
         pass
 
+    ######################################################################
+    # App resources
+    ######################################################################
+
+    def get_screens(self):
+        return [ScreenImpl(js.document.documentElement)]
+
+    ######################################################################
+    # App capabilities
+    ######################################################################
+
+    def beep(self):
+        self.interface.factory.not_implemented("App.beep()")
+
     def show_about_dialog(self):
         name_and_version = f"{self.interface.formal_name}"
 
         if self.interface.version is not None:
             name_and_version += f" v{self.interface.version}"
 
         if self.interface.author is not None:
@@ -182,30 +212,36 @@
         # constructed. Only show the dialog when the promise of <sl-dialog>
         # element construction has been fulfilled.
         def show_dialog(promise):
             about_dialog.show()
 
         js.customElements.whenDefined("sl-dialog").then(show_dialog)
 
-    def beep(self):
-        self.interface.factory.not_implemented("App.beep()")
+    ######################################################################
+    # Cursor control
+    ######################################################################
 
-    def exit(self):
-        pass
+    def show_cursor(self):
+        self.interface.factory.not_implemented("App.show_cursor()")
+
+    def hide_cursor(self):
+        self.interface.factory.not_implemented("App.hide_cursor()")
+
+    ######################################################################
+    # Window control
+    ######################################################################
 
     def get_current_window(self):
         self.interface.factory.not_implemented("App.get_current_window()")
 
     def set_current_window(self):
         self.interface.factory.not_implemented("App.set_current_window()")
 
+    ######################################################################
+    # Full screen control
+    ######################################################################
+
     def enter_full_screen(self, windows):
         self.interface.factory.not_implemented("App.enter_full_screen()")
 
     def exit_full_screen(self, windows):
         self.interface.factory.not_implemented("App.exit_full_screen()")
-
-    def show_cursor(self):
-        self.interface.factory.not_implemented("App.show_cursor()")
-
-    def hide_cursor(self):
-        self.interface.factory.not_implemented("App.hide_cursor()")
```

### Comparing `toga-web-0.4.2/src/toga_web/command.py` & `toga_web-0.4.3/src/toga_web/command.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/dialogs.py` & `toga_web-0.4.3/src/toga_web/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/factory.py` & `toga_web-0.4.3/src/toga_web/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from toga import NotImplementedWarning
+
 from . import dialogs
 from .app import App, MainWindow  # DocumentApp
 from .command import Command
 
 # from .documents import Document
 # from .fonts import Font
 from .icons import Icon
@@ -35,15 +37,15 @@
 
 # from .widgets.tree import Tree
 # from .widgets.webview import WebView
 # from .window import Window
 
 
 def not_implemented(feature):
-    print(f"[Web] Not implemented: {feature}")  # pragma: nocover
+    NotImplementedWarning.warn("Web", feature)  # pragma: nocover
 
 
 __all__ = [
     "not_implemented",
     "App",
     "MainWindow",
     # 'DocumentApp',
```

### Comparing `toga-web-0.4.2/src/toga_web/libs.py` & `toga_web-0.4.3/src/toga_web/libs.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/resources/toga.png` & `toga_web-0.4.3/src/toga_web/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/static/toga.css` & `toga_web-0.4.3/src/toga_web/static/toga.css`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/widgets/base.py` & `toga_web-0.4.3/src/toga_web/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/widgets/button.py` & `toga_web-0.4.3/src/toga_web/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/widgets/progressbar.py` & `toga_web-0.4.3/src/toga_web/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/widgets/switch.py` & `toga_web-0.4.3/src/toga_web/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web/widgets/textinput.py` & `toga_web-0.4.3/src/toga_web/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga-web-0.4.2/src/toga_web.egg-info/PKG-INFO` & `toga_web-0.4.3/src/toga_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: toga-web
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Web backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
-Project-URL: Documentation, https://toga.readthedocs.io/en/latest/
+Project-URL: Documentation, https://toga.readthedocs.io/
 Project-URL: Tracker, https://github.com/beeware/toga/issues
 Project-URL: Source, https://github.com/beeware/toga
+Project-URL: Changelog, https://toga.readthedocs.io/en/stable/background/project/releases.html
 Keywords: gui,widget,cross-platform,toga,web,pyscript,pyodide,wasm
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-web
 ========
 
 A backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `Web platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/web.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/web.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-web-0.4.2/src/toga_web.egg-info/SOURCES.txt` & `toga_web-0.4.3/src/toga_web.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/toga_web/app.py
 src/toga_web/command.py
 src/toga_web/dialogs.py
 src/toga_web/factory.py
 src/toga_web/icons.py
 src/toga_web/libs.py
 src/toga_web/paths.py
+src/toga_web/screens.py
 src/toga_web/window.py
 src/toga_web.egg-info/PKG-INFO
 src/toga_web.egg-info/SOURCES.txt
 src/toga_web.egg-info/dependency_links.txt
 src/toga_web.egg-info/entry_points.txt
 src/toga_web.egg-info/requires.txt
 src/toga_web.egg-info/top_level.txt
```

