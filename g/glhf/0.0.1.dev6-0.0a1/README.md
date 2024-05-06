# Comparing `tmp/glhf-0.0.1.dev6.tar.gz` & `tmp/glhf-0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glhf-0.0.1.dev6.tar", last modified: Mon May  6 04:19:11 2024, max compression
+gzip compressed data, was "glhf-0.0a1.tar", last modified: Sat Mar 16 16:21:46 2024, max compression
```

## Comparing `glhf-0.0.1.dev6.tar` & `glhf-0.0a1.tar`

### file list

```diff
@@ -1,35 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.987130 glhf-0.0.1.dev6/
--rw-rw-rw-   0        0        0    18429 2024-03-16 14:03:23.000000 glhf-0.0.1.dev6/LICENSE
--rw-rw-rw-   0        0        0    22768 2024-05-06 04:19:11.987130 glhf-0.0.1.dev6/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-03-16 14:08:37.000000 glhf-0.0.1.dev6/README.md
--rw-rw-rw-   0        0        0     1006 2024-05-06 04:14:44.000000 glhf-0.0.1.dev6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 04:19:11.987130 glhf-0.0.1.dev6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.706812 glhf-0.0.1.dev6/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.758596 glhf-0.0.1.dev6/src/glhf/
--rw-rw-rw-   0        0        0      113 2024-03-18 16:20:13.000000 glhf-0.0.1.dev6/src/glhf/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-06 06:49:20.000000 glhf-0.0.1.dev6/src/glhf/__main__.py
--rw-rw-rw-   0        0        0     5214 2024-04-16 14:36:44.000000 glhf-0.0.1.dev6/src/glhf/base.py
--rw-rw-rw-   0        0        0     2615 2024-04-14 15:16:12.000000 glhf-0.0.1.dev6/src/glhf/bot.py
--rw-rw-rw-   0        0        0     5125 2024-04-14 15:21:13.000000 glhf-0.0.1.dev6/src/glhf/cli.py
--rw-rw-rw-   0        0        0    13093 2024-05-06 04:12:46.000000 glhf-0.0.1.dev6/src/glhf/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.877129 glhf-0.0.1.dev6/src/glhf/resource/
--rw-rw-rw-   0        0        0    78596 2023-09-14 22:27:18.000000 glhf-0.0.1.dev6/src/glhf/resource/Quicksand-Bold.ttf
--rw-rw-rw-   0        0        0     1813 2024-01-17 15:21:51.000000 glhf-0.0.1.dev6/src/glhf/resource/city.png
--rw-rw-rw-   0        0        0     2121 2024-01-17 15:22:12.000000 glhf-0.0.1.dev6/src/glhf/resource/crown.png
--rw-rw-rw-   0        0        0     1789 2024-01-17 15:21:15.000000 glhf-0.0.1.dev6/src/glhf/resource/mountain.png
--rw-rw-rw-   0        0        0     1252 2024-01-17 15:22:35.000000 glhf-0.0.1.dev6/src/glhf/resource/obstacle.png
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.926481 glhf-0.0.1.dev6/src/glhf/server/
--rw-rw-rw-   0        0        0      127 2024-04-10 05:20:11.000000 glhf-0.0.1.dev6/src/glhf/server/__init__.py
--rw-rw-rw-   0        0        0    16423 2024-04-10 05:37:46.000000 glhf-0.0.1.dev6/src/glhf/server/_local.py
--rw-rw-rw-   0        0        0     4238 2024-04-10 05:20:11.000000 glhf-0.0.1.dev6/src/glhf/server/_socketio.py
--rw-rw-rw-   0        0        0     1039 2024-04-10 05:20:11.000000 glhf-0.0.1.dev6/src/glhf/typing.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.975786 glhf-0.0.1.dev6/src/glhf/utils/
--rw-rw-rw-   0        0        0        0 2024-04-10 05:20:11.000000 glhf-0.0.1.dev6/src/glhf/utils/__init__.py
--rw-rw-rw-   0        0        0     2212 2024-04-10 05:20:11.000000 glhf-0.0.1.dev6/src/glhf/utils/map.py
--rw-rw-rw-   0        0        0     8331 2024-04-10 05:20:11.000000 glhf-0.0.1.dev6/src/glhf/utils/method.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:19:11.979793 glhf-0.0.1.dev6/src/glhf.egg-info/
--rw-rw-rw-   0        0        0    22768 2024-05-06 04:19:11.000000 glhf-0.0.1.dev6/src/glhf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-05-06 04:19:11.000000 glhf-0.0.1.dev6/src/glhf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:19:11.000000 glhf-0.0.1.dev6/src/glhf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-05-06 04:19:11.000000 glhf-0.0.1.dev6/src/glhf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 04:19:11.000000 glhf-0.0.1.dev6/src/glhf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-16 16:21:46.961485 glhf-0.0a1/
+-rw-rw-rw-   0        0        0    18429 2024-03-16 14:03:23.000000 glhf-0.0a1/LICENSE
+-rw-rw-rw-   0        0        0    22690 2024-03-16 16:21:46.946765 glhf-0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-16 14:08:37.000000 glhf-0.0a1/README.md
+drwxrwxrwx   0        0        0        0 2024-03-16 16:21:46.883462 glhf-0.0a1/glhf/
+-rw-rw-rw-   0        0        0      113 2024-03-16 14:56:01.000000 glhf-0.0a1/glhf/__init__.py
+-rw-rw-rw-   0        0        0     5436 2024-03-16 12:58:47.000000 glhf-0.0a1/glhf/base.py
+-rw-rw-rw-   0        0        0     9450 2024-03-16 14:55:30.000000 glhf-0.0a1/glhf/bot.py
+-rw-rw-rw-   0        0        0     7751 2024-03-16 13:03:33.000000 glhf-0.0a1/glhf/client.py
+-rw-rw-rw-   0        0        0    12152 2024-03-15 14:56:03.000000 glhf-0.0a1/glhf/gui.py
+-rw-rw-rw-   0        0        0     8872 2024-03-16 13:25:48.000000 glhf-0.0a1/glhf/helper.py
+-rw-rw-rw-   0        0        0    13990 2024-03-16 13:14:52.000000 glhf-0.0a1/glhf/server.py
+-rw-rw-rw-   0        0        0     1019 2024-02-20 08:32:19.000000 glhf-0.0a1/glhf/typing_.py
+drwxrwxrwx   0        0        0        0 2024-03-16 16:21:46.935977 glhf-0.0a1/glhf.egg-info/
+-rw-rw-rw-   0        0        0    22690 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      889 2024-03-16 14:46:16.000000 glhf-0.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-16 16:21:46.961485 glhf-0.0a1/setup.cfg
```

### Comparing `glhf-0.0.1.dev6/LICENSE` & `glhf-0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `glhf-0.0.1.dev6/PKG-INFO` & `glhf-0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhf
-Version: 0.0.1.dev6
+Version: 0.0a1
 Summary: Good luck, have fun! A generals.io bot framework.
 Author-email: Hong-Chang Huang <seer852741@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -349,19 +349,17 @@
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame-ce==2.4.1
-Requires-Dist: python-socketio[asyncio_client]==5.11.1
+Requires-Dist: python-socketio==5.11.1
 Requires-Dist: ortools==9.9.3963
 Requires-Dist: igraph==0.11.4
-Requires-Dist: fire==0.6.0
-Requires-Dist: rich==13.7.1
 
 # GLHF | Generals.io Bot Framework
 
 :warning: **NOTE: This is a template README and the code is still a work in progress.**
 
 Short description of the repository.
```

