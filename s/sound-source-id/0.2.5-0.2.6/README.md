# Comparing `tmp/sound_source_id-0.2.5.tar.gz` & `tmp/sound_source_id-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound_source_id-0.2.5.tar", last modified: Sun May  5 06:55:16 2024, max compression
+gzip compressed data, was "sound_source_id-0.2.6.tar", last modified: Mon May  6 08:21:16 2024, max compression
```

## Comparing `sound_source_id-0.2.5.tar` & `sound_source_id-0.2.6.tar`

### file list

```diff
@@ -1,164 +1,185 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:16.670008 sound_source_id-0.2.5/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1054 2024-02-05 09:35:07.000000 sound_source_id-0.2.5/.readthedocs.yaml
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.2.5/COPYING.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.2.5/MANIFEST.in
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41752 2024-05-05 06:55:16.669008 sound_source_id-0.2.5/PKG-INFO
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.2.5/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.558658 sound_source_id-0.2.5/icons/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.2.5/icons/audio-headphones.svgz
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 sound_source_id-0.2.5/icons/exit.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.2.5/icons/help-about.svgz
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.2.5/icons/help-contents.svgz
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.2.5/icons/help-contextual.svgz
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.2.5/icons/point-left.svg
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.2.5/icons/point-right.ico
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.2.5/icons/point-right.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.2.5/icons/preferences-other.svgz
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.585663 sound_source_id-0.2.5/make_noises/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.2.5/make_noises/make_pink_noises.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.2.5/make_noises/sndlib.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.759692 sound_source_id-0.2.5/prep-release/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-05 06:54:31.000000 sound_source_id-0.2.5/prep-release/minor_minor_number.txt
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.2.5/prep-release/mkupdate_pyqt5.sh
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2023-06-12 14:48:08.000000 sound_source_id-0.2.5/prep-release/mkupdate_pyqt6.sh
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      184 2023-06-08 21:48:18.000000 sound_source_id-0.2.5/prep-release/pypi_build.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3821 2024-05-02 15:25:43.000000 sound_source_id-0.2.5/prep-release/release.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      478 2023-06-12 14:47:06.000000 sound_source_id-0.2.5/prep-release/sound_source_id.pro
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    19143 2024-05-03 07:10:38.000000 sound_source_id-0.2.5/prep-release/sound_source_id_el.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-05 06:55:01.000000 sound_source_id-0.2.5/prep-release/sound_source_id_en_GB.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    19143 2024-05-03 07:10:38.000000 sound_source_id-0.2.5/prep-release/sound_source_id_en_US.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-05 06:55:01.000000 sound_source_id-0.2.5/prep-release/sound_source_id_es.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    21950 2024-05-05 06:55:01.000000 sound_source_id-0.2.5/prep-release/sound_source_id_fr.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    21015 2024-05-05 06:55:01.000000 sound_source_id-0.2.5/prep-release/sound_source_id_it.ts
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.2.5/prep-release/switch_pyqt5.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.2.5/prep-release/switch_pyqt6.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      217 2023-06-08 21:49:59.000000 sound_source_id-0.2.5/prep-release/win_installer_readme.md
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 10:17:57.000000 sound_source_id-0.2.5/prep-release/win_launch_iss_compiler.bat
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-07 17:49:12.000000 sound_source_id-0.2.5/prep-release/win_launch_iss_compiler.sh
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4077 2024-05-05 06:54:31.000000 sound_source_id-0.2.5/prep-release/win_sound_source_id.iss
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      773 2023-06-12 15:13:58.000000 sound_source_id-0.2.5/prep-release/winbuild.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1364 2024-05-05 06:54:31.000000 sound_source_id-0.2.5/pyproject.toml
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.2.5/resources.qrc
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-05-05 06:55:16.670008 sound_source_id-0.2.5/setup.cfg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1956 2024-05-05 06:54:31.000000 sound_source_id-0.2.5/setup_cx.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.765693 sound_source_id-0.2.5/sound_source_id/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.2.5/sound_source_id/__init__.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)    65651 2024-05-02 19:48:18.000000 sound_source_id-0.2.5/sound_source_id/__main__.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2024-05-05 06:54:31.000000 sound_source_id-0.2.5/sound_source_id/_version_info.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.2.5/sound_source_id/audio_manager.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    19849 2023-06-11 08:20:40.000000 sound_source_id-0.2.5/sound_source_id/dialog_edit_preferences.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15831 2023-06-11 08:22:26.000000 sound_source_id-0.2.5/sound_source_id/dialog_edit_transducers.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.805699 sound_source_id-0.2.5/sound_source_id/doc/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.841705 sound_source_id-0.2.5/sound_source_id/doc/Figures/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.5/sound_source_id/doc/Figures/edit_transducers.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.5/sound_source_id/doc/Figures/sound_source_id_screenshot.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.5/sound_source_id/doc/Figures/stim_file.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.2.5/sound_source_id/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.443639 sound_source_id-0.2.5/sound_source_id/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.844706 sound_source_id-0.2.5/sound_source_id/doc/_build/html/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.907716 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/edit_transducers.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/stim_file.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:14.991730 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/calibration.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/index.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/installation.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/intro.rst.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:15.378794 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/basic.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/doctools.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/documentation_options.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/file.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/jquery.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/language_data.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/minus.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/plus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/pygments.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/searchtools.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/underscore.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7861 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/calibration.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    11522 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/experiment_setup.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3976 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/genindex.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6000 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/index.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7384 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/installation.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6034 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/intro.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      492 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/objects.inv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4375 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5375 2024-05-05 06:55:04.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/html/searchindex.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:15.406799 sound_source_id-0.2.5/sound_source_id/doc/_build/latex/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   223352 2024-05-05 06:55:06.000000 sound_source_id-0.2.5/sound_source_id/doc/_build/latex/sound_source_id.pdf
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.5/sound_source_id/doc/calibration.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2024-05-05 06:54:31.000000 sound_source_id-0.2.5/sound_source_id/doc/conf.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-11 14:03:05.000000 sound_source_id-0.2.5/sound_source_id/doc/experiment_setup.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.5/sound_source_id/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.5/sound_source_id/doc/installation.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.5/sound_source_id/doc/intro.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.2.5/sound_source_id/doc/make.bat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.2.5/sound_source_id/doc/mkdoc.sh
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:32:26.000000 sound_source_id-0.2.5/sound_source_id/doc/requirements.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9341 2024-04-25 10:53:08.000000 sound_source_id-0.2.5/sound_source_id/global_parameters.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:15.698847 sound_source_id-0.2.5/sound_source_id/prm_files/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:16.643004 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise1.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise10.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise11.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise12.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise13.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise14.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise15.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise16.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise17.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise18.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise19.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise2.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise20.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise21.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise22.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise23.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise24.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise25.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise26.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise27.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise28.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise29.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise3.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise30.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise4.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise5.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise6.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise7.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise8.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise9.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      389 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      198 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_2_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      624 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_circle_36_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      421 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      326 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_2_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      356 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_4_front_back.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      427 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_circle_12_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      751 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      646 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1257 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/stim_list.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      459 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_2_speak.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      759 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_4_front_back.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      710 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_8_az_2_elev.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1521 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_circle.csv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      541 2023-06-19 10:37:35.000000 sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_circle_12_tgs.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2024-05-05 06:54:26.000000 sound_source_id-0.2.5/sound_source_id/pyqtver.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)  2972123 2024-05-05 06:55:03.000000 sound_source_id-0.2.5/sound_source_id/qrc_resources.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   175964 2023-05-04 21:44:23.000000 sound_source_id-0.2.5/sound_source_id/sndlib.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      991 2023-06-11 08:24:39.000000 sound_source_id-0.2.5/sound_source_id/utils.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.2.5/sound_source_id/wavpy.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.2.5/sound_source_id/wavpy_sndf.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-05 06:55:16.669008 sound_source_id-0.2.5/sound_source_id.egg-info/
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41752 2024-05-05 06:55:14.000000 sound_source_id-0.2.5/sound_source_id.egg-info/PKG-INFO
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6086 2024-05-05 06:55:14.000000 sound_source_id-0.2.5/sound_source_id.egg-info/SOURCES.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-05 06:55:14.000000 sound_source_id-0.2.5/sound_source_id.egg-info/dependency_links.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2024-05-05 06:55:14.000000 sound_source_id-0.2.5/sound_source_id.egg-info/entry_points.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      127 2024-05-05 06:55:14.000000 sound_source_id-0.2.5/sound_source_id.egg-info/requires.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2024-05-05 06:55:14.000000 sound_source_id-0.2.5/sound_source_id.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:16.098623 sound_source_id-0.2.6/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1054 2024-02-05 09:35:07.000000 sound_source_id-0.2.6/.readthedocs.yaml
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.2.6/COPYING.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      571 2024-05-06 07:52:48.000000 sound_source_id-0.2.6/MANIFEST.in
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41752 2024-05-06 08:21:16.097623 sound_source_id-0.2.6/PKG-INFO
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.2.6/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:13.878257 sound_source_id-0.2.6/icons/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.2.6/icons/audio-headphones.svgz
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 sound_source_id-0.2.6/icons/exit.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.2.6/icons/help-about.svgz
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.2.6/icons/help-contents.svgz
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.2.6/icons/help-contextual.svgz
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.2.6/icons/point-left.svg
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.2.6/icons/point-right.ico
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.2.6/icons/point-right.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.2.6/icons/preferences-other.svgz
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:13.879257 sound_source_id-0.2.6/make_noises/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.2.6/make_noises/make_pink_noises.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.2.6/make_noises/sndlib.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.247318 sound_source_id-0.2.6/prep-release/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-06 08:20:33.000000 sound_source_id-0.2.6/prep-release/minor_minor_number.txt
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.2.6/prep-release/mkupdate_pyqt5.sh
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2023-06-12 14:48:08.000000 sound_source_id-0.2.6/prep-release/mkupdate_pyqt6.sh
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      184 2023-06-08 21:48:18.000000 sound_source_id-0.2.6/prep-release/pypi_build.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3821 2024-05-02 15:25:43.000000 sound_source_id-0.2.6/prep-release/release.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      478 2023-06-12 14:47:06.000000 sound_source_id-0.2.6/prep-release/sound_source_id.pro
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    19143 2024-05-03 07:10:38.000000 sound_source_id-0.2.6/prep-release/sound_source_id_el.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-06 08:20:58.000000 sound_source_id-0.2.6/prep-release/sound_source_id_en_GB.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    19143 2024-05-03 07:10:38.000000 sound_source_id-0.2.6/prep-release/sound_source_id_en_US.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-06 08:20:58.000000 sound_source_id-0.2.6/prep-release/sound_source_id_es.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    21950 2024-05-06 08:20:58.000000 sound_source_id-0.2.6/prep-release/sound_source_id_fr.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    21015 2024-05-06 08:20:58.000000 sound_source_id-0.2.6/prep-release/sound_source_id_it.ts
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.2.6/prep-release/switch_pyqt5.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.2.6/prep-release/switch_pyqt6.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      217 2023-06-08 21:49:59.000000 sound_source_id-0.2.6/prep-release/win_installer_readme.md
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 10:17:57.000000 sound_source_id-0.2.6/prep-release/win_launch_iss_compiler.bat
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-07 17:49:12.000000 sound_source_id-0.2.6/prep-release/win_launch_iss_compiler.sh
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4077 2024-05-06 08:20:33.000000 sound_source_id-0.2.6/prep-release/win_sound_source_id.iss
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      773 2023-06-12 15:13:58.000000 sound_source_id-0.2.6/prep-release/winbuild.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1364 2024-05-06 08:20:33.000000 sound_source_id-0.2.6/pyproject.toml
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.2.6/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-05-06 08:21:16.098623 sound_source_id-0.2.6/setup.cfg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1956 2024-05-06 08:20:33.000000 sound_source_id-0.2.6/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.274322 sound_source_id-0.2.6/sound_source_id/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.2.6/sound_source_id/__init__.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    65651 2024-05-02 19:48:18.000000 sound_source_id-0.2.6/sound_source_id/__main__.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2024-05-06 08:20:33.000000 sound_source_id-0.2.6/sound_source_id/_version_info.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.2.6/sound_source_id/audio_manager.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    19849 2023-06-11 08:20:40.000000 sound_source_id-0.2.6/sound_source_id/dialog_edit_preferences.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15831 2023-06-11 08:22:26.000000 sound_source_id-0.2.6/sound_source_id/dialog_edit_transducers.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.343333 sound_source_id-0.2.6/sound_source_id/doc/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.695392 sound_source_id-0.2.6/sound_source_id/doc/Figures/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.6/sound_source_id/doc/Figures/edit_transducers.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.6/sound_source_id/doc/Figures/sound_source_id_screenshot.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.6/sound_source_id/doc/Figures/stim_file.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.2.6/sound_source_id/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:13.141135 sound_source_id-0.2.6/sound_source_id/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.743399 sound_source_id-0.2.6/sound_source_id/doc/_build/html/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.767403 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/edit_transducers.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/stim_file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:14.981439 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2302 2024-05-06 08:16:44.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/calibration.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2646 2024-05-06 07:57:19.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/index.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/installation.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      438 2024-05-06 07:54:26.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/intro.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:15.084456 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/basic.css
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:15.147466 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/css/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/css/badge_only.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/css/theme.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/doctools.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/documentation_options.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:15.586539 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   683116 2014-02-27 03:42:28.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-Bold.ttf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   208512 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-Bold.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   714640 2014-02-27 03:42:28.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-BoldItalic.ttf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   221928 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-BoldItalic.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   693228 2014-02-27 03:42:28.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-Italic.ttf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   219592 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-Italic.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   661592 2014-02-27 03:42:28.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-Regular.ttf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   203936 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/Lato-Regular.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    52828 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/RobotoSlab-Bold.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    52532 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/RobotoSlab-Regular.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   165742 2016-10-24 15:52:54.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.eot
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   444379 2016-10-24 15:52:54.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.svg
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   165548 2016-10-24 15:52:54.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.ttf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    98024 2016-10-24 15:52:54.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.woff
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    77160 2016-10-24 15:52:54.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.woff2
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/jquery.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:15.605542 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/js/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/js/theme.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/language_data.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/minus.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/plus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/pygments.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/searchtools.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/underscore.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7961 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/calibration.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11520 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/experiment_setup.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3976 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/genindex.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6000 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/index.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7384 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/installation.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6036 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/intro.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      492 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/objects.inv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4375 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5486 2024-05-06 08:21:00.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/html/searchindex.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:15.605542 sound_source_id-0.2.6/sound_source_id/doc/_build/latex/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   246788 2024-05-06 08:21:02.000000 sound_source_id-0.2.6/sound_source_id/doc/_build/latex/sound_source_id.pdf
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2302 2024-05-06 08:16:44.000000 sound_source_id-0.2.6/sound_source_id/doc/calibration.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2024-05-06 08:20:33.000000 sound_source_id-0.2.6/sound_source_id/doc/conf.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2646 2024-05-06 07:57:19.000000 sound_source_id-0.2.6/sound_source_id/doc/experiment_setup.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.6/sound_source_id/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.6/sound_source_id/doc/installation.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      438 2024-05-06 07:54:26.000000 sound_source_id-0.2.6/sound_source_id/doc/intro.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.2.6/sound_source_id/doc/make.bat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.2.6/sound_source_id/doc/mkdoc.sh
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:32:26.000000 sound_source_id-0.2.6/sound_source_id/doc/requirements.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9341 2024-04-25 10:53:08.000000 sound_source_id-0.2.6/sound_source_id/global_parameters.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:15.742565 sound_source_id-0.2.6/sound_source_id/prm_files/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:16.095623 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise1.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise10.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise11.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise12.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise13.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise14.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise15.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise16.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise17.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise18.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise19.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise2.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise20.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise21.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise22.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise23.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise24.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise25.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise26.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise27.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise28.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise29.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise3.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise30.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise4.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise5.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise6.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise7.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise8.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise9.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      389 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      198 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_2_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      624 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_circle_36_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      421 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      326 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_2_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      356 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_4_front_back.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      427 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_circle_12_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      751 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      646 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1257 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/stim_list.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      459 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_2_speak.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      759 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_4_front_back.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      710 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_8_az_2_elev.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1521 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_circle.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      541 2023-06-19 10:37:35.000000 sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_circle_12_tgs.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2024-05-06 08:20:32.000000 sound_source_id-0.2.6/sound_source_id/pyqtver.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)  2972123 2024-05-06 08:20:58.000000 sound_source_id-0.2.6/sound_source_id/qrc_resources.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   175964 2023-05-04 21:44:23.000000 sound_source_id-0.2.6/sound_source_id/sndlib.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      991 2023-06-11 08:24:39.000000 sound_source_id-0.2.6/sound_source_id/utils.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.2.6/sound_source_id/wavpy.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.2.6/sound_source_id/wavpy_sndf.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-06 08:21:16.097623 sound_source_id-0.2.6/sound_source_id.egg-info/
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41752 2024-05-06 08:21:13.000000 sound_source_id-0.2.6/sound_source_id.egg-info/PKG-INFO
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7253 2024-05-06 08:21:13.000000 sound_source_id-0.2.6/sound_source_id.egg-info/SOURCES.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-06 08:21:13.000000 sound_source_id-0.2.6/sound_source_id.egg-info/dependency_links.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2024-05-06 08:21:13.000000 sound_source_id-0.2.6/sound_source_id.egg-info/entry_points.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      127 2024-05-06 08:21:13.000000 sound_source_id-0.2.6/sound_source_id.egg-info/requires.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2024-05-06 08:21:13.000000 sound_source_id-0.2.6/sound_source_id.egg-info/top_level.txt
```

### Comparing `sound_source_id-0.2.5/.readthedocs.yaml` & `sound_source_id-0.2.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/COPYING.txt` & `sound_source_id-0.2.6/COPYING.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/PKG-INFO` & `sound_source_id-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sound_source_id-0.2.5/icons/audio-headphones.svgz` & `sound_source_id-0.2.6/icons/audio-headphones.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/exit.svg` & `sound_source_id-0.2.6/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/help-about.svgz` & `sound_source_id-0.2.6/icons/help-about.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/help-contents.svgz` & `sound_source_id-0.2.6/icons/help-contents.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/help-contextual.svgz` & `sound_source_id-0.2.6/icons/help-contextual.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/point-left.svg` & `sound_source_id-0.2.6/icons/point-left.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/point-right.ico` & `sound_source_id-0.2.6/icons/point-right.ico`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/point-right.svg` & `sound_source_id-0.2.6/icons/point-right.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/icons/preferences-other.svgz` & `sound_source_id-0.2.6/icons/preferences-other.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/make_noises/make_pink_noises.py` & `sound_source_id-0.2.6/make_noises/make_pink_noises.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/make_noises/sndlib.py` & `sound_source_id-0.2.6/make_noises/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/mkupdate_pyqt6.sh` & `sound_source_id-0.2.6/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/release.py` & `sound_source_id-0.2.6/prep-release/release.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/sound_source_id_el.ts` & `sound_source_id-0.2.6/prep-release/sound_source_id_el.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/sound_source_id_en_GB.ts` & `sound_source_id-0.2.6/prep-release/sound_source_id_en_GB.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.2.6/prep-release/sound_source_id_en_US.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/sound_source_id_es.ts` & `sound_source_id-0.2.6/prep-release/sound_source_id_es.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/sound_source_id_fr.ts` & `sound_source_id-0.2.6/prep-release/sound_source_id_fr.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/sound_source_id_it.ts` & `sound_source_id-0.2.6/prep-release/sound_source_id_it.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/switch_pyqt5.py` & `sound_source_id-0.2.6/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/switch_pyqt6.py` & `sound_source_id-0.2.6/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/win_launch_iss_compiler.sh` & `sound_source_id-0.2.6/prep-release/win_launch_iss_compiler.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/prep-release/win_sound_source_id.iss` & `sound_source_id-0.2.6/prep-release/win_sound_source_id.iss`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "sound_source_id"
-#define MyAppVersion "0.2.5"
+#define MyAppVersion "0.2.6"
 #define MyAppPublisher "Samuele Carcagno"
 #define MyAppURL "https://samcarcagno.altervista.org/sound_source_id/sound_source_id.html"
 #define MyAppExeName "sound_source_id.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application. Do not use the same AppId value in installers for other applications.
 ; (To generate a new GUID, click Tools | Generate GUID inside the IDE.)
