# Comparing `tmp/bokeh_joystick_widget-0.3.0.tar.gz` & `tmp/bokeh_joystick_widget-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokeh_joystick_widget-0.3.0.tar", max compression
+gzip compressed data, was "bokeh_joystick_widget-0.3.1.tar", max compression
```

## Comparing `bokeh_joystick_widget-0.3.0.tar` & `bokeh_joystick_widget-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2024-04-27 13:27:59.218205 bokeh_joystick_widget-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1645 2024-05-06 12:54:41.637153 bokeh_joystick_widget-0.3.0/README.md
--rw-r--r--   0        0        0     1205 2024-05-06 12:56:01.622945 bokeh_joystick_widget-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1142 2024-05-06 12:48:37.586617 bokeh_joystick_widget-0.3.0/src/bokeh_joystick_widget/__init__.py
--rw-r--r--   0        0        0    17001 2024-05-06 12:33:41.622968 bokeh_joystick_widget-0.3.0/src/bokeh_joystick_widget/joystick.ts
--rw-r--r--   0        0        0     2301 2024-05-06 12:52:45.526456 bokeh_joystick_widget-0.3.0/src/bokeh_joystick_widget/joystick_widget.ts
--rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.3.0/setup.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-27 13:27:59.218205 bokeh_joystick_widget-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     1652 2024-05-06 12:58:55.339295 bokeh_joystick_widget-0.3.1/README.md
+-rw-r--r--   0        0        0     1198 2024-05-06 13:00:45.437061 bokeh_joystick_widget-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1142 2024-05-06 12:48:37.586617 bokeh_joystick_widget-0.3.1/src/bokeh_joystick_widget/__init__.py
+-rw-r--r--   0        0        0    17001 2024-05-06 12:33:41.622968 bokeh_joystick_widget-0.3.1/src/bokeh_joystick_widget/joystick.ts
+-rw-r--r--   0        0        0     2301 2024-05-06 12:52:45.526456 bokeh_joystick_widget-0.3.1/src/bokeh_joystick_widget/joystick_widget.ts
+-rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.3.1/setup.py
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.3.1/PKG-INFO
```

### Comparing `bokeh_joystick_widget-0.3.0/LICENSE.md` & `bokeh_joystick_widget-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.3.0/README.md` & `bokeh_joystick_widget-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 
 - Get the example JS demo widget/bokeh model to work - whatever that widget is. - done
 - Figure out how to get values back to the python end with it. - done
 - Figure out how to swap their control for the joystick (however hacky) - done
     - Note - this is a TS file from the original, adapted here. The DOM element change
       is important.
 - Figure out how to make that tidier. - done
-- Figure out how to publish to PyPi (alpha) and test in a pip installed test.
+- Figure out how to publish to PyPi (alpha) and test in a pip installed test. - done
```

### Comparing `bokeh_joystick_widget-0.3.0/pyproject.toml` & `bokeh_joystick_widget-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry]
 name = "bokeh-joystick-widget"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Bokeh on screen gesture/mouse drag based joystick widget for use in a dashboard with controls"
 authors = ["Danny Staple <danny@orionrobots.co.uk>"]