### Comparing `glhf-0.0.1.dev6/README.md` & `glhf-0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `glhf-0.0.1.dev6/pyproject.toml` & `glhf-0.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [build-system]
 requires = ["setuptools>=69.1.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glhf"
-version = "0.0.1.dev6"
+version = "0.0a1"
 dependencies = [
   "pygame-ce==2.4.1",
-  "python-socketio[asyncio_client]==5.11.1",
+  "python-socketio==5.11.1",
   "ortools==9.9.3963",
   "igraph==0.11.4",
-  "fire==0.6.0",
-  "rich==13.7.1",
 ]
 requires-python = ">= 3.12"
 authors = [{ name = "Hong-Chang Huang", email = "seer852741@gmail.com" }]
 description = "Good luck, have fun! A generals.io bot framework."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
@@ -23,10 +21,7 @@
   "Development Status :: 2 - Pre-Alpha",
   "Topic :: Software Development :: Libraries",
   "Topic :: Games/Entertainment :: Real Time Strategy",
   "Topic :: Games/Entertainment :: Simulation",
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Programming Language :: Python :: 3.12",
 ]
-
-[tool.setuptools.package-data]
-"glhf.resource" = ["*"]
```

### Comparing `glhf-0.0.1.dev6/src/glhf/gui.py` & `glhf-0.0a1/glhf/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-from __future__ import annotations
-
 from functools import lru_cache
 from itertools import product
-from multiprocessing import Process, Queue
 from os import PathLike
-from pathlib import Path
-from queue import Empty
-import time
-from typing import IO, Any, Generator, Protocol, Self, Sequence
+from threading import Event, Thread
+from typing import IO, Sequence
 
 import pygame
-import pygame.font
+from pygame import (
+    Color,
+    Rect,
+    Surface,
+    Vector2,
+    display,
+    draw,
+    event,
+    font,
+    image,
+    mouse,
+    sprite,
+    time,
+    transform,
+)
+
+from glhf.helper import event_method, patch, queue_method
+from glhf.typing_ import GameUpdateDict
 
