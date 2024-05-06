# Comparing `tmp/beets-bpmanalyser-1.4.0.tar.gz` & `tmp/beets-bpmanalyser-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beets-bpmanalyser-1.4.0.tar", last modified: Fri May  3 20:31:27 2024, max compression
+gzip compressed data, was "dist/beets-bpmanalyser-1.4.1.tar", last modified: Mon May  6 14:34:38 2024, max compression
```

## Comparing `beets-bpmanalyser-1.4.0.tar` & `beets-bpmanalyser-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     5766 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1293 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6278 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2038 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/get_song_bpm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-03 20:31:27.000000 beets-bpmanalyser-1.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1489 2024-05-03 20:31:16.000000 beets-bpmanalyser-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5868 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/analyser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7357 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-06 14:34:38.000000 beets-bpmanalyser-1.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1489 2024-05-06 14:34:29.000000 beets-bpmanalyser-1.4.1/setup.py
```

### Comparing `beets-bpmanalyser-1.4.0/LICENSE.txt` & `beets-bpmanalyser-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.4.0/PKG-INFO` & `beets-bpmanalyser-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,146 +1,145 @@
 Metadata-Version: 2.1
 Name: beets-bpmanalyser
-Version: 1.4.0
+Version: 1.4.1
 Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
 Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
 Description: [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser)
         [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginBpmAnalyser/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginBpmAnalyser?branch=master)
         [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
         [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
         
         # BPM Analyser (Beets Plugin)
         
-        The *beets-bpmanalyser* plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
+        The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
         
         This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
         
-        
         ## Installation
+        
         The plugin can be installed via:
         
         ```shell script
         $ pip install beets-bpmanalyser
         ```
         
         It has two dependencies: [numpy](https://pypi.org/project/numpy/) and [aubio](https://pypi.org/project/aubio/) both of which will be installed automatically when installing the plugin itself.
         
-        
         ## Usage
+        
         Activate the plugin in your configuration file:
         
         ```yaml
         plugins:
           - bpmanalyser
           # [...]
         ```
         
         Check if plugin is loaded with `beet version`. It should list 'bpmanalyser' amongst the loaded plugins.
         
         Your default configuration is:
+        
         ```yaml
         bpmanalyser:
           auto: no
           dry-run: no
           write: yes
           threads: 2
           force: no
           quiet: no
         ```
         
         You can set the `auto` option if you would like to execute the analysis during import. In this case, the `threads` option is ignored (beets import is already multithreaded).
         
-        
-        The other configuration options can also be set from the command line when running the plugin. 
+        The other configuration options can also be set from the command line when running the plugin.
         Here are the options explained:
         
-        *-d, --dry-run*     : Do not update the library or the media files. Only display the bpm values.
-        
-        *-f, --force*       : By default only songs with no bpm value (bpm:0) are analysed. Use this option to force the analysis regardless of the current bpm value.
+        _-d, --dry-run_ : Do not update the library or the media files. Only display the bpm values.
         
-        *-w, --write*       : Write the bpm values directly to the media files.
+        _-f, --force_ : By default only songs with no bpm value (bpm:0) are analysed. Use this option to force the analysis regardless of the current bpm value.
         
-        *-t THREADS, --threads=THREADS*: Set the number of processes that can run in parallel. It will default to the number of cores of your processor(s).
+        _-w, --write_ : Write the bpm values directly to the media files.
         
-        *-q, --quiet*       : Do not display any output from the command.
+        _-t THREADS, --threads=THREADS_: Set the number of processes that can run in parallel. By default it is set to AUTO (`threads: AUTO`) and it will use half of the number of cores of your processor(s) have. You can set this to any number to specify how many concurrent threads you want to run.
         
-        *-v, --version*     : Displays the version number of the plugin.
+        _-q, --quiet_ : Do not display any output from the command.
         
+        _-v, --version_ : Displays the version number of the plugin.
         
-            
         ### Examples:
         
         Calculate but show only (do not store) tempo information on all AC/DC songs:
         
             $ beet bpmanalyser --dry-run artist:AC/DC
-            
+        
         Update tempo information on all songs where it is missing:
         
             $ beet bpmanalyser bpm:0
-            
+        
         Force the update of tempo information on all songs where it has already been set:
         
             $ beet bpmanalyser -f ^bpm:0
         
-        
         ## Accuracy
+        
         BPM values from acousticbrainz:
+        
         ```shell script
         $ beet -c dev.yml acousticbrainz artist:AC/DC
         acousticbrainz: getting data for: [format:MP3][bpm:121.106361389] ::: /_TmpMusic_/A/AC_DC/High Voltage/01. Baby, Please Don't Go.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:117.203399658] ::: /_TmpMusic_/A/AC_DC/High Voltage/02. She's Got Balls.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:106.826393127] ::: /_TmpMusic_/A/AC_DC/High Voltage/03. Little Lover.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:119.486862183] ::: /_TmpMusic_/A/AC_DC/High Voltage/04. Stick Around.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:133.189102173] ::: /_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:128.054992676] ::: /_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:123.012046814] ::: /_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:136.914703369] ::: /_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3
         ```
         
         BPM values calculated by aubio:
+        
         ```shell script
         $ beet -c dev.yml bpmanalyser artist:AC/DC -df
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/01. Baby, Please Don't Go.mp3] bpm: 122
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/02. She's Got Balls.mp3] bpm: 117
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/03. Little Lover.mp3] bpm: 106
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/04. Stick Around.mp3] bpm: 120
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3] bpm: 132
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3] bpm: 128
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3] bpm: 125
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3] bpm: 139
         ```
-         
         
         ## Issues
+        
         If something is not working as expected please use the Issue tracker.
         If the documentation is not clear please use the Issue tracker.
         If you have a feature request please use the Issue tracker.
         In any other situation please use the Issue tracker.
         
-        
         ## Other plugins by the same author
+        
         - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
         - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
         - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
         - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
         - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
         - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
         - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
         
-        
         ## Acknowledgements
-        Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin. 
         
+        Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin.
         
         ## Final Remarks
-        Enjoy!
         
+        Enjoy!
         
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `beets-bpmanalyser-1.4.0/README.md` & `beets-bpmanalyser-1.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,131 +1,130 @@
 [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginBpmAnalyser/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginBpmAnalyser?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # BPM Analyser (Beets Plugin)
 
-The *beets-bpmanalyser* plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
+The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
 
 This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
 
-
 ## Installation
+
 The plugin can be installed via:
 
 ```shell script
 $ pip install beets-bpmanalyser
 ```
 
 It has two dependencies: [numpy](https://pypi.org/project/numpy/) and [aubio](https://pypi.org/project/aubio/) both of which will be installed automatically when installing the plugin itself.
 
-
 ## Usage
+
 Activate the plugin in your configuration file:
 
 ```yaml
 plugins:
   - bpmanalyser
   # [...]
 ```
 
 Check if plugin is loaded with `beet version`. It should list 'bpmanalyser' amongst the loaded plugins.
 
 Your default configuration is:
+
 ```yaml
 bpmanalyser:
   auto: no
   dry-run: no
   write: yes
   threads: 2
   force: no
   quiet: no
 ```
 
 You can set the `auto` option if you would like to execute the analysis during import. In this case, the `threads` option is ignored (beets import is already multithreaded).
 
-
-The other configuration options can also be set from the command line when running the plugin. 
+The other configuration options can also be set from the command line when running the plugin.
 Here are the options explained:
 
-*-d, --dry-run*     : Do not update the library or the media files. Only display the bpm values.
-
-*-f, --force*       : By default only songs with no bpm value (bpm:0) are analysed. Use this option to force the analysis regardless of the current bpm value.
+_-d, --dry-run_ : Do not update the library or the media files. Only display the bpm values.
 
-*-w, --write*       : Write the bpm values directly to the media files.
+_-f, --force_ : By default only songs with no bpm value (bpm:0) are analysed. Use this option to force the analysis regardless of the current bpm value.
 
-*-t THREADS, --threads=THREADS*: Set the number of processes that can run in parallel. It will default to the number of cores of your processor(s).
+_-w, --write_ : Write the bpm values directly to the media files.
 
-*-q, --quiet*       : Do not display any output from the command.
+_-t THREADS, --threads=THREADS_: Set the number of processes that can run in parallel. By default it is set to AUTO (`threads: AUTO`) and it will use half of the number of cores of your processor(s) have. You can set this to any number to specify how many concurrent threads you want to run.
 
-*-v, --version*     : Displays the version number of the plugin.
+_-q, --quiet_ : Do not display any output from the command.
 
+_-v, --version_ : Displays the version number of the plugin.
 
-    
 ### Examples:
 
 Calculate but show only (do not store) tempo information on all AC/DC songs:
 
     $ beet bpmanalyser --dry-run artist:AC/DC
-    
+
 Update tempo information on all songs where it is missing:
 
     $ beet bpmanalyser bpm:0
-    
+
 Force the update of tempo information on all songs where it has already been set:
 
     $ beet bpmanalyser -f ^bpm:0
 
-
 ## Accuracy
+
 BPM values from acousticbrainz:
+
 ```shell script
 $ beet -c dev.yml acousticbrainz artist:AC/DC
 acousticbrainz: getting data for: [format:MP3][bpm:121.106361389] ::: /_TmpMusic_/A/AC_DC/High Voltage/01. Baby, Please Don't Go.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:117.203399658] ::: /_TmpMusic_/A/AC_DC/High Voltage/02. She's Got Balls.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:106.826393127] ::: /_TmpMusic_/A/AC_DC/High Voltage/03. Little Lover.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:119.486862183] ::: /_TmpMusic_/A/AC_DC/High Voltage/04. Stick Around.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:133.189102173] ::: /_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:128.054992676] ::: /_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:123.012046814] ::: /_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3
 acousticbrainz: getting data for: [format:MP3][bpm:136.914703369] ::: /_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3
 ```
 
 BPM values calculated by aubio:
+
 ```shell script
 $ beet -c dev.yml bpmanalyser artist:AC/DC -df
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/01. Baby, Please Don't Go.mp3] bpm: 122
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/02. She's Got Balls.mp3] bpm: 117
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/03. Little Lover.mp3] bpm: 106
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/04. Stick Around.mp3] bpm: 120
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3] bpm: 132
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3] bpm: 128
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3] bpm: 125
 bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3] bpm: 139
 ```
- 
 
 ## Issues
+
 If something is not working as expected please use the Issue tracker.
 If the documentation is not clear please use the Issue tracker.
 If you have a feature request please use the Issue tracker.
 In any other situation please use the Issue tracker.
 
-
 ## Other plugins by the same author
+
 - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
 - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
 - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
 - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
 - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
 - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
 - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
 
-
 ## Acknowledgements
-Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin. 
 
+Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin.
 
 ## Final Remarks
-Enjoy!
 
+Enjoy!
```

