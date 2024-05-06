# Comparing `tmp/scenebuilder-0.1.3.tar.gz` & `tmp/scenebuilder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenebuilder-0.1.3.tar", max compression
+gzip compressed data, was "scenebuilder-0.1.4.tar", max compression
```

## Comparing `scenebuilder-0.1.3.tar` & `scenebuilder-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.3/LICENSE
--rw-r--r--   0        0        0     3443 2024-05-05 23:21:43.167541 scenebuilder-0.1.3/README.md
--rw-r--r--   0        0        0      473 2024-05-05 23:52:00.762314 scenebuilder-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       38 2024-05-05 17:53:13.810692 scenebuilder-0.1.3/scenebuilder/__init__.py
--rw-r--r--   0        0        0      851 2024-05-05 23:20:30.173794 scenebuilder-0.1.3/scenebuilder/actions_stack.py
--rw-r--r--   0        0        0     4262 2024-05-05 23:20:28.835485 scenebuilder-0.1.3/scenebuilder/construction.py
--rw-r--r--   0        0        0     4909 2024-05-05 23:20:22.042742 scenebuilder-0.1.3/scenebuilder/entities.py
--rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.3/scenebuilder/mixins.py
--rw-r--r--   0        0        0     2204 2024-05-05 23:20:15.139535 scenebuilder-0.1.3/scenebuilder/observer_utils.py
--rw-r--r--   0        0        0     4341 2024-05-05 23:20:14.044613 scenebuilder-0.1.3/scenebuilder/patches.py
--rw-r--r--   0        0        0    20431 2024-05-05 23:24:43.233779 scenebuilder-0.1.3/scenebuilder/scenebuilder.py
--rw-r--r--   0        0        0     1711 2024-05-05 23:20:11.172433 scenebuilder-0.1.3/scenebuilder/ui_components.py
--rw-r--r--   0        0        0     3449 2024-05-05 18:55:06.173234 scenebuilder-0.1.3/scenebuilder/utils.py
--rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 scenebuilder-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3665 2024-05-06 09:27:57.007567 scenebuilder-0.1.4/README.md
+-rw-r--r--   0        0        0      486 2024-05-06 09:29:22.928854 scenebuilder-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-06 09:11:58.678352 scenebuilder-0.1.4/scenebuilder/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-06 09:09:11.273082 scenebuilder-0.1.4/scenebuilder/actions_stack.py
+-rw-r--r--   0        0        0     4206 2024-05-06 09:09:05.634947 scenebuilder-0.1.4/scenebuilder/construction.py
+-rw-r--r--   0        0        0     4909 2024-05-05 23:20:22.042742 scenebuilder-0.1.4/scenebuilder/entities.py
+-rw-r--r--   0        0        0      601 2024-05-06 09:05:40.973167 scenebuilder-0.1.4/scenebuilder/main.py
+-rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.4/scenebuilder/mixins.py
+-rw-r--r--   0        0        0     2194 2024-05-06 09:08:29.586634 scenebuilder-0.1.4/scenebuilder/observer_utils.py
+-rw-r--r--   0        0        0     4329 2024-05-06 09:08:22.356210 scenebuilder-0.1.4/scenebuilder/patches.py
+-rw-r--r--   0        0        0    20347 2024-05-06 09:08:16.420109 scenebuilder-0.1.4/scenebuilder/scenebuilder.py
+-rw-r--r--   0        0        0     1698 2024-05-06 09:11:58.711638 scenebuilder-0.1.4/scenebuilder/ui_components.py
+-rw-r--r--   0        0        0     3763 2024-05-06 09:11:58.729421 scenebuilder-0.1.4/scenebuilder/utils.py
+-rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 scenebuilder-0.1.4/PKG-INFO
```

### Comparing `scenebuilder-0.1.3/LICENSE` & `scenebuilder-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.3/README.md` & `scenebuilder-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-
 # SceneBuilder
 
 ## Overview