-from glhf.typing import GameStartDict, GameUpdateDict
-from glhf.utils.map import patch
+__all__ = ("PygameGUI",)
 
 type AnyPath = str | bytes | PathLike[str] | PathLike[bytes]
 type FileArg = AnyPath | IO[bytes] | IO[str]
 type Coordinate = Sequence[float]
 
-RESDIR = Path(__file__).parent / "resource"
 PALETTE = (
     0x222222FF,
     0x393939FF,
     0x808080FF,
     0xBBBBBBFF,
     0xDCDCDCFF,
     0xFF0000FF,
@@ -35,38 +45,39 @@
     0x800080FF,
     0x800000FF,
     0xB09F30FF,
     0x9A6324FF,
     0x0000FFFF,
     0x483D8BFF,
 )
-PALETTE = tuple(map(pygame.Color, PALETTE))
-WHITE = pygame.Color("white")
-BLACK = pygame.Color("black")
-# ARROWS = "↑↓←→"
+PALETTE = tuple(map(Color, PALETTE))
+ARROWS = "↑↓←→"
+WHITE = Color("white")
+BLACK = Color("black")
 
 
 class CachedResource:
     __slots__ = "font_", "city", "crown", "mountain", "obstacle"
 
     def __init__(
         self,
-        font_: FileArg = RESDIR / "Quicksand-Bold.ttf",
-        city: FileArg = RESDIR / "city.png",
-        crown: FileArg = RESDIR / "crown.png",
-        mountain: FileArg = RESDIR / "mountain.png",
-        obstacle: FileArg = RESDIR / "obstacle.png",
+        font_: FileArg = "glhf/resource/Quicksand-Bold.ttf",
+        city: FileArg = "glhf/resource/city.png",
+        crown: FileArg = "glhf/resource/crown.png",
+        mountain: FileArg = "glhf/resource/mountain.png",
+        obstacle: FileArg = "glhf/resource/obstacle.png",
     ) -> None:
         self.font_ = font_
-        self.city = pygame.image.load(city).convert_alpha()
-        self.crown = pygame.image.load(crown).convert_alpha()
-        self.mountain = pygame.image.load(mountain).convert_alpha()
-        self.obstacle = pygame.image.load(obstacle).convert_alpha()
+        load = image.load
+        self.city = load(city).convert_alpha()
+        self.crown = load(crown).convert_alpha()
+        self.mountain = load(mountain).convert_alpha()
+        self.obstacle = load(obstacle).convert_alpha()
 
-    def render_cell(self, size: int, terrain: int, army: int) -> pygame.Surface:
+    def render_cell(self, size: int, terrain: int, army: int) -> Surface:
         """
         Render the terrain without army.
 
         Args:
             size (int): The size of the cell.
             terrain (int): The terrain value.
 
@@ -89,37 +100,37 @@
 
         """
         if army and terrain >= 0:
             return self.render_terrain_army(size, terrain, army)
         return self.render_terrain(size, terrain)
 
     @lru_cache(256)
-    def render_terrain_army(self, size: int, terrain: int, army: int) -> pygame.Surface:
+    def render_terrain_army(self, size: int, terrain: int, army: int) -> Surface:
         cell = self.render_terrain(size, terrain).copy()
         cell.blit(*self.render_army(size, army))
         return cell
 
     @lru_cache(16)
-    def get_font(self, size: int) -> pygame.font.Font:
-        return pygame.font.Font(self.font_, round((size - 12) ** 0.5) + 10)
+    def get_font(self, size: int) -> font.Font:
+        return font.Font(self.font_, round((size - 12) ** 0.5) + 10)
 
     @lru_cache(512)
-    def render_army(self, size: int, army: int) -> tuple[pygame.Surface, pygame.Rect]:
+    def render_army(self, size: int, army: int) -> tuple[Surface, Rect]:
         s = str(army)
         render = self.get_font(size).render
         text = render(s, True, WHITE)
         shadow = render(s, True, BLACK)
-        surf = pygame.transform.box_blur(shadow, 2)
+        surf = transform.box_blur(shadow, 2)
         surf.blit(text, (0, 0))
         m = size // 2
         rect = surf.get_rect(center=(m, m))
         return surf, rect
 
     @lru_cache(256)
-    def render_terrain(self, size: int, terrain: int) -> pygame.Surface:
+    def render_terrain(self, size: int, terrain: int) -> Surface:
         if terrain < 0:
             if terrain < -2:
                 cell = self.render_index(size, 1)
                 if terrain == -4:
                     cell.blit(*self.render_image(size, self.obstacle))
             elif terrain < -1:
                 cell = self.render_index(size, 3)
@@ -136,102 +147,100 @@
         else:
             cell = self.render_index(size, 2)
             if terrain == 37:
                 cell.blit(*self.render_image(size, self.city))
         return cell
 
     @classmethod
-    def render_index(cls, size: int, index: int) -> pygame.Surface:
-        cell = pygame.Surface((size, size))
+    def render_index(cls, size: int, index: int) -> Surface:
+        cell = Surface((size, size))
         if index == 1:
             cell.fill(PALETTE[1])
         else:
             s = size - 1