```

### Comparing `sound_source_id-0.2.5/prep-release/winbuild.py` & `sound_source_id-0.2.6/prep-release/winbuild.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/pyproject.toml` & `sound_source_id-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sound_source_id"
-    version="0.2.5"
+    version="0.2.6"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python application for running sound localization experiments"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `sound_source_id-0.2.5/resources.qrc` & `sound_source_id-0.2.6/resources.qrc`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/setup_cx.py` & `sound_source_id-0.2.6/setup_cx.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,11 +41,11 @@
     Executable('sound_source_id\\__main__.py',
                base=base,
                target_name = 'sound_source_id',
                icon='icons/point-right.ico')
 ]
 
 setup(name='sound_source_id',
-    version="0.2.5",
+    version="0.2.6",
       description = '',
       options = {'build_exe': build_options},
       executables = executables)
```

### Comparing `sound_source_id-0.2.5/sound_source_id/__main__.py` & `sound_source_id-0.2.6/sound_source_id/__main__.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/audio_manager.py` & `sound_source_id-0.2.6/sound_source_id/audio_manager.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/dialog_edit_preferences.py` & `sound_source_id-0.2.6/sound_source_id/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/dialog_edit_transducers.py` & `sound_source_id-0.2.6/sound_source_id/dialog_edit_transducers.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/Figures/edit_transducers.png` & `sound_source_id-0.2.6/sound_source_id/doc/Figures/edit_transducers.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/Figures/sound_source_id_screenshot.png` & `sound_source_id-0.2.6/sound_source_id/doc/Figures/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/Figures/stim_file.png` & `sound_source_id-0.2.6/sound_source_id/doc/Figures/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/Makefile` & `sound_source_id-0.2.6/sound_source_id/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/edit_transducers.png` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/edit_transducers.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_images/stim_file.png` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_images/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/calibration.rst.txt` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/calibration.rst.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 
 .. figure:: Figures/edit_transducers.png
    :scale: 75%
    :alt: Edit transducers dialog
 
    Edit transducers dialog
 
-Most of the fields should be pretty much self-explanatory. Using this
-dialog you can add headphones/speakers models to the transducers database. In `sound_source_id` levels are referenced to the level that would be output by a full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the ``Max Level`` field you should enter the level in dB SPL that is output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with a SPL meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.
+Most of the fields should be pretty much self explanatory. Using this dialog you can add headphones/speakers models to the transducers database. In `sound_source_id` levels are referenced to the level that would be output by a full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the ``Max Level`` field you should enter the level in dB SPL that is output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with an SPL meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.
 
-The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be reasonably loud as to avoid signal-to-noise ratio issues, but not too loud as to cause distortions or damage your hearing in the measurement process. Once I've found a reasonable level, by trial and error, I measure the actual level with an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the experiment and note it down.
+The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be reasonably high as to avoid signal-to-noise ratio issues, but not so high as to cause distortions or damage your hearing in the measurement process. Once I've found a reasonable level, by trial and error, I measure the actual level with an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the experiment, and note it down.
 
-We can measure the RMS level of the WAV file with the noise used for calibration, let's call it :math:`rmsnoise`. A full amplitude sinusoid has a root-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the level of a sinusoid at max amplitude and our calibration noise will be equal to:
+We can measure the root-mean-square (RMS) level of the WAV file with the noise used for calibration, let's call it :math:`RMS_{noise}`. A full amplitude sinusoid has an RMS amplitude of :math:`1/\sqrt{2} = 0.707`. The difference in dB between the level of a sinusoid at max amplitude and our calibration noise will be equal to:
 
 .. math::
 
-   dbdiff = 20*log10((1/sqrt(2))/rmsnoise)
+   \Delta_{dB} = 20\log_{10}\left(\frac{1/\sqrt{2}}{RMS_{noise}}\right)
 
-Therefore, if our calibration noise had a level (measured with the SPL meter) or :math:`x` dB SPL, a sinusoid at max amplitude would have a level of:
+Therefore, if our calibration noise had a level (measured with the SPL meter) of :math:`x` dB SPL, a sinusoid at max amplitude would have a level of:
 
 .. math::
 
-   maxlev = x + dbdiff
+   maxlev = x + \Delta_{dB}
 
 this is the value that you need to enter in the ``Max Level`` field of the transducers calibration table for the loudspeakers in question.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _sec-experiment_setup:
 
-****************
+***************
 Parameters file
-****************
+***************
 
-The settings for a test are stored in a parameters file (which is a simple text file). An example parameters file is shown below::
+The settings for a test are stored in a parameters file, which is a plain text file. An example parameters file is shown below::
 
   angles : -70, -60, -50, -40, -30, -20, -10, 0, 10, 20, 30, 40, 50, 60, 70
   labels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
   channels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
   n_chan : 15
   n_blocks : 1
   stim_list_file : stim_list.csv
@@ -26,17 +26,17 @@
   - `n_blocks`: the number of blocks, that is how many times the test will be repeated
   - `stim_list_file`: the path (absolute or relative) to the file containing the stimulation list (see below)
   - `randomize`: if `true` the stim_list_file will be shuffled before each block repetition
   - `demo_stim`: the path to the WAV file to be used for the demo
   - `demo_stim_lev`: the sound level (in dB SPL) to be used for the demo
 
     
-**************************
+****************
 Stimulation file
-**************************
+****************
 
 Stimulation files specify the stimuli that will be played on each trial of the test. Figure :ref:`fig-stim_file` shows an example stimulation file.
 
 .. _fig-stim_file:
 
 .. figure:: Figures/stim_file.png
    :scale: 50%
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/index.rst.txt` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_sources/installation.rst.txt` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/basic.css` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/doctools.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/jquery.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/language_data.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/pygments.css` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/searchtools.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/sphinx_highlight.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/_static/underscore.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/calibration.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/calibration.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Sound Level Calibration &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>Sound Level Calibration &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -81,37 +81,36 @@
 <p>Figure <a class="reference internal" href="#fig-edit-transducers"><span class="std std-ref">Edit transducers dialog</span></a> shows a screenshot of the <code class="docutils literal notranslate"><span class="pre">Transducers</span></code> dialog which is used for setting calibration values.</p>
 <figure class="align-default" id="id1">
 <span id="fig-edit-transducers"></span><a class="reference internal image-reference" href="_images/edit_transducers.png"><img alt="Edit transducers dialog" src="_images/edit_transducers.png" style="width: 577.5px; height: 288.75px;" /></a>
 <figcaption>
 <p><span class="caption-text">Edit transducers dialog</span><a class="headerlink" href="#id1" title="Permalink to this image"></a></p>
 </figcaption>
 </figure>
-<p>Most of the fields should be pretty much self-explanatory. Using this
-dialog you can add headphones/speakers models to the transducers database. In <cite>sound_source_id</cite> levels are referenced to the level that would be output by a full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the <code class="docutils literal notranslate"><span class="pre">Max</span> <span class="pre">Level</span></code> field you should enter the level in dB SPL that is output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with a SPL meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.</p>
-<p>The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be reasonably loud as to avoid signal-to-noise ratio issues, but not too loud as to cause distortions or damage your hearing in the measurement process. Once I’ve found a reasonable level, by trial and error, I measure the actual level with an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the experiment and note it down.</p>
-<p>We can measure the RMS level of the WAV file with the noise used for calibration, let’s call it <span class="math notranslate nohighlight">\(rmsnoise\)</span>. A full amplitude sinusoid has a root-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the level of a sinusoid at max amplitude and our calibration noise will be equal to:</p>
+<p>Most of the fields should be pretty much self explanatory. Using this dialog you can add headphones/speakers models to the transducers database. In <cite>sound_source_id</cite> levels are referenced to the level that would be output by a full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the <code class="docutils literal notranslate"><span class="pre">Max</span> <span class="pre">Level</span></code> field you should enter the level in dB SPL that is output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with an SPL meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.</p>
+<p>The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be reasonably high as to avoid signal-to-noise ratio issues, but not so high as to cause distortions or damage your hearing in the measurement process. Once I’ve found a reasonable level, by trial and error, I measure the actual level with an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the experiment, and note it down.</p>
+<p>We can measure the root-mean-square (RMS) level of the WAV file with the noise used for calibration, let’s call it <span class="math notranslate nohighlight">\(RMS_{noise}\)</span>. A full amplitude sinusoid has an RMS amplitude of <span class="math notranslate nohighlight">\(1/\sqrt{2} = 0.707\)</span>. The difference in dB between the level of a sinusoid at max amplitude and our calibration noise will be equal to:</p>
 <div class="math notranslate nohighlight">
-\[dbdiff = 20*log10((1/sqrt(2))/rmsnoise)\]</div>
-<p>Therefore, if our calibration noise had a level (measured with the SPL meter) or <span class="math notranslate nohighlight">\(x\)</span> dB SPL, a sinusoid at max amplitude would have a level of:</p>
+\[\Delta_{dB} = 20\log_{10}\left(\frac{1/\sqrt{2}}{RMS_{noise}}\right)\]</div>
+<p>Therefore, if our calibration noise had a level (measured with the SPL meter) of <span class="math notranslate nohighlight">\(x\)</span> dB SPL, a sinusoid at max amplitude would have a level of:</p>
 <div class="math notranslate nohighlight">
-\[maxlev = x + dbdiff\]</div>
+\[maxlev = x + \Delta_{dB}\]</div>
 <p>this is the value that you need to enter in the <code class="docutils literal notranslate"><span class="pre">Max</span> <span class="pre">Level</span></code> field of the transducers calibration table for the loudspeakers in question.</p>
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="experiment_setup.html" class="btn btn-neutral float-left" title="Parameters file" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
@@ -12,38 +12,38 @@
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ SSoouunndd LLeevveell CCaalliibbrraattiioonn_? ************
 Figure _E_d_i_t_ _t_r_a_n_s_d_u_c_e_r_s_ _d_i_a_l_o_g shows a screenshot of the Transducers dialog
 which is used for setting calibration values.
 _[_E_d_i_t_ _t_r_a_n_s_d_u_c_e_r_s_ _d_i_a_l_o_g_]
 Edit transducers dialog_
-Most of the fields should be pretty much self-explanatory. Using this dialog
+Most of the fields should be pretty much self explanatory. Using this dialog
 you can add headphones/speakers models to the transducers database.
 Insound_source_idlevels are referenced to the level that would be output by a
 full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the Max
 Level field you should enter the level in dB SPL that is output by the
 transducer for a full amplitude sinusoid . However, getting reliable readings
-for a pure tone with a SPL meter is difficult, therefore, typically a noise is
+for a pure tone with an SPL meter is difficult, therefore, typically a noise is
 used for calibrating loudspeakers.
 The procedure I normally use for calibrating loudspeakers is to save on disk a
 noise stimulus as a wav file. I filter the noise within the operating range of
 the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be
-reasonably loud as to avoid signal-to-noise ratio issues, but not too loud as
-to cause distortions or damage your hearing in the measurement process. Once
-I’ve found a reasonable level, by trial and error, I measure the actual level
-with an SPL meter held at the position where the listener head would be located
-relative to the loudspeaker during the experiment and note it down.
-We can measure the RMS level of the WAV file with the noise used for
-calibration, let’s call it \(rmsnoise\). A full amplitude sinusoid has a root-
-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the
-level of a sinusoid at max amplitude and our calibration noise will be equal
-to:
-\[dbdiff = 20*log10((1/sqrt(2))/rmsnoise)\]
+reasonably high as to avoid signal-to-noise ratio issues, but not so high as to
+cause distortions or damage your hearing in the measurement process. Once I’ve
+found a reasonable level, by trial and error, I measure the actual level with
+an SPL meter held at the position where the listener head would be located
+relative to the loudspeaker during the experiment, and note it down.
+We can measure the root-mean-square (RMS) level of the WAV file with the noise
+used for calibration, let’s call it \(RMS_{noise}\). A full amplitude sinusoid
+has an RMS amplitude of \(1/\sqrt{2} = 0.707\). The difference in dB between
+the level of a sinusoid at max amplitude and our calibration noise will be
+equal to:
+\[\Delta_{dB} = 20\log_{10}\left(\frac{1/\sqrt{2}}{RMS_{noise}}\right)\]
 Therefore, if our calibration noise had a level (measured with the SPL meter)
-or \(x\) dB SPL, a sinusoid at max amplitude would have a level of:
-\[maxlev = x + dbdiff\]
+of \(x\) dB SPL, a sinusoid at max amplitude would have a level of:
+\[maxlev = x + \Delta_{dB}\]
 this is the value that you need to enter in the Max Level field of the
 transducers calibration table for the loudspeakers in question.
 _P_r_e_v_i_o_u_s
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/experiment_setup.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/experiment_setup.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Parameters file &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>Parameters file &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -74,15 +74,15 @@
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="parameters-file">
 <span id="sec-experiment-setup"></span><h1>Parameters file<a class="headerlink" href="#parameters-file" title="Permalink to this heading"></a></h1>
-<p>The settings for a test are stored in a parameters file (which is a simple text file). An example parameters file is shown below:</p>
+<p>The settings for a test are stored in a parameters file, which is a plain text file. An example parameters file is shown below:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">angles</span> <span class="p">:</span> <span class="o">-</span><span class="mi">70</span><span class="p">,</span> <span class="o">-</span><span class="mi">60</span><span class="p">,</span> <span class="o">-</span><span class="mi">50</span><span class="p">,</span> <span class="o">-</span><span class="mi">40</span><span class="p">,</span> <span class="o">-</span><span class="mi">30</span><span class="p">,</span> <span class="o">-</span><span class="mi">20</span><span class="p">,</span> <span class="o">-</span><span class="mi">10</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">20</span><span class="p">,</span> <span class="mi">30</span><span class="p">,</span> <span class="mi">40</span><span class="p">,</span> <span class="mi">50</span><span class="p">,</span> <span class="mi">60</span><span class="p">,</span> <span class="mi">70</span>
 <span class="n">labels</span> <span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">,</span> <span class="mi">7</span><span class="p">,</span> <span class="mi">8</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">11</span><span class="p">,</span> <span class="mi">12</span><span class="p">,</span> <span class="mi">13</span><span class="p">,</span> <span class="mi">14</span><span class="p">,</span> <span class="mi">15</span>
 <span class="n">channels</span> <span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">,</span> <span class="mi">7</span><span class="p">,</span> <span class="mi">8</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">11</span><span class="p">,</span> <span class="mi">12</span><span class="p">,</span> <span class="mi">13</span><span class="p">,</span> <span class="mi">14</span><span class="p">,</span> <span class="mi">15</span>
 <span class="n">n_chan</span> <span class="p">:</span> <span class="mi">15</span>
 <span class="n">n_blocks</span> <span class="p">:</span> <span class="mi">1</span>
 <span class="n">stim_list_file</span> <span class="p">:</span> <span class="n">stim_list</span><span class="o">.</span><span class="n">csv</span>
 <span class="n">randomize</span> <span class="p">:</span> <span class="n">true</span>
@@ -134,15 +134,15 @@
         <a href="installation.html" class="btn btn-neutral float-left" title="Installation" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="calibration.html" class="btn btn-neutral float-right" title="Sound Level Calibration" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
 _s_o_u_n_d___s_o_u_r_c_e___i_d
     * Parameters file
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ PPaarraammeetteerrss ffiillee_? ************
-The settings for a test are stored in a parameters file (which is a simple text
-file). An example parameters file is shown below:
+The settings for a test are stored in a parameters file, which is a plain text
+file. An example parameters file is shown below:
 angles : -70, -60, -50, -40, -30, -20, -10, 0, 10, 20, 30, 40, 50, 60, 70
 labels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
 channels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
 n_chan : 15
 n_blocks : 1
 stim_list_file : stim_list.csv
 randomize : true
@@ -61,9 +61,9 @@
          * roving: a level rove, actual sound level will be euqual to the
            base level plus a value drawn from a random uniform
            distribution between +/- the roving level
          * feedback: iftrue, feedback will be given to the listener at the
            end of each trial
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/genindex.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>Index &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -83,15 +83,15 @@
            </div>
           </div>
           <footer>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
 _s_o_u_n_d___s_o_u_r_c_e___i_d
     * Index
 ===============================================================================
 ************ IInnddeexx ************
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/index.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -103,15 +103,15 @@
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="intro.html" class="btn btn-neutral float-right" title="sound_source_id" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
@@ -20,9 +20,9 @@
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
 ************ IInnddiicceess aanndd ttaabblleess_? ************
     * _I_n_d_e_x
     * _M_o_d_u_l_e_ _I_n_d_e_x
     * _S_e_a_r_c_h_ _P_a_g_e
 _N_e_x_t
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/installation.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/installation.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>Installation &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -119,15 +119,15 @@
         <a href="intro.html" class="btn btn-neutral float-left" title="sound_source_id" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="experiment_setup.html" class="btn btn-neutral float-right" title="Parameters file" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
@@ -37,9 +37,9 @@
 pyalsaaudio can be also used. Depending on how you want sound to be played, you
 need to install:
          * pyalsaaudio _h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_p_y_a_l_s_a_a_u_d_i_o_/
 or SoX:
          * _h_t_t_p_s_:_/_/_s_o_x_._s_o_u_r_c_e_f_o_r_g_e_._n_e_t_/
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/intro.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/intro.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>sound_source_id &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>sound_source_id &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -74,15 +74,15 @@
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="sound-source-id">
 <h1><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code><a class="headerlink" href="#sound-source-id" title="Permalink to this heading"></a></h1>
-<p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> is program for testing static sound localization. The interface is shown in Figure <a class="reference internal" href="#fig-sound-source-id-screenshot"><span class="std std-ref">Screenshot of the sound_source_id interface.</span></a>.</p>
+<p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> is a program for testing static sound localization. The interface is shown in Figure <a class="reference internal" href="#fig-sound-source-id-screenshot"><span class="std std-ref">Screenshot of the sound_source_id interface.</span></a>.</p>
 <figure class="align-default" id="id1">
 <span id="fig-sound-source-id-screenshot"></span><a class="reference internal image-reference" href="_images/sound_source_id_screenshot.png"><img alt="Screenshot of the ``sound_source_id`` interface." src="_images/sound_source_id_screenshot.png" style="width: 624.0px; height: 311.5px;" /></a>
 <figcaption>
 <p><span class="caption-text">Screenshot of the <code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> interface.</span><a class="headerlink" href="#id1" title="Permalink to this image"></a></p>
 </figcaption>
 </figure>
 </section>
@@ -94,15 +94,15 @@
         <a href="index.html" class="btn btn-neutral float-left" title="Welcome to sound_source_id’s documentation!" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="installation.html" class="btn btn-neutral float-right" title="Installation" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
 _s_o_u_n_d___s_o_u_r_c_e___i_d
     * sound_source_id
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ ssoouunndd__ssoouurrccee__iidd_? ************
-sound_source_id is program for testing static sound localization. The interface
-is shown in Figure _S_c_r_e_e_n_s_h_o_t_ _o_f_ _t_h_e_ _s_o_u_n_d___s_o_u_r_c_e___i_d_ _i_n_t_e_r_f_a_c_e_..
+sound_source_id is a program for testing static sound localization. The
+interface is shown in Figure _S_c_r_e_e_n_s_h_o_t_ _o_f_ _t_h_e_ _s_o_u_n_d___s_o_u_r_c_e___i_d_ _i_n_t_e_r_f_a_c_e_..
 _[_S_c_r_e_e_n_s_h_o_t_ _o_f_ _t_h_e_ _`_`_s_o_u_n_d___s_o_u_r_c_e___i_d_`_`_ _i_n_t_e_r_f_a_c_e_._]
 Screenshot of the sound_source_id interface._
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/search.html` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; sound_source_id 0.2.5 documentation</title>
+  <title>Search &mdash; sound_source_id 0.2.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.5
+                0.2.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -91,15 +91,15 @@
            </div>
           </div>
           <footer>
 
   <hr/>
 
   <div role="contentinfo">
