# Comparing `tmp/shrillecho-1.0.9.tar.gz` & `tmp/shrillecho-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrillecho-1.0.9.tar", max compression
+gzip compressed data, was "shrillecho-1.1.0.tar", max compression
```

## Comparing `shrillecho-1.0.9.tar` & `shrillecho-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,149 @@
--rw-r--r--   0        0        0     1165 2024-03-14 18:28:34.729665 shrillecho-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       32 2023-09-23 15:03:19.005437 shrillecho-1.0.9/shrillecho/__init__.py
--rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.0.9/shrillecho/artist/__init__.py
--rw-r--r--   0        0        0     1568 2024-03-14 02:00:56.862224 shrillecho-1.0.9/shrillecho/artist/spotify_artist.py
--rw-r--r--   0        0        0       29 2023-09-23 15:03:19.005437 shrillecho-1.0.9/shrillecho/auth/__init__.py
--rw-r--r--   0        0        0     2816 2024-03-12 19:28:42.468224 shrillecho-1.0.9/shrillecho/auth/local_auth.py
--rw-r--r--   0        0        0     7710 2024-03-14 02:52:08.767896 shrillecho-1.0.9/shrillecho/auth/oauth.py
--rw-r--r--   0        0        0      156 2024-03-12 19:27:15.771836 shrillecho-1.0.9/shrillecho/auth/spotify_auth.py
--rw-r--r--   0        0        0        0 2024-03-11 21:00:35.951586 shrillecho-1.0.9/shrillecho/player/__init__.py
--rw-r--r--   0        0        0      359 2024-03-11 22:18:56.285682 shrillecho-1.0.9/shrillecho/player/spotify_player.py
--rw-r--r--   0        0        0       24 2023-09-23 15:03:19.005437 shrillecho-1.0.9/shrillecho/playlist/__init__.py
--rw-r--r--   0        0        0     2306 2024-03-11 22:16:24.766938 shrillecho-1.0.9/shrillecho/playlist/archive/playlist_engine.py
--rw-r--r--   0        0        0     2537 2024-03-14 18:27:45.696787 shrillecho-1.0.9/shrillecho/playlist/spotify_playlist.py
--rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.0.9/shrillecho/scraping/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 18:59:09.355126 shrillecho-1.0.9/shrillecho/spotify/__init__.py
--rw-r--r--   0        0        0    14904 2024-03-14 18:27:42.691863 shrillecho-1.0.9/shrillecho/spotify/client.py
--rw-r--r--   0        0        0        0 2024-03-11 20:48:31.986990 shrillecho-1.0.9/shrillecho/track/__init__.py
--rw-r--r--   0        0        0     1543 2024-03-14 02:15:50.692208 shrillecho-1.0.9/shrillecho/track/spotify_track.py
--rw-r--r--   0        0        0        0 2023-10-14 18:10:24.959970 shrillecho-1.0.9/shrillecho/types/__init__.py
--rw-r--r--   0        0        0     2602 2024-03-11 22:15:02.628111 shrillecho-1.0.9/shrillecho/types/album_types.py
--rw-r--r--   0        0        0        0 2024-01-12 21:14:57.528149 shrillecho-1.0.9/shrillecho/types/archive_delete/__init__.py
--rw-r--r--   0        0        0     5529 2024-03-11 22:16:14.402147 shrillecho-1.0.9/shrillecho/types/archive_delete/all.py
--rw-r--r--   0        0        0      650 2024-01-12 22:18:43.706893 shrillecho-1.0.9/shrillecho/types/artist_types.py
--rw-r--r--   0        0        0      962 2023-11-05 23:56:12.988932 shrillecho-1.0.9/shrillecho/types/base_types.py
--rw-r--r--   0        0        0      778 2024-01-07 02:24:43.414159 shrillecho-1.0.9/shrillecho/types/component_types.py
--rw-r--r--   0        0        0     2009 2024-03-14 01:17:47.656638 shrillecho-1.0.9/shrillecho/types/playlist_types.py
--rw-r--r--   0        0        0     3586 2024-01-12 21:16:04.765172 shrillecho-1.0.9/shrillecho/types/soundcloud_types.py
--rw-r--r--   0        0        0     2893 2024-03-11 22:16:36.226683 shrillecho-1.0.9/shrillecho/types/track_types.py
--rw-r--r--   0        0        0      756 2024-01-12 21:44:55.909131 shrillecho-1.0.9/shrillecho/types/user_types.py
--rw-r--r--   0        0        0       20 2023-09-23 15:03:19.005437 shrillecho-1.0.9/shrillecho/user/__init__.py
--rw-r--r--   0        0        0      686 2023-10-14 14:17:27.008634 shrillecho-1.0.9/shrillecho/user/user.py
--rw-r--r--   0        0        0       32 2023-09-23 15:03:19.009896 shrillecho-1.0.9/shrillecho/utility/__init__.py
--rw-r--r--   0        0        0        0 2024-01-07 02:10:54.084812 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/__init__.py
--rw-r--r--   0        0        0     5236 2024-03-14 02:20:06.773370 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/async_spotify.py
--rw-r--r--   0        0        0      949 2024-01-07 02:19:15.222777 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/cache.py
--rw-r--r--   0        0        0     3492 2024-03-11 22:16:21.293179 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/discovery.py
--rw-r--r--   0        0        0     8352 2024-03-11 22:16:31.726296 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/general.py
--rw-r--r--   0        0        0      928 2024-03-13 02:07:04.021894 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/old_cache.py
--rw-r--r--   0        0        0      773 2024-03-11 21:41:34.182076 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/parsers.py
--rw-r--r--   0        0        0     2659 2024-03-11 22:16:23.348559 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/playlist.py
--rw-r--r--   0        0        0     3613 2024-01-07 02:19:15.149506 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/scraper.py
--rw-r--r--   0        0        0     3512 2024-01-07 02:19:15.215743 shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/spotify_client.py
--rw-r--r--   0        0        0     3012 2024-03-14 03:42:57.139360 shrillecho-1.0.9/shrillecho/utility/cache.py
--rw-r--r--   0        0        0      310 2024-03-12 20:22:02.409580 shrillecho-1.0.9/shrillecho/utility/general_utility.py
--rw-r--r--   0        0        0    11617 2024-03-11 22:16:15.022138 shrillecho-1.0.9/shrillecho/utility/soundcloud_converter.py
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 shrillecho-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1165 2024-05-06 12:10:03.033808 shrillecho-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-09-23 15:03:19.005437 shrillecho-1.1.0/shrillecho/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:55:44.836628 shrillecho-1.1.0/shrillecho/album/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-17 21:40:51.698889 shrillecho-1.1.0/shrillecho/album/album_controller.py
+-rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.1.0/shrillecho/artist/__init__.py
+-rw-r--r--   0        0        0      160 2023-09-23 15:05:30.663260 shrillecho-1.1.0/shrillecho/artist/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2024-03-14 02:58:16.623582 shrillecho-1.1.0/shrillecho/artist/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    11625 2024-04-17 20:29:10.940781 shrillecho-1.1.0/shrillecho/artist/__pycache__/spotify_artist.cpython-312.pyc
+-rw-r--r--   0        0        0     2748 2024-04-21 22:40:07.469215 shrillecho-1.1.0/shrillecho/artist/artist_controller.py
+-rw-r--r--   0        0        0     1009 2024-04-17 20:01:34.862797 shrillecho-1.1.0/shrillecho/artist/sp_artist.py
+-rw-r--r--   0        0        0     8785 2024-04-17 20:29:10.024946 shrillecho-1.1.0/shrillecho/artist/spotify_artist.py
+-rw-r--r--   0        0        0       29 2023-09-23 15:03:19.005437 shrillecho-1.1.0/shrillecho/auth/__init__.py
+-rw-r--r--   0        0        0      193 2023-09-23 15:05:30.403768 shrillecho-1.1.0/shrillecho/auth/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      178 2024-03-09 15:04:18.657207 shrillecho-1.1.0/shrillecho/auth/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4720 2024-03-12 19:30:51.569168 shrillecho-1.1.0/shrillecho/auth/__pycache__/local_auth.cpython-312.pyc
+-rw-r--r--   0        0        0     5424 2024-03-13 22:52:25.720959 shrillecho-1.1.0/shrillecho/auth/__pycache__/oauth.cpython-311.pyc
+-rw-r--r--   0        0        0    11554 2024-03-17 00:55:57.542250 shrillecho-1.1.0/shrillecho/auth/__pycache__/oauth.cpython-312.pyc
+-rw-r--r--   0        0        0      525 2024-03-12 19:28:02.938593 shrillecho-1.1.0/shrillecho/auth/__pycache__/spotify_auth.cpython-312.pyc
+-rw-r--r--   0        0        0     2816 2024-03-12 19:28:42.468224 shrillecho-1.1.0/shrillecho/auth/local_auth.py
+-rw-r--r--   0        0        0     7720 2024-03-17 00:55:39.759059 shrillecho-1.1.0/shrillecho/auth/oauth.py
+-rw-r--r--   0        0        0      156 2024-03-12 19:27:15.771836 shrillecho-1.1.0/shrillecho/auth/spotify_auth.py
+-rw-r--r--   0        0        0        0 2024-03-11 21:00:35.951586 shrillecho-1.1.0/shrillecho/player/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-09 21:02:32.629853 shrillecho-1.1.0/shrillecho/player/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      904 2024-04-09 21:02:32.631375 shrillecho-1.1.0/shrillecho/player/__pycache__/spotify_player.cpython-312.pyc
+-rw-r--r--   0        0        0      359 2024-03-11 22:18:56.285682 shrillecho-1.1.0/shrillecho/player/spotify_player.py
+-rw-r--r--   0        0        0       24 2023-09-23 15:03:19.005437 shrillecho-1.1.0/shrillecho/playlist/__init__.py
+-rw-r--r--   0        0        0      192 2023-09-23 17:32:16.346106 shrillecho-1.1.0/shrillecho/playlist/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      177 2024-03-09 15:02:13.039686 shrillecho-1.1.0/shrillecho/playlist/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1940 2024-04-20 10:39:20.711449 shrillecho-1.1.0/shrillecho/playlist/__pycache__/playlist_controller.cpython-312.pyc
+-rw-r--r--   0        0        0     4070 2024-01-12 22:36:57.888928 shrillecho-1.1.0/shrillecho/playlist/__pycache__/playlist_engine.cpython-311.pyc
+-rw-r--r--   0        0        0     3763 2024-03-09 15:02:13.041686 shrillecho-1.1.0/shrillecho/playlist/__pycache__/playlist_engine.cpython-312.pyc
+-rw-r--r--   0        0        0     5128 2024-04-21 21:13:00.466645 shrillecho-1.1.0/shrillecho/playlist/__pycache__/spotify_playlist.cpython-312.pyc
+-rw-r--r--   0        0        0     7244 2024-04-20 10:45:03.486766 shrillecho-1.1.0/shrillecho/playlist/__pycache__/virtual_playlist.cpython-312.pyc
+-rw-r--r--   0        0        0     3776 2024-03-11 22:58:55.429565 shrillecho-1.1.0/shrillecho/playlist/archive/__pycache__/playlist_engine.cpython-312.pyc
+-rw-r--r--   0        0        0     2306 2024-03-11 22:16:24.766938 shrillecho-1.1.0/shrillecho/playlist/archive/playlist_engine.py
+-rw-r--r--   0        0        0     1221 2024-04-17 22:20:31.920970 shrillecho-1.1.0/shrillecho/playlist/playlist_controller.py
+-rw-r--r--   0        0        0     4389 2024-04-21 20:26:12.833324 shrillecho-1.1.0/shrillecho/playlist/spotify_playlist.py
+-rw-r--r--   0        0        0     4256 2024-04-20 10:44:19.895473 shrillecho-1.1.0/shrillecho/playlist/virtual_playlist.py
+-rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.1.0/shrillecho/scraping/__init__.py
+-rw-r--r--   0        0        0      162 2023-09-23 15:05:30.663260 shrillecho-1.1.0/shrillecho/scraping/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      146 2024-03-14 18:38:34.308684 shrillecho-1.1.0/shrillecho/scraping/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3653 2024-04-17 19:53:12.059070 shrillecho-1.1.0/shrillecho/scraping/__pycache__/browser_auth.cpython-312.pyc
+-rw-r--r--   0        0        0     2051 2024-04-17 19:46:10.197061 shrillecho-1.1.0/shrillecho/scraping/browser_auth.py
+-rw-r--r--   0        0        0        0 2024-03-12 18:59:09.355126 shrillecho-1.1.0/shrillecho/spotify/__init__.py
+-rw-r--r--   0        0        0      145 2024-03-12 19:19:14.425028 shrillecho-1.1.0/shrillecho/spotify/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    22970 2024-04-28 00:26:11.161172 shrillecho-1.1.0/shrillecho/spotify/__pycache__/client.cpython-312.pyc
+-rw-r--r--   0        0        0     3480 2024-04-21 21:54:52.990207 shrillecho-1.1.0/shrillecho/spotify/__pycache__/task_scheduler.cpython-312.pyc
+-rw-r--r--   0        0        0    16853 2024-04-28 00:26:00.407579 shrillecho-1.1.0/shrillecho/spotify/client.py
+-rw-r--r--   0        0        0     2489 2024-04-21 21:54:39.662490 shrillecho-1.1.0/shrillecho/spotify/task_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:48:31.986990 shrillecho-1.1.0/shrillecho/track/__init__.py
+-rw-r--r--   0        0        0      143 2024-03-11 22:58:59.259675 shrillecho-1.1.0/shrillecho/track/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7545 2024-04-11 22:51:50.359779 shrillecho-1.1.0/shrillecho/track/__pycache__/spotify_track.cpython-312.pyc
+-rw-r--r--   0        0        0     2379 2024-04-12 23:08:45.923483 shrillecho-1.1.0/shrillecho/track/__pycache__/tracks_wrapper.cpython-312.pyc
+-rw-r--r--   0        0        0     5159 2024-04-11 22:51:22.177465 shrillecho-1.1.0/shrillecho/track/spotify_track.py
+-rw-r--r--   0        0        0        0 2023-10-14 18:10:24.959970 shrillecho-1.1.0/shrillecho/types/__init__.py
+-rw-r--r--   0        0        0      155 2023-10-14 18:10:25.750276 shrillecho-1.1.0/shrillecho/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      143 2024-03-09 15:02:13.064686 shrillecho-1.1.0/shrillecho/types/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4307 2024-03-11 22:58:55.468913 shrillecho-1.1.0/shrillecho/types/__pycache__/album_types.cpython-312.pyc
+-rw-r--r--   0        0        0     5278 2024-01-12 22:34:54.354054 shrillecho-1.1.0/shrillecho/types/__pycache__/albums.cpython-311.pyc
+-rw-r--r--   0        0        0     4292 2024-03-09 15:04:17.730511 shrillecho-1.1.0/shrillecho/types/__pycache__/albums.cpython-312.pyc
+-rw-r--r--   0        0        0     2658 2024-04-17 20:27:50.732389 shrillecho-1.1.0/shrillecho/types/__pycache__/artist_types.cpython-312.pyc
+-rw-r--r--   0        0        0     1908 2024-01-12 22:34:54.356055 shrillecho-1.1.0/shrillecho/types/__pycache__/artists.cpython-311.pyc
+-rw-r--r--   0        0        0     1538 2024-03-09 15:04:17.731520 shrillecho-1.1.0/shrillecho/types/__pycache__/artists.cpython-312.pyc
+-rw-r--r--   0        0        0     3173 2023-11-05 23:56:15.061834 shrillecho-1.1.0/shrillecho/types/__pycache__/base_types.cpython-311.pyc
+-rw-r--r--   0        0        0     2488 2024-03-09 15:02:13.071687 shrillecho-1.1.0/shrillecho/types/__pycache__/base_types.cpython-312.pyc
+-rw-r--r--   0        0        0     1736 2024-03-11 22:58:55.436070 shrillecho-1.1.0/shrillecho/types/__pycache__/component_types.cpython-312.pyc
+-rw-r--r--   0        0        0     2134 2024-01-07 02:24:45.003341 shrillecho-1.1.0/shrillecho/types/__pycache__/components.cpython-311.pyc
+-rw-r--r--   0        0        0     1731 2024-03-09 15:02:13.068686 shrillecho-1.1.0/shrillecho/types/__pycache__/components.cpython-312.pyc
+-rw-r--r--   0        0        0     3496 2024-03-14 02:19:29.826797 shrillecho-1.1.0/shrillecho/types/__pycache__/playlist_types.cpython-312.pyc
+-rw-r--r--   0        0        0     4298 2024-01-12 22:34:54.294325 shrillecho-1.1.0/shrillecho/types/__pycache__/playlists.cpython-311.pyc
+-rw-r--r--   0        0        0     3472 2024-03-09 15:02:13.067686 shrillecho-1.1.0/shrillecho/types/__pycache__/playlists.cpython-312.pyc
+-rw-r--r--   0        0        0     6664 2024-02-24 03:23:54.874109 shrillecho-1.1.0/shrillecho/types/__pycache__/sc.cpython-311.pyc
+-rw-r--r--   0        0        0     5792 2024-03-09 16:03:46.602847 shrillecho-1.1.0/shrillecho/types/__pycache__/sc.cpython-312.pyc
+-rw-r--r--   0        0        0     5806 2024-03-14 03:15:29.847360 shrillecho-1.1.0/shrillecho/types/__pycache__/soundcloud_types.cpython-312.pyc
+-rw-r--r--   0        0        0     7857 2024-04-27 21:55:25.752930 shrillecho-1.1.0/shrillecho/types/__pycache__/track_types.cpython-312.pyc
+-rw-r--r--   0        0        0     7020 2024-03-06 18:45:37.173792 shrillecho-1.1.0/shrillecho/types/__pycache__/tracks.cpython-311.pyc
+-rw-r--r--   0        0        0     5798 2024-03-09 15:04:17.728996 shrillecho-1.1.0/shrillecho/types/__pycache__/tracks.cpython-312.pyc
+-rw-r--r--   0        0        0     1463 2024-03-11 22:58:55.480875 shrillecho-1.1.0/shrillecho/types/__pycache__/user_types.cpython-312.pyc
+-rw-r--r--   0        0        0     1755 2024-01-12 22:34:54.365174 shrillecho-1.1.0/shrillecho/types/__pycache__/users.cpython-311.pyc
+-rw-r--r--   0        0        0     1458 2024-03-09 15:04:17.742095 shrillecho-1.1.0/shrillecho/types/__pycache__/users.cpython-312.pyc
+-rw-r--r--   0        0        0     2602 2024-03-11 22:15:02.628111 shrillecho-1.1.0/shrillecho/types/album_types.py
+-rw-r--r--   0        0        0      158 2024-04-09 21:02:35.162480 shrillecho-1.1.0/shrillecho/types/archive_delete/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      521 2024-04-09 21:02:35.163998 shrillecho-1.1.0/shrillecho/types/archive_delete/__pycache__/all.cpython-312.pyc
+-rw-r--r--   0        0        0     5529 2024-03-11 22:16:14.402147 shrillecho-1.1.0/shrillecho/types/archive_delete/all.py
+-rw-r--r--   0        0        0     1031 2024-04-17 19:58:21.480197 shrillecho-1.1.0/shrillecho/types/artist_types.py
+-rw-r--r--   0        0        0      962 2023-11-05 23:56:12.988932 shrillecho-1.1.0/shrillecho/types/base_types.py
+-rw-r--r--   0        0        0      778 2024-01-07 02:24:43.414159 shrillecho-1.1.0/shrillecho/types/component_types.py
+-rw-r--r--   0        0        0     2009 2024-03-14 01:17:47.656638 shrillecho-1.1.0/shrillecho/types/playlist_types.py
+-rw-r--r--   0        0        0     3586 2024-01-12 21:16:04.765172 shrillecho-1.1.0/shrillecho/types/soundcloud_types.py
+-rw-r--r--   0        0        0     4410 2024-04-27 21:53:11.373531 shrillecho-1.1.0/shrillecho/types/track_types.py
+-rw-r--r--   0        0        0      756 2024-01-12 21:44:55.909131 shrillecho-1.1.0/shrillecho/types/user_types.py
+-rw-r--r--   0        0        0       20 2023-09-23 15:03:19.005437 shrillecho-1.1.0/shrillecho/user/__init__.py
+-rw-r--r--   0        0        0      169 2024-03-20 18:56:34.599945 shrillecho-1.1.0/shrillecho/user/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2383 2024-04-05 21:59:11.376769 shrillecho-1.1.0/shrillecho/user/__pycache__/user.cpython-312.pyc
+-rw-r--r--   0        0        0     1374 2024-04-05 21:57:12.175049 shrillecho-1.1.0/shrillecho/user/user.py
+-rw-r--r--   0        0        0       32 2023-09-23 15:03:19.009896 shrillecho-1.1.0/shrillecho/utility/__init__.py
+-rw-r--r--   0        0        0      199 2023-09-23 15:05:30.663260 shrillecho-1.1.0/shrillecho/utility/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2024-03-09 15:04:18.655207 shrillecho-1.1.0/shrillecho/utility/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     8287 2024-03-11 01:30:11.865570 shrillecho-1.1.0/shrillecho/utility/__pycache__/async_spotify.cpython-311.pyc
+-rw-r--r--   0        0        0     7428 2024-03-14 02:20:08.969425 shrillecho-1.1.0/shrillecho/utility/__pycache__/async_spotify.cpython-312.pyc
+-rw-r--r--   0        0        0     6573 2024-04-27 23:25:08.256052 shrillecho-1.1.0/shrillecho/utility/__pycache__/cache.cpython-312.pyc
+-rw-r--r--   0        0        0     3087 2024-03-13 01:50:28.638381 shrillecho-1.1.0/shrillecho/utility/__pycache__/database.cpython-312.pyc
+-rw-r--r--   0        0        0      780 2024-03-09 21:26:52.160307 shrillecho-1.1.0/shrillecho/utility/__pycache__/general_utility.cpython-311.pyc
+-rw-r--r--   0        0        0     2815 2024-03-25 22:08:35.635006 shrillecho-1.1.0/shrillecho/utility/__pycache__/general_utility.cpython-312.pyc
+-rw-r--r--   0        0        0    14623 2024-03-11 01:30:11.500906 shrillecho-1.1.0/shrillecho/utility/__pycache__/misc_functions_sort.cpython-311.pyc
+-rw-r--r--   0        0        0    13308 2024-03-11 01:30:28.931611 shrillecho-1.1.0/shrillecho/utility/__pycache__/misc_functions_sort.cpython-312.pyc
+-rw-r--r--   0        0        0     1386 2024-02-16 01:22:08.428409 shrillecho-1.1.0/shrillecho/utility/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0     1217 2024-03-09 15:04:20.128181 shrillecho-1.1.0/shrillecho/utility/__pycache__/mongo.cpython-312.pyc
+-rw-r--r--   0        0        0     1650 2024-04-09 21:02:35.293918 shrillecho-1.1.0/shrillecho/utility/__pycache__/neo4j.cpython-312.pyc
+-rw-r--r--   0        0        0     1471 2024-03-13 02:26:41.144982 shrillecho-1.1.0/shrillecho/utility/__pycache__/old_cache.cpython-312.pyc
+-rw-r--r--   0        0        0     1298 2024-03-11 22:58:59.263675 shrillecho-1.1.0/shrillecho/utility/__pycache__/parsers.cpython-312.pyc
+-rw-r--r--   0        0        0    23150 2023-11-12 23:14:00.569468 shrillecho-1.1.0/shrillecho/utility/__pycache__/sc_to_spot.cpython-311.pyc
+-rw-r--r--   0        0        0    21256 2023-11-17 00:36:52.587124 shrillecho-1.1.0/shrillecho/utility/__pycache__/sc_to_spot_core.cpython-311.pyc
+-rw-r--r--   0        0        0    23316 2023-11-13 22:16:16.303604 shrillecho-1.1.0/shrillecho/utility/__pycache__/sc_to_spot_new.cpython-311.pyc
+-rw-r--r--   0        0        0    21113 2024-03-05 21:41:22.471298 shrillecho-1.1.0/shrillecho/utility/__pycache__/soundcloud_converter.cpython-311.pyc
+-rw-r--r--   0        0        0    18602 2024-03-14 03:15:29.645819 shrillecho-1.1.0/shrillecho/utility/__pycache__/soundcloud_converter.cpython-312.pyc
+-rw-r--r--   0        0        0      178 2024-02-17 22:31:33.962371 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      166 2024-03-09 22:11:54.464156 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7449 2024-03-14 18:38:34.871820 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/async_spotify.cpython-312.pyc
+-rw-r--r--   0        0        0      168 2024-04-09 21:02:39.480019 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/batch_dump.cpython-312.pyc
+-rw-r--r--   0        0        0     2563 2024-02-17 22:53:45.596137 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-311.pyc
+-rw-r--r--   0        0        0     2239 2024-04-09 21:02:39.484564 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-312.pyc
+-rw-r--r--   0        0        0     6325 2024-02-17 22:31:33.964370 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-311.pyc
+-rw-r--r--   0        0        0     5837 2024-04-09 21:02:39.496708 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-312.pyc
+-rw-r--r--   0        0        0    10837 2024-02-17 22:31:34.179654 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-311.pyc
+-rw-r--r--   0        0        0     9559 2024-03-11 22:58:59.061429 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-312.pyc
+-rw-r--r--   0        0        0     1492 2024-03-14 18:38:34.891285 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/old_cache.cpython-312.pyc
+-rw-r--r--   0        0        0     1319 2024-04-09 21:02:39.548705 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/parsers.cpython-312.pyc
+-rw-r--r--   0        0        0     4145 2024-02-17 22:53:45.598135 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-311.pyc
+-rw-r--r--   0        0        0     3752 2024-04-09 21:02:39.498227 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-312.pyc
+-rw-r--r--   0        0        0     7036 2024-02-17 22:31:34.272143 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-311.pyc
+-rw-r--r--   0        0        0     6309 2024-03-09 22:11:55.082764 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-312.pyc
+-rw-r--r--   0        0        0     5429 2024-02-17 22:31:34.177147 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-311.pyc
+-rw-r--r--   0        0        0     5185 2024-04-01 21:30:38.435593 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-312.pyc
+-rw-r--r--   0        0        0     5236 2024-03-14 02:20:06.773370 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/async_spotify.py
+-rw-r--r--   0        0        0    11306 2024-03-23 00:03:32.882594 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/batch_dump.py
+-rw-r--r--   0        0        0      949 2024-01-07 02:19:15.222777 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/cache.py
+-rw-r--r--   0        0        0     3492 2024-03-11 22:16:21.293179 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/discovery.py
+-rw-r--r--   0        0        0     8352 2024-03-11 22:16:31.726296 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/general.py
+-rw-r--r--   0        0        0      928 2024-03-13 02:07:04.021894 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/old_cache.py
+-rw-r--r--   0        0        0      773 2024-03-11 21:41:34.182076 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/parsers.py
+-rw-r--r--   0        0        0     2659 2024-03-11 22:16:23.348559 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/playlist.py
+-rw-r--r--   0        0        0     3613 2024-01-07 02:19:15.149506 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/scraper.py
+-rw-r--r--   0        0        0     4322 2024-04-01 21:30:24.666771 shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/spotify_client.py
+-rw-r--r--   0        0        0     4063 2024-04-27 23:19:42.172878 shrillecho-1.1.0/shrillecho/utility/cache.py
+-rw-r--r--   0        0        0     2055 2024-03-25 21:52:17.491416 shrillecho-1.1.0/shrillecho/utility/general_utility.py
+-rw-r--r--   0        0        0     1163 2024-04-01 18:53:56.991612 shrillecho-1.1.0/shrillecho/utility/neo4j.py
+-rw-r--r--   0        0        0    11617 2024-03-11 22:16:15.022138 shrillecho-1.1.0/shrillecho/utility/soundcloud_converter.py
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 shrillecho-1.1.0/PKG-INFO
```

### Comparing `shrillecho-1.0.9/pyproject.toml` & `shrillecho-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shrillecho"
-version = "1.0.9"
+version = "1.1.0"
 description = "Music Tool"
 authors = ["simon balfe <sbmain17@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 spotipy = ">=2.23.0,<2.24.0"
 python-dotenv = ">=1.0.0,<1.1.0"
```

### Comparing `shrillecho-1.0.9/shrillecho/auth/local_auth.py` & `shrillecho-1.1.0/shrillecho/auth/local_auth.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/auth/oauth.py` & `shrillecho-1.1.0/shrillecho/auth/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             "grant_type": "refresh_token",
             "refresh_token": refresh_token
         }
         
         response = requests.post(refresh_url, headers=headers, data=body)
         
         if response.status_code == 200:
