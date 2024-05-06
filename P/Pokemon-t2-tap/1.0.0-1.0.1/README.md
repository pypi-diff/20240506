# Comparing `tmp/Pokemon_t2_tap-1.0.0.tar.gz` & `tmp/Pokemon_t2_tap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokemon_t2_tap-1.0.0.tar", last modified: Sun May  5 07:18:05 2024, max compression
+gzip compressed data, was "pokemon_t2_tap-1.0.1.tar", last modified: Mon May  6 07:22:48 2024, max compression
```

## Comparing `Pokemon_t2_tap-1.0.0.tar` & `Pokemon_t2_tap-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 07:18:05.657827 pokemon_t2_tap-1.0.0/
--rw-rw-rw-   0        0        0      248 2024-05-05 07:18:05.650825 pokemon_t2_tap-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-05 07:18:05.543298 pokemon_t2_tap-1.0.0/Pokemon-t2-tap/
--rw-rw-rw-   0        0        0       43 2024-05-05 05:18:54.000000 pokemon_t2_tap-1.0.0/Pokemon-t2-tap/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-05-04 17:00:49.000000 pokemon_t2_tap-1.0.0/Pokemon-t2-tap/pokemon.csv
--rw-rw-rw-   0        0        0      806 2024-05-05 05:20:05.000000 pokemon_t2_tap-1.0.0/Pokemon-t2-tap/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:18:05.646824 pokemon_t2_tap-1.0.0/Pokemon_t2_tap.egg-info/
--rw-rw-rw-   0        0        0      248 2024-05-05 07:18:05.000000 pokemon_t2_tap-1.0.0/Pokemon_t2_tap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-05 07:18:05.000000 pokemon_t2_tap-1.0.0/Pokemon_t2_tap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 07:18:05.000000 pokemon_t2_tap-1.0.0/Pokemon_t2_tap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 07:18:05.000000 pokemon_t2_tap-1.0.0/Pokemon_t2_tap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-05 07:18:05.000000 pokemon_t2_tap-1.0.0/Pokemon_t2_tap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      997 2024-05-05 05:32:13.000000 pokemon_t2_tap-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 07:18:05.659826 pokemon_t2_tap-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      431 2024-05-05 05:27:34.000000 pokemon_t2_tap-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:22:48.664047 pokemon_t2_tap-1.0.1/
+-rw-rw-rw-   0        0        0      248 2024-05-06 07:22:48.659042 pokemon_t2_tap-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 07:22:48.598578 pokemon_t2_tap-1.0.1/Pokemon-t2-tap/
+-rw-rw-rw-   0        0        0       43 2024-05-05 05:18:54.000000 pokemon_t2_tap-1.0.1/Pokemon-t2-tap/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-05-04 17:00:49.000000 pokemon_t2_tap-1.0.1/Pokemon-t2-tap/pokemon.csv
+-rw-rw-rw-   0        0        0      810 2024-05-06 07:18:05.000000 pokemon_t2_tap-1.0.1/Pokemon-t2-tap/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:22:48.655043 pokemon_t2_tap-1.0.1/Pokemon_t2_tap.egg-info/
+-rw-rw-rw-   0        0        0      248 2024-05-06 07:22:48.000000 pokemon_t2_tap-1.0.1/Pokemon_t2_tap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-06 07:22:48.000000 pokemon_t2_tap-1.0.1/Pokemon_t2_tap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:22:48.000000 pokemon_t2_tap-1.0.1/Pokemon_t2_tap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 07:22:48.000000 pokemon_t2_tap-1.0.1/Pokemon_t2_tap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-06 07:22:48.000000 pokemon_t2_tap-1.0.1/Pokemon_t2_tap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      997 2024-05-05 05:32:13.000000 pokemon_t2_tap-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 07:22:48.664047 pokemon_t2_tap-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      419 2024-05-06 07:21:52.000000 pokemon_t2_tap-1.0.1/setup.py
```

### Comparing `pokemon_t2_tap-1.0.0/Pokemon-t2-tap/pokemon.csv` & `pokemon_t2_tap-1.0.1/Pokemon-t2-tap/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokemon_t2_tap-1.0.0/Pokemon-t2-tap/random_pokemon.py` & `pokemon_t2_tap-1.0.1/Pokemon-t2-tap/random_pokemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import pkg_resources
 import pandas as pd
 
 class RandomPokemon:
-    FILE_PATH = pkg_resources.resources_filiename(__name__, 'pokemon.csv')
+
+    FILE_PATH = pkg_resources.resources_filename(__name__, 'pokemon.csv')
 
     def __init__(self):
         self._file = pd.read_csv(RandomPokemon.FILE_PATH)
         self._pokemon = None
         self._number = None
         self._name = None
         self._type = None
 
     def generate_random(self):
         self._pokemon = self._file.sample()
-        self._number = self._pokemon['#'].values[0]
-        self._name = self._pokemon['Name'].values[0]
-        self._type = self._pokemon['Type 1'].values[0]
+        self._number = self._pokemon["#"].values[0]
+        self._name = self._pokemon["Name"].values[0]
+        self._type1 = self._pokemon["Type 1"].values[0]
 
     def getPokemon(self):
         return self._pokemon
 
     def getNumber(self):
         return self._number
 
     def getName(self):
         return self._name
 
     def getType1(self):
-        return self._type1
+        return self._type1
```

### Comparing `pokemon_t2_tap-1.0.0/README.md` & `pokemon_t2_tap-1.0.1/README.md`

 * *Files identical despite different names*