-    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+    <p>&#169; Copyright 2022-2024, Samuele Carcagno.</p>
   </div>
 
   Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
     <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
     provided by <a href="https://readthedocs.org">Read the Docs</a>.
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.5
+0.2.6
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
 _s_o_u_n_d___s_o_u_r_c_e___i_d
     * Search
 ===============================================================================
 Please activate JavaScript to enable the search functionality.
 ===============================================================================
-© Copyright 2022-2023, Samuele Carcagno.
+© Copyright 2022-2024, Samuele Carcagno.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/html/searchindex.js` & `sound_source_id-0.2.6/sound_source_id/doc/_build/html/searchindex.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -6,28 +6,28 @@
         "The": [0, 1, 4],
         "set": [0, 1],
         "test": [1, 3, 4],
         "ar": [0, 1],
         "store": 1,
         "which": [0, 1],
         "i": [0, 1, 3, 4],
-        "simpl": 1,
+        "simpl": [],
         "text": 1,
         "an": [0, 1],
         "exampl": 1,
         "shown": [1, 4],
         "below": 1,
         "angl": 1,
         "70": 1,
         "60": 1,
         "50": 1,
         "40": 1,
         "30": 1,
         "20": [0, 1],
-        "10": 1,
+        "10": [0, 1],
         "0": [0, 1],
         "label": 1,
         "1": [0, 1],
         "2": [0, 1],
         "3": 1,
         "4": 1,
         "5": 1,
