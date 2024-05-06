# Comparing `tmp/bokeh_joystick_widget-0.1.0.tar.gz` & `tmp/bokeh_joystick_widget-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokeh_joystick_widget-0.1.0.tar", max compression
+gzip compressed data, was "bokeh_joystick_widget-0.2.0.tar", max compression
```

## Comparing `bokeh_joystick_widget-0.1.0.tar` & `bokeh_joystick_widget-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2024-04-27 13:27:59.218205 bokeh_joystick_widget-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1149 2024-05-05 19:30:28.539104 bokeh_joystick_widget-0.1.0/README.md
--rw-r--r--   0        0        0     1205 2024-04-27 15:40:05.187680 bokeh_joystick_widget-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      923 2024-05-05 19:34:31.370191 bokeh_joystick_widget-0.1.0/src/bokeh_joystick_widget/__init__.py
--rw-r--r--   0        0        0    16833 2024-05-05 18:27:31.987208 bokeh_joystick_widget-0.1.0/src/bokeh_joystick_widget/joystick.ts
--rw-r--r--   0        0        0     2284 2024-05-05 19:20:39.455354 bokeh_joystick_widget-0.1.0/src/bokeh_joystick_widget/joystick_widget.ts
--rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.1.0/setup.py
--rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-27 13:27:59.218205 bokeh_joystick_widget-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1573 2024-05-06 11:01:46.472177 bokeh_joystick_widget-0.2.0/README.md
+-rw-r--r--   0        0        0     1205 2024-05-06 11:00:07.996084 bokeh_joystick_widget-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      923 2024-05-05 19:34:31.370191 bokeh_joystick_widget-0.2.0/src/bokeh_joystick_widget/__init__.py
+-rw-r--r--   0        0        0    17003 2024-05-06 12:25:29.222769 bokeh_joystick_widget-0.2.0/src/bokeh_joystick_widget/joystick.ts
+-rw-r--r--   0        0        0     2284 2024-05-06 12:22:20.293044 bokeh_joystick_widget-0.2.0/src/bokeh_joystick_widget/joystick_widget.ts
+-rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.2.0/setup.py
+-rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 bokeh_joystick_widget-0.2.0/PKG-INFO
```

### Comparing `bokeh_joystick_widget-0.1.0/LICENSE.md` & `bokeh_joystick_widget-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.1.0/README.md` & `bokeh_joystick_widget-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,44 @@
 
 The widget has x and y properties that are updated as the joystick is moved. The x and y properties are in the range -100 to 100.
 
 The widget makes use of <https://github.com/bobboteck/JoyStick/>.
 
 ## Setup
 
+Install with pip:
+
+```bash
+pip install bokeh-joystick-widget
+```
+
+Or poetry:
+
+```bash
+poetry add bokeh-joystick-widget
+```
+
 ## Usage
 
+In your bokeh app, you can use the joystick widget like this:
+
+```python
+from bokeh_joystick_widget import JoystickWidget
+:
+# some plot
+:
+joystick = JoystickWidget()
+joystick.on_change("position", lambda attr, old, new: print(f'x: {new["x"]}, y: {new["y"]}'))
+:
+:
+show(column(joystick, plot))
+```
+
+
+
 ## Examples
 
 There are two examples:
 
 - examples/static_joystick_example.py - show a column with a plot and the joystick, then exit.
 - examples/console_joystick_example.py - show a plot and the joystick in a bokeh server app. Callbacks from the front end drive console logs of the joystick position.
```

### Comparing `bokeh_joystick_widget-0.1.0/pyproject.toml` & `bokeh_joystick_widget-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry]
 name = "bokeh-joystick-widget"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Bokeh on screen gesture/mouse drag based joystick widget for use in a dashboard with controls"
 authors = ["Danny Staple <danny@orionrobots.co.uk>"]
 license = "LICENSE.md"
 readme = "README.md"
 packages = [
   {include = "bokeh_joystick_widget", from = "src"}
 ]
