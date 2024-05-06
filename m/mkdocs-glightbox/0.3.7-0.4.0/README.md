# Comparing `tmp/mkdocs-glightbox-0.3.7.tar.gz` & `tmp/mkdocs-glightbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-glightbox-0.3.7.tar", last modified: Wed Jan 24 15:16:44 2024, max compression
+gzip compressed data, was "mkdocs-glightbox-0.4.0.tar", last modified: Mon May  6 14:31:39 2024, max compression
```

## Comparing `mkdocs-glightbox-0.3.7.tar` & `mkdocs-glightbox-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-01-24 15:16:44.293160 mkdocs-glightbox-0.3.7/
--rw-r--r--   0 blueswen   (501) staff       (20)     1065 2022-06-10 06:58:58.000000 mkdocs-glightbox-0.3.7/LICENSE
--rw-r--r--   0 blueswen   (501) staff       (20)       37 2022-07-15 16:30:44.000000 mkdocs-glightbox-0.3.7/MANIFEST.in
--rw-r--r--   0 blueswen   (501) staff       (20)     4879 2024-01-24 15:16:44.293024 mkdocs-glightbox-0.3.7/PKG-INFO
--rw-r--r--   0 blueswen   (501) staff       (20)     4453 2024-01-24 15:07:40.000000 mkdocs-glightbox-0.3.7/README.md
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-01-24 15:16:44.290205 mkdocs-glightbox-0.3.7/mkdocs_glightbox/
--rw-r--r--   0 blueswen   (501) staff       (20)        0 2022-06-12 06:19:32.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/__init__.py
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-01-24 15:16:44.291514 mkdocs-glightbox-0.3.7/mkdocs_glightbox/__pycache__/
--rw-r--r--   0 blueswen   (501) staff       (20)      165 2022-11-15 14:31:20.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 blueswen   (501) staff       (20)     7177 2024-01-24 14:50:51.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-01-24 15:16:44.292755 mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/
--rw-r--r--   0 blueswen   (501) staff       (20)     1096 2022-06-10 06:42:44.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/LICENSE.md
--rw-r--r--   0 blueswen   (501) staff       (20)    13749 2022-06-07 11:18:17.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/glightbox.min.css
--rw-r--r--   0 blueswen   (501) staff       (20)    56280 2022-06-07 11:18:23.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/glightbox.min.js
--rw-r--r--   0 blueswen   (501) staff       (20)     9808 2024-01-24 14:50:48.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox/plugin.py
-drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-01-24 15:16:44.291074 mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/
--rw-r--r--   0 blueswen   (501) staff       (20)     4879 2024-01-24 15:16:44.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/PKG-INFO
--rw-r--r--   0 blueswen   (501) staff       (20)      528 2024-01-24 15:16:44.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/SOURCES.txt
--rw-r--r--   0 blueswen   (501) staff       (20)        1 2024-01-24 15:16:44.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/dependency_links.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       69 2024-01-24 15:16:44.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/entry_points.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       17 2024-01-24 15:16:44.000000 mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/top_level.txt
--rw-r--r--   0 blueswen   (501) staff       (20)       38 2024-01-24 15:16:44.293201 mkdocs-glightbox-0.3.7/setup.cfg
--rw-rw-r--   0 blueswen   (501) staff       (20)      816 2024-01-24 15:08:13.000000 mkdocs-glightbox-0.3.7/setup.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-05-06 14:31:39.078081 mkdocs-glightbox-0.4.0/
+-rw-r--r--   0 blueswen   (501) staff       (20)     1065 2022-06-10 06:58:58.000000 mkdocs-glightbox-0.4.0/LICENSE
+-rw-r--r--   0 blueswen   (501) staff       (20)       37 2022-07-15 16:30:44.000000 mkdocs-glightbox-0.4.0/MANIFEST.in
+-rw-r--r--   0 blueswen   (501) staff       (20)     6124 2024-05-06 14:31:39.077931 mkdocs-glightbox-0.4.0/PKG-INFO
+-rw-r--r--   0 blueswen   (501) staff       (20)     5698 2024-05-06 14:21:55.000000 mkdocs-glightbox-0.4.0/README.md
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-05-06 14:31:39.073020 mkdocs-glightbox-0.4.0/mkdocs_glightbox/
+-rw-r--r--   0 blueswen   (501) staff       (20)        0 2022-06-12 06:19:32.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/__init__.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-05-06 14:31:39.074510 mkdocs-glightbox-0.4.0/mkdocs_glightbox/__pycache__/
+-rw-r--r--   0 blueswen   (501) staff       (20)      165 2022-11-15 14:31:20.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 blueswen   (501) staff       (20)     7524 2024-05-06 13:29:06.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-05-06 14:31:39.076949 mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/
+-rw-r--r--   0 blueswen   (501) staff       (20)     1096 2022-06-10 06:42:44.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/LICENSE.md
+-rw-r--r--   0 blueswen   (501) staff       (20)    13749 2022-06-07 11:18:17.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/glightbox.min.css
+-rw-r--r--   0 blueswen   (501) staff       (20)    56280 2022-06-07 11:18:23.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/glightbox.min.js
+-rw-r--r--   0 blueswen   (501) staff       (20)    10595 2024-05-06 13:19:06.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox/plugin.py
+drwxr-xr-x   0 blueswen   (501) staff       (20)        0 2024-05-06 14:31:39.074056 mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/
+-rw-r--r--   0 blueswen   (501) staff       (20)     6124 2024-05-06 14:31:39.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/PKG-INFO
+-rw-r--r--   0 blueswen   (501) staff       (20)      528 2024-05-06 14:31:39.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/SOURCES.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)        1 2024-05-06 14:31:39.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/dependency_links.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       69 2024-05-06 14:31:39.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/entry_points.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       17 2024-05-06 14:31:39.000000 mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/top_level.txt
+-rw-r--r--   0 blueswen   (501) staff       (20)       38 2024-05-06 14:31:39.078127 mkdocs-glightbox-0.4.0/setup.cfg
+-rw-rw-r--   0 blueswen   (501) staff       (20)      816 2024-05-06 14:22:05.000000 mkdocs-glightbox-0.4.0/setup.py
```

### Comparing `mkdocs-glightbox-0.3.7/LICENSE` & `mkdocs-glightbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.7/PKG-INFO` & `mkdocs-glightbox-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-glightbox
-Version: 0.3.7
+Version: 0.4.0
 Summary: MkDocs plugin supports image lightbox with GLightbox.
 Home-page: https://blueswen.github.io/mkdocs-glightbox
 Author: Blueswen
 Author-email: blueswen.tw@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
 Keywords: mkdocs,plugin,lightbox
@@ -63,14 +63,15 @@
            draggable: true
            skip_classes:
              - custom-skip-class-name
            auto_caption: false
            caption_position: bottom
            background: white
            shadow: true
+           manual: false
     ```
 
     | Option | Default | Description |
     |---|---|---|
     | touchNavigation | true | Enable or disable the touch navigation (swipe). |
     | loop | false | Loop slides on end. |
     | effect | zoom | Name of the effect on lightbox open. (zoom, fade, none) |
@@ -80,21 +81,29 @@
     | zoomable | true | Enable or disable zoomable images. |
     | draggable | true | Enable or disable mouse drag to go prev and next slide. |
     | skip_classes | [ ] | Disable lightbox of those image with specific custom class name. |
     | auto_caption | false | Enable or disable using alt of image as caption title automatically. |
     | caption_position | bottom | Default captions position. (bottom, top, left, right) |
     | background | white | The background CSS of lightbox image. The background will shown when the image is transparent. You can use any CSS value for the background for example `#74b9ff` or `Gainsboro` or `none` for nothing. |
     | shadow | true | Enable or disable the shadow of lightbox image. Disable it when the background is `none` to prevent shadow around the transparent image. |