-license = "LICENSE.md"
+license = "MIT"
 readme = "README.md"
 packages = [
   {include = "bokeh_joystick_widget", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `bokeh_joystick_widget-0.3.0/src/bokeh_joystick_widget/__init__.py` & `bokeh_joystick_widget-0.3.1/src/bokeh_joystick_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.3.0/src/bokeh_joystick_widget/joystick.ts` & `bokeh_joystick_widget-0.3.1/src/bokeh_joystick_widget/joystick.ts`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.3.0/src/bokeh_joystick_widget/joystick_widget.ts` & `bokeh_joystick_widget-0.3.1/src/bokeh_joystick_widget/joystick_widget.ts`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.3.0/setup.py` & `bokeh_joystick_widget-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['bokeh>=3.4.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'bokeh-joystick-widget',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A Bokeh on screen gesture/mouse drag based joystick widget for use in a dashboard with controls',
-    'long_description': '# Bokeh Joystick Widget\n\nThis is a custom widget for the Python Bokeh library that allows you to control a joystick via mouse drags or touch gestures.\n\nThe widget has x and y properties that are updated as the joystick is moved. The x and y properties are in the range -100 to 100.\n\nThe widget is derived from <https://github.com/bobboteck/JoyStick/>.\n\n## Setup\n\nInstall with pip:\n\n```bash\npip install bokeh-joystick-widget\n```\n\nOr poetry:\n\n```bash\npoetry add bokeh-joystick-widget\n```\n\n## Usage\n\nIn your bokeh app, you can use the joystick widget like this:\n\n```python\nfrom bokeh_joystick_widget import JoystickWidget\n:\n# some plot\n:\njoystick = JoystickWidget()\njoystick.on_change("position", lambda attr, old, new: print(f\'x: {new["x"]}, y: {new["y"]}\'))\n:\n:\nshow(column(joystick, plot))\n```\n\n## Examples\n\nThere are 3 examples:\n\n- examples/static_joystick_example.py - show a column with a plot and the joystick, then exit.\n- examples/console_joystick_example.py - show a plot and the joystick in a bokeh server app. Callbacks from the front end drive console logs of the joystick position.\n- examples/bigger_joystick.py - Scale the size of the rendered joystick.\n\n## Roadmap\n\n- Get the example JS demo widget/bokeh model to work - whatever that widget is. - done\n- Figure out how to get values back to the python end with it. - done\n- Figure out how to swap their control for the joystick (however hacky) - done\n    - Note - this is a TS file from the original, adapted here. The DOM element change\n      is important.\n- Figure out how to make that tidier. - done\n- Figure out how to publish to PyPi (alpha) and test in a pip installed test.\n',
+    'long_description': '# Bokeh Joystick Widget\n\nThis is a custom widget for the Python Bokeh library that allows you to control a joystick via mouse drags or touch gestures.\n\nThe widget has x and y properties that are updated as the joystick is moved. The x and y properties are in the range -100 to 100.\n\nThe widget is derived from <https://github.com/bobboteck/JoyStick/>.\n\n## Setup\n\nInstall with pip:\n\n```bash\npip install bokeh-joystick-widget\n```\n\nOr poetry:\n\n```bash\npoetry add bokeh-joystick-widget\n```\n\n## Usage\n\nIn your bokeh app, you can use the joystick widget like this:\n\n```python\nfrom bokeh_joystick_widget import JoystickWidget\n:\n# some plot\n:\njoystick = JoystickWidget()\njoystick.on_change("position", lambda attr, old, new: print(f\'x: {new["x"]}, y: {new["y"]}\'))\n:\n:\nshow(column(joystick, plot))\n```\n\n## Examples\n\nThere are 3 examples:\n\n- examples/static_joystick_example.py - show a column with a plot and the joystick, then exit.\n- examples/console_joystick_example.py - show a plot and the joystick in a bokeh server app. Callbacks from the front end drive console logs of the joystick position.\n- examples/bigger_joystick.py - Scale the size of the rendered joystick.\n\n## Roadmap\n\n- Get the example JS demo widget/bokeh model to work - whatever that widget is. - done\n- Figure out how to get values back to the python end with it. - done\n- Figure out how to swap their control for the joystick (however hacky) - done\n    - Note - this is a TS file from the original, adapted here. The DOM element change\n      is important.\n- Figure out how to make that tidier. - done\n- Figure out how to publish to PyPi (alpha) and test in a pip installed test. - done\n',
     'author': 'Danny Staple',
     'author_email': 'danny@orionrobots.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `bokeh_joystick_widget-0.3.0/PKG-INFO` & `bokeh_joystick_widget-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bokeh-joystick-widget
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Bokeh on screen gesture/mouse drag based joystick widget for use in a dashboard with controls
-License: LICENSE.md
+License: MIT
 Author: Danny Staple
 Author-email: danny@orionrobots.co.uk
 Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=3.4.1,<4.0.0)
 Description-Content-Type: text/markdown
 
@@ -64,9 +64,9 @@
 
 - Get the example JS demo widget/bokeh model to work - whatever that widget is. - done
 - Figure out how to get values back to the python end with it. - done
 - Figure out how to swap their control for the joystick (however hacky) - done
     - Note - this is a TS file from the original, adapted here. The DOM element change
       is important.
 - Figure out how to make that tidier. - done
-- Figure out how to publish to PyPi (alpha) and test in a pip installed test.
+- Figure out how to publish to PyPi (alpha) and test in a pip installed test. - done
```