```

### Comparing `bokeh_joystick_widget-0.1.0/src/bokeh_joystick_widget/__init__.py` & `bokeh_joystick_widget-0.2.0/src/bokeh_joystick_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.1.0/src/bokeh_joystick_widget/joystick.ts` & `bokeh_joystick_widget-0.2.0/src/bokeh_joystick_widget/joystick.ts`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,21 @@
   externalLineWidth: 2,
   externalStrokeColor: "#008000",
   autoReturnToCenter: true,
 };
 
 export type JoyStickCallback = (stickStatus: StickStatus) => void;
 
+function hasTouch(): boolean {
+  const isTouchCapable = "ontouchstart" in document.documentElement ||
+    'ontouchstart' in window ||
+    navigator.maxTouchPoints > 0;
+  return isTouchCapable;
+}
+
 export class JoyStick {
   private title: string;
   private width: number;
   private height: number;
   private internalFillColor: string;
   private internalLineWidth: number;
   private internalStrokeColor: string;
@@ -203,38 +210,38 @@
     this.stickStatus = defaultStickStatus;
     this.pressed = false;
     // Used to save current position of stick
     this.movedX = this.centerX;
     this.movedY = this.centerY;
 
     // Check if the device support the touch or not
-    if ("ontouchstart" in document.documentElement) {
+    if (hasTouch()) {
       this.canvas.addEventListener(
         "touchstart",
         this.onTouchStart.bind(this),
         false
       );
-      document.addEventListener(
+      container.addEventListener(
         "touchmove",
         this.onTouchMove.bind(this),
         false
       );
-      document.addEventListener("touchend", this.onTouchEnd.bind(this), false);
+      container.addEventListener("touchend", this.onTouchEnd.bind(this), false);
     } else {
       this.canvas.addEventListener(
         "mousedown",
         this.onMouseDown.bind(this),
         false
       );
-      document.addEventListener(
+      container.addEventListener(
         "mousemove",
         this.onMouseMove.bind(this),
         false
       );
-      document.addEventListener("mouseup", this.onMouseUp.bind(this), false);
+      container.addEventListener("mouseup", this.onMouseUp.bind(this), false);
     }
 
     // Draw the object
     this.drawExternal();
     this.drawInternal();
   }
 
@@ -427,15 +434,15 @@
       100 * ((this.movedY - this.centerY) / this.maxMoveStick) * -1;
     this.stickStatus.cardinalDirection = this.getCardinalDirection();
     this.callback(this.stickStatus);
   }
 
   getCardinalDirection() {
     let result = "";
-    const orizontal = this.movedX - this.centerX;
+    const horizontal = this.movedX - this.centerX;
     const vertical = this.movedY - this.centerY;
 
     if (
       vertical >= this.directionVerticalLimitNeg &&
       vertical <= this.directionVerticalLimitPos
     ) {
       result = "C";
@@ -443,22 +450,22 @@
     if (vertical < this.directionVerticalLimitNeg) {
       result = "N";
     }
     if (vertical > this.directionVerticalLimitPos) {
       result = "S";
     }
 
-    if (orizontal < this.directionHorizontalLimitNeg) {
+    if (horizontal < this.directionHorizontalLimitNeg) {
       if (result === "C") {
         result = "W";
       } else {
         result += "W";
       }
     }
-    if (orizontal > this.directionHorizontalLimitPos) {
+    if (horizontal > this.directionHorizontalLimitPos) {
       if (result === "C") {
         result = "E";
       } else {
         result += "E";
       }
     }
 
@@ -472,15 +479,15 @@
     return this.canvas.width;
   }
 
   /**
    * @desc The height of canvas
    * @return Number of pixel height
    */
-  public getHeigh() {
+  public getHeight() {
     return this.canvas.height;
   }
 
   /**
    * @desc The X position of the cursor relative to the canvas that contains it and to its dimensions
    * @return Number that indicate relative position
    */
@@ -493,23 +500,23 @@
    * @return Number that indicate relative position
    */
   public getPosY() {
     return this.movedY;
   }
 
   /**
-   * @desc Normalizzed value of X move of stick
+   * @desc Normalized value of X move of stick
    * @return Integer from -100 to +100
    */
   public getX() {
     return 100 * ((this.movedX - this.centerX) / this.maxMoveStick);
   }
 
   /**
-   * @desc Normalizzed value of Y move of stick
+   * @desc Normalized value of Y move of stick
    * @return Integer from -100 to +100
    */
   public getY() {
     return 100 * ((this.movedY - this.centerY) / this.maxMoveStick) * -1;
   }
 
   /**
```

### Comparing `bokeh_joystick_widget-0.1.0/src/bokeh_joystick_widget/joystick_widget.ts` & `bokeh_joystick_widget-0.2.0/src/bokeh_joystick_widget/joystick_widget.ts`

 * *Files identical despite different names*