-            pygame.draw.rect(cell, PALETTE[index], (1, 1, s, s))
-            pygame.draw.rect(cell, BLACK, (0, 0, size, size), 1)
+            draw.rect(cell, PALETTE[index], (1, 1, s, s))
+            draw.rect(cell, BLACK, (0, 0, size, size), 1)
         return cell
 
     @classmethod
-    def render_image(
-        cls, size: int, image: pygame.Surface
-    ) -> tuple[pygame.Surface, pygame.Rect]:
+    def render_image(cls, size: int, image: Surface) -> tuple[Surface, Rect]:
         s = size * 25 // 32
         m = size // 2
-        surf = pygame.transform.smoothscale(image, (s, s))
+        surf = transform.smoothscale(image, (s, s))
         rect = surf.get_rect(center=(m, m))
         return surf, rect
 
     @classmethod
     def all_cache_info(cls):
         return {
             "font": cls.get_font.cache_info(),
             "army": cls.render_army.cache_info(),
             "terrain": cls.render_terrain.cache_info(),
             "all": cls.render_terrain_army.cache_info(),
         }
 
 
-class BackgroundSprite(pygame.sprite.DirtySprite):
+class BackgroundSprite(sprite.DirtySprite):
     def __init__(self, *group) -> None:
         super().__init__(*group)
-        self.image = pygame.Surface((0, 0))
+        self.image = Surface((0, 0))
         self.rect = self.image.get_rect()
         self.layer = 0
 
     def fast_update(
         self,
         window_resize: bool,
         window_size: tuple[int, int] | None = None,
     ) -> None:
-        assert isinstance(self.rect, pygame.Rect)
+        assert isinstance(self.rect, Rect)
         if window_resize:
-            window_size = window_size or pygame.display.get_window_size()
-            self.image = pygame.Surface(window_size)
+            window_size = window_size or display.get_window_size()
+            self.image = Surface(window_size)
             self.rect.size = window_size
             self.image.fill(PALETTE[0])
             self.dirty = 1
 
 
-class MapSprite(pygame.sprite.DirtySprite):
+class MapSprite(sprite.DirtySprite):
     # image: Surface
     # rect: Rect
 
     def __init__(
         self,
         *groups,
         window_size: tuple[int, int] | None = None,
     ) -> None:
         super().__init__(*groups)
-        x, y = window_size or pygame.display.get_window_size()
+        x, y = window_size or display.get_window_size()
         self.zoom = 3
         self.cell_size = 12