+        
             return response.json()
         else:
             return f"Failed to refresh token. Status code: {response.status_code}, Response: {response.text}", None
 
     def get_client_access_token(self):
         client_id = os.environ.get("SPOTIPY_CLIENT_ID")
         client_secret = os.environ.get("SPOTIPY_CLIENT_SECRET")
```

### Comparing `shrillecho-1.0.9/shrillecho/playlist/archive/playlist_engine.py` & `shrillecho-1.1.0/shrillecho/playlist/archive/playlist_engine.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/spotify/client.py` & `shrillecho-1.1.0/shrillecho/spotify/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,327 +1,376 @@
 import asyncio
 from dataclasses import asdict, dataclass
 import math
+import random
 import time
 from typing import List, Optional, Type, Union
 from annotated_types import T
 from fastclasses_json import dataclass_json
 import httpx
 import json
 import os
 
+import requests
+import strawberry
+
 from shrillecho.auth.local_auth import authenticate_local
 from shrillecho.auth.oauth import ClientCredentials, OAuthCredentials
-from shrillecho.types.album_types import ArtistAlbums, SeveralAlbums
-from shrillecho.types.artist_types import Artist, SeveralArtists
+from shrillecho.spotify.task_scheduler import TaskScheduler
+from shrillecho.types.album_types import Album, AlbumTracks, ArtistAlbums, SeveralAlbums, SimplifiedAlbum, SimplifiedTrack
+from shrillecho.types.artist_types import Artist, FollowedArtists, SeveralArtists
 from shrillecho.types.playlist_types import Playlist, PlaylistTrack, PlaylistTracks, SimplifiedPlaylistObject, UserPlaylists