+
 **SceneBuilder** is a Python package that provides a Matplotlib-based GUI for designing 2D test environments in a 10x10m grid for use in multiagent path planning algorithms. Users can draw polygons to represent obstacles and arrows to indicate the starting and ending points of each agent's path.
 
+<!-- ![Scene Example 1](/assets/scene1.png){width=10 height=10} -->
+<p align="center">
+  <img src="/assets/scene1.png" alt="First Image" width="40%" />
+  <img src="/assets/scene2.png" alt="Second Image" width="40%" />
+</p>
+
 ## Installation
 
 To install SceneBuilder, run the following command:
 
 ```bash
 pip install scenebuilder
 ```
-This command installs SceneBuilder along with all required dependencies, ensuring that everything needed to run the GUI is properly set up.
+
+This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
+
+
 
 ## Getting Started
 
 ### Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
@@ -30,14 +39,15 @@
 scene = SceneBuilder()
 
 # Open the GUI to draw a scene
 scene.draw_scene()
 ```
 
 Load in an existing compatible json file for modification:
+
 ```python
 scene.load_scene("path/to/your_file.json")
 scene.draw_scene()
 ```
 
 Specify the path to save your output json to:
 
@@ -61,21 +71,21 @@
 
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
-- **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui. 
+- **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
 - **Remove unwanted points**: To remove unwanted points (either obstacle vertices or a drone start point), press escape.
 - **Undo drone/obstacle placement**: To remove the last obstacle or drone, press ctrl+z.
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
 ## Saving Scenes
 
-Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths. 
+Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
 
-***Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory.***
+**_Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory._**
 
 ## Contributing
 
-Contributions to SceneBuilder are welcome! If you have suggestions for improvements or new features, feel free to create an issue or pull request on our GitHub repository.
+Contributions to SceneBuilder are welcome! If you have suggestions for improvements or new features, feel free to create an issue or pull request on our GitHub repository.
```

### Comparing `scenebuilder-0.1.3/scenebuilder/actions_stack.py` & `scenebuilder-0.1.4/scenebuilder/actions_stack.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.3/scenebuilder/construction.py` & `scenebuilder-0.1.4/scenebuilder/construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import matplotlib.pyplot as plt
 
 from matplotlib.lines import Line2D
 from typing import List
-from scenebuilder.entities import Obstacle, Drone
 import numpy as np
-from scenebuilder.patches import ObstaclePatch, DronePatch
-from scenebuilder.patches import Marker
+from .entities import Obstacle, Drone
+from .patches import ObstaclePatch, DronePatch, Marker
 
 
 class PatchManager:
     def __init__(self, ax: plt.Axes):
         self.ax = ax
         self.building_patches: dict[Obstacle, ObstaclePatch] = {}
         self.drone_patches: dict[Drone, DronePatch] = {}
```

### Comparing `scenebuilder-0.1.3/scenebuilder/entities.py` & `scenebuilder-0.1.4/scenebuilder/entities.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.3/scenebuilder/observer_utils.py` & `scenebuilder-0.1.4/scenebuilder/observer_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Callable
+from typing import List
 from abc import ABC, abstractmethod
 
 # Define the Observer interface. This class is an example that could be inherited,
 
 # alternatively define your own call function in the Observable class, such as in InteractivePlot
```

### Comparing `scenebuilder-0.1.3/scenebuilder/patches.py` & `scenebuilder-0.1.4/scenebuilder/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from numpy.typing import ArrayLike
 
 import numpy as np
 from matplotlib.patches import FancyArrow, Polygon
 from matplotlib.lines import Line2D
 import matplotlib.pyplot as plt
 
-from scenebuilder.entities import Drone, Obstacle
+from .entities import Drone, Obstacle
 
 
 class Arrow:
     """Class to create a FancyArrow object"""
 
     def __init__(self, start: ArrayLike, end: ArrayLike, ax: plt.Axes) -> None:
         self.start = np.array(start)