@@ -63,16 +63,16 @@
         "sound": [1, 2, 3, 4],
         "present": 1,
         "note": [0, 1],
         "indic": 1,
         "straight": 1,
         "ahead": 1,
         "90": 1,
-        "right": 1,
-        "left": 1,
+        "right": [0, 1],
+        "left": [0, 1],
         "each": 1,
         "thi": [0, 1, 3],
         "can": [0, 1, 3],
         "number": 1,
         "letter": 1,
         "e": [1, 3],
         "g": [1, 3],
@@ -257,20 +257,20 @@
         "oper": 0,
         "rang": 0,
         "usual": 0,
         "around": 0,
         "05": 0,
         "khz": 0,
         "reason": 0,
-        "loud": 0,
+        "loud": [],
         "avoid": 0,
         "signal": 0,
         "ratio": 0,
         "issu": 0,
-        "too": 0,
+        "too": [],
         "caus": 0,
         "distort": 0,
         "damag": 0,
         "hear": 0,
         "measur": 0,
         "process": 0,
         "onc": 0,
@@ -285,34 +285,42 @@
         "dure": 0,
         "experi": 0,
         "down": 0,
         "we": 0,
         "rm": 0,
         "let": 0,
         "": 0,
-        "rmsnois": 0,
+        "rmsnois": [],
         "A": 0,
         "convent": [],
         "root": 0,
         "mean": 0,
         "squar": 0,
         "sqrt": 0,
         "707": 0,
         "differ": 0,
         "our": 0,
         "equal": 0,