-        self.center = pygame.Vector2(x // 2, y // 2)
-        self.image = pygame.Surface((0, 0))
+        self.center = Vector2(x // 2, y // 2)
+        self.image = Surface((0, 0))
         self.rect = self.image.get_rect(center=self.center)
         self.data = None
         self.layer = 1
         self.resource = CachedResource()
 
         self.map_: list[int] = [0, 0]
         self.cities: list[int] = []
 
         # self._turn = 0
 
     @lru_cache(16)
-    def get_image(self, size: tuple[int, int]) -> pygame.Surface:
-        return pygame.Surface(size)
+    def get_image(self, size: tuple[int, int]) -> Surface:
+        return Surface(size)
 
     def fast_update(
         self,
         zoom: int,
-        move: tuple[float, float] | pygame.Vector2,
+        move: tuple[float, float] | Vector2,
         data: GameUpdateDict | None,
     ) -> None:
-        assert isinstance(self.rect, pygame.Rect)
-        assert isinstance(self.image, pygame.Surface)
+        assert isinstance(self.rect, Rect)
+        assert isinstance(self.image, Surface)
 
         skip = True
         resize = False
 
         if data:
             # if self._turn + 1 < data.turn:
             #     print(f"missing turn {self._turn + 1} to {data.turn - 1}")
@@ -249,15 +258,15 @@
         if not self.data:
             return
 
         if zoom and self.zoom != (z := max(0, min(self.zoom + zoom, 15))):
             skip = False
             resize = True
             s = 12 + z * z
-            p = pygame.mouse.get_pos()
+            p = mouse.get_pos()
             c = self.center
             c -= p
             c *= s / self.cell_size
             c += p
             self.zoom = z
             self.cell_size = s
 
@@ -298,15 +307,15 @@
                 elif armies[i]:
                     terrain[i] = 37
 
             for i in data["generals"]:
                 if i >= 0 and terrain[i] >= 0:
                     terrain[i] += 24
 
-            rr = self.rect.clip((0, 0), pygame.display.get_window_size())
+            rr = self.rect.clip((0, 0), display.get_window_size())
             x, y = self.rect.topleft
             rr.move_ip(-x, -y)
 
             left = rr.left - self.cell_size
             right = rr.right
             top = rr.top - self.cell_size
             bottom = rr.bottom
@@ -318,121 +327,89 @@
                     t = 36
                 surf = res.render_cell(c_size, t, a)
                 img.blit(surf, (x, y))
 
         self.dirty = 1
 
 
-class State(Protocol):
-    def __call__(self, window: pygame.Surface, queue: Queue[Any]) -> Self | None: ...
-
-
-class PygameGUI:
-    def __init__(self) -> None:
-        self.queue: Queue[Any] = Queue()
-        self.process = Process(target=main, args=(self.queue,))
-
-    def game_start(self, data: GameStartDict) -> None:
-        self.queue.put(("game_start", data))
-
-    def game_update(self, data: GameUpdateDict) -> None:
-        self.queue.put(("game_update", data))
-
-    def game_over(self) -> None:
-        self.queue.put(("game_over", None))
-
-    def connect(self) -> None:
-        self.process.start()
-        time.sleep(2)
+class PygameGUI(Thread):
+    WINDOWSIZE = 800, 600
 
-    def disconnect(self) -> None:
-        self.queue.put(None)
-        self.process.join()
+    game_update = queue_method()
+    game_start = event_method()
+    game_over = event_method()
 
+    def __init__(self, **kwargs) -> None:
+        super().__init__(name=f"{type(self).__name__}({id(self):X})", **kwargs)
+        self.quit = Event()
 
-def get_stream[T](queue: Queue[T]) -> Generator[Any, Any, T | None]:
-    while True:
-        try:
-            yield queue.get_nowait()
-        except Empty:
-            return
+    def __enter__(self) -> None:
+        self.start()
 
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        if exc_type is None:
+            self.quit.wait()
+        self.join()
 
-def get_data[T](queue: Queue[T], event: str = "") -> T | None:
-    try:
-        return queue.get_nowait()
-    except Empty:
-        return
-
-
-def state_game(window: pygame.Surface, queue: Queue[Any]) -> State | None:
-    clock = pygame.time.Clock()
-
-    bg = BackgroundSprite()
-    bg.fast_update(True)
-    map_ = MapSprite()
-
-    group = pygame.sprite.LayeredDirty(bg, map_)
-    rects = group.draw(window)
-    pygame.display.update(rects)
-
-    move = pygame.Vector2()
-
-    while True:
-        window_resize = False
-        zoom = 0
-        move.update()
-
-        for e in pygame.event.get():
-            if e.type == pygame.QUIT:
-                return
-            elif e.type == pygame.WINDOWSIZECHANGED:
-                window_resize = True
-            elif e.type == pygame.MOUSEWHEEL:
-                zoom += e.x + e.y
-            elif e.type == pygame.MOUSEMOTION:
-                if e.buttons[0] == 1:
-                    move += e.rel
-
-        data = get_data(queue)
-        if data is not None:
-            if data[0] == "game_update":
-                data = data[1]
-            else:
-                data = None
+    def main(self, window: Surface) -> None:
+        clock = time.Clock()
 
-        bg.fast_update(window_resize)
-        map_.fast_update(zoom, move, data)
+        bg = BackgroundSprite()
+        bg.fast_update(True)
+        map_ = MapSprite()
 
+        group = sprite.LayeredDirty(bg, map_)
         rects = group.draw(window)
-        if rects:
-            pygame.display.update(rects)
-
-        clock.tick(60)
-
+        display.update(rects)
 
-def state_lobby(window: pygame.Surface, queue: Queue[Any]) -> State | None:
-    while True:
-        for e in pygame.event.get():
-            if e.type == pygame.QUIT:
-                return
+        move = Vector2()
 
-            match get_data(queue):
-                case None:
-                    continue
-                case ("game_start", _data):
-                    return state_game
+        while not self.quit.is_set():
+            window_resize = False
+            zoom = 0
+            move.update()
+
+            for e in event.get():
+                if e.type == pygame.QUIT:
+                    self.quit.set()
+                elif e.type == pygame.WINDOWSIZECHANGED:
+                    window_resize = True
+                elif e.type == pygame.MOUSEWHEEL:
+                    zoom += e.x + e.y
+                elif e.type == pygame.MOUSEMOTION:
+                    if e.buttons[0] == 1:
+                        move += e.rel
+
+            bg.fast_update(window_resize)
+            map_.fast_update(zoom, move, self.game_update.get())
+
+            rects = group.draw(window)
+            if rects:
+                pygame.display.update(rects)
+
+            clock.tick(60)
+            # print(f"\r{clock.get_fps():0>7.1f}", end="")
+
+    def run(self) -> None:
+        pygame.init()
+        # pygame.RESIZABLE | pygame.SCALED
+        quit = self.quit
+        game_start = self.game_start
+        try:
+            window = display.set_mode(self.WINDOWSIZE)
+            while not quit.is_set():
+                for e in event.get():
+                    if e.type == pygame.QUIT:
+                        return
+                if game_start.wait():
+                    self.main(window)
+        finally:
+            pygame.quit()
+            quit.set()
 
 
-def main(queue: Queue[Any]) -> None:
-    pygame.init()
-    window = pygame.display.set_mode((800, 600))
-    state: State | None = state_lobby
-    while state is not None:
-        state = state(window, queue)
-    pygame.quit()
+if __name__ == "__main__":
 
+    def main() -> None:
+        pass
 
-if __name__ == "__main__":
-    gui = PygameGUI()
-    gui.connect()
-    gui.disconnect()
+    main()
```

### Comparing `glhf-0.0.1.dev6/src/glhf/typing.py` & `glhf-0.0a1/glhf/typing_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, NamedTuple, TypedDict
+from typing import Literal, TypedDict, NamedTuple, Any
 
 __all__ = "QueueUpdateDict", "GameStartDict", "GameUpdateDict", "GameUpdateTuple"
 
 
 class QueueUpdateDict(TypedDict):
     playerIndices: list[int]
     playerColors: list[int]
@@ -19,17 +19,17 @@
     playerIndex: int
     playerColors: list[int]
     replay_id: str
     chat_room: str
     usernames: list[str]
     teams: list[int]
     game_type: Literal["ffa", "1v1", "custom"]
-    swamps: list[Any]
-    lights: list[Any]
-    options: dict[str, Any]
+    swamps: list
+    lights: list
+    options: list
 
 
 class GameUpdateDict(TypedDict):
     scores: list[dict]
     turn: int
     stars: list[int]
     attackIndex: int
```

### Comparing `glhf-0.0.1.dev6/src/glhf/utils/method.py` & `glhf-0.0a1/glhf/helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,332 +1,361 @@
-from asyncio import Event as AEvent
-from asyncio import Queue as AQueue
-from asyncio import QueueEmpty, Task, create_task
+from __future__ import annotations
+
+from asyncio import Event as _AsyncioEvent
+from asyncio import Queue as _AsyncioQueue
+from asyncio import Task, create_task
+from collections import deque
 from functools import partial, update_wrapper, wraps
-from queue import Empty, Queue
-from threading import Event
 from typing import Any, Callable, Concatenate, Coroutine, Protocol, Self, overload
 
 __all__ = (
-    "methodlike",
-    "streamify",
-    "signalize",
-    "astreamify",
-    "asignalize",
-    "to_coro",
+    "patch",
+    "make_diff",
     "to_task",
+    "to_coro",
+    "asyncio_queueify",
+    "asyncio_eventify",
+    "queue_method",
+    "event_method",
 )
 
 
-# ============================================================
-# typing
-# ============================================================
+def coord_to_name(coord: tuple[int, int]) -> str:
+    """Converts a coordinate to a string representation."""
+    return f"{coord[0]},{coord[1]}"
+
+
+def coord_to_index(coord: tuple[int, int], col: int) -> int:
+    """Converts a coordinate to an index in a 1D list representation."""
+    return coord[0] * col + coord[1]
+
+
+def patch(old: list[int], diff: list[int]) -> list[int]:
+    new = []
+    i = 0
+    len_diff = len(diff)
+    while i < len_diff:
+        n = diff[i]
+        if n:
+            j = len(new)
+            new += old[j : j + n]
+        i += 1
+        if i == len_diff:
+            break
+        n = diff[i]
+        if n:
+            j = i + 1
+            new += diff[j : j + n]
+            i += n
+        i += 1
+    return new
+
+
+def make_diff(new: list[int], old: list[int]) -> list[int]:
+    diff = []
+    i = 0
+    j = 0
+    len_new = len(new)
+    len_old = len(old)
+    len_min = min(len_new, len_old)
+    while True:
+        while j < len_min and new[j] == old[j]:
+            j += 1
+        diff.append(j - i)
+        i = j
+        if j == len_min:
+            if len_new > len_old:
+                diff.append(len_new - len_old)
+                diff += new[len_old:]
+            break
+        while j < len_min and new[j] != old[j]:
+            j += 1
+        if j < len_min:
+            diff.append(j - i)
+            diff += new[i:j]
+            i = j
+        else:
+            diff.append(len_new - i)
+            diff += new[i:len_new]
+            break
+    return diff
+
+
+def to_task[**P, R](
+    wrapped: Callable[P, Coroutine[Any, Any, R]],
+) -> Callable[P, Task[R]]:
+    @wraps(wrapped)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Task[R]:
+        return create_task(wrapped(*args, **kwargs))
+
+    return wrapper
+
+
+def to_coro[**P, R](wrapped: Callable[P, R]) -> Callable[P, Coroutine[Any, Any, R]]:
+    @wraps(wrapped)
+    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+        return wrapped(*args, **kwargs)
+
+    return wrapper
+
 
-type _MethodType[T, **P, R] = Callable[Concatenate[T, P], R]
+type MethodType[T, **P, R] = Callable[Concatenate[T, P], R]
 
 
-class _MethodLike[T, **P, R](Protocol):
+class MethodLikeProtocol[T, **P, R](Protocol):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
         /,
-    ) -> _MethodType[T, P, R]: ...
+    ) -> MethodType[T, P, R]: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
         /,
     ) -> Callable[P, R]: ...
 
 
