# Comparing `tmp/dinosaur_run_game-1.0.1.tar.gz` & `tmp/dinosaur_run_game-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinosaur_run_game-1.0.1.tar", last modified: Mon May  6 16:45:56 2024, max compression
+gzip compressed data, was "dinosaur_run_game-1.0.4.tar", last modified: Mon May  6 17:05:03 2024, max compression
```

## Comparing `dinosaur_run_game-1.0.1.tar` & `dinosaur_run_game-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 16:45:56.555251 dinosaur_run_game-1.0.1/
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)     1064 2024-05-06 05:11:46.000000 dinosaur_run_game-1.0.1/LICENSE
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      217 2024-05-06 16:45:56.555053 dinosaur_run_game-1.0.1/PKG-INFO
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      349 2024-05-06 16:30:13.000000 dinosaur_run_game-1.0.1/README.md
-drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 16:45:56.554868 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      217 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/PKG-INFO
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      274 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/SOURCES.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/dependency_links.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       45 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/entry_points.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        7 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/requires.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/top_level.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       38 2024-05-06 16:45:56.555286 dinosaur_run_game-1.0.1/setup.cfg
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      496 2024-05-06 16:44:43.000000 dinosaur_run_game-1.0.1/setup.py
+drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 17:05:03.265646 dinosaur_run_game-1.0.4/
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)     1064 2024-05-06 05:11:46.000000 dinosaur_run_game-1.0.4/LICENSE
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      222 2024-05-06 17:05:03.265455 dinosaur_run_game-1.0.4/PKG-INFO
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      443 2024-05-06 17:01:55.000000 dinosaur_run_game-1.0.4/README.md
+drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 17:05:03.265301 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      222 2024-05-06 17:05:03.000000 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/PKG-INFO
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      274 2024-05-06 17:05:03.000000 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/SOURCES.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 17:05:03.000000 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/dependency_links.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       45 2024-05-06 17:05:03.000000 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/entry_points.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        7 2024-05-06 17:05:03.000000 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/requires.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 17:05:03.000000 dinosaur_run_game-1.0.4/dinosaur_run_game.egg-info/top_level.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       38 2024-05-06 17:05:03.265683 dinosaur_run_game-1.0.4/setup.cfg
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      455 2024-05-06 17:04:48.000000 dinosaur_run_game-1.0.4/setup.py
```

### Comparing `dinosaur_run_game-1.0.1/LICENSE` & `dinosaur_run_game-1.0.4/LICENSE`

 * *Files identical despite different names*