-        "dbdiff": 0,
-        "log10": 0,
+        "dbdiff": [],
+        "log10": [],
         "had": 0,
         "x": 0,
         "have": 0,
         "maxlev": 0,
         "tabl": 0,
         "question": 0,
-        "pyqt6": 3
+        "pyqt6": 3,
+        "high": 0,
+        "so": 0,
+        "plain": 1,
+        "frac": 0,
+        "cdot": [],
+        "log_": 0,
+        "delta_": 0,
+        "rms_": 0
     },
     "objects": {},
     "objtypes": {},
     "objnames": {},
     "titleterms": {
         "paramet": 1,
         "file": 1,
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.2.6/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Files 18% similar despite different names*

#### Comparing `sound_source_id-0.2.5/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.2.6/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Samuele Carcagno'
-CreationDate: "D:20240505085505+02'00'"
+CreationDate: "D:20240506102101+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20240505085505+02'00'"
+ModDate: "D:20240506102101+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Debian) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'sound_source_id'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 sound_source_id
-Release 0.2.5
+Release 0.2.6
 
 Samuele Carcagno
 
-May 05, 2024
+May 06, 2024
 
 CONTENTS:
 
 1
 
 sound_source_id
 
@@ -49,22 +49,22 @@
 
 CHAPTER
 
 ONE
 
 SOUND_SOURCE_ID
 
-sound_source_id is program for testing static sound localization. The interface is shown in Figure Screenshot of the
-sound_source_id interface..
+sound_source_id is a program for testing static sound localization. The interface is shown in Figure Screenshot of
+the sound_source_id interface..
 
 Fig. 1: Screenshot of the sound_source_id interface.
 
 1
 
-sound_source_id, Release 0.2.5
+sound_source_id, Release 0.2.6
 
 2
 
 Chapter 1. sound_source_id
 
 CHAPTER
 
@@ -94,27 +94,27 @@
 on how you want sound to be played, you need to install:
 • pyalsaaudio https://pypi.org/project/pyalsaaudio/
 or SoX:
 • https://sox.sourceforge.net/
 
 3
 
-sound_source_id, Release 0.2.5
+sound_source_id, Release 0.2.6
 
 4
 
 Chapter 2. Installation
 
 CHAPTER
 
 THREE
 
 PARAMETERS FILE
 
-The settings for a test are stored in a parameters file (which is a simple text file). An example parameters file is shown
+The settings for a test are stored in a parameters file, which is a plain text file. An example parameters file is shown
 below:
 angles : -70, -60, -50, -40, -30, -20, -10, 0, 10, 20, 30, 40, 50, 60, 70
 labels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
 channels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
 n_chan : 15
 n_blocks : 1
 stim_list_file : stim_list.csv
@@ -131,15 +131,15 @@
 • stim_list_file: the path (absolute or relative) to the file containing the stimulation list (see below)
 • randomize: if true the stim_list_file will be shuffled before each block repetition
 • demo_stim: the path to the WAV file to be used for the demo
 • demo_stim_lev: the sound level (in dB SPL) to be used for the demo
 
 5
 
-sound_source_id, Release 0.2.5
+sound_source_id, Release 0.2.6
 
 6
 
 Chapter 3. Parameters file
 
 CHAPTER
 
@@ -160,15 +160,15 @@
 has been correctly calibrated)
 • roving: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform
 distribution between +/- the roving level
 • feedback: if true, feedback will be given to the listener at the end of each trial
 
 7
 