-class _MethodDescriptor[T, **P, R](_MethodLike[T, P, R]):
-    def __set_name__(self, owner: type[T], name: str) -> None:
-        self.name = "_" + name
-
-    def __init__(self, wrapped: _MethodType[T, P, R]) -> None:
-        self.wrapped = wrapped
+def methodlike[T, **P, R](m: MethodType[T, P, R]) -> MethodLikeProtocol[T, P, R]:
+    return m
 
 
-def methodlike[T, **P, R](m: _MethodType[T, P, R]) -> _MethodLike[T, P, R]:
-    return m
+class MethodLike[T, **P, R](MethodLikeProtocol[T, P, R]):
+    def __set_name__(self, owner: type[T], name: str) -> None:
+        self.name = "_" + name
 
 
-# ============================================================
-# synchronous
-# ============================================================
+class _wrappedmethod[T, **P, R](MethodLike[T, P, R]):
+    def __init__(self, wrapped: MethodType[T, P, R]) -> None:
+        self.wrapped = wrapped
 
 
-class _Stream[**P, R]:
+class AsyncioQueue[**P, R](_AsyncioQueue[R | None]):
     __wrapped__: Callable[P, R]
 
     def __init__(self, wrapped: Callable[P, R]) -> None:
+        super().__init__()
         update_wrapper(self, wrapped)