+    | manual | false | When true, lightbox has to be enabled for each image manually by adding `on-glb` class to it or adding `glightbox: true` meta on page.  |
 
     Check more options information on [GLightbox Docs](https://github.com/biati-digital/glightbox#lightbox-options).
 
-5. For more flexibility, you can disable the lightbox with a [specific image](https://blueswen.github.io/mkdocs-glightbox/disable/image/) or a [specific page](https://blueswen.github.io/mkdocs-glightbox/disable/page/).
+5. For more flexibility:
+      1. [Disable by image](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-image.md): Disable the lightbox for specific images. Suitable for a few amount of images that don't need the lightbox effect.
+      2. [Disable by page](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-page.md): Disable the lightbox for specific pages. Suitable for a few amount of pages that don't need the lightbox effect.
+      3. [Enable by image](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-page-enable-by-image.md): Disable the lightbox for specific pages but enable some images on those pages. Suitable for a few amount of images that need the lightbox effect.
+      4. [Disable globally but enable by image or page](https://blueswen.github.io/mkdocs-glightbox/flexibility/enable-by-image-or-page.md): Disable the lightbox globally but enable specific images or specific pages. Suitable for a large number of images or pages that don't need the lightbox effect.
 6. Support lightbox image caption, check more details on [Caption](https://blueswen.github.io/mkdocs-glightbox/caption/caption/).
 7. Support grouping images as galleries, check more details on [Gallery](https://blueswen.github.io/mkdocs-glightbox/gallery/gallery/).
 
+> [!NOTE] 
+> If this is your first time using the MkDocs plugin feature, you should know that MkDocs includes a default plugin named `search`. If you want to keep the search feature, you need to add the `search` plugin back to the `plugins` list.
+
 ## How it works
 
 1. Copy GLightbox script file into `site/assets/javascripts/` directory and CSS file into `site/assets/stylesheets/` directory
 2. Import GLightbox script and CSS file and add javascript code on each page excluded disabled pages
 3. Search all image tags and warp with an anchor tag for GLightbox excluded images with skip class or already warped with an anchor tag
 
 ## License
```

### Comparing `mkdocs-glightbox-0.3.7/README.md` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: mkdocs-glightbox
+Version: 0.4.0
+Summary: MkDocs plugin supports image lightbox with GLightbox.
+Home-page: https://blueswen.github.io/mkdocs-glightbox
+Author: Blueswen
+Author-email: blueswen.tw@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
+Keywords: mkdocs,plugin,lightbox
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MkDocs GLightbox
 
 <p align="center">
 <a target="_blank" href="https://pypi.org/project/mkdocs-glightbox"><img src="https://img.shields.io/pypi/v/mkdocs-glightbox.svg" alt="PyPI version"/></a>
 <a target="_blank" href="https://pypi.org/project/mkdocs-glightbox"><img src="https://img.shields.io/pypi/dm/mkdocs-glightbox.svg" alt="PyPI downloads"/></a>
 <a target="_blank" href="https://codecov.io/gh/blueswen/mkdocs-glightbox"><img src="https://codecov.io/gh/blueswen/mkdocs-glightbox/branch/main/graph/badge.svg?token=KAJS3NU81H" alt="Codecov"/></a>
 </p>
@@ -49,14 +63,15 @@
            draggable: true
            skip_classes:
              - custom-skip-class-name
            auto_caption: false
            caption_position: bottom
            background: white
            shadow: true
+           manual: false
     ```
 
     | Option | Default | Description |
     |---|---|---|
     | touchNavigation | true | Enable or disable the touch navigation (swipe). |
     | loop | false | Loop slides on end. |
     | effect | zoom | Name of the effect on lightbox open. (zoom, fade, none) |
@@ -66,23 +81,33 @@
     | zoomable | true | Enable or disable zoomable images. |
     | draggable | true | Enable or disable mouse drag to go prev and next slide. |
     | skip_classes | [ ] | Disable lightbox of those image with specific custom class name. |
     | auto_caption | false | Enable or disable using alt of image as caption title automatically. |
     | caption_position | bottom | Default captions position. (bottom, top, left, right) |
     | background | white | The background CSS of lightbox image. The background will shown when the image is transparent. You can use any CSS value for the background for example `#74b9ff` or `Gainsboro` or `none` for nothing. |
     | shadow | true | Enable or disable the shadow of lightbox image. Disable it when the background is `none` to prevent shadow around the transparent image. |
+    | manual | false | When true, lightbox has to be enabled for each image manually by adding `on-glb` class to it or adding `glightbox: true` meta on page.  |
 
     Check more options information on [GLightbox Docs](https://github.com/biati-digital/glightbox#lightbox-options).
 
-5. For more flexibility, you can disable the lightbox with a [specific image](https://blueswen.github.io/mkdocs-glightbox/disable/image/) or a [specific page](https://blueswen.github.io/mkdocs-glightbox/disable/page/).
+5. For more flexibility:
+      1. [Disable by image](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-image.md): Disable the lightbox for specific images. Suitable for a few amount of images that don't need the lightbox effect.
+      2. [Disable by page](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-page.md): Disable the lightbox for specific pages. Suitable for a few amount of pages that don't need the lightbox effect.
+      3. [Enable by image](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-page-enable-by-image.md): Disable the lightbox for specific pages but enable some images on those pages. Suitable for a few amount of images that need the lightbox effect.
+      4. [Disable globally but enable by image or page](https://blueswen.github.io/mkdocs-glightbox/flexibility/enable-by-image-or-page.md): Disable the lightbox globally but enable specific images or specific pages. Suitable for a large number of images or pages that don't need the lightbox effect.
 6. Support lightbox image caption, check more details on [Caption](https://blueswen.github.io/mkdocs-glightbox/caption/caption/).
 7. Support grouping images as galleries, check more details on [Gallery](https://blueswen.github.io/mkdocs-glightbox/gallery/gallery/).
 
+> [!NOTE] 
+> If this is your first time using the MkDocs plugin feature, you should know that MkDocs includes a default plugin named `search`. If you want to keep the search feature, you need to add the `search` plugin back to the `plugins` list.
+
 ## How it works
 
 1. Copy GLightbox script file into `site/assets/javascripts/` directory and CSS file into `site/assets/stylesheets/` directory
 2. Import GLightbox script and CSS file and add javascript code on each page excluded disabled pages
 3. Search all image tags and warp with an anchor tag for GLightbox excluded images with skip class or already warped with an anchor tag
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Blueswen/mkdocs-glightbox/blob/main/LICENSE) file for details.
+
+
```

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox/__pycache__/plugin.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jan 24 14:50:48 2024 UTC, .py size: 9808 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,449 +1,471 @@
-00000000: 610d 0d0a 0000 0000 c823 b165 5026 0000  a........#.eP&..
+00000000: 610d 0d0a 0000 0000 cad8 3866 6329 0000  a.........8fc)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6501 a00a 650b a101 5a0c 6502 6a0d  ..e...e...Z.e.j.
 00000080: a00e 6502 6a0d a00f 6510 a101 a101 5a11  ..e.j...e.....Z.
 00000090: 4700 6405 6406 8400 6406 6509 8303 5a12  G.d.d...d.e...Z.
 000000a0: 6401 5300 2907 e900 0000 004e 2901 da05  d.S.)......N)...
 000000b0: 7574 696c 7329 01da 0e63 6f6e 6669 675f  utils)...config_
 000000c0: 6f70 7469 6f6e 7329 01da 0a42 6173 6550  options)...BaseP
 000000d0: 6c75 6769 6e63 0000 0000 0000 0000 0000  luginc..........
-000000e0: 0000 0000 0000 1100 0000 4000 0000 730c  ..........@...s.
+000000e0: 0000 0000 0000 1200 0000 4000 0000 731c  ..........@...s.
 000000f0: 0100 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
 00000100: 0265 046a 0565 0664 0364 048d 0266 0264  .e.j.e.d.d...f.d
 00000110: 0565 046a 0565 0664 0664 048d 0266 0264  .e.j.e.d.d...f.d
 00000120: 0765 046a 0764 0864 0964 048d 0266 0264  .e.j.d.d.d...f.d
 00000130: 0a65 046a 0764 0b64 0c64 048d 0266 0264  .e.j.d.d.d...f.d
 00000140: 0d65 046a 0565 0864 0e64 048d 0266 0264  .e.j.e.d.d...f.d
 00000150: 0f65 046a 0565 0864 0e64 048d 0266 0264  .e.j.e.d.d...f.d
 00000160: 1065 046a 0565 0664 0364 048d 0266 0264  .e.j.e.d.d...f.d
 00000170: 1165 046a 0565 0664 0364 048d 0266 0264  .e.j.e.d.d...f.d
 00000180: 1265 046a 0565 0967 0064 048d 0266 0264  .e.j.e.g.d...f.d
 00000190: 1365 046a 0565 0664 0664 048d 0266 0264  .e.j.e.d.d...f.d
 000001a0: 1465 046a 0764 1564 1664 048d 0266 0264  .e.j.d.d.d...f.d
 000001b0: 1765 046a 0565 0864 1864 048d 0266 0264  .e.j.e.d.d...f.d
-000001c0: 1965 046a 0565 0664 0364 048d 0266 0266  .e.j.e.d.d...f.f
-000001d0: 0d5a 0a64 1a64 1b84 005a 0b64 1c64 1d84  .Z.d.d...Z.d.d..
-000001e0: 005a 0c64 1e64 1f84 005a 0d64 2064 2184  .Z.d.d...Z.d d!.
-000001f0: 005a 0e64 2264 2384 005a 0f64 2453 0029  .Z.d"d#..Z.d$S.)
-00000200: 25da 0e4c 6967 6874 626f 7850 6c75 6769  %..LightboxPlugi
-00000210: 6e7a 1641 6464 206c 6967 6874 626f 7820  nz.Add lightbox 
-00000220: 746f 204d 6b44 6f63 73da 0f74 6f75 6368  to MkDocs..touch
-00000230: 4e61 7669 6761 7469 6f6e 5429 01da 0764  NavigationT)...d
-00000240: 6566 6175 6c74 da04 6c6f 6f70 46da 0665  efault..loopF..e
-00000250: 6666 6563 7429 03da 047a 6f6f 6dda 0466  ffect)...zoom..f
-00000260: 6164 65da 046e 6f6e 6572 0a00 0000 da0c  ade..noner......
-00000270: 736c 6964 655f 6566 6665 6374 2904 da05  slide_effect)...
-00000280: 736c 6964 6572 0a00 0000 720b 0000 0072  slider....r....r
-00000290: 0c00 0000 720e 0000 00da 0577 6964 7468  ....r......width
-000002a0: da04 6175 746f da06 6865 6967 6874 da08  ..auto..height..
-000002b0: 7a6f 6f6d 6162 6c65 da09 6472 6167 6761  zoomable..dragga
-000002c0: 626c 65da 0c73 6b69 705f 636c 6173 7365  ble..skip_classe
-000002d0: 73da 0c61 7574 6f5f 6361 7074 696f 6eda  s..auto_caption.
-000002e0: 1063 6170 7469 6f6e 5f70 6f73 6974 696f  .caption_positio
-000002f0: 6e29 04da 0662 6f74 746f 6dda 0374 6f70  n)...bottom..top
-00000300: da04 6c65 6674 da05 7269 6768 7472 1700  ..left..rightr..
-00000310: 0000 da0a 6261 636b 6772 6f75 6e64 da05  ....background..
-00000320: 7768 6974 65da 0673 6861 646f 7763 0200  white..shadowc..
-00000330: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000340: 0000 4300 0000 7338 0000 007c 0164 0119  ..C...s8...|.d..
-00000350: 006a 0064 026b 027c 005f 017c 006a 016f  .j.d.k.|._.|.j.o
-00000360: 3064 037c 0164 0419 0076 006f 307c 0164  0d.|.d...v.o0|.d
-00000370: 0419 0064 0319 006a 026a 037c 005f 0464  ...d...j.j.|._.d
-00000380: 0053 0029 054e da05 7468 656d 65da 086d  .S.).N..theme..m
-00000390: 6174 6572 6961 6c7a 106d 6174 6572 6961  aterialz.materia
-000003a0: 6c2f 7072 6976 6163 79da 0770 6c75 6769  l/privacy..plugi
-000003b0: 6e73 2905 da04 6e61 6d65 da0e 7573 696e  ns)...name..usin
-000003c0: 675f 6d61 7465 7269 616c da06 636f 6e66  g_material..conf
-000003d0: 6967 da07 656e 6162 6c65 64da 1675 7369  ig..enabled..usi
-000003e0: 6e67 5f6d 6174 6572 6961 6c5f 7072 6976  ng_material_priv
-000003f0: 6163 7929 02da 0473 656c 6672 2300 0000  acy)...selfr#...
-00000400: a900 7227 0000 00fa 482f 5573 6572 732f  ..r'....H/Users/
-00000410: 626c 7565 7377 656e 2f70 726f 6a65 6374  blueswen/project
-00000420: 732f 6c61 622f 6d6b 646f 6373 2d67 6c69  s/lab/mkdocs-gli
-00000430: 6768 7462 6f78 2f6d 6b64 6f63 735f 676c  ghtbox/mkdocs_gl
-00000440: 6967 6874 626f 782f 706c 7567 696e 2e70  ightbox/plugin.p
-00000450: 79da 096f 6e5f 636f 6e66 6967 2700 0000  y..on_config'...
-00000460: 730c 0000 0000 0110 0206 010a ff02 020e  s...............
-00000470: fd7a 184c 6967 6874 626f 7850 6c75 6769  .z.LightboxPlugi
-00000480: 6e2e 6f6e 5f63 6f6e 6669 6763 0400 0000  n.on_configc....
-00000490: 0000 0000 0000 0000 0c00 0000 0600 0000  ................
-000004a0: 0b00 0000 73b0 0100 0064 017c 026a 0076  ....s....d.|.j.v
-000004b0: 0072 207c 026a 00a0 0164 0164 02a1 0264  .r |.j...d.d...d
-000004c0: 0375 0072 207c 0153 0074 026a 0364 0474  .u.r |.S.t.j.d.t
-000004d0: 026a 0464 058d 027d 0574 026a 0364 0674  .j.d...}.t.j.d.t
-000004e0: 026a 0464 058d 027d 0664 0774 05a0 0674  .j.d...}.d.t...t
-000004f0: 05a0 0764 08a1 017c 026a 08a1 029b 0064  ...d...|.j.....d
-00000500: 099d 037d 077c 05a0 0964 0a7c 079b 0064  ...}.|...d.|...d
-00000510: 0b9d 037c 01a1 027d 0164 0c7d 087c 0864  ...|...}.d.}.|.d
-00000520: 0d7c 006a 0a64 0e19 009b 0064 0f9d 0337  .|.j.d.....d...7
-00000530: 007d 087c 006a 0a64 1019 0073 9c7c 0864  .}.|.j.d...s.|.d
-00000540: 1137 007d 087c 0364 1219 006a 0b64 136b  .7.}.|.d...j.d.k
-00000550: 0272 b27c 0864 1437 007d 087c 05a0 0964  .r.|.d.7.}.|...d
-00000560: 157c 089b 0064 169d 037c 01a1 027d 0164  .|...d...|...}.d
-00000570: 1774 05a0 0674 05a0 0764 18a1 017c 026a  .t...t...d...|.j
-00000580: 08a1 029b 0064 199d 037d 097c 05a0 0964  .....d...}.|...d
-00000590: 0a7c 099b 0064 0b9d 037c 01a1 027d 0174  .|...d...|...}.t
-000005a0: 0c7c 006a 0a83 0189 0087 0066 0164 1a64  .|.j.......f.d.d
-000005b0: 1b84 0864 1c44 0083 017d 0a88 00a0 0164  ...d.D...}.....d
-000005c0: 1d64 1ea1 027c 0a64 1f3c 0088 00a0 0164  .d...|.d.<.....d
-000005d0: 1d64 1ea1 027c 0a64 203c 0088 00a0 0164  .d...|.d <.....d
-000005e0: 2164 22a1 027c 0a64 233c 0064 247d 0b7c  !d"..|.d#<.d$}.|
-000005f0: 006a 0d90 0172 567c 0b64 2537 007d 0b7c  .j...rV|.d%7.}.|
-00000600: 0b64 2674 0ea0 0f7c 0aa1 019b 0064 279d  .d&t...|.....d'.
-00000610: 0337 007d 0b7c 006a 1090 0173 8c64 287c  .7.}.|.j...s.d(|
-00000620: 0364 1219 006a 11a0 0164 2967 00a1 0276  .d...j...d)g...v
-00000630: 0090 0172 9864 2a7c 0b17 0064 2b17 007d  ...r.d*|...d+..}
-00000640: 0b7c 06a0 0964 2c7c 0b9b 0064 2d9d 037c  .|...d,|...d-..|
-00000650: 01a1 027d 017c 0153 0029 2e7a 5441 6464  ...}.|.S.).zTAdd
-00000660: 2063 7373 206c 696e 6b20 7461 672c 206a   css link tag, j
-00000670: 6176 6173 6372 6970 7420 7363 7269 7074  avascript script
-00000680: 2074 6167 2c20 616e 6420 6a61 7661 7363   tag, and javasc
-00000690: 7269 7074 2063 6f64 6520 746f 2069 6e69  ript code to ini
-000006a0: 7469 616c 697a 6520 474c 6967 6874 626f  tialize GLightbo
-000006b0: 78da 0967 6c69 6768 7462 6f78 5446 7a13  x..glightboxTFz.
-000006c0: 3c68 6561 643e 282e 2a3f 293c 5c2f 6865  <head>(.*?)<\/he
-000006d0: 6164 3e29 01da 0566 6c61 6773 7a12 3c62  ad>)...flagsz.<b
-000006e0: 6f64 7928 2e2a 3f29 3c5c 2f62 6f64 793e  ody(.*?)<\/body>
-000006f0: 7a0c 3c6c 696e 6b20 6872 6566 3d22 7a24  z.<link href="z$
-00000700: 6173 7365 7473 2f73 7479 6c65 7368 6565  assets/styleshee
-00000710: 7473 2f67 6c69 6768 7462 6f78 2e6d 696e  ts/glightbox.min
-00000720: 2e63 7373 7a14 2220 7265 6c3d 2273 7479  .cssz." rel="sty
-00000730: 6c65 7368 6565 7422 2f3e 7a09 3c68 6561  lesheet"/>z.<hea
-00000740: 643e 5c31 207a 073c 2f68 6561 643e 7aac  d>\1 z.</head>z.
-00000750: 0a20 2020 2068 746d 6c2e 676c 6967 6874  .    html.glight
-00000760: 626f 782d 6f70 656e 207b 206f 7665 7266  box-open { overf
-00000770: 6c6f 773a 2069 6e69 7469 616c 3b20 6865  low: initial; he
-00000780: 6967 6874 3a20 3130 3025 3b20 7d0a 2020  ight: 100%; }.  
-00000790: 2020 2e67 736c 6964 652d 7469 746c 6520    .gslide-title 
-000007a0: 7b20 6d61 7267 696e 2d74 6f70 3a20 3070  { margin-top: 0p
-000007b0: 783b 2075 7365 722d 7365 6c65 6374 3a20  x; user-select: 
-000007c0: 7465 7874 3b20 7d0a 2020 2020 2e67 736c  text; }.    .gsl
-000007d0: 6964 652d 6465 7363 207b 2063 6f6c 6f72  ide-desc { color
-000007e0: 3a20 2336 3636 3b20 7573 6572 2d73 656c  : #666; user-sel
-000007f0: 6563 743a 2074 6578 743b 207d 7a25 0a20  ect: text; }z%. 
-00000800: 2020 202e 6773 6c69 6465 2d69 6d61 6765     .gslide-image
-00000810: 2069 6d67 207b 2062 6163 6b67 726f 756e   img { backgroun
-00000820: 643a 2072 1b00 0000 7a03 3b20 7d72 1d00  d: r....z.; }r..
-00000830: 0000 7a67 0a20 2020 202e 676c 6967 6874  ..zg.    .glight
-00000840: 626f 782d 636c 6561 6e20 2e67 736c 6964  box-clean .gslid
-00000850: 652d 6d65 6469 6120 7b0a 2020 2020 2020  e-media {.      
-00000860: 2020 2d77 6562 6b69 742d 626f 782d 7368    -webkit-box-sh
-00000870: 6164 6f77 3a20 6e6f 6e65 3b0a 2020 2020  adow: none;.    
-00000880: 2020 2020 626f 782d 7368 6164 6f77 3a20      box-shadow: 
-00000890: 6e6f 6e65 3b0a 2020 2020 7d72 1e00 0000  none;.    }r....
-000008a0: 721f 0000 0061 6c01 0000 0a20 2020 202e  r....al....    .
-000008b0: 6773 6372 6f6c 6c62 6172 2d66 6978 6572  gscrollbar-fixer
-000008c0: 207b 2070 6164 6469 6e67 2d72 6967 6874   { padding-right
-000008d0: 3a20 3135 7078 3b20 7d0a 2020 2020 2e67  : 15px; }.    .g
-000008e0: 6465 7363 2d69 6e6e 6572 207b 2066 6f6e  desc-inner { fon
-000008f0: 742d 7369 7a65 3a20 302e 3735 7265 6d3b  t-size: 0.75rem;
-00000900: 207d 0a20 2020 2062 6f64 795b 6461 7461   }.    body[data
-00000910: 2d6d 642d 636f 6c6f 722d 7363 6865 6d65  -md-color-scheme
-00000920: 3d22 736c 6174 6522 5d20 2e67 6465 7363  ="slate"] .gdesc
-00000930: 2d69 6e6e 6572 207b 2062 6163 6b67 726f  -inner { backgro
-00000940: 756e 643a 2076 6172 282d 2d6d 642d 6465  und: var(--md-de
-00000950: 6661 756c 742d 6267 2d63 6f6c 6f72 293b  fault-bg-color);
-00000960: 7d0a 2020 2020 626f 6479 5b64 6174 612d  }.    body[data-
-00000970: 6d64 2d63 6f6c 6f72 2d73 6368 656d 653d  md-color-scheme=
-00000980: 2273 6c61 7465 225d 202e 6773 6c69 6465  "slate"] .gslide
-00000990: 2d74 6974 6c65 207b 2063 6f6c 6f72 3a20  -title { color: 
-000009a0: 7661 7228 2d2d 6d64 2d64 6566 6175 6c74  var(--md-default
-000009b0: 2d66 672d 636f 6c6f 7229 3b7d 0a20 2020  -fg-color);}.   
-000009c0: 2062 6f64 795b 6461 7461 2d6d 642d 636f   body[data-md-co
-000009d0: 6c6f 722d 7363 6865 6d65 3d22 736c 6174  lor-scheme="slat
-000009e0: 6522 5d20 2e67 736c 6964 652d 6465 7363  e"] .gslide-desc
-000009f0: 207b 2063 6f6c 6f72 3a20 7661 7228 2d2d   { color: var(--
-00000a00: 6d64 2d64 6566 6175 6c74 2d66 672d 636f  md-default-fg-co
-00000a10: 6c6f 7229 3b7d 7a0f 3c68 6561 643e 5c31  lor);}z.<head>\1
-00000a20: 3c73 7479 6c65 3e7a 0f3c 2f73 7479 6c65  <style>z.</style
-00000a30: 3e3c 2f68 6561 643e 7a0d 3c73 6372 6970  ></head>z.<scrip
-00000a40: 7420 7372 633d 227a 2361 7373 6574 732f  t src="z#assets/
-00000a50: 6a61 7661 7363 7269 7074 732f 676c 6967  javascripts/glig
-00000a60: 6874 626f 782e 6d69 6e2e 6a73 7a0b 223e  htbox.min.jsz.">
-00000a70: 3c2f 7363 7269 7074 3e63 0100 0000 0000  </script>c......
-00000a80: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-00000a90: 0000 7316 0000 0069 007c 005d 0e7d 017c  ..s....i.|.].}.|
-00000aa0: 0188 007c 0119 0093 0271 0453 0072 2700  ...|.....q.S.r'.
-00000ab0: 0000 7227 0000 00a9 02da 022e 30da 016b  ..r'........0..k
-00000ac0: a901 da0d 706c 7567 696e 5f63 6f6e 6669  ....plugin_confi
-00000ad0: 6772 2700 0000 7228 0000 00da 0a3c 6469  gr'...r(.....<di
-00000ae0: 6374 636f 6d70 3e59 0000 0073 0400 0000  ctcomp>Y...s....
-00000af0: 0602 02ff 7a2f 4c69 6768 7462 6f78 506c  ....z/LightboxPl
-00000b00: 7567 696e 2e6f 6e5f 706f 7374 5f70 6167  ugin.on_post_pag
-00000b10: 652e 3c6c 6f63 616c 733e 2e3c 6469 6374  e.<locals>.<dict
-00000b20: 636f 6d70 3e29 0472 0600 0000 7208 0000  comp>).r....r...
-00000b30: 0072 1200 0000 7213 0000 0072 0900 0000  .r....r....r....
-00000b40: 720a 0000 005a 0a6f 7065 6e45 6666 6563  r....Z.openEffec
-00000b50: 745a 0b63 6c6f 7365 4566 6665 6374 720d  tZ.closeEffectr.
-00000b60: 0000 0072 0e00 0000 5a0b 736c 6964 6545  ...r....Z.slideE
-00000b70: 6666 6563 74da 007a a564 6f63 756d 656e  ffect..z.documen
-00000b80: 742e 7175 6572 7953 656c 6563 746f 7241  t.querySelectorA
-00000b90: 6c6c 2827 2e67 6c69 6768 7462 6f78 2729  ll('.glightbox')
-00000ba0: 2e66 6f72 4561 6368 2866 756e 6374 696f  .forEach(functio
-00000bb0: 6e28 656c 656d 656e 7429 207b 0a20 2020  n(element) {.   
-00000bc0: 2076 6172 2069 6d67 5372 6320 3d20 656c   var imgSrc = el
-00000bd0: 656d 656e 742e 7175 6572 7953 656c 6563  ement.querySelec
-00000be0: 746f 7228 2769 6d67 2729 2e73 7263 3b0a  tor('img').src;.
-00000bf0: 2020 2020 656c 656d 656e 742e 7365 7441      element.setA
-00000c00: 7474 7269 6275 7465 2827 6872 6566 272c  ttribute('href',
-00000c10: 2069 6d67 5372 6329 3b0a 7d29 3b0a 7a1b   imgSrc);.});.z.
-00000c20: 636f 6e73 7420 6c69 6768 7462 6f78 203d  const lightbox =
-00000c30: 2047 4c69 6768 7462 6f78 287a 0229 3b7a   GLightbox(z.);z
-00000c40: 126e 6176 6967 6174 696f 6e2e 696e 7374  .navigation.inst
-00000c50: 616e 74da 0866 6561 7475 7265 737a 1b64  ant..featuresz.d
-00000c60: 6f63 756d 656e 7424 2e73 7562 7363 7269  ocument$.subscri
-00000c70: 6265 2828 2920 3d3e 207b 7a02 7d29 7a0f  be(() => {z.})z.
-00000c80: 3c62 6f64 795c 313c 7363 7269 7074 3e7a  <body\1<script>z
-00000c90: 103c 2f73 6372 6970 743e 3c2f 626f 6479  .</script></body
-00000ca0: 3e29 12da 046d 6574 61da 0367 6574 da02  >)...meta..get..
-00000cb0: 7265 da07 636f 6d70 696c 65da 0644 4f54  re..compile..DOT
-00000cc0: 414c 4c72 0200 0000 da10 6765 745f 7265  ALLr......get_re
-00000cd0: 6c61 7469 7665 5f75 726c da0d 6e6f 726d  lative_url..norm
-00000ce0: 616c 697a 655f 7572 6cda 0375 726c da03  alize_url..url..
-00000cf0: 7375 6272 2300 0000 7221 0000 00da 0464  subr#...r!.....d
-00000d00: 6963 7472 2500 0000 da04 6a73 6f6e da05  ictr%.....json..
-00000d10: 6475 6d70 7372 2200 0000 da05 5f76 6172  dumpsr"....._var
-00000d20: 7329 0c72 2600 0000 da06 6f75 7470 7574  s).r&.....output
-00000d30: da04 7061 6765 7223 0000 00da 066b 7761  ..pager#.....kwa
-00000d40: 7267 735a 0a68 6561 645f 7265 6765 785a  rgsZ.head_regexZ
-00000d50: 0a62 6f64 795f 7265 6765 785a 0863 7373  .body_regexZ.css
-00000d60: 5f6c 696e 6b5a 0963 7373 5f70 6174 6368  _linkZ.css_patch
-00000d70: 5a09 6a73 5f73 6372 6970 745a 096c 625f  Z.js_scriptZ.lb_
-00000d80: 636f 6e66 6967 5a07 6a73 5f63 6f64 6572  configZ.js_coder
-00000d90: 2700 0000 722f 0000 0072 2800 0000 da0c  '...r/...r(.....
-00000da0: 6f6e 5f70 6f73 745f 7061 6765 2f00 0000  on_post_page/...
-00000db0: 7344 0000 0000 031c 0104 0310 0110 031c  sD..............
-00000dc0: 0114 0304 0404 0108 ff0a 020a 0108 050e  ................
-00000dd0: 0108 0614 031c 0114 030a 010a 0202 fe06  ................
-00000de0: 0410 0110 0110 0104 0108 0108 0516 0114  ................
-00000df0: 0104 ff08 040c 0114 027a 1b4c 6967 6874  .........z.Light
-00000e00: 626f 7850 6c75 6769 6e2e 6f6e 5f70 6f73  boxPlugin.on_pos
-00000e10: 745f 7061 6765 6304 0000 0000 0000 0000  t_pagec.........
-00000e20: 0000 0006 0000 0006 0000 000b 0000 0073  ...............s
-00000e30: 7600 0000 6401 8800 6a00 7600 7220 8800  v...d...j.v.r ..
-00000e40: 6a00 a001 6401 6402 a102 6403 7500 7220  j...d.d...d.u.r 
-00000e50: 7c01 5300 8702 6601 6404 6405 8408 6406  |.S...f.d.d...d.
-00000e60: 4400 8301 8901 6700 6407 a201 8903 8803  D.....g.d.......
-00000e70: 6408 6701 8802 6a02 6409 1900 1700 3700  d.g...j.d.....7.
-00000e80: 8903 7403 a004 640a a101 7d05 7c05 a005  ..t...d...}.|...
-00000e90: 8700 8701 8702 8703 6604 640b 640c 8408  ........f.d.d...
-00000ea0: 7c01 a102 7d01 7c01 5300 290d 7a4c 5772  |...}.|.S.).zLWr
-00000eb0: 6170 2069 6d67 2074 6167 2077 6974 6820  ap img tag with 
-00000ec0: 616e 6368 6f72 2074 6167 2077 6974 6820  anchor tag with 
-00000ed0: 676c 6967 6874 626f 7820 636c 6173 7320  glightbox class 
-00000ee0: 616e 6420 6174 7472 6962 7574 6573 2066  and attributes f
-00000ef0: 726f 6d20 636f 6e66 6967 722a 0000 0054  rom configr*...T
-00000f00: 4663 0100 0000 0000 0000 0000 0000 0200  Fc..............
-00000f10: 0000 0500 0000 1300 0000 731c 0000 0069  ..........s....i
-00000f20: 007c 005d 147d 017c 0174 0088 006a 0183  .|.].}.|.t...j..
-00000f30: 017c 0119 0093 0271 0453 0072 2700 0000  .|.....q.S.r'...
-00000f40: 2902 723d 0000 0072 2300 0000 722c 0000  ).r=...r#...r,..
-00000f50: 0029 0172 2600 0000 7227 0000 0072 2800  .).r&...r'...r(.
-00000f60: 0000 7231 0000 0076 0000 00f3 0000 0000  ..r1...v........
-00000f70: 7a32 4c69 6768 7462 6f78 506c 7567 696e  z2LightboxPlugin
-00000f80: 2e6f 6e5f 7061 6765 5f63 6f6e 7465 6e74  .on_page_content
-00000f90: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00000fa0: 6f6d 703e 2902 720f 0000 0072 1100 0000  omp>).r....r....
-00000fb0: 2903 5a08 656d 6f6a 696f 6e65 5a07 7477  ).Z.emojioneZ.tw
-00000fc0: 656d 6f6a 695a 0667 656d 6f6a 697a 076f  emojiZ.gemojiz.o
-00000fd0: 6666 2d67 6c62 7214 0000 007a 513c 615c  ff-glbr....zQ<a\
-00000fe0: 625b 5e3e 5d2a 3e28 3f3a 5c73 2a3c 5b5e  b[^>]*>(?:\s*<[^
-00000ff0: 3e5d 2b3e 5c73 2a29 2a3c 696d 675c 625b  >]+>\s*)*<img\b[
-00001000: 5e3e 5d2a 3e28 3f3a 5c73 2a3c 5b5e 3e5d  ^>]*>(?:\s*<[^>]
-00001010: 2b3e 5c73 2a29 2a3c 2f61 3e7c 3c69 6d67  +>\s*)*</a>|<img
-00001020: 283f 503c 6174 7472 3e2e 2a3f 293e 6301  (?P<attr>.*?)>c.
-00001030: 0000 0000 0000 0000 0000 0001 0000 0006  ................
-00001040: 0000 0013 0000 0073 1200 0000 8802 a000  .......s........
-00001050: 7c00 8801 8803 8800 6a01 a104 5300 2901  |.......j...S.).
-00001060: 4e29 02da 1477 7261 705f 696d 675f 7769  N)...wrap_img_wi
-00001070: 7468 5f61 6e63 686f 7272 3400 0000 2901  th_anchorr4...).
-00001080: da05 6d61 7463 68a9 0472 4200 0000 7230  ..match..rB...r0
-00001090: 0000 0072 2600 0000 da0a 736b 6970 5f63  ...r&.....skip_c
-000010a0: 6c61 7373 7227 0000 0072 2800 0000 da08  lassr'...r(.....
-000010b0: 3c6c 616d 6264 613e 8100 0000 7304 0000  <lambda>....s...
-000010c0: 0004 010a ff7a 304c 6967 6874 626f 7850  .....z0LightboxP
-000010d0: 6c75 6769 6e2e 6f6e 5f70 6167 655f 636f  lugin.on_page_co
-000010e0: 6e74 656e 742e 3c6c 6f63 616c 733e 2e3c  ntent.<locals>.<
-000010f0: 6c61 6d62 6461 3e29 0672 3400 0000 7235  lambda>).r4...r5
-00001100: 0000 0072 2300 0000 7236 0000 0072 3700  ...r#...r6...r7.
-00001110: 0000 723c 0000 0029 0672 2600 0000 da04  ..r<...).r&.....
-00001120: 6874 6d6c 7242 0000 0072 2300 0000 7243  htmlrB...r#...rC
-00001130: 0000 00da 0770 6174 7465 726e 7227 0000  .....patternr'..
-00001140: 0072 4800 0000 7228 0000 00da 0f6f 6e5f  .rH...r(.....on_
-00001150: 7061 6765 5f63 6f6e 7465 6e74 7100 0000  page_contentq...
-00001160: 731a 0000 0000 031c 0104 0112 0208 0214  s...............
-00001170: 0304 0102 ff04 0304 0110 0302 fc04 077a  ...............z
-00001180: 1e4c 6967 6874 626f 7850 6c75 6769 6e2e  .LightboxPlugin.
-00001190: 6f6e 5f70 6167 655f 636f 6e74 656e 7463  on_page_contentc
-000011a0: 0500 0000 0000 0000 0000 0000 1200 0000  ................
-000011b0: 0b00 0000 4300 0000 737a 0200 0090 027a  ....C...sz.....z
-000011c0: 2674 00a0 0164 01a1 017d 057c 05a0 027c  &t...d...}.|...|
-000011d0: 01a0 0364 02a1 01a1 0172 2a7c 01a0 0364  ...d.....r*|...d
-000011e0: 02a1 0157 0053 007c 01a0 0364 02a1 017d  ...W.S.|...d...}
-000011f0: 067c 01a0 0364 03a1 017d 0774 00a0 0464  .|...d...}.t...d
-00001200: 047c 07a1 027d 0864 0564 0684 007c 0844  .|...}.d.d...|.D
-00001210: 0083 017d 087c 04a0 0564 0764 08a1 0272  ...}.|...d.d...r
-00001220: 7464 097c 0876 0172 8a7c 0657 0053 006e  td.|.v.r.|.W.S.n
-00001230: 1674 067c 0383 0174 067c 0883 0140 0072  .t.|...t.|...@.r
-00001240: 8a7c 0657 0053 007c 006a 0772 9664 0a7d  .|.W.S.|.j.r.d.}
-00001250: 096e 1e74 00a0 0864 0b7c 07a1 02a0 0364  .n.t...d.|.....d
-00001260: 0ca1 017d 0a64 0d7c 0a9b 0064 0e9d 037d  ...}.d.|...d...}
-00001270: 097c 02a0 09a1 0044 005d 1e5c 027d 0b7d  .|.....D.].\.}.}
-00001280: 0c7c 0964 0f7c 0b9b 0064 107c 0c9b 0064  .|.d.|...d.|...d
-00001290: 119d 0537 007d 0971 bc67 0064 12a2 017d  ...7.}.q.g.d...}
-000012a0: 0d7c 0d44 0090 015d 287d 0e64 137c 0e9b  .|.D...](}.d.|..
-000012b0: 009d 027d 0f7c 0f64 146b 0290 0172 8074  ...}.|.d.k...r.t
-000012c0: 00a0 0864 157c 07a1 027d 107c 006a 0a64  ...d.|...}.|.j.d
-000012d0: 1619 0090 0173 3664 177c 0476 0090 0172  .....s6d.|.v...r
-000012e0: 6a7c 04a0 0564 1764 08a1 0264 1875 0090  j|...d.d...d.u..
-000012f0: 0172 6a7c 1090 0172 487c 10a0 0364 0ca1  .rj|...rH|...d..
-00001300: 017d 106e 2074 00a0 0864 197c 07a1 027d  .}.n t...d.|...}
-00001310: 107c 1090 0172 647c 10a0 0364 0ca1 016e  .|...rd|...d...n
-00001320: 0264 1a7d 106e 147c 1090 0172 7a7c 10a0  .d.}.n.|...rz|..
-00001330: 0364 0ca1 016e 0264 1a7d 106e 587c 0f64  .d...n.d.}.nX|.d
-00001340: 1b6b 0290 0172 b274 00a0 0864 1c7c 07a1  .k...r.t...d.|..
-00001350: 027d 107c 1090 0172 a67c 10a0 0364 0ca1  .}.|...r.|...d..
-00001360: 016e 087c 006a 0a64 1d19 007d 106e 2674  .n.|.j.d...}.n&t
-00001370: 00a0 087c 0f9b 0064 1e9d 027c 07a1 027d  ...|...d...|...}
-00001380: 107c 1090 0172 d47c 10a0 0364 0ca1 016e  .|...r.|...d...n
-00001390: 0264 1a7d 107c 1064 1a6b 0372 e87c 0f64  .d.}.|.d.k.r.|.d
-000013a0: 1b6b 0290 0172 fc7c 0964 1f7c 109b 0064  .k...r.|.d.|...d
-000013b0: 119d 0337 007d 0971 e87c 0964 207c 0f9b  ...7.}.q.|.d |..
-000013c0: 0064 107c 109b 0064 119d 0537 007d 0971  .d.|...d...7.}.q
-000013d0: e87c 0964 217c 069b 0064 229d 0337 007d  .|.d!|...d"..7.}
-000013e0: 097c 0957 0053 0004 0074 0b90 0279 7401  .|.W.S...t...yt.
-000013f0: 007d 1101 007a 3274 0ca0 0d64 237c 119b  .}...z2t...d#|..
-00001400: 0064 207c 01a0 0364 02a1 019b 009d 04a1  .d |...d........
-00001410: 0101 007c 01a0 0364 02a1 0157 0006 0059  ...|...d...W...Y
-00001420: 0064 247d 117e 1153 0064 247d 117e 1130  .d$}.~.S.d$}.~.0
-00001430: 0030 0064 2453 0029 257a 2057 7261 7020  .0.d$S.)%z Wrap 
-00001440: 696d 6167 6520 7461 6773 2077 6974 6820  image tags with 
-00001450: 616e 6368 6f72 2074 6167 737a 103c 6128  anchor tagsz.<a(
-00001460: 3f50 3c61 7474 723e 2e2a 3f29 3e72 0100  ?P<attr>.*?)>r..
-00001470: 0000 da04 6174 7472 7a0f 636c 6173 733d  ....attrz.class=
-00001480: 2228 5b5e 225d 2b29 2263 0100 0000 0000  "([^"]+)"c......
-00001490: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
-000014a0: 0000 731e 0000 0067 007c 005d 167d 017c  ..s....g.|.].}.|
-000014b0: 01a0 00a1 0044 005d 087d 027c 0291 0371  .....D.].}.|...q
-000014c0: 1071 0453 0072 2700 0000 2901 da05 7370  .q.S.r'...)...sp
-000014d0: 6c69 7429 0372 2d00 0000 7247 0000 00da  lit).r-...rG....
-000014e0: 0163 7227 0000 0072 2700 0000 7228 0000  .cr'...r'...r(..
-000014f0: 00da 0a3c 6c69 7374 636f 6d70 3e93 0000  ...<listcomp>...
-00001500: 0072 4500 0000 7a37 4c69 6768 7462 6f78  .rE...z7Lightbox
-00001510: 506c 7567 696e 2e77 7261 705f 696d 675f  Plugin.wrap_img_
-00001520: 7769 7468 5f61 6e63 686f 722e 3c6c 6f63  with_anchor.<loc
-00001530: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
-00001540: 1067 6c69 6768 7462 6f78 2d6d 616e 7561  .glightbox-manua
-00001550: 6c46 7a06 6f6e 2d67 6c62 7a26 3c61 2063  lFz.on-glbz&<a c
-00001560: 6c61 7373 3d22 676c 6967 6874 626f 7822  lass="glightbox"
-00001570: 2064 6174 612d 7479 7065 3d22 696d 6167   data-type="imag
-00001580: 6522 7a14 7372 633d 5b5c 225c 275d 285b  e"z.src=[\"\']([
-00001590: 5e5c 225c 275d 2b29 e901 0000 007a 1b3c  ^\"\']+).....z.<
-000015a0: 6120 636c 6173 733d 2267 6c69 6768 7462  a class="glightb
-000015b0: 6f78 2220 6872 6566 3d22 7a13 2220 6461  ox" href="z." da
-000015c0: 7461 2d74 7970 653d 2269 6d61 6765 227a  ta-type="image"z
-000015d0: 0620 6461 7461 2d7a 023d 22fa 0122 2904  . data-z.="..").
-000015e0: da05 7469 746c 65da 0b64 6573 6372 6970  ..title..descrip
-000015f0: 7469 6f6e 7a10 6361 7074 696f 6e2d 706f  tionz.caption-po
-00001600: 7369 7469 6f6e 5a07 6761 6c6c 6572 797a  sitionZ.galleryz
-00001610: 0564 6174 612d 7a0a 6461 7461 2d74 6974  .data-z.data-tit
-00001620: 6c65 7a17 6461 7461 2d74 6974 6c65 3d5b  lez.data-title=[
-00001630: 5c22 5d28 5b5e 5c22 5d2b 2972 1500 0000  \"]([^\"]+)r....
-00001640: 7a16 676c 6967 6874 626f 782e 6175 746f  z.glightbox.auto
-00001650: 5f63 6170 7469 6f6e 547a 1061 6c74 3d5b  _captionTz.alt=[
-00001660: 5c22 5d28 5b5e 5c22 5d2b 2972 3200 0000  \"]([^\"]+)r2...
-00001670: 7a15 6461 7461 2d63 6170 7469 6f6e 2d70  z.data-caption-p
-00001680: 6f73 6974 696f 6e7a 2264 6174 612d 6361  ositionz"data-ca
-00001690: 7074 696f 6e2d 706f 7369 7469 6f6e 3d5b  ption-position=[
-000016a0: 5c22 5d28 5b5e 5c22 5d2b 2972 1600 0000  \"]([^\"]+)r....
-000016b0: 7a0b 3d5b 225d 285b 5e22 5d2b 297a 1520  z.=["]([^"]+)z. 
-000016c0: 6461 7461 2d64 6573 632d 706f 7369 7469  data-desc-positi
-000016d0: 6f6e 3d22 fa01 20fa 013e 7a04 3c2f 613e  on=".. ..>z.</a>
-000016e0: 7a2b 4572 726f 7220 696e 2077 7261 7070  z+Error in wrapp
-000016f0: 696e 6720 696d 6720 7461 6720 7769 7468  ing img tag with
-00001700: 2061 6e63 686f 7220 7461 673a 204e 290e   anchor tag: N).
-00001710: 7236 0000 0072 3700 0000 7247 0000 00da  r6...r7...rG....
-00001720: 0567 726f 7570 da07 6669 6e64 616c 6c72  .group..findallr
-00001730: 3500 0000 da03 7365 7472 2500 0000 da06  5.....setr%.....
-00001740: 7365 6172 6368 da05 6974 656d 7372 2300  search..itemsr#.
-00001750: 0000 da09 4578 6365 7074 696f 6eda 036c  ....Exception..l
-00001760: 6f67 da07 7761 726e 696e 6729 1272 2600  og..warning).r&.
-00001770: 0000 7247 0000 0072 3000 0000 7249 0000  ..rG...r0...rI..
-00001780: 0072 3400 0000 5a09 615f 7061 7474 6572  .r4...Z.a_patter
-00001790: 6e5a 0769 6d67 5f74 6167 5a08 696d 675f  nZ.img_tagZ.img_
-000017a0: 6174 7472 da07 636c 6173 7365 735a 0561  attr..classesZ.a
-000017b0: 5f74 6167 da03 7372 6372 2e00 0000 da01  _tag..srcr......
-000017c0: 765a 0d73 6c69 6465 5f6f 7074 696f 6e73  vZ.slide_options
-000017d0: da06 6f70 7469 6f6e 724e 0000 00da 0376  ..optionrN.....v
-000017e0: 616c da01 6572 2700 0000 7227 0000 0072  al..er'...r'...r
-000017f0: 2800 0000 7246 0000 0089 0000 0073 6400  (...rF.......sd.
-00001800: 0000 0002 0401 0a01 1001 0c02 0a01 0a01  ................
-00001810: 0c01 0e02 0c01 0801 0802 1001 0602 0602  ................
-00001820: 0602 1201 0c02 1001 1801 0806 0a01 0a01  ................
-00001830: 0a01 0c01 0c01 06ff 0402 0efe 0404 0601  ................
-00001840: 0c02 0c01 1602 1601 0a01 0c01 1c02 1201  ................
-00001850: 1403 0802 0a01 1202 1801 1001 0601 1001  ................
-00001860: 0401 14ff 0403 7a23 4c69 6768 7462 6f78  ......z#Lightbox
-00001870: 506c 7567 696e 2e77 7261 705f 696d 675f  Plugin.wrap_img_
-00001880: 7769 7468 5f61 6e63 686f 7263 0200 0000  with_anchorc....
-00001890: 0000 0000 0000 0000 0600 0000 0700 0000  ................
-000018a0: 4b00 0000 7376 0000 0074 006a 01a0 027c  K...sv...t.j...|
-000018b0: 0164 0119 0064 02a1 027d 0374 006a 01a0  .d...d...}.t.j..
-000018c0: 027c 0364 03a1 027d 0474 03a0 0474 006a  .|.d...}.t...t.j
-000018d0: 01a0 0274 0564 0464 05a1 0374 006a 01a0  ...t.d.d...t.j..
-000018e0: 027c 0464 05a1 02a1 0201 0074 006a 01a0  .|.d.......t.j..
-000018f0: 027c 0364 06a1 027d 0574 03a0 0474 006a  .|.d...}.t...t.j
-00001900: 01a0 0274 0564 0464 07a1 0374 006a 01a0  ...t.d.d...t.j..
-00001910: 027c 0564 07a1 02a1 0201 0064 0853 0029  .|.d.......d.S.)
-00001920: 097a 3543 6f70 7920 676c 6967 6874 626f  .z5Copy glightbo
-00001930: 7822 7320 6373 7320 616e 6420 6a73 2066  x"s css and js f
-00001940: 696c 6573 2074 6f20 6173 7365 7473 2064  iles to assets d
-00001950: 6972 6563 746f 7279 da08 7369 7465 5f64  irectory..site_d
-00001960: 6972 5a06 6173 7365 7473 5a0b 7374 796c  irZ.assetsZ.styl
-00001970: 6573 6865 6574 7372 2a00 0000 7a11 676c  esheetsr*...z.gl
-00001980: 6967 6874 626f 782e 6d69 6e2e 6373 735a  ightbox.min.cssZ
-00001990: 0b6a 6176 6173 6372 6970 7473 7a10 676c  .javascriptsz.gl
-000019a0: 6967 6874 626f 782e 6d69 6e2e 6a73 4e29  ightbox.min.jsN)
-000019b0: 06da 026f 73da 0470 6174 68da 046a 6f69  ...os..path..joi
-000019c0: 6e72 0200 0000 da09 636f 7079 5f66 696c  nr......copy_fil
-000019d0: 65da 0962 6173 655f 7061 7468 2906 7226  e..base_path).r&
-000019e0: 0000 0072 2300 0000 7243 0000 005a 106f  ...r#...rC...Z.o
-000019f0: 7574 7075 745f 6261 7365 5f70 6174 685a  utput_base_pathZ
-00001a00: 0863 7373 5f70 6174 685a 076a 735f 7061  .css_pathZ.js_pa
-00001a10: 7468 7227 0000 0072 2700 0000 7228 0000  thr'...r'...r(..
-00001a20: 00da 0d6f 6e5f 706f 7374 5f62 7569 6c64  ...on_post_build
-00001a30: d000 0000 7316 0000 0000 0312 010e 0104  ....s...........
-00001a40: 010e 010c fe04 040e 0104 010e 010c fe7a  ...............z
-00001a50: 1c4c 6967 6874 626f 7850 6c75 6769 6e2e  .LightboxPlugin.
-00001a60: 6f6e 5f70 6f73 745f 6275 696c 644e 2910  on_post_buildN).
-00001a70: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001a80: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001a90: 6d65 5f5f da07 5f5f 646f 635f 5f72 0300  me__..__doc__r..
-00001aa0: 0000 da04 5479 7065 da04 626f 6f6c da06  ....Type..bool..
-00001ab0: 4368 6f69 6365 da03 7374 72da 046c 6973  Choice..str..lis
-00001ac0: 74da 0d63 6f6e 6669 675f 7363 6865 6d65  t..config_scheme
-00001ad0: 7229 0000 0072 4400 0000 724d 0000 0072  r)...rD...rM...r
-00001ae0: 4600 0000 726c 0000 0072 2700 0000 7227  F...rl...r'...r'
-00001af0: 0000 0072 2700 0000 7228 0000 0072 0500  ...r'...r(...r..
-00001b00: 0000 0e00 0000 7330 0000 0008 0104 0310  ......s0........
-00001b10: 0110 0110 0202 010c fe02 0410 0110 0110  ................
-00001b20: 0110 0110 0110 0202 010c fe02 0410 0110  ................
-00001b30: ed04 1608 0808 4208 1808 4772 0500 0000  ......B...Gr....
-00001b40: 2913 723e 0000 00da 076c 6f67 6769 6e67  ).r>.....logging
-00001b50: 7267 0000 0072 3600 0000 da06 6d6b 646f  rg...r6.....mkdo
-00001b60: 6373 7202 0000 005a 0d6d 6b64 6f63 732e  csr....Z.mkdocs.
-00001b70: 636f 6e66 6967 7203 0000 005a 0e6d 6b64  configr....Z.mkd
-00001b80: 6f63 732e 706c 7567 696e 7372 0400 0000  ocs.pluginsr....
-00001b90: da09 6765 744c 6f67 6765 7272 6d00 0000  ..getLoggerrm...
-00001ba0: 725e 0000 0072 6800 0000 da07 6469 726e  r^...rh.....dirn
-00001bb0: 616d 65da 0761 6273 7061 7468 da08 5f5f  ame..abspath..__
-00001bc0: 6669 6c65 5f5f 726b 0000 0072 0500 0000  file__rk...r....
-00001bd0: 7227 0000 0072 2700 0000 7227 0000 0072  r'...r'...r'...r
-00001be0: 2800 0000 da08 3c6d 6f64 756c 653e 0100  (.....<module>..
-00001bf0: 0000 7312 0000 0008 0108 0108 0108 020c  ..s.............
-00001c00: 010c 010c 020a 0114 03                   .........
+000001c0: 1965 046a 0565 0664 0364 048d 0266 0264  .e.j.e.d.d...f.d
+000001d0: 1a65 046a 0565 0664 0664 048d 0266 0266  .e.j.e.d.d...f.f
+000001e0: 0e5a 0a64 1b64 1c84 005a 0b64 1d64 1e84  .Z.d.d...Z.d.d..
+000001f0: 005a 0c64 1f64 2084 005a 0d64 2164 2284  .Z.d.d ..Z.d!d".
+00000200: 005a 0e64 2364 2484 005a 0f64 2553 0029  .Z.d#d$..Z.d%S.)
+00000210: 26da 0e4c 6967 6874 626f 7850 6c75 6769  &..LightboxPlugi
+00000220: 6e7a 1641 6464 206c 6967 6874 626f 7820  nz.Add lightbox 
+00000230: 746f 204d 6b44 6f63 73da 0f74 6f75 6368  to MkDocs..touch
+00000240: 4e61 7669 6761 7469 6f6e 5429 01da 0764  NavigationT)...d
+00000250: 6566 6175 6c74 da04 6c6f 6f70 46da 0665  efault..loopF..e
+00000260: 6666 6563 7429 03da 047a 6f6f 6dda 0466  ffect)...zoom..f
+00000270: 6164 65da 046e 6f6e 6572 0a00 0000 da0c  ade..noner......
+00000280: 736c 6964 655f 6566 6665 6374 2904 da05  slide_effect)...
+00000290: 736c 6964 6572 0a00 0000 720b 0000 0072  slider....r....r
+000002a0: 0c00 0000 720e 0000 00da 0577 6964 7468  ....r......width
+000002b0: da04 6175 746f da06 6865 6967 6874 da08  ..auto..height..
+000002c0: 7a6f 6f6d 6162 6c65 da09 6472 6167 6761  zoomable..dragga
+000002d0: 626c 65da 0c73 6b69 705f 636c 6173 7365  ble..skip_classe
+000002e0: 73da 0c61 7574 6f5f 6361 7074 696f 6eda  s..auto_caption.
+000002f0: 1063 6170 7469 6f6e 5f70 6f73 6974 696f  .caption_positio
+00000300: 6e29 04da 0662 6f74 746f 6dda 0374 6f70  n)...bottom..top
+00000310: da04 6c65 6674 da05 7269 6768 7472 1700  ..left..rightr..
+00000320: 0000 da0a 6261 636b 6772 6f75 6e64 da05  ....background..
+00000330: 7768 6974 65da 0673 6861 646f 77da 066d  white..shadow..m
+00000340: 616e 7561 6c63 0200 0000 0000 0000 0000  anualc..........
+00000350: 0000 0200 0000 0300 0000 4300 0000 7338  ..........C...s8
+00000360: 0000 007c 0164 0119 006a 0064 026b 027c  ...|.d...j.d.k.|
+00000370: 005f 017c 006a 016f 3064 037c 0164 0419  ._.|.j.o0d.|.d..
+00000380: 0076 006f 307c 0164 0419 0064 0319 006a  .v.o0|.d...d...j
+00000390: 026a 037c 005f 0464 0053 0029 054e da05  .j.|._.d.S.).N..
+000003a0: 7468 656d 65da 086d 6174 6572 6961 6c7a  theme..materialz
+000003b0: 106d 6174 6572 6961 6c2f 7072 6976 6163  .material/privac
+000003c0: 79da 0770 6c75 6769 6e73 2905 da04 6e61  y..plugins)...na
+000003d0: 6d65 da0e 7573 696e 675f 6d61 7465 7269  me..using_materi
+000003e0: 616c da06 636f 6e66 6967 da07 656e 6162  al..config..enab
+000003f0: 6c65 64da 1675 7369 6e67 5f6d 6174 6572  led..using_mater
+00000400: 6961 6c5f 7072 6976 6163 7929 02da 0473  ial_privacy)...s
+00000410: 656c 6672 2400 0000 a900 7228 0000 00fa  elfr$.....r(....
+00000420: 482f 5573 6572 732f 626c 7565 7377 656e  H/Users/blueswen
+00000430: 2f70 726f 6a65 6374 732f 6c61 622f 6d6b  /projects/lab/mk
+00000440: 646f 6373 2d67 6c69 6768 7462 6f78 2f6d  docs-glightbox/m
+00000450: 6b64 6f63 735f 676c 6967 6874 626f 782f  kdocs_glightbox/
+00000460: 706c 7567 696e 2e70 79da 096f 6e5f 636f  plugin.py..on_co
+00000470: 6e66 6967 2800 0000 730c 0000 0000 0110  nfig(...s.......
+00000480: 0206 010a ff02 020e fd7a 184c 6967 6874  .........z.Light
+00000490: 626f 7850 6c75 6769 6e2e 6f6e 5f63 6f6e  boxPlugin.on_con
+000004a0: 6669 6763 0400 0000 0000 0000 0000 0000  figc............
+000004b0: 0c00 0000 0600 0000 0b00 0000 73aa 0100  ............s...
+000004c0: 0064 017c 026a 0076 0072 207c 026a 00a0  .d.|.j.v.r |.j..
+000004d0: 0164 0164 02a1 0264 0375 0072 207c 0153  .d.d...d.u.r |.S
+000004e0: 0074 026a 0364 0474 026a 0464 058d 027d  .t.j.d.t.j.d...}
+000004f0: 0574 026a 0364 0674 026a 0464 058d 027d  .t.j.d.t.j.d...}
+00000500: 0664 0774 05a0 0674 05a0 0764 08a1 017c  .d.t...t...d...|
+00000510: 026a 08a1 029b 0064 099d 037d 077c 05a0  .j.....d...}.|..
+00000520: 0964 0a7c 079b 0064 0b9d 037c 01a1 027d  .d.|...d...|...}
+00000530: 0164 0c7d 087c 0864 0d7c 006a 0a64 0e19  .d.}.|.d.|.j.d..
+00000540: 009b 0064 0f9d 0337 007d 087c 006a 0a64  ...d...7.}.|.j.d
+00000550: 1019 0073 9c7c 0864 1137 007d 087c 0364  ...s.|.d.7.}.|.d
+00000560: 1219 006a 0b64 136b 0272 b27c 0864 1437  ...j.d.k.r.|.d.7
+00000570: 007d 087c 05a0 0964 157c 089b 0064 169d  .}.|...d.|...d..
+00000580: 037c 01a1 027d 0164 1774 05a0 0674 05a0  .|...}.d.t...t..
+00000590: 0764 18a1 017c 026a 08a1 029b 0064 199d  .d...|.j.....d..
+000005a0: 037d 097c 05a0 0964 0a7c 099b 0064 0b9d  .}.|...d.|...d..
+000005b0: 037c 01a1 027d 0174 0c7c 006a 0a83 0189  .|...}.t.|.j....
+000005c0: 0087 0066 0164 1a64 1b84 0864 1c44 0083  ...f.d.d...d.D..
+000005d0: 017d 0a88 00a0 0164 1d64 1ea1 027c 0a64  .}.....d.d...|.d
+000005e0: 1f3c 0088 00a0 0164 1d64 1ea1 027c 0a64  .<.....d.d...|.d
+000005f0: 203c 0088 00a0 0164 2164 22a1 027c 0a64   <.....d!d"..|.d
+00000600: 233c 0064 247d 0b7c 006a 0d90 0172 567c  #<.d$}.|.j...rV|
+00000610: 0b64 2537 007d 0b7c 0b64 2674 0ea0 0f7c  .d%7.}.|.d&t...|
+00000620: 0aa1 019b 0064 279d 0337 007d 0b7c 006a  .....d'..7.}.|.j
+00000630: 1090 0173 8a64 287c 0364 1219 00a0 0164  ...s.d(|.d.....d
+00000640: 2967 00a1 0276 0090 0172 927c 0b64 2a37  )g...v...r.|.d*7
+00000650: 007d 0b7c 06a0 0964 2b7c 0b9b 0064 2c9d  .}.|...d+|...d,.
+00000660: 037c 01a1 027d 017c 0153 0029 2d7a 5441  .|...}.|.S.)-zTA
+00000670: 6464 2063 7373 206c 696e 6b20 7461 672c  dd css link tag,
+00000680: 206a 6176 6173 6372 6970 7420 7363 7269   javascript scri
+00000690: 7074 2074 6167 2c20 616e 6420 6a61 7661  pt tag, and java
+000006a0: 7363 7269 7074 2063 6f64 6520 746f 2069  script code to i
+000006b0: 6e69 7469 616c 697a 6520 474c 6967 6874  nitialize GLight
+000006c0: 626f 78da 0967 6c69 6768 7462 6f78 5446  box..glightboxTF
+000006d0: 7a13 3c68 6561 643e 282e 2a3f 293c 5c2f  z.<head>(.*?)<\/
+000006e0: 6865 6164 3e29 01da 0566 6c61 6773 7a12  head>)...flagsz.
+000006f0: 3c62 6f64 7928 2e2a 3f29 3c5c 2f62 6f64  <body(.*?)<\/bod
+00000700: 793e 7a0c 3c6c 696e 6b20 6872 6566 3d22  y>z.<link href="
+00000710: 7a24 6173 7365 7473 2f73 7479 6c65 7368  z$assets/stylesh
+00000720: 6565 7473 2f67 6c69 6768 7462 6f78 2e6d  eets/glightbox.m
+00000730: 696e 2e63 7373 7a14 2220 7265 6c3d 2273  in.cssz." rel="s
+00000740: 7479 6c65 7368 6565 7422 2f3e 7a09 3c68  tylesheet"/>z.<h
+00000750: 6561 643e 5c31 207a 073c 2f68 6561 643e  ead>\1 z.</head>
+00000760: 7aac 0a20 2020 2068 746d 6c2e 676c 6967  z..    html.glig
+00000770: 6874 626f 782d 6f70 656e 207b 206f 7665  htbox-open { ove
+00000780: 7266 6c6f 773a 2069 6e69 7469 616c 3b20  rflow: initial; 
+00000790: 6865 6967 6874 3a20 3130 3025 3b20 7d0a  height: 100%; }.
+000007a0: 2020 2020 2e67 736c 6964 652d 7469 746c      .gslide-titl
+000007b0: 6520 7b20 6d61 7267 696e 2d74 6f70 3a20  e { margin-top: 
+000007c0: 3070 783b 2075 7365 722d 7365 6c65 6374  0px; user-select
+000007d0: 3a20 7465 7874 3b20 7d0a 2020 2020 2e67  : text; }.    .g
+000007e0: 736c 6964 652d 6465 7363 207b 2063 6f6c  slide-desc { col
+000007f0: 6f72 3a20 2336 3636 3b20 7573 6572 2d73  or: #666; user-s
+00000800: 656c 6563 743a 2074 6578 743b 207d 7a25  elect: text; }z%
+00000810: 0a20 2020 202e 6773 6c69 6465 2d69 6d61  .    .gslide-ima
+00000820: 6765 2069 6d67 207b 2062 6163 6b67 726f  ge img { backgro
+00000830: 756e 643a 2072 1b00 0000 7a03 3b20 7d72  und: r....z.; }r
+00000840: 1d00 0000 7a67 0a20 2020 202e 676c 6967  ....zg.    .glig
+00000850: 6874 626f 782d 636c 6561 6e20 2e67 736c  htbox-clean .gsl
+00000860: 6964 652d 6d65 6469 6120 7b0a 2020 2020  ide-media {.    
+00000870: 2020 2020 2d77 6562 6b69 742d 626f 782d      -webkit-box-
+00000880: 7368 6164 6f77 3a20 6e6f 6e65 3b0a 2020  shadow: none;.  
+00000890: 2020 2020 2020 626f 782d 7368 6164 6f77        box-shadow
+000008a0: 3a20 6e6f 6e65 3b0a 2020 2020 7d72 1f00  : none;.    }r..
+000008b0: 0000 7220 0000 0061 6c01 0000 0a20 2020  ..r ...al....   
+000008c0: 202e 6773 6372 6f6c 6c62 6172 2d66 6978   .gscrollbar-fix
+000008d0: 6572 207b 2070 6164 6469 6e67 2d72 6967  er { padding-rig
+000008e0: 6874 3a20 3135 7078 3b20 7d0a 2020 2020  ht: 15px; }.    
+000008f0: 2e67 6465 7363 2d69 6e6e 6572 207b 2066  .gdesc-inner { f
+00000900: 6f6e 742d 7369 7a65 3a20 302e 3735 7265  ont-size: 0.75re
+00000910: 6d3b 207d 0a20 2020 2062 6f64 795b 6461  m; }.    body[da
+00000920: 7461 2d6d 642d 636f 6c6f 722d 7363 6865  ta-md-color-sche
+00000930: 6d65 3d22 736c 6174 6522 5d20 2e67 6465  me="slate"] .gde
+00000940: 7363 2d69 6e6e 6572 207b 2062 6163 6b67  sc-inner { backg
+00000950: 726f 756e 643a 2076 6172 282d 2d6d 642d  round: var(--md-
+00000960: 6465 6661 756c 742d 6267 2d63 6f6c 6f72  default-bg-color
+00000970: 293b 7d0a 2020 2020 626f 6479 5b64 6174  );}.    body[dat
+00000980: 612d 6d64 2d63 6f6c 6f72 2d73 6368 656d  a-md-color-schem
+00000990: 653d 2273 6c61 7465 225d 202e 6773 6c69  e="slate"] .gsli
+000009a0: 6465 2d74 6974 6c65 207b 2063 6f6c 6f72  de-title { color
+000009b0: 3a20 7661 7228 2d2d 6d64 2d64 6566 6175  : var(--md-defau
+000009c0: 6c74 2d66 672d 636f 6c6f 7229 3b7d 0a20  lt-fg-color);}. 
+000009d0: 2020 2062 6f64 795b 6461 7461 2d6d 642d     body[data-md-
+000009e0: 636f 6c6f 722d 7363 6865 6d65 3d22 736c  color-scheme="sl
+000009f0: 6174 6522 5d20 2e67 736c 6964 652d 6465  ate"] .gslide-de
+00000a00: 7363 207b 2063 6f6c 6f72 3a20 7661 7228  sc { color: var(
+00000a10: 2d2d 6d64 2d64 6566 6175 6c74 2d66 672d  --md-default-fg-
+00000a20: 636f 6c6f 7229 3b7d 7a0f 3c68 6561 643e  color);}z.<head>
+00000a30: 5c31 3c73 7479 6c65 3e7a 0f3c 2f73 7479  \1<style>z.</sty
+00000a40: 6c65 3e3c 2f68 6561 643e 7a0d 3c73 6372  le></head>z.<scr
+00000a50: 6970 7420 7372 633d 227a 2361 7373 6574  ipt src="z#asset
+00000a60: 732f 6a61 7661 7363 7269 7074 732f 676c  s/javascripts/gl
+00000a70: 6967 6874 626f 782e 6d69 6e2e 6a73 7a0b  ightbox.min.jsz.
+00000a80: 223e 3c2f 7363 7269 7074 3e63 0100 0000  "></script>c....
+00000a90: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00000aa0: 1300 0000 7316 0000 0069 007c 005d 0e7d  ....s....i.|.].}
+00000ab0: 017c 0188 007c 0119 0093 0271 0453 0072  .|...|.....q.S.r
+00000ac0: 2800 0000 7228 0000 00a9 02da 022e 30da  (...r(........0.
+00000ad0: 016b a901 da0d 706c 7567 696e 5f63 6f6e  .k....plugin_con
+00000ae0: 6669 6772 2800 0000 7229 0000 00da 0a3c  figr(...r).....<
+00000af0: 6469 6374 636f 6d70 3e5a 0000 0073 0400  dictcomp>Z...s..
+00000b00: 0000 0602 02ff 7a2f 4c69 6768 7462 6f78  ......z/Lightbox
+00000b10: 506c 7567 696e 2e6f 6e5f 706f 7374 5f70  Plugin.on_post_p
+00000b20: 6167 652e 3c6c 6f63 616c 733e 2e3c 6469  age.<locals>.<di
+00000b30: 6374 636f 6d70 3e29 0472 0600 0000 7208  ctcomp>).r....r.
+00000b40: 0000 0072 1200 0000 7213 0000 0072 0900  ...r....r....r..
+00000b50: 0000 720a 0000 005a 0a6f 7065 6e45 6666  ..r....Z.openEff
+00000b60: 6563 745a 0b63 6c6f 7365 4566 6665 6374  ectZ.closeEffect
+00000b70: 720d 0000 0072 0e00 0000 5a0b 736c 6964  r....r....Z.slid
+00000b80: 6545 6666 6563 74da 0061 7401 0000 646f  eEffect..at...do
+00000b90: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
+00000ba0: 6374 6f72 416c 6c28 272e 676c 6967 6874  ctorAll('.glight
+00000bb0: 626f 7827 292e 666f 7245 6163 6828 6675  box').forEach(fu
+00000bc0: 6e63 7469 6f6e 2865 6c65 6d65 6e74 2920  nction(element) 
+00000bd0: 7b0a 2020 2020 7472 7920 7b0a 2020 2020  {.    try {.    
+00000be0: 2020 2020 7661 7220 696d 6720 3d20 656c      var img = el
+00000bf0: 656d 656e 742e 7175 6572 7953 656c 6563  ement.querySelec
+00000c00: 746f 7228 2769 6d67 2729 3b0a 2020 2020  tor('img');.    
+00000c10: 2020 2020 6966 2028 696d 6720 2626 2069      if (img && i
+00000c20: 6d67 2e73 7263 2920 7b0a 2020 2020 2020  mg.src) {.      
+00000c30: 2020 2020 2020 656c 656d 656e 742e 7365        element.se
+00000c40: 7441 7474 7269 6275 7465 2827 6872 6566  tAttribute('href
+00000c50: 272c 2069 6d67 2e73 7263 293b 0a20 2020  ', img.src);.   
+00000c60: 2020 2020 207d 2065 6c73 6520 7b0a 2020       } else {.  
+00000c70: 2020 2020 2020 2020 2020 636f 6e73 6f6c            consol
+00000c80: 652e 6c6f 6728 274e 6f20 696d 6720 656c  e.log('No img el
+00000c90: 656d 656e 7420 7769 7468 2073 7263 2061  ement with src a
+00000ca0: 7474 7269 6275 7465 2066 6f75 6e64 2729  ttribute found')
+00000cb0: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
+00000cc0: 7d20 6361 7463 6820 2865 7272 6f72 2920  } catch (error) 
+00000cd0: 7b0a 2020 2020 2020 2020 636f 6e73 6f6c  {.        consol
+00000ce0: 652e 6c6f 6728 2745 7272 6f72 3a27 2c20  e.log('Error:', 
+00000cf0: 6572 726f 7229 3b0a 2020 2020 7d0a 7d29  error);.    }.})
+00000d00: 3b0a 7a1b 636f 6e73 7420 6c69 6768 7462  ;.z.const lightb
+00000d10: 6f78 203d 2047 4c69 6768 7462 6f78 287a  ox = GLightbox(z
+00000d20: 0329 3b0a 7a12 6e61 7669 6761 7469 6f6e  .);.z.navigation
+00000d30: 2e69 6e73 7461 6e74 da08 6665 6174 7572  .instant..featur
+00000d40: 6573 7a32 646f 6375 6d65 6e74 242e 7375  esz2document$.su
+00000d50: 6273 6372 6962 6528 2829 203d 3e20 7b20  bscribe(() => { 
+00000d60: 6c69 6768 7462 6f78 2e72 656c 6f61 6428  lightbox.reload(
+00000d70: 2920 7d29 3b0a 7a23 3c62 6f64 795c 313c  ) });.z#<body\1<
+00000d80: 7363 7269 7074 2069 643d 2269 6e69 742d  script id="init-
+00000d90: 676c 6967 6874 626f 7822 3e7a 103c 2f73  glightbox">z.</s
+00000da0: 6372 6970 743e 3c2f 626f 6479 3e29 11da  cript></body>)..
+00000db0: 046d 6574 61da 0367 6574 da02 7265 da07  .meta..get..re..
+00000dc0: 636f 6d70 696c 65da 0644 4f54 414c 4c72  compile..DOTALLr
+00000dd0: 0200 0000 da10 6765 745f 7265 6c61 7469  ......get_relati
+00000de0: 7665 5f75 726c da0d 6e6f 726d 616c 697a  ve_url..normaliz
+00000df0: 655f 7572 6cda 0375 726c da03 7375 6272  e_url..url..subr
+00000e00: 2400 0000 7222 0000 00da 0464 6963 7472  $...r".....dictr
+00000e10: 2600 0000 da04 6a73 6f6e da05 6475 6d70  &.....json..dump
+00000e20: 7372 2300 0000 290c 7227 0000 00da 066f  sr#...).r'.....o
+00000e30: 7574 7075 74da 0470 6167 6572 2400 0000  utput..pager$...
+00000e40: da06 6b77 6172 6773 5a0a 6865 6164 5f72  ..kwargsZ.head_r
+00000e50: 6567 6578 5a0a 626f 6479 5f72 6567 6578  egexZ.body_regex
+00000e60: 5a08 6373 735f 6c69 6e6b 5a09 6373 735f  Z.css_linkZ.css_
+00000e70: 7061 7463 685a 096a 735f 7363 7269 7074  patchZ.js_script
+00000e80: 5a09 6c62 5f63 6f6e 6669 675a 076a 735f  Z.lb_configZ.js_
+00000e90: 636f 6465 7228 0000 0072 3000 0000 7229  coder(...r0...r)
+00000ea0: 0000 00da 0c6f 6e5f 706f 7374 5f70 6167  .....on_post_pag
+00000eb0: 6530 0000 0073 4800 0000 0003 1c01 0403  e0...sH.........
+00000ec0: 1001 1003 1c01 1403 0404 0401 08ff 0a02  ................
+00000ed0: 0a01 0805 0e01 0806 1403 1c01 1403 0a01  ................
+00000ee0: 0a02 02fe 0604 1001 1001 1001 0401 0801  ................
+00000ef0: 080d 1601 1201 04ff 0804 0801 0401 0cff  ................
+00000f00: 0404 7a1b 4c69 6768 7462 6f78 506c 7567  ..z.LightboxPlug
+00000f10: 696e 2e6f 6e5f 706f 7374 5f70 6167 6563  in.on_post_pagec
+00000f20: 0400 0000 0000 0000 0000 0000 0600 0000  ................
+00000f30: 0600 0000 0b00 0000 7376 0000 0064 0188  ........sv...d..
+00000f40: 006a 0076 0072 2088 006a 00a0 0164 0164  .j.v.r ..j...d.d
+00000f50: 02a1 0264 0375 0072 207c 0153 0087 0266  ...d.u.r |.S...f
+00000f60: 0164 0464 0584 0864 0644 0083 0189 0167  .d.d...d.D.....g
+00000f70: 0064 07a2 0189 0388 0364 0867 0188 026a  .d.......d.g...j
+00000f80: 0264 0919 0017 0037 0089 0374 03a0 0464  .d.....7...t...d
+00000f90: 0aa1 017d 057c 05a0 0587 0087 0187 0287  ...}.|..........
+00000fa0: 0366 0464 0b64 0c84 087c 01a1 027d 017c  .f.d.d...|...}.|
+00000fb0: 0153 0029 0d7a 4c57 7261 7020 696d 6720  .S.).zLWrap img 
+00000fc0: 7461 6720 7769 7468 2061 6e63 686f 7220  tag with anchor 
+00000fd0: 7461 6720 7769 7468 2067 6c69 6768 7462  tag with glightb
+00000fe0: 6f78 2063 6c61 7373 2061 6e64 2061 7474  ox class and att
+00000ff0: 7269 6275 7465 7320 6672 6f6d 2063 6f6e  ributes from con
+00001000: 6669 6772 2b00 0000 5446 6301 0000 0000  figr+...TFc.....
+00001010: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00001020: 0000 0073 1c00 0000 6900 7c00 5d14 7d01  ...s....i.|.].}.
+00001030: 7c01 7400 8800 6a01 8301 7c01 1900 9302  |.t...j...|.....
+00001040: 7104 5300 7228 0000 0029 0272 3e00 0000  q.S.r(...).r>...
+00001050: 7224 0000 0072 2d00 0000 2901 7227 0000  r$...r-...).r'..
+00001060: 0072 2800 0000 7229 0000 0072 3200 0000  .r(...r)...r2...
+00001070: 8100 0000 f300 0000 007a 324c 6967 6874  .........z2Light
+00001080: 626f 7850 6c75 6769 6e2e 6f6e 5f70 6167  boxPlugin.on_pag
+00001090: 655f 636f 6e74 656e 742e 3c6c 6f63 616c  e_content.<local
+000010a0: 733e 2e3c 6469 6374 636f 6d70 3e29 0272  s>.<dictcomp>).r
+000010b0: 0f00 0000 7211 0000 0029 035a 0865 6d6f  ....r....).Z.emo
+000010c0: 6a69 6f6e 655a 0774 7765 6d6f 6a69 5a06  jioneZ.twemojiZ.
+000010d0: 6765 6d6f 6a69 7a07 6f66 662d 676c 6272  gemojiz.off-glbr
+000010e0: 1400 0000 7a51 3c61 5c62 5b5e 3e5d 2a3e  ....zQ<a\b[^>]*>
+000010f0: 283f 3a5c 732a 3c5b 5e3e 5d2b 3e5c 732a  (?:\s*<[^>]+>\s*
+00001100: 292a 3c69 6d67 5c62 5b5e 3e5d 2a3e 283f  )*<img\b[^>]*>(?
+00001110: 3a5c 732a 3c5b 5e3e 5d2b 3e5c 732a 292a  :\s*<[^>]+>\s*)*
+00001120: 3c2f 613e 7c3c 696d 6728 3f50 3c61 7474  </a>|<img(?P<att
+00001130: 723e 2e2a 3f29 3e63 0100 0000 0000 0000  r>.*?)>c........
+00001140: 0000 0000 0100 0000 0600 0000 1300 0000  ................
+00001150: 7312 0000 0088 02a0 007c 0088 0188 0388  s........|......
+00001160: 006a 01a1 0453 0029 014e 2902 da14 7772  .j...S.).N)...wr
+00001170: 6170 5f69 6d67 5f77 6974 685f 616e 6368  ap_img_with_anch
+00001180: 6f72 7235 0000 0029 01da 056d 6174 6368  orr5...)...match
+00001190: a904 7242 0000 0072 3100 0000 7227 0000  ..rB...r1...r'..
+000011a0: 00da 0a73 6b69 705f 636c 6173 7372 2800  ...skip_classr(.
+000011b0: 0000 7229 0000 00da 083c 6c61 6d62 6461  ..r).....<lambda
+000011c0: 3e8c 0000 0073 0400 0000 0401 0aff 7a30  >....s........z0
+000011d0: 4c69 6768 7462 6f78 506c 7567 696e 2e6f  LightboxPlugin.o
+000011e0: 6e5f 7061 6765 5f63 6f6e 7465 6e74 2e3c  n_page_content.<
+000011f0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00001200: 2906 7235 0000 0072 3600 0000 7224 0000  ).r5...r6...r$..
+00001210: 0072 3700 0000 7238 0000 0072 3d00 0000  .r7...r8...r=...
+00001220: 2906 7227 0000 00da 0468 746d 6c72 4200  ).r'.....htmlrB.
+00001230: 0000 7224 0000 0072 4300 0000 da07 7061  ..r$...rC.....pa
+00001240: 7474 6572 6e72 2800 0000 7248 0000 0072  tternr(...rH...r
+00001250: 2900 0000 da0f 6f6e 5f70 6167 655f 636f  ).....on_page_co
+00001260: 6e74 656e 747c 0000 0073 1a00 0000 0003  ntent|...s......
+00001270: 1c01 0401 1202 0802 1403 0401 02ff 0403  ................
+00001280: 0401 1003 02fc 0407 7a1e 4c69 6768 7462  ........z.Lightb
+00001290: 6f78 506c 7567 696e 2e6f 6e5f 7061 6765  oxPlugin.on_page
+000012a0: 5f63 6f6e 7465 6e74 6305 0000 0000 0000  _contentc.......
+000012b0: 0000 0000 0012 0000 000b 0000 0043 0000  .............C..
+000012c0: 0073 ba02 0000 9002 7a66 7400 a001 6401  .s......zft...d.
+000012d0: a101 7d05 7c05 a002 7c01 a003 6402 a101  ..}.|...|...d...
+000012e0: a101 722a 7c01 a003 6402 a101 5700 5300  ..r*|...d...W.S.
+000012f0: 7c01 a003 6402 a101 7d06 7c01 a003 6403  |...d...}.|...d.
+00001300: a101 7d07 7400 a004 6404 7c07 a102 7d08  ..}.t...d.|...}.
+00001310: 6405 6406 8400 7c08 4400 8301 7d08 7c00  d.d...|.D...}.|.
+00001320: 6a05 6407 1900 728a 7c04 a006 6408 6409  j.d...r.|...d.d.
+00001330: a102 640a 7500 728a 7407 7c03 8301 7407  ..d.u.r.t.|...t.
+00001340: 7c08 8301 4000 72c6 7c06 5700 5300 6e3c  |...@.r.|.W.S.n<
+00001350: 7c04 a006 640b 640c a102 73a0 7c00 6a05  |...d.d...s.|.j.
+00001360: 6407 1900 72b0 640d 7c08 7601 72c6 7c06  d...r.d.|.v.r.|.
+00001370: 5700 5300 6e16 7407 7c03 8301 7407 7c08  W.S.n.t.|...t.|.
+00001380: 8301 4000 72c6 7c06 5700 5300 7c00 6a08  ..@.r.|.W.S.|.j.
+00001390: 72d2 640e 7d09 6e1e 7400 a009 640f 7c07  r.d.}.n.t...d.|.
+000013a0: a102 a003 6410 a101 7d0a 6411 7c0a 9b00  ....d...}.d.|...
+000013b0: 6412 9d03 7d09 7c02 a00a a100 4400 5d1e  d...}.|.....D.].
+000013c0: 5c02 7d0b 7d0c 7c09 6413 7c0b 9b00 6414  \.}.}.|.d.|...d.
+000013d0: 7c0c 9b00 6415 9d05 3700 7d09 71f8 6700  |...d...7.}.q.g.
+000013e0: 6416 a201 7d0d 7c0d 4400 9001 5d2c 7d0e  d...}.|.D...],}.
+000013f0: 6417 7c0e 9b00 9d02 7d0f 7c0f 6418 6b02  d.|.....}.|.d.k.
+00001400: 9001 72bc 7400 a009 6419 7c07 a102 7d10  ..r.t...d.|...}.
+00001410: 7c00 6a05 641a 1900 9001 7372 641b 7c04  |.j.d.....srd.|.
+00001420: 7600 9001 72a6 7c04 a006 641b 640c a102  v...r.|...d.d...
+00001430: 640a 7500 9001 72a6 7c10 9001 7284 7c10  d.u...r.|...r.|.
+00001440: a003 6410 a101 7d10 6e20 7400 a009 641c  ..d...}.n t...d.
+00001450: 7c07 a102 7d10 7c10 9001 72a0 7c10 a003  |...}.|...r.|...
+00001460: 6410 a101 6e02 641d 7d10 6e14 7c10 9001  d...n.d.}.n.|...
+00001470: 72b6 7c10 a003 6410 a101 6e02 641d 7d10  r.|...d...n.d.}.
+00001480: 6e58 7c0f 641e 6b02 9001 72ee 7400 a009  nX|.d.k...r.t...
+00001490: 641f 7c07 a102 7d10 7c10 9001 72e2 7c10  d.|...}.|...r.|.
+000014a0: a003 6410 a101 6e08 7c00 6a05 6420 1900  ..d...n.|.j.d ..
+000014b0: 7d10 6e26 7400 a009 7c0f 9b00 6421 9d02  }.n&t...|...d!..
+000014c0: 7c07 a102 7d10 7c10 9002 7210 7c10 a003  |...}.|...r.|...
+000014d0: 6410 a101 6e02 641d 7d10 7c10 641d 6b03  d...n.d.}.|.d.k.
+000014e0: 9001 7224 7c0f 641e 6b02 9002 723a 7c09  ..r$|.d.k...r:|.
+000014f0: 6422 7c10 9b00 6415 9d03 3700 7d09 6e16  d"|...d...7.}.n.
+00001500: 7c09 6423 7c0f 9b00 6414 7c10 9b00 6415  |.d#|...d.|...d.
+00001510: 9d05 3700 7d09 9001 7124 7c09 6424 7c06  ..7.}...q$|.d$|.
+00001520: 9b00 6425 9d03 3700 7d09 7c09 5700 5300  ..d%..7.}.|.W.S.
+00001530: 0400 740b 9002 79b4 0100 7d11 0100 7a32  ..t...y...}...z2
+00001540: 740c a00d 6426 7c11 9b00 6423 7c01 a003  t...d&|...d#|...
+00001550: 6402 a101 9b00 9d04 a101 0100 7c01 a003  d...........|...
+00001560: 6402 a101 5700 0600 5900 6409 7d11 7e11  d...W...Y.d.}.~.
+00001570: 5300 6409 7d11 7e11 3000 3000 6409 5300  S.d.}.~.0.0.d.S.
+00001580: 2927 7a20 5772 6170 2069 6d61 6765 2074  )'z Wrap image t
+00001590: 6167 7320 7769 7468 2061 6e63 686f 7220  ags with anchor 
+000015a0: 7461 6773 7a10 3c61 283f 503c 6174 7472  tagsz.<a(?P<attr
+000015b0: 3e2e 2a3f 293e 7201 0000 00da 0461 7474  >.*?)>r......att
+000015c0: 727a 0f63 6c61 7373 3d22 285b 5e22 5d2b  rz.class="([^"]+
+000015d0: 2922 6301 0000 0000 0000 0000 0000 0003  )"c.............
+000015e0: 0000 0004 0000 0053 0000 0073 1e00 0000  .......S...s....
+000015f0: 6700 7c00 5d16 7d01 7c01 a000 a100 4400  g.|.].}.|.....D.
+00001600: 5d08 7d02 7c02 9103 7110 7104 5300 7228  ].}.|...q.q.S.r(
+00001610: 0000 0029 01da 0573 706c 6974 2903 722e  ...)...split).r.
+00001620: 0000 0072 4700 0000 da01 6372 2800 0000  ...rG.....cr(...
+00001630: 7228 0000 0072 2900 0000 da0a 3c6c 6973  r(...r).....<lis
+00001640: 7463 6f6d 703e 9e00 0000 7245 0000 007a  tcomp>....rE...z
+00001650: 374c 6967 6874 626f 7850 6c75 6769 6e2e  7LightboxPlugin.
+00001660: 7772 6170 5f69 6d67 5f77 6974 685f 616e  wrap_img_with_an
+00001670: 6368 6f72 2e3c 6c6f 6361 6c73 3e2e 3c6c  chor.<locals>.<l
+00001680: 6973 7463 6f6d 703e 721e 0000 0072 2b00  istcomp>r....r+.
+00001690: 0000 4e54 7a10 676c 6967 6874 626f 782d  ..NTz.glightbox-
+000016a0: 6d61 6e75 616c 467a 066f 6e2d 676c 627a  manualFz.on-glbz
+000016b0: 263c 6120 636c 6173 733d 2267 6c69 6768  &<a class="gligh
+000016c0: 7462 6f78 2220 6461 7461 2d74 7970 653d  tbox" data-type=
+000016d0: 2269 6d61 6765 227a 1473 7263 3d5b 5c22  "image"z.src=[\"
+000016e0: 5c27 5d28 5b5e 5c22 5c27 5d2b 29e9 0100  \']([^\"\']+)...
+000016f0: 0000 7a1b 3c61 2063 6c61 7373 3d22 676c  ..z.<a class="gl
+00001700: 6967 6874 626f 7822 2068 7265 663d 227a  ightbox" href="z
+00001710: 1322 2064 6174 612d 7479 7065 3d22 696d  ." data-type="im
+00001720: 6167 6522 7a06 2064 6174 612d 7a02 3d22  age"z. data-z.="
+00001730: fa01 2229 04da 0574 6974 6c65 da0b 6465  ..")...title..de
+00001740: 7363 7269 7074 696f 6e7a 1063 6170 7469  scriptionz.capti
+00001750: 6f6e 2d70 6f73 6974 696f 6e5a 0767 616c  on-positionZ.gal
+00001760: 6c65 7279 7a05 6461 7461 2d7a 0a64 6174  leryz.data-z.dat
+00001770: 612d 7469 746c 657a 1764 6174 612d 7469  a-titlez.data-ti
+00001780: 746c 653d 5b5c 225d 285b 5e5c 225d 2b29  tle=[\"]([^\"]+)
+00001790: 7215 0000 007a 1667 6c69 6768 7462 6f78  r....z.glightbox
+000017a0: 2e61 7574 6f5f 6361 7074 696f 6e7a 1061  .auto_captionz.a
+000017b0: 6c74 3d5b 5c22 5d28 5b5e 5c22 5d2b 2972  lt=[\"]([^\"]+)r
+000017c0: 3300 0000 7a15 6461 7461 2d63 6170 7469  3...z.data-capti
+000017d0: 6f6e 2d70 6f73 6974 696f 6e7a 2264 6174  on-positionz"dat
+000017e0: 612d 6361 7074 696f 6e2d 706f 7369 7469  a-caption-positi
+000017f0: 6f6e 3d5b 5c22 5d28 5b5e 5c22 5d2b 2972  on=[\"]([^\"]+)r
+00001800: 1600 0000 7a0b 3d5b 225d 285b 5e22 5d2b  ....z.=["]([^"]+
+00001810: 297a 1520 6461 7461 2d64 6573 632d 706f  )z. data-desc-po
+00001820: 7369 7469 6f6e 3d22 fa01 20fa 013e 7a04  sition=".. ..>z.
+00001830: 3c2f 613e 7a2b 4572 726f 7220 696e 2077  </a>z+Error in w
+00001840: 7261 7070 696e 6720 696d 6720 7461 6720  rapping img tag 
+00001850: 7769 7468 2061 6e63 686f 7220 7461 673a  with anchor tag:
+00001860: 2029 0e72 3700 0000 7238 0000 0072 4700   ).r7...r8...rG.
+00001870: 0000 da05 6772 6f75 70da 0766 696e 6461  ....group..finda
+00001880: 6c6c 7224 0000 0072 3600 0000 da03 7365  llr$...r6.....se
+00001890: 7472 2600 0000 da06 7365 6172 6368 da05  tr&.....search..
+000018a0: 6974 656d 73da 0945 7863 6570 7469 6f6e  items..Exception
+000018b0: da03 6c6f 67da 0777 6172 6e69 6e67 2912  ..log..warning).
+000018c0: 7227 0000 0072 4700 0000 7231 0000 0072  r'...rG...r1...r
+000018d0: 4900 0000 7235 0000 005a 0961 5f70 6174  I...r5...Z.a_pat
+000018e0: 7465 726e 5a07 696d 675f 7461 675a 0869  ternZ.img_tagZ.i
+000018f0: 6d67 5f61 7474 72da 0763 6c61 7373 6573  mg_attr..classes
+00001900: 5a05 615f 7461 67da 0373 7263 722f 0000  Z.a_tag..srcr/..
+00001910: 00da 0176 5a0d 736c 6964 655f 6f70 7469  ...vZ.slide_opti
+00001920: 6f6e 73da 066f 7074 696f 6e72 4e00 0000  ons..optionrN...
+00001930: da03 7661 6cda 0165 7228 0000 0072 2800  ..val..er(...r(.
+00001940: 0000 7229 0000 0072 4600 0000 9400 0000  ..r)...rF.......
+00001950: 736a 0000 0000 0204 010a 0110 010c 020a  sj..............
+00001960: 010a 010c 010e 021a 0210 0208 0116 0208  ................
+00001970: 0208 0110 0206 0206 0206 0212 010c 0210  ................
+00001980: 0118 0108 060a 010a 010a 010c 010c 0106  ................
+00001990: ff04 020e fe04 0406 010c 020c 0116 0216  ................
+000019a0: 010a 010c 011c 0212 0114 030a 020a 0112  ................
+000019b0: 021a 0110 0106 0110 0104 0114 ff04 037a  ...............z
+000019c0: 234c 6967 6874 626f 7850 6c75 6769 6e2e  #LightboxPlugin.
+000019d0: 7772 6170 5f69 6d67 5f77 6974 685f 616e  wrap_img_with_an
+000019e0: 6368 6f72 6302 0000 0000 0000 0000 0000  chorc...........
+000019f0: 0006 0000 0007 0000 004b 0000 0073 7600  .........K...sv.
+00001a00: 0000 7400 6a01 a002 7c01 6401 1900 6402  ..t.j...|.d...d.
+00001a10: a102 7d03 7400 6a01 a002 7c03 6403 a102  ..}.t.j...|.d...
+00001a20: 7d04 7403 a004 7400 6a01 a002 7405 6404  }.t...t.j...t.d.
+00001a30: 6405 a103 7400 6a01 a002 7c04 6405 a102  d...t.j...|.d...
+00001a40: a102 0100 7400 6a01 a002 7c03 6406 a102  ....t.j...|.d...
+00001a50: 7d05 7403 a004 7400 6a01 a002 7405 6404  }.t...t.j...t.d.
+00001a60: 6407 a103 7400 6a01 a002 7c05 6407 a102  d...t.j...|.d...
+00001a70: a102 0100 6408 5300 2909 7a35 436f 7079  ....d.S.).z5Copy
+00001a80: 2067 6c69 6768 7462 6f78 2273 2063 7373   glightbox"s css
+00001a90: 2061 6e64 206a 7320 6669 6c65 7320 746f   and js files to
+00001aa0: 2061 7373 6574 7320 6469 7265 6374 6f72   assets director
+00001ab0: 79da 0873 6974 655f 6469 725a 0661 7373  y..site_dirZ.ass
+00001ac0: 6574 735a 0b73 7479 6c65 7368 6565 7473  etsZ.stylesheets
+00001ad0: 722b 0000 007a 1167 6c69 6768 7462 6f78  r+...z.glightbox
+00001ae0: 2e6d 696e 2e63 7373 5a0b 6a61 7661 7363  .min.cssZ.javasc
+00001af0: 7269 7074 737a 1067 6c69 6768 7462 6f78  riptsz.glightbox
+00001b00: 2e6d 696e 2e6a 734e 2906 da02 6f73 da04  .min.jsN)...os..
+00001b10: 7061 7468 da04 6a6f 696e 7202 0000 00da  path..joinr.....
+00001b20: 0963 6f70 795f 6669 6c65 da09 6261 7365  .copy_file..base
+00001b30: 5f70 6174 6829 0672 2700 0000 7224 0000  _path).r'...r$..
+00001b40: 0072 4300 0000 5a10 6f75 7470 7574 5f62  .rC...Z.output_b
+00001b50: 6173 655f 7061 7468 5a08 6373 735f 7061  ase_pathZ.css_pa
+00001b60: 7468 5a07 6a73 5f70 6174 6872 2800 0000  thZ.js_pathr(...
+00001b70: 7228 0000 0072 2900 0000 da0d 6f6e 5f70  r(...r).....on_p
+00001b80: 6f73 745f 6275 696c 64e2 0000 0073 1600  ost_build....s..
+00001b90: 0000 0003 1201 0e01 0401 0e01 0cfe 0404  ................
+00001ba0: 0e01 0401 0e01 0cfe 7a1c 4c69 6768 7462  ........z.Lightb
+00001bb0: 6f78 506c 7567 696e 2e6f 6e5f 706f 7374  oxPlugin.on_post
+00001bc0: 5f62 7569 6c64 4e29 10da 085f 5f6e 616d  _buildN)...__nam
+00001bd0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00001be0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00001bf0: 5f64 6f63 5f5f 7203 0000 00da 0454 7970  _doc__r......Typ
+00001c00: 65da 0462 6f6f 6cda 0643 686f 6963 65da  e..bool..Choice.
+00001c10: 0373 7472 da04 6c69 7374 da0d 636f 6e66  .str..list..conf
+00001c20: 6967 5f73 6368 656d 6572 2a00 0000 7244  ig_schemer*...rD
+00001c30: 0000 0072 4d00 0000 7246 0000 0072 6c00  ...rM...rF...rl.
+00001c40: 0000 7228 0000 0072 2800 0000 7228 0000  ..r(...r(...r(..
+00001c50: 0072 2900 0000 7205 0000 000e 0000 0073  .r)...r........s
+00001c60: 3200 0000 0801 0403 1001 1001 1002 0201  2...............
+00001c70: 0cfe 0204 1001 1001 1001 1001 1001 1002  ................
+00001c80: 0201 0cfe 0204 1001 1001 10ec 0417 0808  ................
+00001c90: 084c 0818 084e 7205 0000 0029 1372 3f00  .L...Nr....).r?.
+00001ca0: 0000 da07 6c6f 6767 696e 6772 6700 0000  ....loggingrg...
+00001cb0: 7237 0000 00da 066d 6b64 6f63 7372 0200  r7.....mkdocsr..
+00001cc0: 0000 5a0d 6d6b 646f 6373 2e63 6f6e 6669  ..Z.mkdocs.confi
+00001cd0: 6772 0300 0000 5a0e 6d6b 646f 6373 2e70  gr....Z.mkdocs.p
+00001ce0: 6c75 6769 6e73 7204 0000 00da 0967 6574  luginsr......get
+00001cf0: 4c6f 6767 6572 726d 0000 0072 5e00 0000  Loggerrm...r^...
+00001d00: 7268 0000 00da 0764 6972 6e61 6d65 da07  rh.....dirname..
+00001d10: 6162 7370 6174 68da 085f 5f66 696c 655f  abspath..__file_
+00001d20: 5f72 6b00 0000 7205 0000 0072 2800 0000  _rk...r....r(...
+00001d30: 7228 0000 0072 2800 0000 7229 0000 00da  r(...r(...r)....
+00001d40: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
+00001d50: 0000 0801 0801 0801 0802 0c01 0c01 0c02  ................
+00001d60: 0a01 1403                                ....
```

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/LICENSE.md` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/glightbox.min.css` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox/glightbox/glightbox.min.js` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox/glightbox/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox/plugin.py` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         ("auto_caption", config_options.Type(bool, default=False)),
         (
             "caption_position",
             config_options.Choice(("bottom", "top", "left", "right"), default="bottom"),
         ),
         ("background", config_options.Type(str, default="white")),
         ("shadow", config_options.Type(bool, default=True)),
+        ("manual", config_options.Type(bool, default=False)),
     )
 
     def on_config(self, config):
         self.using_material = config["theme"].name == "material"
         self.using_material_privacy = (
             self.using_material
             and "material/privacy" in config["plugins"]
@@ -92,25 +93,35 @@
         }
         lb_config["openEffect"] = plugin_config.get("effect", "zoom")
         lb_config["closeEffect"] = plugin_config.get("effect", "zoom")
         lb_config["slideEffect"] = plugin_config.get("slide_effect", "slide")
         js_code = ""
         if self.using_material_privacy:
             js_code += """document.querySelectorAll('.glightbox').forEach(function(element) {
-    var imgSrc = element.querySelector('img').src;
-    element.setAttribute('href', imgSrc);
+    try {
+        var img = element.querySelector('img');
+        if (img && img.src) {
+            element.setAttribute('href', img.src);
+        } else {
+            console.log('No img element with src attribute found');
+        }
+    } catch (error) {
+        console.log('Error:', error);
+    }
 });
 """
-        js_code += f"const lightbox = GLightbox({json.dumps(lb_config)});"
-        if self.using_material or "navigation.instant" in config["theme"]._vars.get(
+        js_code += f"const lightbox = GLightbox({json.dumps(lb_config)});\n"
+        if self.using_material or "navigation.instant" in config["theme"].get(
             "features", []
         ):
             # support compatible with mkdocs-material Instant loading feature
-            js_code = "document$.subscribe(() => {" + js_code + "})"
-        output = body_regex.sub(f"<body\\1<script>{js_code}</script></body>", output)
+            js_code += "document$.subscribe(() => { lightbox.reload() });\n"
+        output = body_regex.sub(
+            f'<body\\1<script id="init-glightbox">{js_code}</script></body>', output
+        )
 
         return output
 
     def on_page_content(self, html, page, config, **kwargs):
         """Wrap img tag with anchor tag with glightbox class and attributes from config"""
         # skip page with meta glightbox is false
         if "glightbox" in page.meta and page.meta.get("glightbox", True) is False:
@@ -142,20 +153,27 @@
                 return match.group(0)
 
             img_tag = match.group(0)
             img_attr = match.group("attr")
             classes = re.findall(r'class="([^"]+)"', img_attr)
             classes = [c for match in classes for c in match.split()]
 
-            if meta.get("glightbox-manual", False):
-                if "on-glb" not in classes:
-                    return img_tag
-            else:
+            if self.config["manual"] and meta.get("glightbox", None) is True:
+                # with manual mode but enable glightbox in page meta
                 if set(skip_class) & set(classes):
+                    # skip image with off-glb and specific class
+                    return img_tag
+            elif meta.get("glightbox-manual", False) or self.config["manual"]:
+                # disable by page meta or global config
+                if "on-glb" not in classes:
+                    # skip image without on-glb class
                     return img_tag
+            elif set(skip_class) & set(classes):
+                # skip image with off-glb and specific class
+                return img_tag
 
             if self.using_material_privacy:
                 # skip href attribute if using material privacy plugin, will be set by js code
                 a_tag = '<a class="glightbox" data-type="image"'
             else:
                 src = re.search(r"src=[\"\']([^\"\']+)", img_attr).group(1)
                 a_tag = f'<a class="glightbox" href="{src}" data-type="image"'
```

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/PKG-INFO` & `mkdocs-glightbox-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mkdocs-glightbox
-Version: 0.3.7
-Summary: MkDocs plugin supports image lightbox with GLightbox.
-Home-page: https://blueswen.github.io/mkdocs-glightbox
-Author: Blueswen
-Author-email: blueswen.tw@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/Blueswen/mkdocs-glightbox
-Keywords: mkdocs,plugin,lightbox
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MkDocs GLightbox
 
 <p align="center">
 <a target="_blank" href="https://pypi.org/project/mkdocs-glightbox"><img src="https://img.shields.io/pypi/v/mkdocs-glightbox.svg" alt="PyPI version"/></a>
 <a target="_blank" href="https://pypi.org/project/mkdocs-glightbox"><img src="https://img.shields.io/pypi/dm/mkdocs-glightbox.svg" alt="PyPI downloads"/></a>
 <a target="_blank" href="https://codecov.io/gh/blueswen/mkdocs-glightbox"><img src="https://codecov.io/gh/blueswen/mkdocs-glightbox/branch/main/graph/badge.svg?token=KAJS3NU81H" alt="Codecov"/></a>
 </p>
@@ -63,14 +49,15 @@
            draggable: true
            skip_classes:
              - custom-skip-class-name
            auto_caption: false
            caption_position: bottom
            background: white
            shadow: true
+           manual: false
     ```
 
     | Option | Default | Description |
     |---|---|---|
     | touchNavigation | true | Enable or disable the touch navigation (swipe). |
     | loop | false | Loop slides on end. |
     | effect | zoom | Name of the effect on lightbox open. (zoom, fade, none) |
@@ -80,25 +67,31 @@
     | zoomable | true | Enable or disable zoomable images. |
     | draggable | true | Enable or disable mouse drag to go prev and next slide. |
     | skip_classes | [ ] | Disable lightbox of those image with specific custom class name. |
     | auto_caption | false | Enable or disable using alt of image as caption title automatically. |
     | caption_position | bottom | Default captions position. (bottom, top, left, right) |
     | background | white | The background CSS of lightbox image. The background will shown when the image is transparent. You can use any CSS value for the background for example `#74b9ff` or `Gainsboro` or `none` for nothing. |
     | shadow | true | Enable or disable the shadow of lightbox image. Disable it when the background is `none` to prevent shadow around the transparent image. |
+    | manual | false | When true, lightbox has to be enabled for each image manually by adding `on-glb` class to it or adding `glightbox: true` meta on page.  |
 
     Check more options information on [GLightbox Docs](https://github.com/biati-digital/glightbox#lightbox-options).
 
-5. For more flexibility, you can disable the lightbox with a [specific image](https://blueswen.github.io/mkdocs-glightbox/disable/image/) or a [specific page](https://blueswen.github.io/mkdocs-glightbox/disable/page/).
+5. For more flexibility:
+      1. [Disable by image](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-image.md): Disable the lightbox for specific images. Suitable for a few amount of images that don't need the lightbox effect.
+      2. [Disable by page](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-page.md): Disable the lightbox for specific pages. Suitable for a few amount of pages that don't need the lightbox effect.
+      3. [Enable by image](https://blueswen.github.io/mkdocs-glightbox/flexibility/disable-by-page-enable-by-image.md): Disable the lightbox for specific pages but enable some images on those pages. Suitable for a few amount of images that need the lightbox effect.
+      4. [Disable globally but enable by image or page](https://blueswen.github.io/mkdocs-glightbox/flexibility/enable-by-image-or-page.md): Disable the lightbox globally but enable specific images or specific pages. Suitable for a large number of images or pages that don't need the lightbox effect.
 6. Support lightbox image caption, check more details on [Caption](https://blueswen.github.io/mkdocs-glightbox/caption/caption/).
 7. Support grouping images as galleries, check more details on [Gallery](https://blueswen.github.io/mkdocs-glightbox/gallery/gallery/).
 
+> [!NOTE] 
+> If this is your first time using the MkDocs plugin feature, you should know that MkDocs includes a default plugin named `search`. If you want to keep the search feature, you need to add the `search` plugin back to the `plugins` list.
+
 ## How it works
 
 1. Copy GLightbox script file into `site/assets/javascripts/` directory and CSS file into `site/assets/stylesheets/` directory
 2. Import GLightbox script and CSS file and add javascript code on each page excluded disabled pages
 3. Search all image tags and warp with an anchor tag for GLightbox excluded images with skip class or already warped with an anchor tag
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Blueswen/mkdocs-glightbox/blob/main/LICENSE) file for details.
-
-
```

### Comparing `mkdocs-glightbox-0.3.7/mkdocs_glightbox.egg-info/SOURCES.txt` & `mkdocs-glightbox-0.4.0/mkdocs_glightbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-glightbox-0.3.7/setup.py` & `mkdocs-glightbox-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-glightbox",
-    version="0.3.7",
+    version="0.4.0",
     author="Blueswen",
     author_email="blueswen.tw@gmail.com",
     url="https://blueswen.github.io/mkdocs-glightbox",
     project_urls={
         "Source": "https://github.com/Blueswen/mkdocs-glightbox",
     },
     keywords=["mkdocs", "plugin", "lightbox"],
```

