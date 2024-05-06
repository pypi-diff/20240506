# Comparing `tmp/dinosaur_run_game-1.0.0.tar.gz` & `tmp/dinosaur_run_game-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinosaur_run_game-1.0.0.tar", last modified: Mon May  6 16:28:00 2024, max compression
+gzip compressed data, was "dinosaur_run_game-1.0.1.tar", last modified: Mon May  6 16:45:56 2024, max compression
```

## Comparing `dinosaur_run_game-1.0.0.tar` & `dinosaur_run_game-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 16:28:00.420121 dinosaur_run_game-1.0.0/
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)     1064 2024-05-06 05:11:46.000000 dinosaur_run_game-1.0.0/LICENSE
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      217 2024-05-06 16:28:00.419951 dinosaur_run_game-1.0.0/PKG-INFO
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      250 2024-05-06 16:02:52.000000 dinosaur_run_game-1.0.0/README.md
-drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 16:28:00.419777 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      217 2024-05-06 16:28:00.000000 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/PKG-INFO
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      274 2024-05-06 16:28:00.000000 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/SOURCES.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 16:28:00.000000 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/dependency_links.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       53 2024-05-06 16:28:00.000000 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/entry_points.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        7 2024-05-06 16:28:00.000000 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/requires.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 16:28:00.000000 dinosaur_run_game-1.0.0/dinosaur_run_game.egg-info/top_level.txt
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       38 2024-05-06 16:28:00.420159 dinosaur_run_game-1.0.0/setup.cfg
--rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      558 2024-05-06 16:26:37.000000 dinosaur_run_game-1.0.0/setup.py
+drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 16:45:56.555251 dinosaur_run_game-1.0.1/
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)     1064 2024-05-06 05:11:46.000000 dinosaur_run_game-1.0.1/LICENSE
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      217 2024-05-06 16:45:56.555053 dinosaur_run_game-1.0.1/PKG-INFO
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      349 2024-05-06 16:30:13.000000 dinosaur_run_game-1.0.1/README.md
+drwxr-xr-x   0 worasitdaimongkol   (501) staff       (20)        0 2024-05-06 16:45:56.554868 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      217 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/PKG-INFO
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      274 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/SOURCES.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/dependency_links.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       45 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/entry_points.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        7 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/requires.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)        1 2024-05-06 16:45:56.000000 dinosaur_run_game-1.0.1/dinosaur_run_game.egg-info/top_level.txt
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)       38 2024-05-06 16:45:56.555286 dinosaur_run_game-1.0.1/setup.cfg
+-rw-r--r--   0 worasitdaimongkol   (501) staff       (20)      496 2024-05-06 16:44:43.000000 dinosaur_run_game-1.0.1/setup.py
```

### Comparing `dinosaur_run_game-1.0.0/LICENSE` & `dinosaur_run_game-1.0.1/LICENSE`

 * *Files identical despite different names*