-        self._queue: Queue[R | None] = Queue()
+        self._tasks: set[Task] = set()
+        self._close = _AsyncioEvent()
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
         item = self.__wrapped__(*args, **kwargs)
-        self._queue.put_nowait(item)
+        task = create_task(self.put(item))
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.remove)
         return item
 
-    def __iter__(self) -> Self:
+    def __aiter__(self) -> Self:
         return self
 
-    def __next__(self) -> R:
-        q = self._queue
-        item = q.get()
-        q.task_done()
+    async def __anext__(self) -> R:
+        item = await self.get()
+        self.task_done()
         if item is None:
-            raise StopIteration()
-        return item
-
-    def wait(self) -> R | None:
-        q = self._queue
-        item = q.get()
-        q.task_done()
+            raise StopAsyncIteration()
         return item
 
-    def get(self) -> R | None:
-        q = self._queue
-        try:
-            item = q.get_nowait()
-        except Empty:
-            return None
-        else:
-            q.task_done()
-            return item
-
-    def close(self) -> None:
-        self._queue.put_nowait(None)
+    def close(self) -> Task[None]:
+        return create_task(self.put(None))
 
 
-class _Signal[**P, R]:
-    __wrapped__: Callable[P, R]
-
-    def __init__(self, wrapped: Callable[P, R]) -> None:
-        update_wrapper(self, wrapped)
-        self.event = Event()
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        self.event.set()
-        return self.__wrapped__(*args, **kwargs)
-
-    def get(self) -> bool:
-        s = self.event.is_set()
-        if s:
-            self.event.clear()
-        return s
-
-    def wait(self) -> None:
-        self.event.wait()
-        self.event.clear()
-
-
-class streamify[T, **P, R](_MethodDescriptor[T, P, R]):
+class asyncio_queueify[T, **P, R](_wrappedmethod[T, P, R]):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> MethodType[T, P, R]: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _Stream[P, R]: ...
+    ) -> AsyncioQueue[P, R]: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
             return self.wrapped
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _Stream(partial(self.wrapped, instance))
+            x = AsyncioQueue(partial(self.wrapped, instance))
             setattr(instance, self.name, x)
         return x
 
 
-class signalize[T, **P, R](_MethodDescriptor[T, P, R]):
+class AsyncioEvent[**P, R](_AsyncioEvent):
+    __wrapped__: Callable[P, R]
+
+    def __init__(self, wrapped: Callable[P, R]) -> None:
+        super().__init__()
+        update_wrapper(self, wrapped)
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
+        res = self.__wrapped__(*args, **kwargs)
+        self.set()
+        return res
+
+
+class asyncio_eventify[T, **P, R](_wrappedmethod[T, P, R]):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> MethodType[T, P, R]: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _Signal[P, R]: ...
+    ) -> AsyncioEvent[P, R]: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
             return self.wrapped
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _Signal(partial(self.wrapped, instance))
+            x = AsyncioEvent(partial(self.wrapped, instance))
             setattr(instance, self.name, x)
         return x
 
 