```

### Comparing `scenebuilder-0.1.3/scenebuilder/scenebuilder.py` & `scenebuilder-0.1.4/scenebuilder/scenebuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 
 import numpy as np
 
-from scenebuilder.entities import Drone, Obstacle
-from scenebuilder.utils import distance_between_points, create_json, get_from_json
-from scenebuilder.utils import load_from_json, validate_json_path
-from scenebuilder.construction import PatchManager
-from scenebuilder.actions_stack import ActionsStack
-from scenebuilder.ui_components import UIComponents
-from scenebuilder.observer_utils import Observer, Observable
+from .entities import Drone, Obstacle
+from .utils import distance_between_points, create_json, get_from_json
+from .utils import load_from_json, validate_json_path
+from .construction import PatchManager
+from .actions_stack import ActionsStack
+from .ui_components import UIComponents
+from .observer_utils import Observer, Observable
 from threading import Timer
 
 
 class SceneBuilder(Observer, Observable):
 
     CLICK_THRESHOLD = 0.14
     FIG_SIZE = (8, 8)
```

### Comparing `scenebuilder-0.1.3/scenebuilder/ui_components.py` & `scenebuilder-0.1.4/scenebuilder/ui_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
-from scenebuilder.observer_utils import Observable
+from .observer_utils import Observable
 
 
 class UIComponents(Observable):
     def __init__(self, ax: plt.Axes):
         super().__init__()
         self.ax = ax
         self.fig = ax.figure
@@ -20,15 +20,15 @@
                 "label": "Reset",
                 "callback": self.on_reset,
             },
             "create_json": {
                 "axis": self.fig.add_axes([0.33, 0.01, 0.15, 0.05]),
                 "label": "Create JSON",
                 "callback": self.on_json,
-            } 
+            },
         }
 
         # Initialize buttons and register callbacks
         for key, btn_info in self.buttons.items():
             button = plt.Button(btn_info["axis"], btn_info["label"])
             button.on_clicked(btn_info["callback"])
             self.buttons[key]["button"] = button
@@ -43,8 +43,7 @@
         self.notify_observers("switch_mode")
 
     def on_reset(self, event):
         self.notify_observers("reset")
 
     def on_json(self, event):
         self.notify_observers("create_json")
-
```

### Comparing `scenebuilder-0.1.3/scenebuilder/utils.py` & `scenebuilder-0.1.4/scenebuilder/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.typing import ArrayLike
 
 # from scenebuilder.json_utils import dump_to_json
-from scenebuilder.entities import Drone, Obstacle
+from .entities import Drone, Obstacle
 
 # file to store useful json utilities
 import json, os, sys
 from pathlib import Path
 
 
 def distance_between_points(p1: ArrayLike, p2: ArrayLike) -> float:
