# Comparing `tmp/shrillecho-1.1.1.tar.gz` & `tmp/shrillecho-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrillecho-1.1.1.tar", max compression
+gzip compressed data, was "shrillecho-1.1.2.tar", max compression
```

## Comparing `shrillecho-1.1.1.tar` & `shrillecho-1.1.2.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0     1165 2024-05-06 13:56:09.658641 shrillecho-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       32 2023-09-23 15:03:19.005437 shrillecho-1.1.1/shrillecho/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 20:55:44.836628 shrillecho-1.1.1/shrillecho/album/__init__.py
--rw-r--r--   0        0        0      987 2024-04-17 21:40:51.698889 shrillecho-1.1.1/shrillecho/album/album_controller.py
--rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.1.1/shrillecho/artist/__init__.py
--rw-r--r--   0        0        0      160 2023-09-23 15:05:30.663260 shrillecho-1.1.1/shrillecho/artist/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2024-03-14 02:58:16.623582 shrillecho-1.1.1/shrillecho/artist/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    11625 2024-04-17 20:29:10.940781 shrillecho-1.1.1/shrillecho/artist/__pycache__/spotify_artist.cpython-312.pyc
--rw-r--r--   0        0        0     2748 2024-04-21 22:40:07.469215 shrillecho-1.1.1/shrillecho/artist/artist_controller.py
--rw-r--r--   0        0        0     1009 2024-04-17 20:01:34.862797 shrillecho-1.1.1/shrillecho/artist/sp_artist.py
--rw-r--r--   0        0        0     8785 2024-04-17 20:29:10.024946 shrillecho-1.1.1/shrillecho/artist/spotify_artist.py
--rw-r--r--   0        0        0       29 2023-09-23 15:03:19.005437 shrillecho-1.1.1/shrillecho/auth/__init__.py
--rw-r--r--   0        0        0      193 2023-09-23 15:05:30.403768 shrillecho-1.1.1/shrillecho/auth/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      178 2024-03-09 15:04:18.657207 shrillecho-1.1.1/shrillecho/auth/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4720 2024-03-12 19:30:51.569168 shrillecho-1.1.1/shrillecho/auth/__pycache__/local_auth.cpython-312.pyc
--rw-r--r--   0        0        0     5424 2024-03-13 22:52:25.720959 shrillecho-1.1.1/shrillecho/auth/__pycache__/oauth.cpython-311.pyc
--rw-r--r--   0        0        0    11554 2024-03-17 00:55:57.542250 shrillecho-1.1.1/shrillecho/auth/__pycache__/oauth.cpython-312.pyc
--rw-r--r--   0        0        0      525 2024-03-12 19:28:02.938593 shrillecho-1.1.1/shrillecho/auth/__pycache__/spotify_auth.cpython-312.pyc
--rw-r--r--   0        0        0     2816 2024-03-12 19:28:42.468224 shrillecho-1.1.1/shrillecho/auth/local_auth.py
--rw-r--r--   0        0        0     7720 2024-03-17 00:55:39.759059 shrillecho-1.1.1/shrillecho/auth/oauth.py
--rw-r--r--   0        0        0      156 2024-03-12 19:27:15.771836 shrillecho-1.1.1/shrillecho/auth/spotify_auth.py
--rw-r--r--   0        0        0        0 2024-03-11 21:00:35.951586 shrillecho-1.1.1/shrillecho/player/__init__.py
--rw-r--r--   0        0        0      144 2024-04-09 21:02:32.629853 shrillecho-1.1.1/shrillecho/player/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      904 2024-04-09 21:02:32.631375 shrillecho-1.1.1/shrillecho/player/__pycache__/spotify_player.cpython-312.pyc
--rw-r--r--   0        0        0      359 2024-03-11 22:18:56.285682 shrillecho-1.1.1/shrillecho/player/spotify_player.py
--rw-r--r--   0        0        0       24 2023-09-23 15:03:19.005437 shrillecho-1.1.1/shrillecho/playlist/__init__.py
--rw-r--r--   0        0        0      192 2023-09-23 17:32:16.346106 shrillecho-1.1.1/shrillecho/playlist/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      177 2024-03-09 15:02:13.039686 shrillecho-1.1.1/shrillecho/playlist/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1940 2024-04-20 10:39:20.711449 shrillecho-1.1.1/shrillecho/playlist/__pycache__/playlist_controller.cpython-312.pyc
--rw-r--r--   0        0        0     4070 2024-01-12 22:36:57.888928 shrillecho-1.1.1/shrillecho/playlist/__pycache__/playlist_engine.cpython-311.pyc
--rw-r--r--   0        0        0     3763 2024-03-09 15:02:13.041686 shrillecho-1.1.1/shrillecho/playlist/__pycache__/playlist_engine.cpython-312.pyc
--rw-r--r--   0        0        0     5128 2024-04-21 21:13:00.466645 shrillecho-1.1.1/shrillecho/playlist/__pycache__/spotify_playlist.cpython-312.pyc
--rw-r--r--   0        0        0     7244 2024-04-20 10:45:03.486766 shrillecho-1.1.1/shrillecho/playlist/__pycache__/virtual_playlist.cpython-312.pyc
--rw-r--r--   0        0        0     3776 2024-03-11 22:58:55.429565 shrillecho-1.1.1/shrillecho/playlist/archive/__pycache__/playlist_engine.cpython-312.pyc
--rw-r--r--   0        0        0     2306 2024-03-11 22:16:24.766938 shrillecho-1.1.1/shrillecho/playlist/archive/playlist_engine.py
--rw-r--r--   0        0        0     1221 2024-04-17 22:20:31.920970 shrillecho-1.1.1/shrillecho/playlist/playlist_controller.py
--rw-r--r--   0        0        0     4389 2024-04-21 20:26:12.833324 shrillecho-1.1.1/shrillecho/playlist/spotify_playlist.py
--rw-r--r--   0        0        0     4256 2024-04-20 10:44:19.895473 shrillecho-1.1.1/shrillecho/playlist/virtual_playlist.py
--rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.1.1/shrillecho/scraping/__init__.py
--rw-r--r--   0        0        0      162 2023-09-23 15:05:30.663260 shrillecho-1.1.1/shrillecho/scraping/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      146 2024-03-14 18:38:34.308684 shrillecho-1.1.1/shrillecho/scraping/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3653 2024-04-17 19:53:12.059070 shrillecho-1.1.1/shrillecho/scraping/__pycache__/browser_auth.cpython-312.pyc
--rw-r--r--   0        0        0     2051 2024-04-17 19:46:10.197061 shrillecho-1.1.1/shrillecho/scraping/browser_auth.py
--rw-r--r--   0        0        0        0 2024-03-12 18:59:09.355126 shrillecho-1.1.1/shrillecho/spotify/__init__.py
--rw-r--r--   0        0        0      145 2024-03-12 19:19:14.425028 shrillecho-1.1.1/shrillecho/spotify/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    22970 2024-04-28 00:26:11.161172 shrillecho-1.1.1/shrillecho/spotify/__pycache__/client.cpython-312.pyc
--rw-r--r--   0        0        0     3480 2024-04-21 21:54:52.990207 shrillecho-1.1.1/shrillecho/spotify/__pycache__/task_scheduler.cpython-312.pyc
--rw-r--r--   0        0        0    16853 2024-04-28 00:26:00.407579 shrillecho-1.1.1/shrillecho/spotify/client.py
--rw-r--r--   0        0        0     2489 2024-04-21 21:54:39.662490 shrillecho-1.1.1/shrillecho/spotify/task_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-11 20:48:31.986990 shrillecho-1.1.1/shrillecho/track/__init__.py
--rw-r--r--   0        0        0      143 2024-03-11 22:58:59.259675 shrillecho-1.1.1/shrillecho/track/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7545 2024-04-11 22:51:50.359779 shrillecho-1.1.1/shrillecho/track/__pycache__/spotify_track.cpython-312.pyc
--rw-r--r--   0        0        0     2379 2024-04-12 23:08:45.923483 shrillecho-1.1.1/shrillecho/track/__pycache__/tracks_wrapper.cpython-312.pyc
--rw-r--r--   0        0        0     5159 2024-04-11 22:51:22.177465 shrillecho-1.1.1/shrillecho/track/spotify_track.py
--rw-r--r--   0        0        0        0 2023-10-14 18:10:24.959970 shrillecho-1.1.1/shrillecho/types/__init__.py
--rw-r--r--   0        0        0      155 2023-10-14 18:10:25.750276 shrillecho-1.1.1/shrillecho/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      143 2024-03-09 15:02:13.064686 shrillecho-1.1.1/shrillecho/types/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4307 2024-03-11 22:58:55.468913 shrillecho-1.1.1/shrillecho/types/__pycache__/album_types.cpython-312.pyc
--rw-r--r--   0        0        0     5278 2024-01-12 22:34:54.354054 shrillecho-1.1.1/shrillecho/types/__pycache__/albums.cpython-311.pyc
--rw-r--r--   0        0        0     4292 2024-03-09 15:04:17.730511 shrillecho-1.1.1/shrillecho/types/__pycache__/albums.cpython-312.pyc
--rw-r--r--   0        0        0     2658 2024-04-17 20:27:50.732389 shrillecho-1.1.1/shrillecho/types/__pycache__/artist_types.cpython-312.pyc
--rw-r--r--   0        0        0     1908 2024-01-12 22:34:54.356055 shrillecho-1.1.1/shrillecho/types/__pycache__/artists.cpython-311.pyc
--rw-r--r--   0        0        0     1538 2024-03-09 15:04:17.731520 shrillecho-1.1.1/shrillecho/types/__pycache__/artists.cpython-312.pyc
--rw-r--r--   0        0        0     3173 2023-11-05 23:56:15.061834 shrillecho-1.1.1/shrillecho/types/__pycache__/base_types.cpython-311.pyc
--rw-r--r--   0        0        0     2488 2024-03-09 15:02:13.071687 shrillecho-1.1.1/shrillecho/types/__pycache__/base_types.cpython-312.pyc
--rw-r--r--   0        0        0     1736 2024-03-11 22:58:55.436070 shrillecho-1.1.1/shrillecho/types/__pycache__/component_types.cpython-312.pyc
--rw-r--r--   0        0        0     2134 2024-01-07 02:24:45.003341 shrillecho-1.1.1/shrillecho/types/__pycache__/components.cpython-311.pyc
--rw-r--r--   0        0        0     1731 2024-03-09 15:02:13.068686 shrillecho-1.1.1/shrillecho/types/__pycache__/components.cpython-312.pyc
--rw-r--r--   0        0        0     3496 2024-03-14 02:19:29.826797 shrillecho-1.1.1/shrillecho/types/__pycache__/playlist_types.cpython-312.pyc
--rw-r--r--   0        0        0     4298 2024-01-12 22:34:54.294325 shrillecho-1.1.1/shrillecho/types/__pycache__/playlists.cpython-311.pyc
--rw-r--r--   0        0        0     3472 2024-03-09 15:02:13.067686 shrillecho-1.1.1/shrillecho/types/__pycache__/playlists.cpython-312.pyc
--rw-r--r--   0        0        0     6664 2024-02-24 03:23:54.874109 shrillecho-1.1.1/shrillecho/types/__pycache__/sc.cpython-311.pyc
--rw-r--r--   0        0        0     5792 2024-03-09 16:03:46.602847 shrillecho-1.1.1/shrillecho/types/__pycache__/sc.cpython-312.pyc
--rw-r--r--   0        0        0     5806 2024-03-14 03:15:29.847360 shrillecho-1.1.1/shrillecho/types/__pycache__/soundcloud_types.cpython-312.pyc
--rw-r--r--   0        0        0     7857 2024-04-27 21:55:25.752930 shrillecho-1.1.1/shrillecho/types/__pycache__/track_types.cpython-312.pyc
--rw-r--r--   0        0        0     7020 2024-03-06 18:45:37.173792 shrillecho-1.1.1/shrillecho/types/__pycache__/tracks.cpython-311.pyc
--rw-r--r--   0        0        0     5798 2024-03-09 15:04:17.728996 shrillecho-1.1.1/shrillecho/types/__pycache__/tracks.cpython-312.pyc
--rw-r--r--   0        0        0     1463 2024-03-11 22:58:55.480875 shrillecho-1.1.1/shrillecho/types/__pycache__/user_types.cpython-312.pyc
--rw-r--r--   0        0        0     1755 2024-01-12 22:34:54.365174 shrillecho-1.1.1/shrillecho/types/__pycache__/users.cpython-311.pyc
--rw-r--r--   0        0        0     1458 2024-03-09 15:04:17.742095 shrillecho-1.1.1/shrillecho/types/__pycache__/users.cpython-312.pyc
--rw-r--r--   0        0        0     2602 2024-03-11 22:15:02.628111 shrillecho-1.1.1/shrillecho/types/album_types.py
--rw-r--r--   0        0        0      158 2024-04-09 21:02:35.162480 shrillecho-1.1.1/shrillecho/types/archive_delete/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      521 2024-04-09 21:02:35.163998 shrillecho-1.1.1/shrillecho/types/archive_delete/__pycache__/all.cpython-312.pyc
--rw-r--r--   0        0        0     5529 2024-03-11 22:16:14.402147 shrillecho-1.1.1/shrillecho/types/archive_delete/all.py
--rw-r--r--   0        0        0     1031 2024-04-17 19:58:21.480197 shrillecho-1.1.1/shrillecho/types/artist_types.py
--rw-r--r--   0        0        0      962 2023-11-05 23:56:12.988932 shrillecho-1.1.1/shrillecho/types/base_types.py
--rw-r--r--   0        0        0      778 2024-01-07 02:24:43.414159 shrillecho-1.1.1/shrillecho/types/component_types.py
--rw-r--r--   0        0        0     2009 2024-03-14 01:17:47.656638 shrillecho-1.1.1/shrillecho/types/playlist_types.py
--rw-r--r--   0        0        0     3586 2024-01-12 21:16:04.765172 shrillecho-1.1.1/shrillecho/types/soundcloud_types.py
--rw-r--r--   0        0        0     4410 2024-04-27 21:53:11.373531 shrillecho-1.1.1/shrillecho/types/track_types.py
--rw-r--r--   0        0        0      756 2024-01-12 21:44:55.909131 shrillecho-1.1.1/shrillecho/types/user_types.py
--rw-r--r--   0        0        0       20 2023-09-23 15:03:19.005437 shrillecho-1.1.1/shrillecho/user/__init__.py
--rw-r--r--   0        0        0      169 2024-03-20 18:56:34.599945 shrillecho-1.1.1/shrillecho/user/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2383 2024-04-05 21:59:11.376769 shrillecho-1.1.1/shrillecho/user/__pycache__/user.cpython-312.pyc
--rw-r--r--   0        0        0     1374 2024-04-05 21:57:12.175049 shrillecho-1.1.1/shrillecho/user/user.py
--rw-r--r--   0        0        0       32 2023-09-23 15:03:19.009896 shrillecho-1.1.1/shrillecho/utility/__init__.py
--rw-r--r--   0        0        0      199 2023-09-23 15:05:30.663260 shrillecho-1.1.1/shrillecho/utility/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      184 2024-03-09 15:04:18.655207 shrillecho-1.1.1/shrillecho/utility/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     8287 2024-03-11 01:30:11.865570 shrillecho-1.1.1/shrillecho/utility/__pycache__/async_spotify.cpython-311.pyc
--rw-r--r--   0        0        0     7428 2024-03-14 02:20:08.969425 shrillecho-1.1.1/shrillecho/utility/__pycache__/async_spotify.cpython-312.pyc
--rw-r--r--   0        0        0     6573 2024-04-27 23:25:08.256052 shrillecho-1.1.1/shrillecho/utility/__pycache__/cache.cpython-312.pyc
--rw-r--r--   0        0        0     3087 2024-03-13 01:50:28.638381 shrillecho-1.1.1/shrillecho/utility/__pycache__/database.cpython-312.pyc
--rw-r--r--   0        0        0      780 2024-03-09 21:26:52.160307 shrillecho-1.1.1/shrillecho/utility/__pycache__/general_utility.cpython-311.pyc
--rw-r--r--   0        0        0     2815 2024-03-25 22:08:35.635006 shrillecho-1.1.1/shrillecho/utility/__pycache__/general_utility.cpython-312.pyc
--rw-r--r--   0        0        0    14623 2024-03-11 01:30:11.500906 shrillecho-1.1.1/shrillecho/utility/__pycache__/misc_functions_sort.cpython-311.pyc
--rw-r--r--   0        0        0    13308 2024-03-11 01:30:28.931611 shrillecho-1.1.1/shrillecho/utility/__pycache__/misc_functions_sort.cpython-312.pyc
--rw-r--r--   0        0        0     1386 2024-02-16 01:22:08.428409 shrillecho-1.1.1/shrillecho/utility/__pycache__/mongo.cpython-311.pyc
--rw-r--r--   0        0        0     1217 2024-03-09 15:04:20.128181 shrillecho-1.1.1/shrillecho/utility/__pycache__/mongo.cpython-312.pyc
--rw-r--r--   0        0        0     1650 2024-04-09 21:02:35.293918 shrillecho-1.1.1/shrillecho/utility/__pycache__/neo4j.cpython-312.pyc
--rw-r--r--   0        0        0     1471 2024-03-13 02:26:41.144982 shrillecho-1.1.1/shrillecho/utility/__pycache__/old_cache.cpython-312.pyc
--rw-r--r--   0        0        0     1298 2024-03-11 22:58:59.263675 shrillecho-1.1.1/shrillecho/utility/__pycache__/parsers.cpython-312.pyc
--rw-r--r--   0        0        0    23150 2023-11-12 23:14:00.569468 shrillecho-1.1.1/shrillecho/utility/__pycache__/sc_to_spot.cpython-311.pyc
--rw-r--r--   0        0        0    21256 2023-11-17 00:36:52.587124 shrillecho-1.1.1/shrillecho/utility/__pycache__/sc_to_spot_core.cpython-311.pyc
--rw-r--r--   0        0        0    23316 2023-11-13 22:16:16.303604 shrillecho-1.1.1/shrillecho/utility/__pycache__/sc_to_spot_new.cpython-311.pyc
--rw-r--r--   0        0        0    21113 2024-03-05 21:41:22.471298 shrillecho-1.1.1/shrillecho/utility/__pycache__/soundcloud_converter.cpython-311.pyc
--rw-r--r--   0        0        0    18602 2024-03-14 03:15:29.645819 shrillecho-1.1.1/shrillecho/utility/__pycache__/soundcloud_converter.cpython-312.pyc
--rw-r--r--   0        0        0      178 2024-02-17 22:31:33.962371 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      166 2024-03-09 22:11:54.464156 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7449 2024-03-14 18:38:34.871820 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/async_spotify.cpython-312.pyc
--rw-r--r--   0        0        0      168 2024-04-09 21:02:39.480019 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/batch_dump.cpython-312.pyc
--rw-r--r--   0        0        0     2563 2024-02-17 22:53:45.596137 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-311.pyc
--rw-r--r--   0        0        0     2239 2024-04-09 21:02:39.484564 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-312.pyc
--rw-r--r--   0        0        0     6325 2024-02-17 22:31:33.964370 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-311.pyc
--rw-r--r--   0        0        0     5837 2024-04-09 21:02:39.496708 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-312.pyc
--rw-r--r--   0        0        0    10837 2024-02-17 22:31:34.179654 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-311.pyc
--rw-r--r--   0        0        0     9559 2024-03-11 22:58:59.061429 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-312.pyc
--rw-r--r--   0        0        0     1492 2024-03-14 18:38:34.891285 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/old_cache.cpython-312.pyc
--rw-r--r--   0        0        0     1319 2024-04-09 21:02:39.548705 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/parsers.cpython-312.pyc
--rw-r--r--   0        0        0     4145 2024-02-17 22:53:45.598135 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-311.pyc
--rw-r--r--   0        0        0     3752 2024-04-09 21:02:39.498227 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-312.pyc
--rw-r--r--   0        0        0     7036 2024-02-17 22:31:34.272143 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-311.pyc
--rw-r--r--   0        0        0     6309 2024-03-09 22:11:55.082764 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-312.pyc
--rw-r--r--   0        0        0     5429 2024-02-17 22:31:34.177147 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-311.pyc
--rw-r--r--   0        0        0     5185 2024-04-01 21:30:38.435593 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-312.pyc
--rw-r--r--   0        0        0     5236 2024-03-14 02:20:06.773370 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/async_spotify.py
--rw-r--r--   0        0        0    11306 2024-03-23 00:03:32.882594 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/batch_dump.py
--rw-r--r--   0        0        0      949 2024-01-07 02:19:15.222777 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/cache.py
--rw-r--r--   0        0        0     3492 2024-03-11 22:16:21.293179 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/discovery.py
--rw-r--r--   0        0        0     8352 2024-03-11 22:16:31.726296 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/general.py
--rw-r--r--   0        0        0      928 2024-03-13 02:07:04.021894 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/old_cache.py
--rw-r--r--   0        0        0      773 2024-03-11 21:41:34.182076 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/parsers.py
--rw-r--r--   0        0        0     2659 2024-03-11 22:16:23.348559 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/playlist.py
--rw-r--r--   0        0        0     3613 2024-01-07 02:19:15.149506 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/scraper.py
--rw-r--r--   0        0        0     4322 2024-04-01 21:30:24.666771 shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/spotify_client.py
--rw-r--r--   0        0        0     4063 2024-04-27 23:19:42.172878 shrillecho-1.1.1/shrillecho/utility/cache.py
--rw-r--r--   0        0        0     2055 2024-03-25 21:52:17.491416 shrillecho-1.1.1/shrillecho/utility/general_utility.py
--rw-r--r--   0        0        0     1163 2024-04-01 18:53:56.991612 shrillecho-1.1.1/shrillecho/utility/neo4j.py
--rw-r--r--   0        0        0    11617 2024-03-11 22:16:15.022138 shrillecho-1.1.1/shrillecho/utility/soundcloud_converter.py
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 shrillecho-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1165 2024-05-06 14:29:25.611488 shrillecho-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-09-23 15:03:19.005437 shrillecho-1.1.2/shrillecho/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:55:44.836628 shrillecho-1.1.2/shrillecho/album/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-17 21:40:51.698889 shrillecho-1.1.2/shrillecho/album/album_controller.py
+-rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.1.2/shrillecho/artist/__init__.py
+-rw-r--r--   0        0        0      160 2023-09-23 15:05:30.663260 shrillecho-1.1.2/shrillecho/artist/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2024-03-14 02:58:16.623582 shrillecho-1.1.2/shrillecho/artist/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    11625 2024-04-17 20:29:10.940781 shrillecho-1.1.2/shrillecho/artist/__pycache__/spotify_artist.cpython-312.pyc
+-rw-r--r--   0        0        0     2748 2024-04-21 22:40:07.469215 shrillecho-1.1.2/shrillecho/artist/artist_controller.py
+-rw-r--r--   0        0        0     1009 2024-04-17 20:01:34.862797 shrillecho-1.1.2/shrillecho/artist/sp_artist.py
+-rw-r--r--   0        0        0     8785 2024-04-17 20:29:10.024946 shrillecho-1.1.2/shrillecho/artist/spotify_artist.py
+-rw-r--r--   0        0        0       29 2023-09-23 15:03:19.005437 shrillecho-1.1.2/shrillecho/auth/__init__.py
+-rw-r--r--   0        0        0      193 2023-09-23 15:05:30.403768 shrillecho-1.1.2/shrillecho/auth/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      178 2024-03-09 15:04:18.657207 shrillecho-1.1.2/shrillecho/auth/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4720 2024-03-12 19:30:51.569168 shrillecho-1.1.2/shrillecho/auth/__pycache__/local_auth.cpython-312.pyc
+-rw-r--r--   0        0        0     5424 2024-03-13 22:52:25.720959 shrillecho-1.1.2/shrillecho/auth/__pycache__/oauth.cpython-311.pyc
+-rw-r--r--   0        0        0    11554 2024-03-17 00:55:57.542250 shrillecho-1.1.2/shrillecho/auth/__pycache__/oauth.cpython-312.pyc
+-rw-r--r--   0        0        0      525 2024-03-12 19:28:02.938593 shrillecho-1.1.2/shrillecho/auth/__pycache__/spotify_auth.cpython-312.pyc
+-rw-r--r--   0        0        0     2816 2024-03-12 19:28:42.468224 shrillecho-1.1.2/shrillecho/auth/local_auth.py
+-rw-r--r--   0        0        0     7720 2024-03-17 00:55:39.759059 shrillecho-1.1.2/shrillecho/auth/oauth.py
+-rw-r--r--   0        0        0      156 2024-03-12 19:27:15.771836 shrillecho-1.1.2/shrillecho/auth/spotify_auth.py
+-rw-r--r--   0        0        0        0 2024-03-11 21:00:35.951586 shrillecho-1.1.2/shrillecho/player/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-09 21:02:32.629853 shrillecho-1.1.2/shrillecho/player/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      904 2024-04-09 21:02:32.631375 shrillecho-1.1.2/shrillecho/player/__pycache__/spotify_player.cpython-312.pyc
+-rw-r--r--   0        0        0      359 2024-03-11 22:18:56.285682 shrillecho-1.1.2/shrillecho/player/spotify_player.py
+-rw-r--r--   0        0        0       24 2023-09-23 15:03:19.005437 shrillecho-1.1.2/shrillecho/playlist/__init__.py
+-rw-r--r--   0        0        0      192 2023-09-23 17:32:16.346106 shrillecho-1.1.2/shrillecho/playlist/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      177 2024-03-09 15:02:13.039686 shrillecho-1.1.2/shrillecho/playlist/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1940 2024-04-20 10:39:20.711449 shrillecho-1.1.2/shrillecho/playlist/__pycache__/playlist_controller.cpython-312.pyc
+-rw-r--r--   0        0        0     4070 2024-01-12 22:36:57.888928 shrillecho-1.1.2/shrillecho/playlist/__pycache__/playlist_engine.cpython-311.pyc
+-rw-r--r--   0        0        0     3763 2024-03-09 15:02:13.041686 shrillecho-1.1.2/shrillecho/playlist/__pycache__/playlist_engine.cpython-312.pyc
+-rw-r--r--   0        0        0     5128 2024-04-21 21:13:00.466645 shrillecho-1.1.2/shrillecho/playlist/__pycache__/spotify_playlist.cpython-312.pyc
+-rw-r--r--   0        0        0     7244 2024-04-20 10:45:03.486766 shrillecho-1.1.2/shrillecho/playlist/__pycache__/virtual_playlist.cpython-312.pyc
+-rw-r--r--   0        0        0     3776 2024-03-11 22:58:55.429565 shrillecho-1.1.2/shrillecho/playlist/archive/__pycache__/playlist_engine.cpython-312.pyc
+-rw-r--r--   0        0        0     2306 2024-03-11 22:16:24.766938 shrillecho-1.1.2/shrillecho/playlist/archive/playlist_engine.py
+-rw-r--r--   0        0        0     1221 2024-04-17 22:20:31.920970 shrillecho-1.1.2/shrillecho/playlist/playlist_controller.py
+-rw-r--r--   0        0        0     4389 2024-04-21 20:26:12.833324 shrillecho-1.1.2/shrillecho/playlist/spotify_playlist.py
+-rw-r--r--   0        0        0     4256 2024-04-20 10:44:19.895473 shrillecho-1.1.2/shrillecho/playlist/virtual_playlist.py
+-rw-r--r--   0        0        0        0 2023-09-23 15:03:19.005437 shrillecho-1.1.2/shrillecho/scraping/__init__.py
+-rw-r--r--   0        0        0      162 2023-09-23 15:05:30.663260 shrillecho-1.1.2/shrillecho/scraping/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      146 2024-03-14 18:38:34.308684 shrillecho-1.1.2/shrillecho/scraping/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3653 2024-04-17 19:53:12.059070 shrillecho-1.1.2/shrillecho/scraping/__pycache__/browser_auth.cpython-312.pyc
+-rw-r--r--   0        0        0     2051 2024-04-17 19:46:10.197061 shrillecho-1.1.2/shrillecho/scraping/browser_auth.py
+-rw-r--r--   0        0        0        0 2024-03-12 18:59:09.355126 shrillecho-1.1.2/shrillecho/spotify/__init__.py
+-rw-r--r--   0        0        0      145 2024-03-12 19:19:14.425028 shrillecho-1.1.2/shrillecho/spotify/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    22970 2024-04-28 00:26:11.161172 shrillecho-1.1.2/shrillecho/spotify/__pycache__/client.cpython-312.pyc
+-rw-r--r--   0        0        0     3480 2024-04-21 21:54:52.990207 shrillecho-1.1.2/shrillecho/spotify/__pycache__/task_scheduler.cpython-312.pyc
+-rw-r--r--   0        0        0    16853 2024-05-06 14:27:50.228980 shrillecho-1.1.2/shrillecho/spotify/client.py
+-rw-r--r--   0        0        0     2489 2024-04-21 21:54:39.662490 shrillecho-1.1.2/shrillecho/spotify/task_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:48:31.986990 shrillecho-1.1.2/shrillecho/track/__init__.py
+-rw-r--r--   0        0        0      143 2024-03-11 22:58:59.259675 shrillecho-1.1.2/shrillecho/track/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7545 2024-04-11 22:51:50.359779 shrillecho-1.1.2/shrillecho/track/__pycache__/spotify_track.cpython-312.pyc
+-rw-r--r--   0        0        0     2379 2024-04-12 23:08:45.923483 shrillecho-1.1.2/shrillecho/track/__pycache__/tracks_wrapper.cpython-312.pyc
+-rw-r--r--   0        0        0     5159 2024-04-11 22:51:22.177465 shrillecho-1.1.2/shrillecho/track/spotify_track.py
+-rw-r--r--   0        0        0        0 2023-10-14 18:10:24.959970 shrillecho-1.1.2/shrillecho/types/__init__.py
+-rw-r--r--   0        0        0      155 2023-10-14 18:10:25.750276 shrillecho-1.1.2/shrillecho/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      143 2024-03-09 15:02:13.064686 shrillecho-1.1.2/shrillecho/types/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4307 2024-03-11 22:58:55.468913 shrillecho-1.1.2/shrillecho/types/__pycache__/album_types.cpython-312.pyc
+-rw-r--r--   0        0        0     5278 2024-01-12 22:34:54.354054 shrillecho-1.1.2/shrillecho/types/__pycache__/albums.cpython-311.pyc
+-rw-r--r--   0        0        0     4292 2024-03-09 15:04:17.730511 shrillecho-1.1.2/shrillecho/types/__pycache__/albums.cpython-312.pyc
+-rw-r--r--   0        0        0     2658 2024-04-17 20:27:50.732389 shrillecho-1.1.2/shrillecho/types/__pycache__/artist_types.cpython-312.pyc
+-rw-r--r--   0        0        0     1908 2024-01-12 22:34:54.356055 shrillecho-1.1.2/shrillecho/types/__pycache__/artists.cpython-311.pyc
+-rw-r--r--   0        0        0     1538 2024-03-09 15:04:17.731520 shrillecho-1.1.2/shrillecho/types/__pycache__/artists.cpython-312.pyc
+-rw-r--r--   0        0        0     3173 2023-11-05 23:56:15.061834 shrillecho-1.1.2/shrillecho/types/__pycache__/base_types.cpython-311.pyc
+-rw-r--r--   0        0        0     2488 2024-03-09 15:02:13.071687 shrillecho-1.1.2/shrillecho/types/__pycache__/base_types.cpython-312.pyc
+-rw-r--r--   0        0        0     1736 2024-03-11 22:58:55.436070 shrillecho-1.1.2/shrillecho/types/__pycache__/component_types.cpython-312.pyc
+-rw-r--r--   0        0        0     2134 2024-01-07 02:24:45.003341 shrillecho-1.1.2/shrillecho/types/__pycache__/components.cpython-311.pyc
+-rw-r--r--   0        0        0     1731 2024-03-09 15:02:13.068686 shrillecho-1.1.2/shrillecho/types/__pycache__/components.cpython-312.pyc
+-rw-r--r--   0        0        0     3496 2024-03-14 02:19:29.826797 shrillecho-1.1.2/shrillecho/types/__pycache__/playlist_types.cpython-312.pyc
+-rw-r--r--   0        0        0     4298 2024-01-12 22:34:54.294325 shrillecho-1.1.2/shrillecho/types/__pycache__/playlists.cpython-311.pyc
+-rw-r--r--   0        0        0     3472 2024-03-09 15:02:13.067686 shrillecho-1.1.2/shrillecho/types/__pycache__/playlists.cpython-312.pyc
+-rw-r--r--   0        0        0     6664 2024-02-24 03:23:54.874109 shrillecho-1.1.2/shrillecho/types/__pycache__/sc.cpython-311.pyc
+-rw-r--r--   0        0        0     5792 2024-03-09 16:03:46.602847 shrillecho-1.1.2/shrillecho/types/__pycache__/sc.cpython-312.pyc
+-rw-r--r--   0        0        0     5806 2024-03-14 03:15:29.847360 shrillecho-1.1.2/shrillecho/types/__pycache__/soundcloud_types.cpython-312.pyc
+-rw-r--r--   0        0        0     7857 2024-04-27 21:55:25.752930 shrillecho-1.1.2/shrillecho/types/__pycache__/track_types.cpython-312.pyc
+-rw-r--r--   0        0        0     7020 2024-03-06 18:45:37.173792 shrillecho-1.1.2/shrillecho/types/__pycache__/tracks.cpython-311.pyc
+-rw-r--r--   0        0        0     5798 2024-03-09 15:04:17.728996 shrillecho-1.1.2/shrillecho/types/__pycache__/tracks.cpython-312.pyc
+-rw-r--r--   0        0        0     1463 2024-03-11 22:58:55.480875 shrillecho-1.1.2/shrillecho/types/__pycache__/user_types.cpython-312.pyc
+-rw-r--r--   0        0        0     1755 2024-01-12 22:34:54.365174 shrillecho-1.1.2/shrillecho/types/__pycache__/users.cpython-311.pyc
+-rw-r--r--   0        0        0     1458 2024-03-09 15:04:17.742095 shrillecho-1.1.2/shrillecho/types/__pycache__/users.cpython-312.pyc
+-rw-r--r--   0        0        0     2602 2024-03-11 22:15:02.628111 shrillecho-1.1.2/shrillecho/types/album_types.py
+-rw-r--r--   0        0        0      158 2024-04-09 21:02:35.162480 shrillecho-1.1.2/shrillecho/types/archive_delete/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      521 2024-04-09 21:02:35.163998 shrillecho-1.1.2/shrillecho/types/archive_delete/__pycache__/all.cpython-312.pyc
+-rw-r--r--   0        0        0     5529 2024-03-11 22:16:14.402147 shrillecho-1.1.2/shrillecho/types/archive_delete/all.py
+-rw-r--r--   0        0        0     1031 2024-04-17 19:58:21.480197 shrillecho-1.1.2/shrillecho/types/artist_types.py
+-rw-r--r--   0        0        0      962 2023-11-05 23:56:12.988932 shrillecho-1.1.2/shrillecho/types/base_types.py
+-rw-r--r--   0        0        0      778 2024-01-07 02:24:43.414159 shrillecho-1.1.2/shrillecho/types/component_types.py
+-rw-r--r--   0        0        0     2009 2024-03-14 01:17:47.656638 shrillecho-1.1.2/shrillecho/types/playlist_types.py
+-rw-r--r--   0        0        0     3586 2024-01-12 21:16:04.765172 shrillecho-1.1.2/shrillecho/types/soundcloud_types.py
+-rw-r--r--   0        0        0     4410 2024-04-27 21:53:11.373531 shrillecho-1.1.2/shrillecho/types/track_types.py
+-rw-r--r--   0        0        0      756 2024-01-12 21:44:55.909131 shrillecho-1.1.2/shrillecho/types/user_types.py
+-rw-r--r--   0        0        0       20 2023-09-23 15:03:19.005437 shrillecho-1.1.2/shrillecho/user/__init__.py
+-rw-r--r--   0        0        0      169 2024-03-20 18:56:34.599945 shrillecho-1.1.2/shrillecho/user/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2383 2024-04-05 21:59:11.376769 shrillecho-1.1.2/shrillecho/user/__pycache__/user.cpython-312.pyc
+-rw-r--r--   0        0        0     1374 2024-04-05 21:57:12.175049 shrillecho-1.1.2/shrillecho/user/user.py
+-rw-r--r--   0        0        0       32 2023-09-23 15:03:19.009896 shrillecho-1.1.2/shrillecho/utility/__init__.py
+-rw-r--r--   0        0        0      199 2023-09-23 15:05:30.663260 shrillecho-1.1.2/shrillecho/utility/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2024-03-09 15:04:18.655207 shrillecho-1.1.2/shrillecho/utility/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     8287 2024-03-11 01:30:11.865570 shrillecho-1.1.2/shrillecho/utility/__pycache__/async_spotify.cpython-311.pyc
+-rw-r--r--   0        0        0     7428 2024-03-14 02:20:08.969425 shrillecho-1.1.2/shrillecho/utility/__pycache__/async_spotify.cpython-312.pyc
+-rw-r--r--   0        0        0     6573 2024-04-27 23:25:08.256052 shrillecho-1.1.2/shrillecho/utility/__pycache__/cache.cpython-312.pyc
+-rw-r--r--   0        0        0     3087 2024-03-13 01:50:28.638381 shrillecho-1.1.2/shrillecho/utility/__pycache__/database.cpython-312.pyc
+-rw-r--r--   0        0        0      780 2024-03-09 21:26:52.160307 shrillecho-1.1.2/shrillecho/utility/__pycache__/general_utility.cpython-311.pyc
+-rw-r--r--   0        0        0     2815 2024-03-25 22:08:35.635006 shrillecho-1.1.2/shrillecho/utility/__pycache__/general_utility.cpython-312.pyc
+-rw-r--r--   0        0        0    14623 2024-03-11 01:30:11.500906 shrillecho-1.1.2/shrillecho/utility/__pycache__/misc_functions_sort.cpython-311.pyc
+-rw-r--r--   0        0        0    13308 2024-03-11 01:30:28.931611 shrillecho-1.1.2/shrillecho/utility/__pycache__/misc_functions_sort.cpython-312.pyc
+-rw-r--r--   0        0        0     1386 2024-02-16 01:22:08.428409 shrillecho-1.1.2/shrillecho/utility/__pycache__/mongo.cpython-311.pyc
+-rw-r--r--   0        0        0     1217 2024-03-09 15:04:20.128181 shrillecho-1.1.2/shrillecho/utility/__pycache__/mongo.cpython-312.pyc
+-rw-r--r--   0        0        0     1650 2024-04-09 21:02:35.293918 shrillecho-1.1.2/shrillecho/utility/__pycache__/neo4j.cpython-312.pyc
+-rw-r--r--   0        0        0     1471 2024-03-13 02:26:41.144982 shrillecho-1.1.2/shrillecho/utility/__pycache__/old_cache.cpython-312.pyc
+-rw-r--r--   0        0        0     1298 2024-03-11 22:58:59.263675 shrillecho-1.1.2/shrillecho/utility/__pycache__/parsers.cpython-312.pyc
+-rw-r--r--   0        0        0    23150 2023-11-12 23:14:00.569468 shrillecho-1.1.2/shrillecho/utility/__pycache__/sc_to_spot.cpython-311.pyc
+-rw-r--r--   0        0        0    21256 2023-11-17 00:36:52.587124 shrillecho-1.1.2/shrillecho/utility/__pycache__/sc_to_spot_core.cpython-311.pyc
+-rw-r--r--   0        0        0    23316 2023-11-13 22:16:16.303604 shrillecho-1.1.2/shrillecho/utility/__pycache__/sc_to_spot_new.cpython-311.pyc
+-rw-r--r--   0        0        0    21113 2024-03-05 21:41:22.471298 shrillecho-1.1.2/shrillecho/utility/__pycache__/soundcloud_converter.cpython-311.pyc
+-rw-r--r--   0        0        0    18602 2024-03-14 03:15:29.645819 shrillecho-1.1.2/shrillecho/utility/__pycache__/soundcloud_converter.cpython-312.pyc
+-rw-r--r--   0        0        0      178 2024-02-17 22:31:33.962371 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      166 2024-03-09 22:11:54.464156 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7449 2024-03-14 18:38:34.871820 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/async_spotify.cpython-312.pyc
+-rw-r--r--   0        0        0      168 2024-04-09 21:02:39.480019 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/batch_dump.cpython-312.pyc
+-rw-r--r--   0        0        0     2563 2024-02-17 22:53:45.596137 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-311.pyc
+-rw-r--r--   0        0        0     2239 2024-04-09 21:02:39.484564 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-312.pyc
+-rw-r--r--   0        0        0     6325 2024-02-17 22:31:33.964370 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-311.pyc
+-rw-r--r--   0        0        0     5837 2024-04-09 21:02:39.496708 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-312.pyc
+-rw-r--r--   0        0        0    10837 2024-02-17 22:31:34.179654 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-311.pyc
+-rw-r--r--   0        0        0     9559 2024-03-11 22:58:59.061429 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-312.pyc
+-rw-r--r--   0        0        0     1492 2024-03-14 18:38:34.891285 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/old_cache.cpython-312.pyc
+-rw-r--r--   0        0        0     1319 2024-04-09 21:02:39.548705 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/parsers.cpython-312.pyc
+-rw-r--r--   0        0        0     4145 2024-02-17 22:53:45.598135 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-311.pyc
+-rw-r--r--   0        0        0     3752 2024-04-09 21:02:39.498227 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-312.pyc
+-rw-r--r--   0        0        0     7036 2024-02-17 22:31:34.272143 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-311.pyc
+-rw-r--r--   0        0        0     6309 2024-03-09 22:11:55.082764 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-312.pyc
+-rw-r--r--   0        0        0     5429 2024-02-17 22:31:34.177147 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-311.pyc
+-rw-r--r--   0        0        0     5185 2024-04-01 21:30:38.435593 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-312.pyc
+-rw-r--r--   0        0        0     5236 2024-03-14 02:20:06.773370 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/async_spotify.py
+-rw-r--r--   0        0        0    11306 2024-03-23 00:03:32.882594 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/batch_dump.py
+-rw-r--r--   0        0        0      949 2024-01-07 02:19:15.222777 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/cache.py
+-rw-r--r--   0        0        0     3492 2024-03-11 22:16:21.293179 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/discovery.py
+-rw-r--r--   0        0        0     8352 2024-03-11 22:16:31.726296 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/general.py
+-rw-r--r--   0        0        0      928 2024-03-13 02:07:04.021894 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/old_cache.py
+-rw-r--r--   0        0        0      773 2024-03-11 21:41:34.182076 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/parsers.py
+-rw-r--r--   0        0        0     2659 2024-03-11 22:16:23.348559 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/playlist.py
+-rw-r--r--   0        0        0     3613 2024-01-07 02:19:15.149506 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/scraper.py
+-rw-r--r--   0        0        0     4322 2024-04-01 21:30:24.666771 shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/spotify_client.py
+-rw-r--r--   0        0        0     4063 2024-04-27 23:19:42.172878 shrillecho-1.1.2/shrillecho/utility/cache.py
+-rw-r--r--   0        0        0     2055 2024-03-25 21:52:17.491416 shrillecho-1.1.2/shrillecho/utility/general_utility.py
+-rw-r--r--   0        0        0     1163 2024-04-01 18:53:56.991612 shrillecho-1.1.2/shrillecho/utility/neo4j.py
+-rw-r--r--   0        0        0    11617 2024-03-11 22:16:15.022138 shrillecho-1.1.2/shrillecho/utility/soundcloud_converter.py
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 shrillecho-1.1.2/PKG-INFO
```

### Comparing `shrillecho-1.1.1/pyproject.toml` & `shrillecho-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shrillecho"
-version = "1.1.1"
+version = "1.1.2"
 description = "Music Tool"
 authors = ["simon balfe <sbmain17@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 spotipy = ">=2.23.0,<2.24.0"
 python-dotenv = ">=1.0.0,<1.1.0"
```

### Comparing `shrillecho-1.1.1/shrillecho/album/album_controller.py` & `shrillecho-1.1.2/shrillecho/album/album_controller.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/artist/__pycache__/spotify_artist.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/artist/__pycache__/spotify_artist.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/artist/artist_controller.py` & `shrillecho-1.1.2/shrillecho/artist/artist_controller.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/artist/sp_artist.py` & `shrillecho-1.1.2/shrillecho/artist/sp_artist.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/artist/spotify_artist.py` & `shrillecho-1.1.2/shrillecho/artist/spotify_artist.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/auth/__pycache__/local_auth.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/auth/__pycache__/local_auth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/auth/__pycache__/oauth.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/auth/__pycache__/oauth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/auth/__pycache__/oauth.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/auth/__pycache__/oauth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/auth/__pycache__/spotify_auth.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/auth/__pycache__/spotify_auth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/auth/local_auth.py` & `shrillecho-1.1.2/shrillecho/auth/local_auth.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/auth/oauth.py` & `shrillecho-1.1.2/shrillecho/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/player/__pycache__/spotify_player.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/player/__pycache__/spotify_player.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/__pycache__/playlist_controller.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/playlist/__pycache__/playlist_controller.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/__pycache__/playlist_engine.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/playlist/__pycache__/playlist_engine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/__pycache__/playlist_engine.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/playlist/__pycache__/playlist_engine.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/__pycache__/spotify_playlist.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/playlist/__pycache__/spotify_playlist.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/__pycache__/virtual_playlist.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/playlist/__pycache__/virtual_playlist.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/archive/__pycache__/playlist_engine.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/playlist/archive/__pycache__/playlist_engine.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/archive/playlist_engine.py` & `shrillecho-1.1.2/shrillecho/playlist/archive/playlist_engine.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/playlist_controller.py` & `shrillecho-1.1.2/shrillecho/playlist/playlist_controller.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/spotify_playlist.py` & `shrillecho-1.1.2/shrillecho/playlist/spotify_playlist.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/playlist/virtual_playlist.py` & `shrillecho-1.1.2/shrillecho/playlist/virtual_playlist.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/scraping/__pycache__/browser_auth.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/scraping/__pycache__/browser_auth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/scraping/browser_auth.py` & `shrillecho-1.1.2/shrillecho/scraping/browser_auth.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/spotify/__pycache__/client.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/spotify/__pycache__/client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/spotify/__pycache__/task_scheduler.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/spotify/__pycache__/task_scheduler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/spotify/client.py` & `shrillecho-1.1.2/shrillecho/spotify/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,23 +168,23 @@
     ############# Shrillecho Implemented Methods #############
 
     @cached(cache_key_prefix="me", class_type=CurrentUserProfile, expiry=3600)
     async def me(self) -> User:
         return await self._get("me", response_type=CurrentUserProfile, req_proxy=False)
     
     async def track(self, track: str) -> Track:
-        return await self._get(f"tracks/{get_id("track", track)}", response_type=Track)
+        return await self._get(f"tracks/{get_id('track', track)}", response_type=Track)
 
     @cached(cache_key_prefix="album", class_type=Album, expiry=3600)
     async def album(self, album: str) -> Track:
-        return await self._get(f"albums/{get_id("album", album)}", response_type=Album)
+        return await self._get(f"albums/{get_id('album', album)}", response_type=Album)
 
     @cached(cache_key_prefix="artist", class_type=Artist, expiry=3600)
     async def artist(self, artist: str) -> Track:
-        return await self._get(f"artists/{get_id("artist", artist)}", response_type=Artist)
+        return await self._get(f"artists/{get_id('artist', artist)}", response_type=Artist)
 
     async def tracks(self, tracks) -> List[Track]:
         tlist = [get_id("track", t) for t in tracks]
         s_tracks: SeveralTracks = await self._get("tracks/?ids=" + ",".join(tlist), response_type=SeveralTracks)
         return s_tracks.tracks
 
     @cached(cache_key_prefix="artist_related", class_type=Artist, expiry=1000)
@@ -197,15 +197,15 @@
         return await self._get("recommendations?limit=50&seed_tracks=5m4Lh4bgiYKSj2MlDcrnxh", response_type=Recc)
     
     async def artists(self, artists: List[str]) -> SeveralArtists:
         artist_ids = [get_id("artist", a) for a in artists]
         return await self._get("artists?ids=" + ",".join(artist_ids), response_type=SeveralArtists)
     
     async def artist_albums_single(self, artist, limit=50, offset=None) -> ArtistAlbums:
-        return await self._get(f"artists/{get_id("artist", artist)}/albums?limit={limit}&offset={offset}", response_type=ArtistAlbums)
+        return await self._get(f"artists/{get_id('artist', artist)}/albums?limit={limit}&offset={offset}", response_type=ArtistAlbums)
         
     async def current_user_followed_artists(self, limit: int = 20, after=None) -> FollowedArtists:
        
         return await self._get(f"me/following?type=artist&limit={limit}&after={after}", response_type=FollowedArtists, req_proxy=False)
        
     async def audio_features(self, track) -> AudioFeatures:
         return await self._get(f"audio-features/{get_id('track', track)}", response_type=AudioFeatures, req_proxy=False)
```

### Comparing `shrillecho-1.1.1/shrillecho/spotify/task_scheduler.py` & `shrillecho-1.1.2/shrillecho/spotify/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/track/__pycache__/spotify_track.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/track/__pycache__/spotify_track.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/track/__pycache__/tracks_wrapper.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/track/__pycache__/tracks_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/track/spotify_track.py` & `shrillecho-1.1.2/shrillecho/track/spotify_track.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/album_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/album_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/albums.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/albums.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/albums.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/albums.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/artist_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/artist_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/artists.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/artists.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/artists.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/artists.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/base_types.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/base_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/base_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/base_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/component_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/component_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/components.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/components.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/components.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/components.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/playlist_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/playlist_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/playlists.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/playlists.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/playlists.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/playlists.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/sc.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/sc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/sc.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/sc.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/soundcloud_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/soundcloud_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/track_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/track_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/tracks.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/tracks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/tracks.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/tracks.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/user_types.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/user_types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/users.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/users.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/__pycache__/users.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/__pycache__/users.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/album_types.py` & `shrillecho-1.1.2/shrillecho/types/album_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/archive_delete/__pycache__/all.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/types/archive_delete/__pycache__/all.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/archive_delete/all.py` & `shrillecho-1.1.2/shrillecho/types/archive_delete/all.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/artist_types.py` & `shrillecho-1.1.2/shrillecho/types/artist_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/base_types.py` & `shrillecho-1.1.2/shrillecho/types/base_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/component_types.py` & `shrillecho-1.1.2/shrillecho/types/component_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/playlist_types.py` & `shrillecho-1.1.2/shrillecho/types/playlist_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/soundcloud_types.py` & `shrillecho-1.1.2/shrillecho/types/soundcloud_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/track_types.py` & `shrillecho-1.1.2/shrillecho/types/track_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/types/user_types.py` & `shrillecho-1.1.2/shrillecho/types/user_types.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/user/__pycache__/user.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/user/__pycache__/user.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/user/user.py` & `shrillecho-1.1.2/shrillecho/user/user.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/async_spotify.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/async_spotify.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/async_spotify.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/async_spotify.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/cache.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/cache.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/database.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/database.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/general_utility.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/general_utility.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/general_utility.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/general_utility.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/misc_functions_sort.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/misc_functions_sort.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/misc_functions_sort.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/misc_functions_sort.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/mongo.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/mongo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/mongo.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/mongo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/neo4j.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/neo4j.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/old_cache.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/old_cache.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/parsers.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/parsers.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/sc_to_spot.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/sc_to_spot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/sc_to_spot_core.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/sc_to_spot_core.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/sc_to_spot_new.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/sc_to_spot_new.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/soundcloud_converter.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/soundcloud_converter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/__pycache__/soundcloud_converter.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/__pycache__/soundcloud_converter.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/async_spotify.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/async_spotify.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/cache.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/discovery.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/general.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/old_cache.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/old_cache.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/parsers.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/parsers.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/playlist.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/scraper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-311.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-312.pyc` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/__pycache__/spotify_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/async_spotify.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/async_spotify.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/batch_dump.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/batch_dump.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/cache.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/cache.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/discovery.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/discovery.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/general.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/general.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/old_cache.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/old_cache.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/parsers.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/parsers.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/playlist.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/playlist.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/scraper.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/scraper.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/archive_maybe_delete/spotify_client.py` & `shrillecho-1.1.2/shrillecho/utility/archive_maybe_delete/spotify_client.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/cache.py` & `shrillecho-1.1.2/shrillecho/utility/cache.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/general_utility.py` & `shrillecho-1.1.2/shrillecho/utility/general_utility.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/neo4j.py` & `shrillecho-1.1.2/shrillecho/utility/neo4j.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/shrillecho/utility/soundcloud_converter.py` & `shrillecho-1.1.2/shrillecho/utility/soundcloud_converter.py`

 * *Files identical despite different names*

### Comparing `shrillecho-1.1.1/PKG-INFO` & `shrillecho-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrillecho
-Version: 1.1.1
+Version: 1.1.2
 Summary: Music Tool
 Author: simon balfe
 Author-email: sbmain17@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