-sound_source_id, Release 0.2.5
+sound_source_id, Release 0.2.6
 
 8
 
 Chapter 4. Stimulation file
 
 CHAPTER
 
@@ -176,37 +176,42 @@
 
 SOUND LEVEL CALIBRATION
 
 Figure Edit transducers dialog shows a screenshot of the Transducers dialog which is used for setting calibration
 values.
 
 Fig. 1: Edit transducers dialog
-Most of the fields should be pretty much self-explanatory. Using this dialog you can add headphones/speakers models to
+Most of the fields should be pretty much self explanatory. Using this dialog you can add headphones/speakers models to
 the transducers database. In sound_source_id levels are referenced to the level that would be output by a full amplitude
 sinusoid (a sinusoid with a peak amplitude of 1). In the Max Level field you should enter the level in dB SPL that is
-output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with a SPL
+output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with an SPL
 meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.
 The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter
 the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be
-reasonably loud as to avoid signal-to-noise ratio issues, but not too loud as to cause distortions or damage your hearing
+reasonably high as to avoid signal-to-noise ratio issues, but not so high as to cause distortions or damage your hearing
 in the measurement process. Once I’ve found a reasonable level, by trial and error, I measure the actual level with
 an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the
-experiment and note it down.
-We can measure the RMS level of the WAV file with the noise used for calibration, let’s call it 𝑟𝑚𝑠𝑛𝑜𝑖𝑠𝑒. A full
-amplitude sinusoid has a root-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the level of
-a sinusoid at max amplitude and our calibration noise will be equal to:
-𝑑𝑏𝑑𝑖𝑓 𝑓 = 20 * 𝑙𝑜𝑔10((1/𝑠𝑞𝑟𝑡(2))/𝑟𝑚𝑠𝑛𝑜𝑖𝑠𝑒)
+experiment, and note it down.
+We can measure the root-mean-square (RMS) level of the WAV file√with the noise used for calibration, let’s call it
+𝑅𝑀 𝑆𝑛𝑜𝑖𝑠𝑒 . A full amplitude sinusoid has an RMS amplitude of 1/ 2 = 0.707. The difference in dB between the
 
 9
 