-from shrillecho.types.track_types import Recc, SavedTrack, SavedTracks, SeveralTracks, Track
-from shrillecho.utility.general_utility import sp_fetch
+from shrillecho.types.soundcloud_types import User
+from shrillecho.types.track_types import AudioFeatures, Recc, SavedTrack, SavedTracks, SeveralTracks, Track
+from shrillecho.types.user_types import CurrentUserProfile
+from shrillecho.utility.archive_maybe_delete.spotify_client import SpotifyClientGlitch
+from shrillecho.utility.general_utility import get_id, sp_fetch
 import spotipy
 # from shrillecho.auth.local_auth import authenticate_local
 from shrillecho.utility.archive_maybe_delete.old_cache import Cache
-from shrillecho.utility.cache import mongo_client, redis_client
+from shrillecho.utility.cache import cached, mongo_client, redis_client
 import redis
 
 @dataclass
 class SpotifyAuthContext:
     client_id: str
     client_secret: str
     scope: str
     redirect_uri: str
 
+
 class SpotifyClient:
 
-    SPOTIFY_API = "https://api.spotify.com/v1/"
+    __spotify_api = "https://api.spotify.com/v1/"
 
     def __init__(self, auth=None, auth_flow: Union[OAuthCredentials | ClientCredentials] = None):
         self.auth = auth
         self.auth_flow = auth_flow