### Comparing `beets-bpmanalyser-1.4.0/beets_bpmanalyser.egg-info/PKG-INFO` & `beets-bpmanalyser-1.4.1/beets_bpmanalyser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,146 +1,145 @@
 Metadata-Version: 2.1
 Name: beets-bpmanalyser
-Version: 1.4.0
+Version: 1.4.1
 Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
 Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
 Description: [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginBpmAnalyser)
         [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginBpmAnalyser/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginBpmAnalyser?branch=master)
         [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
         [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
         
         # BPM Analyser (Beets Plugin)
         
-        The *beets-bpmanalyser* plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
+        The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
         
         This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
         
-        
         ## Installation
+        
         The plugin can be installed via:
         
         ```shell script
         $ pip install beets-bpmanalyser
         ```
         
         It has two dependencies: [numpy](https://pypi.org/project/numpy/) and [aubio](https://pypi.org/project/aubio/) both of which will be installed automatically when installing the plugin itself.
         
-        
         ## Usage
+        
         Activate the plugin in your configuration file:
         
         ```yaml
         plugins:
           - bpmanalyser
           # [...]
         ```
         
         Check if plugin is loaded with `beet version`. It should list 'bpmanalyser' amongst the loaded plugins.
         
         Your default configuration is:
+        
         ```yaml
         bpmanalyser:
           auto: no
           dry-run: no
           write: yes
           threads: 2
           force: no
           quiet: no
         ```
         
         You can set the `auto` option if you would like to execute the analysis during import. In this case, the `threads` option is ignored (beets import is already multithreaded).
         
-        
-        The other configuration options can also be set from the command line when running the plugin. 
+        The other configuration options can also be set from the command line when running the plugin.
         Here are the options explained:
         
-        *-d, --dry-run*     : Do not update the library or the media files. Only display the bpm values.
-        
-        *-f, --force*       : By default only songs with no bpm value (bpm:0) are analysed. Use this option to force the analysis regardless of the current bpm value.
+        _-d, --dry-run_ : Do not update the library or the media files. Only display the bpm values.
         
-        *-w, --write*       : Write the bpm values directly to the media files.
+        _-f, --force_ : By default only songs with no bpm value (bpm:0) are analysed. Use this option to force the analysis regardless of the current bpm value.
         
-        *-t THREADS, --threads=THREADS*: Set the number of processes that can run in parallel. It will default to the number of cores of your processor(s).
+        _-w, --write_ : Write the bpm values directly to the media files.
         
-        *-q, --quiet*       : Do not display any output from the command.
+        _-t THREADS, --threads=THREADS_: Set the number of processes that can run in parallel. By default it is set to AUTO (`threads: AUTO`) and it will use half of the number of cores of your processor(s) have. You can set this to any number to specify how many concurrent threads you want to run.
         
-        *-v, --version*     : Displays the version number of the plugin.
+        _-q, --quiet_ : Do not display any output from the command.
         
+        _-v, --version_ : Displays the version number of the plugin.
         
-            
         ### Examples:
         
         Calculate but show only (do not store) tempo information on all AC/DC songs:
         
             $ beet bpmanalyser --dry-run artist:AC/DC
-            
+        
         Update tempo information on all songs where it is missing:
         
             $ beet bpmanalyser bpm:0
-            
+        
         Force the update of tempo information on all songs where it has already been set:
         
             $ beet bpmanalyser -f ^bpm:0
         
-        
         ## Accuracy
+        
         BPM values from acousticbrainz:
+        
         ```shell script
         $ beet -c dev.yml acousticbrainz artist:AC/DC
         acousticbrainz: getting data for: [format:MP3][bpm:121.106361389] ::: /_TmpMusic_/A/AC_DC/High Voltage/01. Baby, Please Don't Go.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:117.203399658] ::: /_TmpMusic_/A/AC_DC/High Voltage/02. She's Got Balls.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:106.826393127] ::: /_TmpMusic_/A/AC_DC/High Voltage/03. Little Lover.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:119.486862183] ::: /_TmpMusic_/A/AC_DC/High Voltage/04. Stick Around.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:133.189102173] ::: /_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:128.054992676] ::: /_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:123.012046814] ::: /_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3
         acousticbrainz: getting data for: [format:MP3][bpm:136.914703369] ::: /_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3
         ```
         
         BPM values calculated by aubio:
+        
         ```shell script
         $ beet -c dev.yml bpmanalyser artist:AC/DC -df
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/01. Baby, Please Don't Go.mp3] bpm: 122
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/02. She's Got Balls.mp3] bpm: 117
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/03. Little Lover.mp3] bpm: 106
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/04. Stick Around.mp3] bpm: 120
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/05. Soul Stripper.mp3] bpm: 132
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/06. You Ain't Got a Hold on Me.mp3] bpm: 128
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/07. Love Song.mp3] bpm: 125
         bpmanalyser: Song[/_TmpMusic_/A/AC_DC/High Voltage/08. Show Business.mp3] bpm: 139
         ```
-         
         
         ## Issues
+        
         If something is not working as expected please use the Issue tracker.
         If the documentation is not clear please use the Issue tracker.
         If you have a feature request please use the Issue tracker.
         In any other situation please use the Issue tracker.
         
-        
         ## Other plugins by the same author
+        
         - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
         - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
         - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
         - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
         - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
         - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
         - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
         
-        
         ## Acknowledgements
-        Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin. 
         
+        Many thanks to the developers and contributors of the [beets check plugin](https://github.com/geigerzaehler/beets-check). Some structural concepts and best practices were adopted to start on this plugin.
         
         ## Final Remarks
-        Enjoy!
         
+        Enjoy!
         
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/__init__.py` & `beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  Created: 2/23/20, 10:50 PM
 #  License: See LICENSE.txt
 
 import logging
 
 from beets.plugins import BeetsPlugin
-from beets.util import cpu_count
 from beetsplug.bpmanalyser.command import BpmAnalyserCommand
 
 log = logging.getLogger('beets.bpmanalyser')
 
 
 class BpmAnalyserPlugin(BeetsPlugin):
+
     def __init__(self):
         super(BpmAnalyserPlugin, self).__init__()
         self.config.add({
             'auto': False,
             'dry-run': False,
             'write': True,
-            'threads': cpu_count(),
+            'threads': "AUTO",
             'force': False,
             'quiet': False
         })
 
         # On-import analysis.
         if self.config['auto']:
             self.import_stages = [self.imported]
```

### Comparing `beets-bpmanalyser-1.4.0/beetsplug/bpmanalyser/command.py` & `beets-bpmanalyser-1.4.1/beetsplug/bpmanalyser/command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 #  Copyright: Copyright (c) 2020., Adam Jakab
 #
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  Created: 2/23/20, 10:53 PM
 #  License: See LICENSE.txt
 
-import logging
 import os
 import sys
-from concurrent import futures
+import multiprocessing
+import json
+import logging
+import concurrent.futures as cf
+
 from optparse import OptionParser
-from subprocess import Popen, PIPE
+from subprocess import PIPE, Popen
 
 from beets.library import Library as BeatsLibrary, Item
 from beets.ui import Subcommand, decargs
 
 # Module methods
 log = logging.getLogger('beets.bpmanalyser')
 
+# Constants
+__FRAME_RATE__ = 44100
+
 
 class BpmAnalyserCommand(Subcommand):
     config = None
     lib = None
     query = None
     parser = None
 
     cfg_dry_run = False
     cfg_write = True
-    cfg_threads = 1
+    cfg_threads = "AUTO"
     cfg_force = False
     cfg_quiet = False
 
     analyser_script_path = None
 
+    #
+    # Initialize the plugin
+    #
     def __init__(self, cfg):
         self.config = cfg.flatten()
 
         self.cfg_dry_run = self.config.get("dry-run")
         self.cfg_write = self.config.get("write")
         self.cfg_threads = self.config.get("threads")
         self.cfg_force = self.config.get("force")
@@ -58,15 +67,15 @@
             help=u'[default: {}] write the bpm values to the media '
                  u'files'.format(
                 self.cfg_write)
         )
 
         self.parser.add_option(
             '-t', '--threads',
-            action='store', dest='threads', type='int',
+            action='store', dest='threads', type='string',
             default=self.cfg_threads,
             help=u'[default: {}] the number of threads to run in '
                  u'parallel'.format(
                 self.cfg_threads)
         )
 
         self.parser.add_option(
@@ -84,22 +93,32 @@
         )
 
         self.parser.add_option(
             '-v', '--version',
             action='store_true', dest='version', default=self.cfg_version,
             help=u'show plugin version'
         )
+        
+        # set up the analyser script path
+        module_path = os.path.dirname(__file__)
+        self.analyser_script_path = os.path.join(module_path, "analyser.py")
+        if not os.path.isfile(self.analyser_script_path):
+            raise FileNotFoundError("Analyser script not found!")
+        # log.debug("External analyser script path: {}".format(self.analyser_script_path))
 
         # Keep this at the end
         super(BpmAnalyserCommand, self).__init__(
             parser=self.parser,
             name='bpmanalyser',
             help=u'analyse your songs for tempo and write it into the bpm tag'
         )
 
+    #
+    # The main entry function for running the extension
+    #
     def func(self, lib: BeatsLibrary, options, arguments):
         self.cfg_dry_run = options.dryrun
         self.cfg_write = options.write
         self.cfg_threads = options.threads
         self.cfg_force = options.force
         self.cfg_version = options.version
         self.cfg_quiet = options.quiet
@@ -108,91 +127,105 @@
         self.query = decargs(arguments)
 
         if options.version:
             self.show_version_information()
             return
 
         self.analyse_songs()
-
-    def show_version_information(self):
-        from beetsplug.bpmanalyser.version import __version__
-        self._say(
-            "Bpm Analyser(beets-bpmanalyser) plugin for Beets: v{0}".format(
-                __version__))
-
-    def find_analyser_script(self):
-        module_path = os.path.dirname(__file__)
-        self.analyser_script_path = os.path.join(module_path, "get_song_bpm.py")
-        log.debug("External script path: {}".format(self.analyser_script_path))
-        if not os.path.isfile(self.analyser_script_path):
-            raise FileNotFoundError("Analyser script not found!")
-
-    def analyse(self, item: Item):
-        if not self.analyser_script_path:
-            self.find_analyser_script()
-
-        item_path = item.get("path").decode("utf-8")
-        log.debug("Analysing[{0}]...".format(item_path))
-
-        bpm, errors = self.get_bpm_from_analyser_script(item_path)
-
-        if bpm == 0:
-            self._say("Bpm[ERROR]: - {}".format(item_path))
-            # self._say("Bpm[ERROR]: - {}".format(errors))
-        else:
-            self._say("Bpm[{}]: {}".format(bpm, item_path))
-
-        if not self.cfg_dry_run:
-            if bpm != 0:
-                item['bpm'] = bpm
-                if self.cfg_write:
-                    item.try_write()
-                item.store()
-
+        
+        # Because of this pydub issue(https://github.com/jiaaro/pydub/issues/503) the below is necessary for now
+        # to regain console input (can also use reset) - not sure if Windows is affected
+        if os.name != 'nt':
+            os.system('stty echo')
+    
+    #
+    # Setup and trigger analysis
+    #
     def analyse_songs(self):
-        self.find_analyser_script()
+        # self.find_analyser_script()
 
         # Setup the query
         query = self.query
         if not self.cfg_force:
             query_element = "bpm:0"
             query.append(query_element)
 
         # Get the library items
-        # @todo: implement a limit option so that user can decide to do only
-        #  a limited number of items per run
+        # @TODO: implement a limit option so that user can decide to do only a limited number of items per run
         items = self.lib.items(self.query)
 
-        self.execute_on_items(items, self.analyse, msg='Analysing tempo...')
-
-    def get_bpm_from_analyser_script(self, item_path):
-        log.debug(
-            "calling external script: {}".format(self.analyser_script_path))
-
+        self.execute_task_on_items(items)
+    
+    #
+    # Pass all items to multithread Executor
+    #
+    def execute_task_on_items(self, items):
+        total = len(items)
+        taskRef = self.runAnalyser
+        finished = 0
+        
+        max_workers = 1
+        if str(self.cfg_threads).isnumeric():
+            max_workers = int(self.cfg_threads)
+        elif self.cfg_threads == "AUTO":
+            max_workers = round(multiprocessing.cpu_count() * 0.75)
+            
+        self._say("BpmAnalyser exec threads: {}".format(max_workers))
+        
+        # @TODO: create and show a progress bar (--progress-only option)
+        with cf.ThreadPoolExecutor(max_workers) as executor:
+            for result in executor.map(taskRef, items):
+                finished += 1
+            
+        self._say("Done.")
+    
+    def runAnalyser(self, item: Item):
+        item_path = item.get("path").decode("utf-8")
+        log.debug("Analysing[{0}]...".format(item_path))
+        
         proc = Popen([sys.executable, self.analyser_script_path, item_path],
                      stdout=PIPE, stderr=PIPE)
         stdout, stderr = proc.communicate()
 
+        # By default assume unknown error
+        error = True
+        message = "Unknown error!"
+        bpm = 0
+        
+        # On successful execution script should output a json
         try:
-            bpm = int(stdout.decode("utf-8"))
-            errors = ""
-        except ValueError:
-            bpm = 0
-            errors = stderr.decode()
-            if len(errors) > 0:
-                log.debug(errors)
-
-        return bpm, errors
-
-    def execute_on_items(self, items, func, msg=None):
-        total = len(items)
-        finished = 0
-        with futures.ThreadPoolExecutor(max_workers=self.cfg_threads) as e:
-            for _ in e.map(func, items):
-                finished += 1
-                # @create and show a progress bar (--progress-only option)
+            resp = json.loads(stdout)
+            error = resp["error"]
+            message = resp["message"]
+            bpm = resp["bpm"]
+        except Exception:
+            message = message + " Unparsable response."
+            
+        if (proc.returncode != 0 or error == True):
+            log.error("Error({}): {}".format(proc.returncode, message))
+            return False
+        
+        if bpm != 0:
+            if not self.cfg_dry_run:
+                item['bpm'] = bpm
+                if self.cfg_write:
+                    item.try_write()
+                item.store()
+                self._say("Bpm[{}]: {}".format(bpm, item_path))
+            else:
+                self._say("Bpm[DRY-MODE][{}]: {}".format(bpm, item_path))
+        else:
+            log.error("Error: bpm=0 was found. Not setting!")
 
+    # Plugin version Information
+    def show_version_information(self):
+        from beetsplug.bpmanalyser.version import __version__
+        self._say(
+            "Bpm Analyser(beets-bpmanalyser) plugin for Beets: v{0}".format(
+                __version__))
+    
+    # Say something (if not in quiet mode)
     def _say(self, msg):
         if not self.cfg_quiet:
             log.info(msg)
         else:
             log.debug(msg)
```

### Comparing `beets-bpmanalyser-1.4.0/setup.py` & `beets-bpmanalyser-1.4.1/setup.py`

 * *Files identical despite different names*