-sound_source_id, Release 0.2.5
+sound_source_id, Release 0.2.6
 
-Therefore, if our calibration noise had a level (measured with the SPL meter) or 𝑥 dB SPL, a sinusoid at max amplitude
+level of a sinusoid at max amplitude and our calibration noise will be equal to:
+(︃
+)︃
+√
+1/ 2
+∆𝑑𝐵 = 20 log10
+𝑅𝑀 𝑆𝑛𝑜𝑖𝑠𝑒
+Therefore, if our calibration noise had a level (measured with the SPL meter) of 𝑥 dB SPL, a sinusoid at max amplitude
 would have a level of:
-𝑚𝑎𝑥𝑙𝑒𝑣 = 𝑥 + 𝑑𝑏𝑑𝑖𝑓 𝑓
+𝑚𝑎𝑥𝑙𝑒𝑣 = 𝑥 + ∆𝑑𝐵
 this is the value that you need to enter in the Max Level field of the transducers calibration table for the loudspeakers
 in question.
 
 10
 
 Chapter 5. Sound Level Calibration
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/calibration.rst` & `sound_source_id-0.2.6/sound_source_id/doc/calibration.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 
 .. figure:: Figures/edit_transducers.png
    :scale: 75%
    :alt: Edit transducers dialog
 
    Edit transducers dialog
 
-Most of the fields should be pretty much self-explanatory. Using this
-dialog you can add headphones/speakers models to the transducers database. In `sound_source_id` levels are referenced to the level that would be output by a full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the ``Max Level`` field you should enter the level in dB SPL that is output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with a SPL meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.
+Most of the fields should be pretty much self explanatory. Using this dialog you can add headphones/speakers models to the transducers database. In `sound_source_id` levels are referenced to the level that would be output by a full amplitude sinusoid (a sinusoid with a peak amplitude of 1). In the ``Max Level`` field you should enter the level in dB SPL that is output by the transducer for a full amplitude sinusoid . However, getting reliable readings for a pure tone with an SPL meter is difficult, therefore, typically a noise is used for calibrating loudspeakers.
 
-The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be reasonably loud as to avoid signal-to-noise ratio issues, but not too loud as to cause distortions or damage your hearing in the measurement process. Once I've found a reasonable level, by trial and error, I measure the actual level with an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the experiment and note it down.
+The procedure I normally use for calibrating loudspeakers is to save on disk a noise stimulus as a wav file. I filter the noise within the operating range of the SPL meter (usually around 0.05 to 8 kHz). The noise level needs to be reasonably high as to avoid signal-to-noise ratio issues, but not so high as to cause distortions or damage your hearing in the measurement process. Once I've found a reasonable level, by trial and error, I measure the actual level with an SPL meter held at the position where the listener head would be located relative to the loudspeaker during the experiment, and note it down.
 
-We can measure the RMS level of the WAV file with the noise used for calibration, let's call it :math:`rmsnoise`. A full amplitude sinusoid has a root-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the level of a sinusoid at max amplitude and our calibration noise will be equal to:
+We can measure the root-mean-square (RMS) level of the WAV file with the noise used for calibration, let's call it :math:`RMS_{noise}`. A full amplitude sinusoid has an RMS amplitude of :math:`1/\sqrt{2} = 0.707`. The difference in dB between the level of a sinusoid at max amplitude and our calibration noise will be equal to:
 
 .. math::
 
-   dbdiff = 20*log10((1/sqrt(2))/rmsnoise)
+   \Delta_{dB} = 20\log_{10}\left(\frac{1/\sqrt{2}}{RMS_{noise}}\right)
 
-Therefore, if our calibration noise had a level (measured with the SPL meter) or :math:`x` dB SPL, a sinusoid at max amplitude would have a level of:
+Therefore, if our calibration noise had a level (measured with the SPL meter) of :math:`x` dB SPL, a sinusoid at max amplitude would have a level of:
 
 .. math::
 
-   maxlev = x + dbdiff
+   maxlev = x + \Delta_{dB}
 
 this is the value that you need to enter in the ``Max Level`` field of the transducers calibration table for the loudspeakers in question.
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/conf.py` & `sound_source_id-0.2.6/sound_source_id/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'sound_source_id'
-copyright = '2022-2023, Samuele Carcagno'
+copyright = '2022-2024, Samuele Carcagno'
 author = 'Samuele Carcagno'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.2.5"
+version = "0.2.6"
 # The full version, including alpha/beta/rc tags.
-release = "0.2.5"
+release = "0.2.6"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/experiment_setup.rst` & `sound_source_id-0.2.6/sound_source_id/doc/experiment_setup.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _sec-experiment_setup:
 
-****************
+***************
 Parameters file
-****************
+***************
 
