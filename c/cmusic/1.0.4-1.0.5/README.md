# Comparing `tmp/cmusic-1.0.4.tar.gz` & `tmp/cmusic-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmusic-1.0.4.tar", max compression
+gzip compressed data, was "cmusic-1.0.5.tar", max compression
```

## Comparing `cmusic-1.0.4.tar` & `cmusic-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      846 2024-04-24 15:27:09.715496 cmusic-1.0.4/LICENSE
--rw-r--r--   0        0        0     3764 2024-05-04 01:50:08.697910 cmusic-1.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-27 23:05:32.082513 cmusic-1.0.4/cmusic/__init__.py
--rw-r--r--   0        0        0     3940 2024-05-04 01:16:26.452353 cmusic-1.0.4/cmusic/bg_threads.py
--rwxr-xr-x   0        0        0     5733 2024-05-04 02:08:59.137570 cmusic-1.0.4/cmusic/cmusic.py
--rw-r--r--   0        0        0     1303 2024-05-04 02:15:42.134445 cmusic-1.0.4/cmusic/constants.py
--rw-r--r--   0        0        0    19509 2024-05-04 01:16:26.702616 cmusic-1.0.4/cmusic/indexlib.py
--rw-r--r--   0        0        0    24199 2024-05-04 01:16:26.718203 cmusic-1.0.4/cmusic/main.py
--rw-r--r--   0        0        0      418 2024-05-04 02:16:11.224929 cmusic-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 cmusic-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      846 2024-04-24 15:27:09.715496 cmusic-1.0.5/LICENSE
+-rw-r--r--   0        0        0     4141 2024-05-05 16:55:46.249909 cmusic-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 23:05:32.082513 cmusic-1.0.5/cmusic/__init__.py
+-rw-r--r--   0        0        0     3940 2024-05-04 01:16:26.452353 cmusic-1.0.5/cmusic/bg_threads.py
+-rwxr-xr-x   0        0        0     5733 2024-05-04 02:08:59.137570 cmusic-1.0.5/cmusic/cmusic.py
+-rw-r--r--   0        0        0     1303 2024-05-04 02:15:42.134445 cmusic-1.0.5/cmusic/constants.py
+-rw-r--r--   0        0        0    19598 2024-05-05 23:04:00.189780 cmusic-1.0.5/cmusic/indexlib.py
+-rw-r--r--   0        0        0    24199 2024-05-04 01:16:26.718203 cmusic-1.0.5/cmusic/main.py
+-rw-r--r--   0        0        0      418 2024-05-05 23:04:00.192722 cmusic-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 cmusic-1.0.5/PKG-INFO
```

### Comparing `cmusic-1.0.4/LICENSE` & `cmusic-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.4/README.md` & `cmusic-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,32 @@
 brew tap Kokonico/tap
 brew install cmusic
 ```
 -->
 
 ## Usage
 
+Cmusic currently only supports mp3 files. To use the player, you need to index the songs you want to play first.
+
+```sh
+# index a song
+cmusic index <Song File>
+```
+
+example:
+
+```sh
+cmusic index "path/to/song.mp3"
+```
+
+it will walk you through the process of indexing the song.
+
+to play a song, you can use the following command, the name of the song should be the same as the one you set when indexing the song.
+
 ```sh
-# play a Song (must be in the current directory, you can ignore file extensions)
 cmusic play <Song> [--loop] [--shuffle]
 
 ```
 
 pssst, you can also pass multiple Songs to play them in a row._
 
 ```sh
@@ -74,14 +90,15 @@
 - `q` to quit the player.
 - `shift + (+)` to increase the volume.
 - `shift + (-)` to decrease the volume.
 - `e` to enter background mode.
 
 ### commands
 
+- `cmusic index <Song File>` to index a Song
 - `cmusic list` to list all the songs in the library.
 - `cmusic play <Song>` to play a Song.
 - `cmusic version` to display the version of the player.
 - `cmusic search <query>` to search for Songs in the library.
 
 <!-- comment this out for now until I implement it. -->
 
@@ -103,15 +120,15 @@
 - `cmusic play <playlist name> --playlist` to play a playlist.
 
 ## Development setup
 
 To set up the development environment, you need to have Poetry and python 3.12+ installed on your system.
 
 ```sh
-git clone https://github.com/kokonico/cmusic
+git clone https://github.com/Kokonico/cmusic
 cd cmusic
 poetry install
 ```
 
 to install the player to use it in the terminal, you can use the following command.
 
 ```sh
```