### Comparing `bokeh_joystick_widget-0.1.0/setup.py` & `bokeh_joystick_widget-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['bokeh>=3.4.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'bokeh-joystick-widget',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'A Bokeh on screen gesture/mouse drag based joystick widget for use in a dashboard with controls',
-    'long_description': '# Bokeh Joystick Widget\n\nThis is a custom widget for the Python Bokeh library that allows you to control a joystick via mouse drags or touch gestures.\n\nThe widget has x and y properties that are updated as the joystick is moved. The x and y properties are in the range -100 to 100.\n\nThe widget makes use of <https://github.com/bobboteck/JoyStick/>.\n\n## Setup\n\n## Usage\n\n## Examples\n\nThere are two examples:\n\n- examples/static_joystick_example.py - show a column with a plot and the joystick, then exit.\n- examples/console_joystick_example.py - show a plot and the joystick in a bokeh server app. Callbacks from the front end drive console logs of the joystick position.\n\n## Roadmap\n\n- Get the example JS demo widget/bokeh model to work - whatever that widget is. - done\n- Figure out how to get values back to the python end with it. - done\n- Figure out how to swap their control for the joystick (however hacky) - done\n    - Note - this is a TS file from the original, adapted here. The DOM element change\n      is important.\n- Figure out how to make that tidier. - done\n- Figure out how to publish to PyPi (alpha) and test in a pip installed test.\n',
+    'long_description': '# Bokeh Joystick Widget\n\nThis is a custom widget for the Python Bokeh library that allows you to control a joystick via mouse drags or touch gestures.\n\nThe widget has x and y properties that are updated as the joystick is moved. The x and y properties are in the range -100 to 100.\n\nThe widget makes use of <https://github.com/bobboteck/JoyStick/>.\n\n## Setup\n\nInstall with pip:\n\n```bash\npip install bokeh-joystick-widget\n```\n\nOr poetry:\n\n```bash\npoetry add bokeh-joystick-widget\n```\n\n## Usage\n\nIn your bokeh app, you can use the joystick widget like this:\n\n```python\nfrom bokeh_joystick_widget import JoystickWidget\n:\n# some plot\n:\njoystick = JoystickWidget()\njoystick.on_change("position", lambda attr, old, new: print(f\'x: {new["x"]}, y: {new["y"]}\'))\n:\n:\nshow(column(joystick, plot))\n```\n\n\n\n## Examples\n\nThere are two examples:\n\n- examples/static_joystick_example.py - show a column with a plot and the joystick, then exit.\n- examples/console_joystick_example.py - show a plot and the joystick in a bokeh server app. Callbacks from the front end drive console logs of the joystick position.\n\n## Roadmap\n\n- Get the example JS demo widget/bokeh model to work - whatever that widget is. - done\n- Figure out how to get values back to the python end with it. - done\n- Figure out how to swap their control for the joystick (however hacky) - done\n    - Note - this is a TS file from the original, adapted here. The DOM element change\n      is important.\n- Figure out how to make that tidier. - done\n- Figure out how to publish to PyPi (alpha) and test in a pip installed test.\n',
     'author': 'Danny Staple',
     'author_email': 'danny@orionrobots.co.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `bokeh_joystick_widget-0.1.0/PKG-INFO` & `bokeh_joystick_widget-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh-joystick-widget
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Bokeh on screen gesture/mouse drag based joystick widget for use in a dashboard with controls
 License: LICENSE.md
 Author: Danny Staple
 Author-email: danny@orionrobots.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,44 @@
 
 The widget has x and y properties that are updated as the joystick is moved. The x and y properties are in the range -100 to 100.
 
 The widget makes use of <https://github.com/bobboteck/JoyStick/>.
 
 ## Setup
 
+Install with pip:
+
+```bash
+pip install bokeh-joystick-widget
+```
+
+Or poetry:
+
+```bash
+poetry add bokeh-joystick-widget
+```
+
 ## Usage
 
+In your bokeh app, you can use the joystick widget like this:
+
+```python
+from bokeh_joystick_widget import JoystickWidget
+:
+# some plot
+:
+joystick = JoystickWidget()
+joystick.on_change("position", lambda attr, old, new: print(f'x: {new["x"]}, y: {new["y"]}'))
+:
+:
+show(column(joystick, plot))
+```
+
+
+
 ## Examples
 
 There are two examples:
 
 - examples/static_joystick_example.py - show a column with a plot and the joystick, then exit.
 - examples/console_joystick_example.py - show a plot and the joystick in a bokeh server app. Callbacks from the front end drive console logs of the joystick position.
```