-The settings for a test are stored in a parameters file (which is a simple text file). An example parameters file is shown below::
+The settings for a test are stored in a parameters file, which is a plain text file. An example parameters file is shown below::
 
   angles : -70, -60, -50, -40, -30, -20, -10, 0, 10, 20, 30, 40, 50, 60, 70
   labels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
   channels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
   n_chan : 15
   n_blocks : 1
   stim_list_file : stim_list.csv
@@ -26,17 +26,17 @@
   - `n_blocks`: the number of blocks, that is how many times the test will be repeated
   - `stim_list_file`: the path (absolute or relative) to the file containing the stimulation list (see below)
   - `randomize`: if `true` the stim_list_file will be shuffled before each block repetition
   - `demo_stim`: the path to the WAV file to be used for the demo
   - `demo_stim_lev`: the sound level (in dB SPL) to be used for the demo
 
     
-**************************
+****************
 Stimulation file
-**************************
+****************
 
 Stimulation files specify the stimuli that will be played on each trial of the test. Figure :ref:`fig-stim_file` shows an example stimulation file.
 
 .. _fig-stim_file:
 
 .. figure:: Figures/stim_file.png
    :scale: 50%
```

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/index.rst` & `sound_source_id-0.2.6/sound_source_id/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/installation.rst` & `sound_source_id-0.2.6/sound_source_id/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/doc/make.bat` & `sound_source_id-0.2.6/sound_source_id/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/global_parameters.py` & `sound_source_id-0.2.6/sound_source_id/global_parameters.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise1.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise1.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise10.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise10.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise11.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise11.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise12.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise12.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise13.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise13.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise14.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise14.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise15.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise15.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise16.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise16.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise17.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise17.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise18.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise18.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise19.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise19.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise2.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise2.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise20.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise20.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise21.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise21.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise22.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise22.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise23.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise23.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise24.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise24.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise25.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise25.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise26.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise26.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise27.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise27.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise28.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise28.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise29.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise29.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise3.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise3.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise30.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise30.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise4.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise4.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise5.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise5.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise6.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise6.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise7.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise7.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise8.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise8.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/pink_noises/noise9.wav` & `sound_source_id-0.2.6/sound_source_id/prm_files/pink_noises/noise9.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/prm_circle_36_targets.txt` & `sound_source_id-0.2.6/sound_source_id/prm_files/prm_circle_36_targets.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt` & `sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt` & `sound_source_id-0.2.6/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/stim_list.csv` & `sound_source_id-0.2.6/sound_source_id/prm_files/stim_list.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_4_front_back.csv` & `sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_4_front_back.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_8_az_2_elev.csv` & `sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_8_az_2_elev.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_circle.csv` & `sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_circle.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/prm_files/stim_list_circle_12_tgs.csv` & `sound_source_id-0.2.6/sound_source_id/prm_files/stim_list_circle_12_tgs.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/pyqtver.py` & `sound_source_id-0.2.6/sound_source_id/pyqtver.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/qrc_resources.py` & `sound_source_id-0.2.6/sound_source_id/qrc_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -61268,25 +61268,25 @@
 \x00\x00\x00\xa8\x00\x00\x00\x00\x00\x01\x00\x0a\xa9\x04\
 \x00\x00\x019\x1d\x82\xc4\xe8\
 \x00\x00\x00\x1a\x00\x02\x00\x00\x00\x06\x00\x00\x00\x0a\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x0e\xabS\
 \x00\x00\x019\x1d{\xa8\x98\
 \x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x0e\xdcW\
-\x00\x00\x01\x8fG\x88\xddY\
+\x00\x00\x01\x8fL\xfd\xe5H\
 \x00\x00\x02\x0a\x00\x00\x00\x00\x00\x01\x00\x0e\xdc\x7f\
-\x00\x00\x01\x8fG\x88\xddW\
+\x00\x00\x01\x8fL\xfd\xe5F\
 \x00\x00\x01t\x00\x00\x00\x00\x00\x01\x00\x0e\xdcC\
-\x00\x00\x01\x8fG\x88\xddX\
+\x00\x00\x01\x8fL\xfd\xe5G\
 \x00\x00\x01\x0e\x00\x00\x00\x00\x00\x01\x00\x0e\xd4\xfd\
-\x00\x00\x01\x8fG\x88\xddV\
+\x00\x00\x01\x8fL\xfd\xe5D\
 \x00\x00\x01\xd4\x00\x00\x00\x00\x00\x01\x00\x0e\xdck\
-\x00\x00\x01\x8fG\x88\xdd[\
+\x00\x00\x01\x8fL\xfd\xe5J\
 \x00\x00\x01>\x00\x00\x00\x00\x00\x01\x00\x0e\xdc/\
-\x00\x00\x01\x8fG\x88\xddZ\
+\x00\x00\x01\x8fL\xfd\xe5I\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `sound_source_id-0.2.5/sound_source_id/sndlib.py` & `sound_source_id-0.2.6/sound_source_id/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/utils.py` & `sound_source_id-0.2.6/sound_source_id/utils.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/wavpy.py` & `sound_source_id-0.2.6/sound_source_id/wavpy.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id/wavpy_sndf.py` & `sound_source_id-0.2.6/sound_source_id/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.5/sound_source_id.egg-info/PKG-INFO` & `sound_source_id-0.2.6/sound_source_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sound_source_id-0.2.5/sound_source_id.egg-info/SOURCES.txt` & `sound_source_id-0.2.6/sound_source_id.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -94,14 +94,32 @@
 sound_source_id/doc/_build/html/_static/language_data.js
 sound_source_id/doc/_build/html/_static/minus.png
 sound_source_id/doc/_build/html/_static/plus.png
 sound_source_id/doc/_build/html/_static/pygments.css
 sound_source_id/doc/_build/html/_static/searchtools.js
 sound_source_id/doc/_build/html/_static/sphinx_highlight.js
 sound_source_id/doc/_build/html/_static/underscore.js
+sound_source_id/doc/_build/html/_static/css/badge_only.css
+sound_source_id/doc/_build/html/_static/css/theme.css
+sound_source_id/doc/_build/html/_static/fonts/Lato-Bold.ttf
+sound_source_id/doc/_build/html/_static/fonts/Lato-Bold.woff2
+sound_source_id/doc/_build/html/_static/fonts/Lato-BoldItalic.ttf
+sound_source_id/doc/_build/html/_static/fonts/Lato-BoldItalic.woff2
+sound_source_id/doc/_build/html/_static/fonts/Lato-Italic.ttf
+sound_source_id/doc/_build/html/_static/fonts/Lato-Italic.woff2
+sound_source_id/doc/_build/html/_static/fonts/Lato-Regular.ttf
+sound_source_id/doc/_build/html/_static/fonts/Lato-Regular.woff2
+sound_source_id/doc/_build/html/_static/fonts/RobotoSlab-Bold.woff2
+sound_source_id/doc/_build/html/_static/fonts/RobotoSlab-Regular.woff2
+sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.eot
+sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.svg
+sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.ttf
+sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.woff
+sound_source_id/doc/_build/html/_static/fonts/fontawesome-webfont.woff2
+sound_source_id/doc/_build/html/_static/js/theme.js
 sound_source_id/doc/_build/latex/sound_source_id.pdf
 sound_source_id/prm_files/prm.txt
 sound_source_id/prm_files/prm_2_targets.txt
 sound_source_id/prm_files/prm_circle_36_targets.txt
 sound_source_id/prm_files/prm_virtual.txt
 sound_source_id/prm_files/prm_virtual_2_targets.txt
 sound_source_id/prm_files/prm_virtual_4_front_back.txt
```