### Comparing `cmusic-1.0.4/cmusic/bg_threads.py` & `cmusic-1.0.5/cmusic/bg_threads.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.4/cmusic/cmusic.py` & `cmusic-1.0.5/cmusic/cmusic.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.4/cmusic/constants.py` & `cmusic-1.0.5/cmusic/constants.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.4/cmusic/indexlib.py` & `cmusic-1.0.5/cmusic/indexlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,14 +448,16 @@
 
 def delete_playlist(playlist: tuple):
     """delete a playlist"""
     conn = sqlite3.connect(os.path.join(config["library"], "index.db"))
     c = conn.cursor()
     c.execute("DELETE FROM playlists WHERE id = ?", (playlist[0],))
     conn.commit()
+    # delete all songs in the playlist
+    c.execute("DELETE FROM playlist_songs WHERE playlist_id = ?", (playlist[0],))
     conn.close()
     log.log(Info(f"Playlist '{playlist[1]}' deleted."))
 
 
 def list_playlists():
     """list all playlists"""
     conn = sqlite3.connect(os.path.join(config["library"], "index.db"))
@@ -518,16 +520,16 @@
 
 
 def get_playlist_contents(playlist: tuple):
     """get the contents of a playlist"""
     conn = sqlite3.connect(os.path.join(config["library"], "index.db"))
     c = conn.cursor()
     if playlist is None:
-        log.log(Warn(f"Playlist '{playlist[1]}' not found."))
-        print(f"Playlist '{playlist[1]}' not found.")
+        log.log(Warn(f"Playlist not found."))
+        print(f"Playlist not found.")
         return
     c.execute("SELECT * FROM playlist_songs WHERE playlist_id = ?", (playlist[0],))
     songs = c.fetchall()
     song_data = []
     for song in songs:
         c.execute("SELECT * FROM songs WHERE id = ?", (song[1],))
         song_info = c.fetchone()
```

### Comparing `cmusic-1.0.4/cmusic/main.py` & `cmusic-1.0.5/cmusic/main.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.4/PKG-INFO` & `cmusic-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmusic
-Version: 1.0.4
+Version: 1.0.5
 Summary: the CLI music player
 Author: Kokonico
 Author-email: kokonico@duck.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: inquirer (>=3.2.4,<4.0.0)
@@ -50,16 +50,32 @@
 brew tap Kokonico/tap
 brew install cmusic
 ```
 -->
 
 ## Usage
 
+Cmusic currently only supports mp3 files. To use the player, you need to index the songs you want to play first.
+
+```sh
+# index a song
+cmusic index <Song File>
+```
+
+example:
+
+```sh
+cmusic index "path/to/song.mp3"
+```
+
+it will walk you through the process of indexing the song.
+
+to play a song, you can use the following command, the name of the song should be the same as the one you set when indexing the song.
+
 ```sh
-# play a Song (must be in the current directory, you can ignore file extensions)
 cmusic play <Song> [--loop] [--shuffle]
 
 ```
 
 pssst, you can also pass multiple Songs to play them in a row._
 
 ```sh
@@ -90,14 +106,15 @@
 - `q` to quit the player.
 - `shift + (+)` to increase the volume.
 - `shift + (-)` to decrease the volume.
 - `e` to enter background mode.
 
 ### commands
 
+- `cmusic index <Song File>` to index a Song
 - `cmusic list` to list all the songs in the library.
 - `cmusic play <Song>` to play a Song.
 - `cmusic version` to display the version of the player.
 - `cmusic search <query>` to search for Songs in the library.
 
 <!-- comment this out for now until I implement it. -->
 
@@ -119,15 +136,15 @@
 - `cmusic play <playlist name> --playlist` to play a playlist.
 
 ## Development setup
 
 To set up the development environment, you need to have Poetry and python 3.12+ installed on your system.
 
 ```sh
-git clone https://github.com/kokonico/cmusic
+git clone https://github.com/Kokonico/cmusic
 cd cmusic
 poetry install
 ```
 
 to install the player to use it in the terminal, you can use the following command.
 
 ```sh
```