-# ============================================================
-# asynchronous
-# ============================================================
-
-
-class _AStream[**P, R]:
-    __wrapped__: Callable[P, R]
-
-    def __init__(self, wrapped: Callable[P, R]) -> None:
-        update_wrapper(self, wrapped)
-        self._queue: AQueue[R | None] = AQueue()
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        item = self.__wrapped__(*args, **kwargs)
-        self._queue.put_nowait(item)
-        return item
-
-    def __aiter__(self) -> Self:
-        return self
-
-    async def __anext__(self) -> R:
-        q = self._queue
-        item = await q.get()
-        q.task_done()
-        if item is None:
-            raise StopAsyncIteration()
-        return item
-
-    async def wait(self) -> R | None:
-        q = self._queue
-        item = await q.get()
-        q.task_done()
+class _Queue[R](deque[R]):
+    def __call__(self, item: R) -> R:
+        self.append(item)
         return item
 
     def get(self) -> R | None:
-        q = self._queue
         try:
-            item = q.get_nowait()
-        except QueueEmpty:
+            return self.popleft()
+        except IndexError:
             return None
-        else:
-            q.task_done()
-            return item
-
-    def close(self) -> None:
-        self._queue.put_nowait(None)
-
-
-class _ASignal[**P, R]:
-    __wrapped__: Callable[P, R]
 
-    def __init__(self, wrapped: Callable[P, R]) -> None:
-        update_wrapper(self, wrapped)
-        self.event = AEvent()
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        self.event.set()
-        return self.__wrapped__(*args, **kwargs)
 
-    def get(self) -> bool:
-        s = self.event.is_set()
-        if s:
-            self.event.clear()
-        return s
+class queue_method[T, R](MethodLike[T, [R], R]):
+    def __call__(self, instance: T, item: R) -> R:
+        return self.__get__(instance)(item)
 
-    async def wait(self) -> None:
-        await self.event.wait()
-        self.event.clear()
-
-
-class astreamify[T, **P, R](_MethodDescriptor[T, P, R]):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> Self: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _AStream[P, R]: ...
+    ) -> _Queue[R]: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
-            return self.wrapped
+            return self
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _AStream(partial(self.wrapped, instance))
+            x = _Queue()
             setattr(instance, self.name, x)
         return x
 
 
-class asignalize[T, **P, R](_MethodDescriptor[T, P, R]):
+class _Event:
+    def __init__(self) -> None:
+        self._set = False
+
+    def __call__(self) -> None:
+        self.set()
+
+    def set(self) -> None:
+        self._set = True
+
+    def clear(self) -> None:
+        self._set = False
+
+    def wait(self) -> bool:
+        x = self._set
+        if self._set:
+            self.clear()
+        return x
+
+
+class event_method[T](MethodLike[T, [], None]):
+    def __call__(self, instance: T) -> None:
+        return self.__get__(instance)()
+
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> Self: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _ASignal[P, R]: ...
+    ) -> _Event: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
-            return self.wrapped
+            return self
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _ASignal(partial(self.wrapped, instance))
+            x = _Event()
             setattr(instance, self.name, x)
         return x
 
 
-def to_coro[**P, R](wrapped: Callable[P, R]) -> Callable[P, Coroutine[Any, Any, R]]:
-    @wraps(wrapped)
-    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
-        return wrapped(*args, **kwargs)
-
-    return wrapper
-
-
-def to_task[**P, R](
-    wrapped: Callable[P, Coroutine[Any, Any, R]],
-) -> Callable[P, Task[R]]:
-    @wraps(wrapped)
-    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Task[R]:
-        return create_task(wrapped(*args, **kwargs))
-
-    return wrapper
+class Map(list[int]):
+    @property
+    def shape(self) -> list[int]:
+        return self[:2:-1]
+
+    @property
+    def armies(self) -> list[list[int]]:
+        m = self
+        c, r = m[:2]
+        stop = 2 + c * r
+        return [m[i : i + r] for i in range(2, stop, r)]
+
+    @property
+    def terrain(self) -> list[list[int]]:
+        m = self
+        c, r = m[:2]
+        n = c * r
+        start = 2 + n
+        return [m[i : i + r] for i in range(start, start + n, r)]
+
+
+class Cities(list[int]):
+    @property
+    def cities(self) -> list[int]:
+        return self.copy()
```

### Comparing `glhf-0.0.1.dev6/src/glhf.egg-info/PKG-INFO` & `glhf-0.0a1/glhf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhf
-Version: 0.0.1.dev6
+Version: 0.0a1
 Summary: Good luck, have fun! A generals.io bot framework.
 Author-email: Hong-Chang Huang <seer852741@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -349,19 +349,17 @@
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame-ce==2.4.1
-Requires-Dist: python-socketio[asyncio_client]==5.11.1
+Requires-Dist: python-socketio==5.11.1
 Requires-Dist: ortools==9.9.3963
 Requires-Dist: igraph==0.11.4
-Requires-Dist: fire==0.6.0
-Requires-Dist: rich==13.7.1
 
 # GLHF | Generals.io Bot Framework
 
 :warning: **NOTE: This is a template README and the code is still a work in progress.**
 
 Short description of the repository.
```