+        self.access_token = None
         if auth_flow:
             self.access_token = auth_flow.get_access_token()
         else:
             self.access_token = self.auth
         self.temp_spotipy: spotipy.Spotify = spotipy.Spotify(auth=self.access_token)
-        self.http_client: httpx.AsyncClient = httpx.AsyncClient
+        self.http_client: httpx.AsyncClient = httpx.AsyncClient()
         self.redis = redis.Redis(host='localhost', port=6379, db=0)
         self.batch_errors = 0
+        self.rate_lock = asyncio.Event()
+        glitch = SpotifyClientGlitch()
+        self.glitched_token = glitch.access_token
+        self.task_scheduler = TaskScheduler()
+      
+
+        self.batch_param_map = {}
+        self.batch_param_map[SavedTracks] = ()
+        # self.glitched_client_token = glitch.client_token
+      
+    
+    class ShrillechoException(Exception):
+        def __init__(self, message, error_code=None, retry_after: int = None):
+            super().__init__(message)
+            self.error_code = error_code
+            self.retry_after = retry_after
 
-    async def _request(self, 
+
+    def create_get_routine(self, url, resp_type, req_proxy):
+        return (self._get, (url, resp_type, req_proxy))
+       
+    async def _req_proxy(self,
                        method: str, 
                        endpoint: str, 
                        response_type = None,
                        params: Optional[dict] = None, 
                        body: Optional[dict] = None):
         
-        if self.auth:
-            access_token = self.auth
-        elif self.auth_flow:
-            access_token = self.auth_flow.get_access_token()
-        else:
-            raise Exception("No authorization provided to the client")
-
-        headers = {"Authorization" : f"Bearer {access_token}"}
-        
-        async with self.http_client() as client:
-         
-            response = await client.request(method, f"{self.SPOTIFY_API}{endpoint}", params=params, headers=headers, json=body)
-
-            if response.status_code > 300:
-                raise Exception("Spotify Client Error", response.text)
-
-            if response_type:
-                return response_type.from_json(json.dumps(response.json()))
-            else:
-                return response.json()
-        
 
-    async def _async_fetch_urls(self, urls, chunk_size, client, tracks, sp_type):
-        def chunks(lst, n):
-            for i in range(0, len(lst), n):
-                yield lst[i:i + n]
-
-          
-        if self.auth:
-            access_token = self.auth
-        elif self.auth_flow:
-            access_token = self.auth_flow.get_access_token()
+        data = {
+            "params": params,
+            "body": body,
+            "method":  method,
+            "endpoint": f"{self.__spotify_api}{endpoint}"
+        }
+
+
+        response = await self.http_client.post("http://localhost:8002/req", json=data)
+        resp_json = response.json()
+        data= resp_json['data']
+        response.status_code = resp_json['status_code']
+        retry_after = resp_json['retry_after']
+      
+        if response.status_code > 300:
+            retry_after = None
+            if response.status_code == 429:
+                self.rate_lock.set()
+                retry_after = int(retry_after)
+                print(f"sleeping setting lock: {retry_after} seconds")
+                await asyncio.sleep(retry_after)
+                self.rate_lock.clear()
+            
+            print(response.text)
+            raise SpotifyClient.ShrillechoException("Spotify Client Error", error_code=response.status_code, 
+                                                    retry_after=retry_after)
+        if response_type:
+            return response_type.from_json(json.dumps(data))
         else:
-            raise Exception("No authorization provided to the client")
+            return response.json()
+               
 
-        headers = {"Authorization" : f"Bearer {access_token}"}
-
-        for batch in chunks(urls, chunk_size):
-            while len(batch) != 0:
-                print(f"fetching batch size: {len(batch)}")
-                responses = await asyncio.gather(*(client.get(url, headers=headers) for url in batch))
-                passed_responses = []
-                indices_to_remove = []
-                retry = 0
-                for idx, r in enumerate(responses):
-                    if r.status_code == 200:
-                        passed_responses.append(r)
-                        indices_to_remove.append(idx)
-                        # cache the get response for this URL, for retry purposes , wipe it 
-                        # after as we have a complete caching layer, so we dont really want to have this fully caching
-                        # always but maybe consider.
-                    else:
-                        if r.status_code == 429:
-                            retry = int(r.headers.get('Retry-After'))
-                        else:
-                            self.batch_errors += 1 
-                            raise Exception("Batch Error, setting batch size to 10")
-                if retry != 0:
-                    print("rate limit waiting to try again...")
-                    await asyncio.sleep(retry)
-
-                batch = [url for idx, url in enumerate(batch) if idx not in indices_to_remove]
-                if len(passed_responses) > 0:
-                    tracks.extend(sp_fetch(response.json, sp_type) for response in passed_responses)
-            
-    async def _batch_request(self, ep_path: str, initial_item , sp_type: Type[T], *args, chunk_size=25):
-        async with httpx.AsyncClient() as client:
-            urls = []
-            limit = 50
-    
-            items: List[sp_type] = [initial_item]
-        
-            pages = math.ceil(initial_item.total / limit)
+    async def _request(self,
+                       method: str, 
+                       endpoint: str, 
+                       response_type = None,
+                       params: Optional[dict] = None, 
+                       body: Optional[dict] = None, req_proxy: bool = True):
         
-            for page in range(1, pages):
-                urls.append(f"https://api.spotify.com/v1/{ep_path}?limit=50&offset={limit * page}")
-                
-            try:
-                await self._async_fetch_urls(urls, chunk_size, client, items, sp_type)
-            except Exception as e:
-                 if self.batch_errors > 3:
-                      raise Exception("Fatal Error, Batch request failed after 3 retries")
-                 items: List[sp_type] = [initial_item]
-                 await self._async_fetch_urls(urls=urls, client=client, tracks=items, sp_type=sp_type, chunk_size=10)
-
-            self.batch_errors = 0
-
-            """ sort this out, essentially this batcher is designed for paginated requests
-                so we want the items bit all collated into one sequential list
-            """
-            unpacked_items = []
+   
+        req_proxy = False
+        if req_proxy:
+     
+      
+           return await self._req_proxy(method=method, endpoint=endpoint, response_type=response_type, params=params, body=body)
+        
+        headers = {"authorization" : f"Bearer {self.access_token}"}
+        
+        while self.rate_lock.is_set():
+            await asyncio.sleep(1)
+
+        print(f"endpoint: {self.__spotify_api}{endpoint}")
+        response = await self.http_client.request(method, f"{self.__spotify_api}{endpoint}", params=params, headers=headers, json=body)
+        if response.status_code > 300:
+            retry_after = None
+            if response.status_code == 429:
+                self.rate_lock.set()
+                print(response.status_code, response.headers.get('Retry-after'))
+                try:
+                    retry_after = int(response.headers.get('Retry-After'))
+                    print(f"sleeping setting lock: {retry_after} seconds")
+                except:
+                    
+                    retry_after = 5
+                await asyncio.sleep(retry_after)
+                self.rate_lock.clear()
+           
+            # print(response.text)
+            # raise SpotifyClient.ShrillechoException("Spotify Client Error", error_code=response.status_code, 
+            #                                         retry_after=retry_after)
+        if response_type:
+            return response_type.from_json(json.dumps(response.json()))
+        else:
+            return response.json()
         
-            for chunk in items:
-                for cube in chunk.items:
-                        unpacked_items.append(cube)
-
-
-            return unpacked_items
-
-    async def _get(self, endpoint: str, response_type=None, params: Optional[dict]=None):
-        print(f'GETTING: {endpoint}')
-        return await self._request(method="GET", endpoint=endpoint, params=params, response_type=response_type)
+    async def _get(self, endpoint: str, response_type=None,  req_proxy: bool = True , params: Optional[dict]=None):
+     
+        return await self._request(method="GET", endpoint=endpoint, params=params, response_type=response_type, req_proxy=req_proxy)
     
     async def _post(self, endpoint: str, body: dict, params: Optional[dict]=None):
         await self._request(method="POST", endpoint=endpoint, params=params, body=body)
 
-
-
     ############# Shrillecho Implemented Methods #############
 
-    async def me(self) -> SavedTracks:
-        return await self._get("me")
+    @cached(cache_key_prefix="me", class_type=CurrentUserProfile, expiry=3600)
+    async def me(self) -> User:
+        return await self._get("me", response_type=CurrentUserProfile, req_proxy=False)
     
     async def track(self, track: str) -> Track:
-        return await self._get(f"tracks/{track}")
+        return await self._get(f"tracks/{get_id("track", track)}", response_type=Track)
 
-    ################## Spotipy Methods ####################
-
-    async def playlist(self, playlist_id: str) -> Playlist:
-        pl_id = self.temp_spotipy._get_id("artist", playlist_id)
-
-        async def cache_update_function() -> Playlist:
-            return sp_fetch(self.temp_spotipy.playlist, Playlist, pl_id)
-        
-        cache_response: Artist = await redis_client.cache_query(cache_key=f"playlist_{pl_id}", 
-                                        class_type=Playlist, 
-                                        cache_update_function=cache_update_function, 
-                                        expiry=100)
+    @cached(cache_key_prefix="album", class_type=Album, expiry=3600)
+    async def album(self, album: str) -> Track:
+        return await self._get(f"albums/{get_id("album", album)}", response_type=Album)
+
+    @cached(cache_key_prefix="artist", class_type=Artist, expiry=3600)
+    async def artist(self, artist: str) -> Track:
+        return await self._get(f"artists/{get_id("artist", artist)}", response_type=Artist)
+
+    async def tracks(self, tracks) -> List[Track]:
+        tlist = [get_id("track", t) for t in tracks]
+        s_tracks: SeveralTracks = await self._get("tracks/?ids=" + ",".join(tlist), response_type=SeveralTracks)
+        return s_tracks.tracks
+
+    @cached(cache_key_prefix="artist_related", class_type=Artist, expiry=1000)
+    async def artist_related(self, artist: str) -> List[Artist]:
+        artist_id = get_id("artist", artist)
+        several_artists: SeveralArtists = await self._get(f"artists/{artist_id}/related-artists", response_type=SeveralArtists)
+        return several_artists.artists
 
-        return cache_response
+    async def recccs(self) -> Recc:
+        return await self._get("recommendations?limit=50&seed_tracks=5m4Lh4bgiYKSj2MlDcrnxh", response_type=Recc)
     
-    async def artist_related_artists(self, artist: str, invalidate_cache=False) -> List[Artist]:
-
-        async def related_artists() -> SeveralArtists:
-            return sp_fetch(self.temp_spotipy.artist_related_artists, SeveralArtists, artist)
-        
-        if invalidate_cache:
-            self.redis.delete(f"artist_related_{artist}")
-
-        cache_respnse = await redis_client.cache_query(cache_key=f"artist_related_{artist}", 
-                                          cache_update_function=related_artists, 
-                                          expiry=3600, 
-                                          class_type=SeveralArtists)
-        return cache_respnse.artists
+    async def artists(self, artists: List[str]) -> SeveralArtists:
+        artist_ids = [get_id("artist", a) for a in artists]
+        return await self._get("artists?ids=" + ",".join(artist_ids), response_type=SeveralArtists)
     
-
-    async def artist(self, artist_id: str) -> Artist:
-        art_id = self.temp_spotipy._get_id("artist", artist_id)
-
-        async def cache_update_function() -> Artist:
-            return sp_fetch(self.temp_spotipy.artist, Artist, art_id)
+    async def artist_albums_single(self, artist, limit=50, offset=None) -> ArtistAlbums:
+        return await self._get(f"artists/{get_id("artist", artist)}/albums?limit={limit}&offset={offset}", response_type=ArtistAlbums)
         
-        cache_response: Artist = await redis_client.cache_query(cache_key=f"artist_{art_id}", 
-                                        class_type=Artist, 
-                                        cache_update_function=cache_update_function, 
-                                        expiry=100)
-        return cache_response
+    async def current_user_followed_artists(self, limit: int = 20, after=None) -> FollowedArtists:
+       
+        return await self._get(f"me/following?type=artist&limit={limit}&after={after}", response_type=FollowedArtists, req_proxy=False)
+       
+    async def audio_features(self, track) -> AudioFeatures:
+        return await self._get(f"audio-features/{get_id('track', track)}", response_type=AudioFeatures, req_proxy=False)
 
+    ################## Spotipy Methods ####################
 
-    async def artist_albums(self, artist_id: str, album_type: str):
+    async def followed_artists(self):
+        self.temp_spotipy.current_user_followed_artists() 
+        return sp_fetch(self.temp_spotipy.current_user_following_artists)
 
-        return sp_fetch(self.temp_spotipy.artist_albums, ArtistAlbums, artist_id,
-                        album_type=album_type)
+    @cached(cache_key_prefix="playlist", class_type=Playlist, expiry=3600)
+    async def playlist(self, playlist_id: str) -> Playlist:
+        return sp_fetch(self.temp_spotipy.playlist, Playlist, get_id("playlist", playlist_id))
+        
+    @cached(cache_key_prefix="artist_related", class_type=SeveralArtists, expiry=3600)
+    async def artist_related_artists(self, artist: str) -> List[Artist]:
+        
+        return sp_fetch(self.temp_spotipy.artist_related_artists, SeveralArtists, artist)
+       
+    # @cached(cache_key_prefix="artist", class_type=Artist, expiry=3600)
+    # async def artist(self, artist_id: str) -> Artist:
+    #     return sp_fetch(self.temp_spotipy.artist, Artist, get_id("artist", artist_id))
+        
+    # async def artist_albums_single(self, artist, limit=50, offset=None) -> ArtistAlbums:
+    #     return sp_fetch(self.temp_spotipy.artist_albums, ArtistAlbums, artist, limit=limit, offset=offset)
     
     async def albums(self, albums) -> SeveralAlbums:
-        sp_fetch(self.temp_spotipy.albums, SeveralAlbums, albums)
+        return sp_fetch(self.temp_spotipy.albums, SeveralAlbums, albums)
     
-    async def tracks(self, tracks) -> SeveralTracks:
-        sp_fetch(self.temp_spotipy.tracks, SeveralTracks, tracks)
+    # async def tracks(self, tracks) -> SeveralTracks:
+    #     return sp_fetch(self.temp_spotipy.tracks, SeveralTracks, tracks)
 
     async def user_playlist_create(self, user:str , name:str, public: bool):
         return self.temp_spotipy.user_playlist_create(user=user, name=name, public=public)
 
     async def playlist_add_items(self, playlist_id: str, tracks) -> None:
         self.temp_spotipy.playlist_add_items(playlist_id, tracks)
 
     async def current_user_unfollow_playlist(self, playlist_uri) -> None:
         self.temp_spotipy.current_user_unfollow_playlist(playlist_uri)
 
-    async def reccomendations(self, limit, seed_artists=None,seed_genres=None,seed_tracks=None,country=None, track_list=True) -> Recc:
+    async def reccomendations(self, limit, seed_artists=None,seed_genres=None,seed_tracks=None,country=None, track_list=True) -> Recc | List[Track]:
 
         reccs:  Recc = sp_fetch(self.temp_spotipy.recommendations, 
                               Recc, 
                               limit=limit, 
                               seed_tracks=seed_tracks, 
                               seed_artists=seed_artists, seed_genres=seed_genres)
         if track_list:
             return reccs.tracks
     
         return reccs 
 
+                
+    async def current_user_followed_artists(self, limit: int = 20, after=None) -> FollowedArtists :
+        return sp_fetch(self.temp_spotipy.current_user_followed_artists, FollowedArtists, limit=limit, after=after)
+    
     ################### BATCHING METHODS ############################
         
-    async def current_user_saved_tracks(self,limit: int = None, 
-                                        offset: int = None, batch=False,  chunk_size = 25, invalidate_cache=False, track_list=True) -> List[SavedTrack] | SavedTracks:
-        if not batch:
-            return await self._get(f"me/tracks?offset={offset}&limit={limit}")
-        
-        async def batch_request() -> List[SavedTrack]:
-            initial_item = await self._get(f"me/tracks?offset={0}&limit={50}", response_type=SavedTracks)
-            return await self._batch_request(ep_path="me/tracks", 
-                                        initial_item=initial_item,
-                                            sp_type=SavedTracks,
-                                            chunk_size=chunk_size)
-        if invalidate_cache:
-            self.redis.delete("my_tracks")
+    @staticmethod
+    def generate_pagination_batch_urls(ep_path: str, initial_item , query_params = None) -> List[str]:
+        urls = []
+        limit = 50
+        pages = math.ceil(initial_item.total / limit)
+        for page in range(0, pages):
+            urls.append(f"{ep_path}?limit=50&offset={limit * page}")
+        return urls
+    
+    async def batch_pagination_tasks(self, class_type, batch_size=5, *args, **kwargs):
+        """
+            Utilises the task scheduler to batch paginated pages, only works with endpoints
+            that have the items, total, next, limit, offset attributes i.e most pagination endpoints
+
+            NOTE: This unpacks by default the results and expands `tracks` attribute to track, consider making this optional to a granular level
+        """
+
+        req_proxy = True
+        if class_type == SavedTracks:
+            ep_path = "me/tracks"
+            req_proxy = False
+            initial_item = await self._get(f"me/tracks?offset={0}&limit={50}", response_type=SavedTracks, req_proxy=False )
+
+        elif class_type == PlaylistTracks:
+            playlist_id = kwargs.get('playlist_id')
+            ep_path = f"playlists/{playlist_id}/tracks"
+            initial_item = await self._get(f"playlists/{playlist_id}/tracks?offset={0}&limit={50}", response_type=PlaylistTracks)
+
+        elif class_type == UserPlaylists:
+            
+            if kwargs.get('user_id'):
+                user = kwargs.get('user_id')
+                ep_path = f"users/{user}/playlists"
+                user = kwargs.get('user_id')
+                initial_item = await self._get(f"users/{user}/playlists?offset={0}&limit={50}", response_type=UserPlaylists)
+            else:
+                ep_path = "me/playlists"
+               
+                req_proxy = False
+                initial_item = await self._get(f"me/playlists?offset={0}&limit={50}", response_type=UserPlaylists, req_proxy=False)
+
+        elif class_type == AlbumTracks:
+            album_id = kwargs.get('album_id')
+            ep_path = f"albums/{album_id}/tracks"
+            initial_item = await self._get(f"albums/{album_id}/tracks?offset={0}&limit={50}", response_type=AlbumTracks)
+
+        elif class_type == ArtistAlbums:
+            artist = kwargs.get("artist_id")
+    
+            ep_path = f"artists/{artist}/albums"
+            initial_item = await self._get(f"artists/{artist}/albums?offset={0}&limit={50}", response_type=ArtistAlbums)
+
+        urls = SpotifyClient.generate_pagination_batch_urls(ep_path=ep_path, 
+                                                                  initial_item=initial_item )
+        tasks = [
+            self.create_get_routine(url, class_type, req_proxy=req_proxy) for url in urls
+        ]
+
+        self.task_scheduler.load_tasks(tasks)
+
+        return await self.task_scheduler.execute_tasks(batch_size=batch_size, unpack=True)
+
+    @cached(cache_key_prefix="saved_tracks_0", class_type=Track)
+    async def current_user_saved_tracks(self) -> List[Track]:
+        """
+            LIKED SONGS
+        """
+        return await self.batch_pagination_tasks(class_type=SavedTracks, batch_size=5)
+    
+    @cached(cache_key_prefix="my_playlists", class_type=SimplifiedPlaylistObject)
+    async def current_user_saved_playlists(self) -> List[SimplifiedPlaylistObject]:
+        """
+            CURRENT USER PLAYLISTS 
+        """
+        return await self.batch_pagination_tasks(class_type=UserPlaylists, batch_size=1)
+    
+    @cached(cache_key_prefix="user_playlist", class_type=SimplifiedPlaylistObject)
+    async def user_playlists(self, user: str):
+        """
+            SPECIFIC USER PLAYLISTS
+        """
+        return await self.batch_pagination_tasks(class_type=UserPlaylists, batch_size=5, user_id=user)
+    
+    @cached(cache_key_prefix="playlist_tracksss", class_type=Track)
+    async def playlist_tracks(self, playlist_id: str):
+        """
+            TRACKS FROM A PLAYLIST
+
+        """
+        return await self.batch_pagination_tasks(class_type=PlaylistTracks, batch_size=50, playlist_id=get_id("playlist", playlist_id))
+    
+    @cached(cache_key_prefix="album_tracksss", class_type=SimplifiedTrack)
+    async def album_tracks(self, album: str):
+        """
+            TRACKS FROM AN ALBUM
+        """
+    
+      
+        return await self.batch_pagination_tasks(class_type=AlbumTracks, batch_size=2, album_id=get_id('album', album))
+    
+    @cached(cache_key_prefix="artist_albumss", class_type=SimplifiedAlbum)
+    async def artist_albums(self,artist: str):
+        """
+            ALBUMS FROM AN ARTIST
+        """
+    
+        return await self.batch_pagination_tasks(class_type=ArtistAlbums, batch_size=2, artist_id=artist)
 
 
-        saved_tracks: List[SavedTrack] = await redis_client.cache_query(cache_key="my_tracks", 
-                                          cache_update_function=batch_request, 
-                                          expiry=3600, 
-                                          class_type=SavedTrack)
-        if track_list:
-            tracks: List[Track] = []
-            for item in saved_tracks:
-                tracks.append(item.track)
-            return tracks
-
-        return await saved_tracks
-    
-    async def current_user_saved_playlists(self,limit: int = None, 
-                                        offset: int = None,
-                                          batch=False,
-                                          chunk_size=25, invalidate_cache=False) -> List[SimplifiedPlaylistObject] | UserPlaylists:
-        
-        cache_key = "my_playlists_new_cache"
-        ep = "me/playlists"
-        
-        if not batch:
-            return await self._get(f"{ep}?offset={offset}&limit={limit}", response_type=UserPlaylists)
-        
-        async def batch_request() -> List[SimplifiedPlaylistObject]:
-            initial_item = await self._get(f"{ep}?offset={0}&limit={50}", response_type=UserPlaylists)
-            return await self._batch_request(ep_path=ep, 
-                                        initial_item=initial_item,
-                                            sp_type=UserPlaylists,
-                                            chunk_size=chunk_size)
-        if invalidate_cache:
-            self.redis.delete(cache_key)
-
-        print("############ QUERYING CACHE ###################")
-        return await redis_client.cache_query(cache_key=cache_key, 
-                                          cache_update_function=batch_request, 
-                                          expiry=3600, 
-                                          class_type=SimplifiedPlaylistObject)
-
-    async def playlist_tracks(self, playlist_id, limit: int = None, 
-                                        offset: int = None,
-                                          batch=False,
-                                          chunk_size=25, invalidate_cache=False, track_list=True) -> List[PlaylistTrack] | List[Track] | PlaylistTracks:
-        if not batch:
-            return await self._get(f"playlists/{playlist_id}/tracks?offset={offset}&limit={limit}", response_type=PlaylistTracks)
-        
-        async def batch_request() -> List[PlaylistTrack]:
-            initial_item = await self._get(f"playlists/{playlist_id}/tracks?offset={0}&limit={50}", response_type=PlaylistTracks)
-            return await self._batch_request(ep_path=f"playlists/{playlist_id}/tracks", 
-                                        initial_item=initial_item,
-                                            sp_type=PlaylistTracks,
-                                            chunk_size=chunk_size)
-        if invalidate_cache:
-            self.redis.delete(f"playlist_tracks_{playlist_id}")
-
-        playlist_tracks: List[PlaylistTrack] = await redis_client.cache_query(cache_key=f"playlist_tracks_{playlist_id}", 
-                                          cache_update_function=batch_request, 
-                                          expiry=3600, 
-                                          class_type=PlaylistTrack)
-        if track_list:
-            tracks: List[Track] = []
-            for item in playlist_tracks:
-                tracks.append(item.track)
-            return tracks
-        
-        return playlist_tracks
```

### Comparing `shrillecho-1.0.9/shrillecho/types/album_types.py` & `shrillecho-1.1.0/shrillecho/types/album_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/types/archive_delete/all.py` & `shrillecho-1.1.0/shrillecho/types/archive_delete/all.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/types/artist_types.py` & `shrillecho-1.1.0/shrillecho/types/user_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import List, TYPE_CHECKING, Optional
+from __future__ import annotations
+from typing import List
 from .base_types import *
 
+
 @dataclass_json
 @dataclass
-class Artist:
+class CurrentUserProfile:
+    display_name: str
     external_urls: ExternalUrls
     href: str
     id: str
-    name: str
+    images: List[Image]
     type: str
     uri: str
-    followers: Optional[Followers] = None
-    genres: Optional[List[str]] = None
-    images: Optional[List[Image]] = None
-    popularity: Optional[int] = None
+    followers: Followers
+    country: Optional[str] = None
+    product: Optional[str] = None
+    explicit_content: Optional[ExplicitContent] = None
+    email: str = None
+    birthdate: Optional[str] = None
+    policies: Optional[Policies] = None
 
 
 @dataclass_json
 @dataclass
-class SimpleArtist:
+class UserProfile:
+    display_name: str
     external_urls: ExternalUrls
+    followers: Followers
+    href: str
     id: str
-    name: str
+    images: List[Image]
     type: str
     uri: str
-    href: Optional[str] = None
-
-@dataclass_json
-@dataclass
-class SeveralArtists:
-    artists: List[Artist]
-
```

### Comparing `shrillecho-1.0.9/shrillecho/types/base_types.py` & `shrillecho-1.1.0/shrillecho/types/base_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/types/component_types.py` & `shrillecho-1.1.0/shrillecho/types/component_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/types/playlist_types.py` & `shrillecho-1.1.0/shrillecho/types/playlist_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/types/soundcloud_types.py` & `shrillecho-1.1.0/shrillecho/types/soundcloud_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/types/track_types.py` & `shrillecho-1.1.0/shrillecho/types/track_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,33 @@
-from typing import List, TYPE_CHECKING
+from tkinter.tix import CheckList
+from typing import List, TYPE_CHECKING, Self
+
+import strawberry
 from .base_types import *
 from shrillecho.types.album_types import Album
 from shrillecho.types.artist_types import Artist
 from shrillecho.types.component_types import LinkedFrom
 
+import hashlib
+
+def string_to_number(s):
+    if "Among" in s:
+        print(f"input_string : \"{s}\"")
+    # Convert the string to bytes
+    s_bytes = s.encode('utf-8')
+    
+    # Calculate the SHA-256 hash
+    hash_object = hashlib.sha256(s_bytes)
+    hash_value = hash_object.hexdigest()
+    
+    # Convert the hexadecimal hash value to an integer
+    number = int(hash_value, 16)
+    if "Among" in s:
+        print(f"output: {number}")
+    return number
 
 @dataclass_json
 @dataclass
 class Track:
     """ Get track - https://developer.spotify.com/documentation/web-api/reference/get-track """
     album: Album
     artists: List[Artist]
@@ -21,25 +41,46 @@
     id: str
     name: str
     preview_url: str
     track_number: int
     type: str
     uri: str
     is_local: bool
+    popularity: str
     restrictions: Optional[Restrictions] = None
     is_playable: Optional[bool] = None
     linked_from: Optional[LinkedFrom] = None
+    liked: Optional[bool] = None
 
     def __eq__(self, other):
         if isinstance(other, Track):
-            return self.external_ids.isrc == other.external_ids.isrc
+         
+            try:
+                if self.external_ids.isrc == other.external_ids.isrc:
+                    return True 
+                elif (self.artists[0].id == other.artists[0].id) and (self.name == other.name):
+                    return True 
+                
+              
+                return False
+            except:
+             
+                return False
         return False
+    
     def __hash__(self):
-        return hash(self.external_ids.isrc)
-@dataclass_json
+
+        # if we have valid artist use that otherwise just use the name
+        try:
+            return hash((str.lower(self.name), str.lower(self.artists[0].id)))
+        except:
+            return hash((str.lower(self.name)))
+      
+
+
 @dataclass
 class TrackSearchItems:
     href: str
     limit: int
     next: str
     offset: int
     previous: str
@@ -109,16 +150,14 @@
 
 @dataclass_json
 @dataclass
 class TrackInfo:
     href: str
     total: int
 
-
-
 @dataclass_json
 @dataclass
 class SeveralTracks:
     """ Get several tracks - https://developer.spotify.com/documentation/web-api/reference/get-several-tracks"""
     tracks: List[Track]
 
 @dataclass_json
@@ -133,7 +172,29 @@
 
 @dataclass_json
 @dataclass
 class Recc:
     """ Get several tracks - https://developer.spotify.com/documentation/web-api/reference/get-several-tracks"""
     seeds: List[ReccSeed]
     tracks: List[Track]
+
+@dataclass_json
+@dataclass
+class AudioFeatures:
+    acousticness: float
+    analysis_url: str
+    danceability: float
+    duration_ms: int
+    energy: float
+    id: str
+    instrumentalness: float
+    key: int
+    liveness: float
+    loudness: float
+    mode: int
+    speechiness: float
+    tempo: float
+    time_signature: int
+    track_href: str
+    type: str
+    uri: str
+    valence: float
```

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/async_spotify.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/async_spotify.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/cache.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/cache.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/discovery.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/discovery.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/general.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/general.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/old_cache.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/old_cache.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/parsers.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/parsers.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/playlist.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/playlist.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/archive_maybe_delete/scraper.py` & `shrillecho-1.1.0/shrillecho/utility/archive_maybe_delete/scraper.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/shrillecho/utility/cache.py` & `shrillecho-1.1.0/shrillecho/utility/cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from abc import ABC, abstractmethod
 import datetime
+from functools import wraps
+import hashlib
 import json
 from dataclasses import asdict
 from pymongo import MongoClient
 import redis
 
 
 
@@ -54,39 +56,68 @@
 
     def __init__(self, host: str, port: str):
         self.redis_client = redis.Redis(host=host, port=port, db=0)
 
     async def cache_query(self, cache_key: str, cache_update_function, expiry, class_type, **kwargs):
         cached_value = self.redis_client.get(cache_key)
         if cached_value:
-            print(f"getting cached: {cache_key}")
             retrieved_value = json.loads(cached_value)
-
+            # print(f"[REDIS CACHE] Existing entry {cache_key}")
             if isinstance(retrieved_value, list):
                 return [class_type.from_json(json.dumps(item)) for item in retrieved_value]
 
             return class_type.from_json(json.dumps(retrieved_value))
         else:
-            print("############ FETCHIN NEW, NOT CACHED ###################")
-            print(f"refetching {cache_key}")
+            # print(f"[REDIS CACHE] New entry {cache_key}")
             new_value = await cache_update_function()
 
             if isinstance(new_value, list):
-                new_value_dict = [asdict(item) for item in new_value]
+        
+                new_value_dict = []
+
+                for item in new_value:
+                    if item:
+                        new_value_dict.append(asdict(item))
             else:
+
+                print(type(new_value))
                 new_value_dict = asdict(new_value)
 
             self.redis_client.set(cache_key, json.dumps(new_value_dict), ex=expiry)
             
             return new_value
 
 
 mongo_client = Mongo('localhost', '27017', 'shrillecho')
 redis_client = Redis('localhost', '6379')
 
+def cached(cache_key_prefix, class_type, expiry=3600, invalidate_cache=False):
+    def decorator(func):
+        @wraps(func)
+        async def wrapper(*args, **kwargs):
+     
+            args_str = "_".join([str(arg) for arg in args[1:]])
+            kwargs_str = "_".join([f"{k}_{v}" for k, v in kwargs.items()])
+            dynamic_part = f"{args_str}_{kwargs_str}"
+
+            dynamic_hash = hashlib.sha256(dynamic_part.encode()).hexdigest()
+
+
+            full_cache_key = f"{cache_key_prefix}_{dynamic_hash}"
+        
+            # if invalidate_cache:
+            #     await CacheManager.invalidate_cache(full_cache_key)
+
+            async def update_function():
+                return await func(*args, **kwargs)
+            
+            return await redis_client.cache_query(full_cache_key, update_function, expiry, class_type)
+        return wrapper
+    return decorator
+
```

### Comparing `shrillecho-1.0.9/shrillecho/utility/soundcloud_converter.py` & `shrillecho-1.1.0/shrillecho/utility/soundcloud_converter.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.0.9/PKG-INFO` & `shrillecho-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrillecho
-Version: 1.0.9
+Version: 1.1.0
 Summary: Music Tool
 Author: simon balfe
 Author-email: sbmain17@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