@@ -15,22 +15,27 @@
     """
     p1, p2 = np.array(p1), np.array(p2)
     return np.linalg.norm(p1 - p2)
 
 
 def load_from_json(file_path: str) -> dict:
     """Load json file contents into dict"""
+    p = Path(file_path)
+    file_path = p.resolve()
     with open(file_path, "r") as f:
         file_contents = json.load(f)
         return file_contents
 
 
 def dump_to_json(file_path: str, data: dict) -> dict:
     """Write dict to json"""
     # ensure the directory exists
+    p = Path(file_path)
+    # Convert path to absolute path for checking existence and permissions
+    file_path = p.resolve()
     directory = os.path.dirname(file_path)
     if directory:
         os.makedirs(directory, exist_ok=True)
     with open(file_path, "w") as f:
         json.dump(data, f, indent=4)
         return None
 
@@ -46,14 +51,17 @@
     buildings = case_info.get("buildings")
     buildings = [Obstacle(np.array(b["vertices"])) for b in buildings]
     return vehicles, buildings
 
 
 def create_json(path: str, buildings: list[Obstacle], drones: list[Drone]) -> None:
     """Creates the json with the case info and writes it to file at path"""
+    p = Path(path)
+    # Convert path to absolute path for checking existence and permissions
+    abs_path = p.resolve()
     height = 1.2
     # this line adds a third dimension to the x,y coordinates of the building patches and creates a building object from each patch
 
     buildings = [
         {
             "ID": f"B{idx}",
             "vertices": np.hstack(
@@ -68,15 +76,15 @@
 
     vehicles = [
         {"ID": f"V{idx}", "position": v.position.tolist(), "goal": v.goal.tolist()}
         for idx, v in enumerate(drones)
     ]
 
     c = {"scenebuilder": {"buildings": buildings, "vehicles": vehicles}}
-    dump_to_json(path, c)
+    dump_to_json(abs_path, c)
 
 
 # this Class is not finished yet TODO
 class MyEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()  # Convert numpy arrays to lists
@@ -93,15 +101,17 @@
     # Check if the path ends with .json
     if not path.endswith(".json"):
         print(f"The file name '{abs_path.name}' must end with '.json'.")
         sys.exit(1)
 
     # Check if the directory exists and is writable
     if not abs_path.parent.exists() or not abs_path.parent.is_dir():
-        print(f"The directory '{abs_path.parent}' does not exist or is not a directory.")
+        print(
+            f"The directory '{abs_path.parent}' does not exist or is not a directory."
+        )
         sys.exit(1)
 
     if not os.access(abs_path.parent, os.W_OK):
         print(f"The directory '{abs_path.parent}' is not writable.")
         sys.exit(1)
 
     # If all checks are passed, confirm the path is valid
```

### Comparing `scenebuilder-0.1.3/PKG-INFO` & `scenebuilder-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: scenebuilder
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple GUI to create 2D scenes with obstacles and drone paths for multi-agent path planning algorithms
 Author: Adrian del Ser
 Author-email: adrian.delser@gmail.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Description-Content-Type: text/markdown
 
-
 # SceneBuilder
 
 ## Overview
+
 **SceneBuilder** is a Python package that provides a Matplotlib-based GUI for designing 2D test environments in a 10x10m grid for use in multiagent path planning algorithms. Users can draw polygons to represent obstacles and arrows to indicate the starting and ending points of each agent's path.
 
+<!-- ![Scene Example 1](/assets/scene1.png){width=10 height=10} -->
+<p align="center">
+  <img src="/assets/scene1.png" alt="First Image" width="40%" />
+  <img src="/assets/scene2.png" alt="Second Image" width="40%" />
+</p>
+
 ## Installation
 
 To install SceneBuilder, run the following command:
 
 ```bash
 pip install scenebuilder
 ```
-This command installs SceneBuilder along with all required dependencies, ensuring that everything needed to run the GUI is properly set up.
+
+This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
+
+
 
 ## Getting Started
 
 ### Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
@@ -44,14 +53,15 @@
 scene = SceneBuilder()
 
 # Open the GUI to draw a scene
 scene.draw_scene()
 ```
 
 Load in an existing compatible json file for modification:
+
 ```python
 scene.load_scene("path/to/your_file.json")
 scene.draw_scene()
 ```
 
 Specify the path to save your output json to:
 
@@ -75,21 +85,22 @@
 
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
-- **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui. 
+- **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
 - **Remove unwanted points**: To remove unwanted points (either obstacle vertices or a drone start point), press escape.
 - **Undo drone/obstacle placement**: To remove the last obstacle or drone, press ctrl+z.
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
 ## Saving Scenes
 
-Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths. 
+Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
 
-***Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory.***
+**_Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory._**
 
 ## Contributing
 
 Contributions to SceneBuilder are welcome! If you have suggestions for improvements or new features, feel free to create an issue or pull request on our GitHub repository.
+
```

