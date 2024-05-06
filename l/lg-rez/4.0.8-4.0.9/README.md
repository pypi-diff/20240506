# Comparing `tmp/lg_rez-4.0.8.tar.gz` & `tmp/lg_rez-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lg_rez-4.0.8.tar", last modified: Tue Apr 30 17:24:35 2024, max compression
+gzip compressed data, was "lg_rez-4.0.9.tar", last modified: Sun May  5 19:36:15 2024, max compression
```

## Comparing `lg_rez-4.0.8.tar` & `lg_rez-4.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:24:35.316015 lg_rez-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-30 17:24:27.000000 lg_rez-4.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-30 17:24:35.316015 lg_rez-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-30 17:24:27.000000 lg_rez-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:24:35.316015 lg_rez-4.0.8/lg_rez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-30 17:24:35.000000 lg_rez-4.0.8/lg_rez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 17:24:35.000000 lg_rez-4.0.8/lg_rez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:24:35.000000 lg_rez-4.0.8/lg_rez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-30 17:24:35.000000 lg_rez-4.0.8/lg_rez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 17:24:35.000000 lg_rez-4.0.8/lg_rez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:24:35.312015 lg_rez-4.0.8/lgrez/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:24:35.312015 lg_rez-4.0.8/lgrez/bdd/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/model_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/model_ia.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/model_jeu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bdd/model_joueurs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:24:35.312015 lg_rez-4.0.8/lgrez/blocs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/journey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/realshell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    44961 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/blocs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:24:35.316015 lg_rez-4.0.8/lgrez/features/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/actions_publiques.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/annexe.py
--rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/chans.py
--rw-r--r--   0 runner    (1001) docker     (127)    22570 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/gestion_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23693 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/gestion_ia.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/informations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/inscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    27484 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/open_close.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/special.py
--rw-r--r--   0 runner    (1001) docker     (127)    33108 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/taches.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/features/voter_agir.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-30 17:24:27.000000 lg_rez-4.0.8/lgrez/server_structure.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:24:35.316015 lg_rez-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-30 17:24:27.000000 lg_rez-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:36:15.819198 lg_rez-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-05 19:36:07.000000 lg_rez-4.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-05 19:36:15.819198 lg_rez-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-05 19:36:07.000000 lg_rez-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:36:15.815198 lg_rez-4.0.9/lg_rez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-05 19:36:15.000000 lg_rez-4.0.9/lg_rez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-05 19:36:15.000000 lg_rez-4.0.9/lg_rez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:36:15.000000 lg_rez-4.0.9/lg_rez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-05 19:36:15.000000 lg_rez-4.0.9/lg_rez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 19:36:15.000000 lg_rez-4.0.9/lg_rez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:36:15.811198 lg_rez-4.0.9/lgrez/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:36:15.811198 lg_rez-4.0.9/lgrez/bdd/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/model_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/model_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/model_jeu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bdd/model_joueurs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:36:15.815198 lg_rez-4.0.9/lgrez/blocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/realshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44961 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/blocs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:36:15.815198 lg_rez-4.0.9/lgrez/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/actions_publiques.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/annexe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/chans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22570 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/gestion_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23693 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/gestion_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/informations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/inscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27484 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/open_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33108 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/taches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/features/voter_agir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-05 19:36:07.000000 lg_rez-4.0.9/lgrez/server_structure.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 19:36:15.819198 lg_rez-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-05 19:36:07.000000 lg_rez-4.0.9/setup.py
```

### Comparing `lg_rez-4.0.8/LICENSE` & `lg_rez-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/PKG-INFO` & `lg_rez-4.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-rez
-Version: 4.0.8
+Version: 4.0.9
 Summary: Discord bot for organizing Werewolf RP games ESPCI-style
 Home-page: https://github.com/GRI-ESPCI/lg-rez
 Author: Loïc Simon, Tom Lacoma
 Author-email: loic.simon@espci.org, tom.lacoma@espci.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -89,20 +89,20 @@
 
 
 ## NOTE AUX GRIS / MJS
 
 Tout ce qui suit est du blabla READMEsque peu intéressant.
 
 Pour les trucs intéressants, c'est-à-dire les instructions pour lancer une 
-nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/Nouvelle%20saison.md).
+nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/Nouvelle%20saison.md).
 
 
 ## What's New in LG-Rez
 
-Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/CHANGELOG.md)
+Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/CHANGELOG.md)
 or in [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/changelog.html) for
 details.
 
 # 3.0
 
 * Changed all commands to Discord builtin slash commands, using Discordpy 2.0
 * Several major commands changes
@@ -144,28 +144,28 @@
 We strongly recommand to install this package in a dedicated virtualenv
 (`python3 -m venv <yourfolder>`).
 
 
 ### Dependencies
 
 * Python 3.10+
-* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/requirements.txt)
+* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/requirements.txt)
 
 
 
 ## Configuration
 
 To run correctly, the bot needs to be connected to several external services,
 each needing more or less sensitive tokens, stocked as environments variables.
 We support and encourage the use of
 [`python-dotenv`](https://pypi.org/project/python-dotenv/) to read them from
 a `.env` file, but you may prefer exporting them as environment variables.
 
 All necessary variables, prefixed by `LGREZ_`, are listed in
-[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/model.env).
+[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/model.env).
 
 
 ### Configuration Assistant Tool
 
 We provide a command-line assistant tool to help you set up every services and
 generate the `.env` file (which you can later `source` and delete if you wish).
 
@@ -178,15 +178,15 @@
 needed to run the bot (see *Usage* section below).
 
 
 ### Manual configuration
 
 You may prefer to manually write your environment variables, or just check
 instructions regarding a specific one: they can be found in
-[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/CONFIGURE.md).
+[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/CONFIGURE.md).
 
 **Warning**: the Configuration Assistant Tool checks every variable by
 running specific tests, which is not the case for manual configuration,
 so be sure of what you do!
 
 
 
@@ -221,15 +221,15 @@
 
 Since `LGBot` is a subclass of
 [`discord.ext.commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#bot),
 you can use every arguments and methods it supports or subclass it to override
 existing behavior.
 
 We also provide a direct way to customize some parameters of the game and
-of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/lgrez/config.py) module:
+of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/lgrez/config.py) module:
 roles/channels/emoji names, date of season beginning, inscription
 customization... See
 [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/config.html)
 for full API usage information.
 
 See additional attributes and overriden methods on
 [the doc](https://lg-rez.readthedocs.io/) (mostly in French)
@@ -306,15 +306,15 @@
 
 Community contributions are not welcome for now. Get in touch with the authors
 (see below) for any question or suggestion about this project.
 
 
 
 ## License
-This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/LICENSE).
+This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/LICENSE).
 
 © 2020 - 2022 Loïc Simon, Tom Lacoma et al. – Club BD-Jeux × GRIs –
 ESPCI Paris - PSL
 
 Reach us on Discord:
 [LaCarpe#1674](https://discordapp.com/users/264482202966818825),
 [TaupeOrAfk#3218](https://discordapp.com/users/176763552202358785) or by mail: [loic.simon@espci.org](mailto:loic.simon@espci.org),
```

### Comparing `lg_rez-4.0.8/README.md` & `lg_rez-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lg_rez.egg-info/PKG-INFO` & `lg_rez-4.0.9/lg_rez.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-rez
-Version: 4.0.8
+Version: 4.0.9
 Summary: Discord bot for organizing Werewolf RP games ESPCI-style
 Home-page: https://github.com/GRI-ESPCI/lg-rez
 Author: Loïc Simon, Tom Lacoma
 Author-email: loic.simon@espci.org, tom.lacoma@espci.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -89,20 +89,20 @@
 
 
 ## NOTE AUX GRIS / MJS
 
 Tout ce qui suit est du blabla READMEsque peu intéressant.
 
 Pour les trucs intéressants, c'est-à-dire les instructions pour lancer une 
-nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/Nouvelle%20saison.md).
+nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/Nouvelle%20saison.md).
 
 
 ## What's New in LG-Rez
 
-Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/CHANGELOG.md)
+Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/CHANGELOG.md)
 or in [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/changelog.html) for
 details.
 
 # 3.0
 
 * Changed all commands to Discord builtin slash commands, using Discordpy 2.0
 * Several major commands changes
@@ -144,28 +144,28 @@
 We strongly recommand to install this package in a dedicated virtualenv
 (`python3 -m venv <yourfolder>`).
 
 
 ### Dependencies
 
 * Python 3.10+
-* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/requirements.txt)
+* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/requirements.txt)
 
 
 
 ## Configuration
 
 To run correctly, the bot needs to be connected to several external services,
 each needing more or less sensitive tokens, stocked as environments variables.
 We support and encourage the use of
 [`python-dotenv`](https://pypi.org/project/python-dotenv/) to read them from
 a `.env` file, but you may prefer exporting them as environment variables.
 
 All necessary variables, prefixed by `LGREZ_`, are listed in
-[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/model.env).
+[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/model.env).
 
 
 ### Configuration Assistant Tool
 
 We provide a command-line assistant tool to help you set up every services and
 generate the `.env` file (which you can later `source` and delete if you wish).
 
@@ -178,15 +178,15 @@
 needed to run the bot (see *Usage* section below).
 
 
 ### Manual configuration
 
 You may prefer to manually write your environment variables, or just check
 instructions regarding a specific one: they can be found in
-[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/CONFIGURE.md).
+[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/CONFIGURE.md).
 
 **Warning**: the Configuration Assistant Tool checks every variable by
 running specific tests, which is not the case for manual configuration,
 so be sure of what you do!
 
 
 
@@ -221,15 +221,15 @@
 
 Since `LGBot` is a subclass of
 [`discord.ext.commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#bot),
 you can use every arguments and methods it supports or subclass it to override
 existing behavior.
 
 We also provide a direct way to customize some parameters of the game and
-of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/lgrez/config.py) module:
+of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/lgrez/config.py) module:
 roles/channels/emoji names, date of season beginning, inscription
 customization... See
 [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/config.html)
 for full API usage information.
 
 See additional attributes and overriden methods on
 [the doc](https://lg-rez.readthedocs.io/) (mostly in French)
@@ -306,15 +306,15 @@
 
 Community contributions are not welcome for now. Get in touch with the authors
 (see below) for any question or suggestion about this project.
 
 
 
 ## License
-This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.8/LICENSE).
+This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.9/LICENSE).
 
 © 2020 - 2022 Loïc Simon, Tom Lacoma et al. – Club BD-Jeux × GRIs –
 ESPCI Paris - PSL
 
 Reach us on Discord:
 [LaCarpe#1674](https://discordapp.com/users/264482202966818825),
 [TaupeOrAfk#3218](https://discordapp.com/users/176763552202358785) or by mail: [loic.simon@espci.org](mailto:loic.simon@espci.org),
```

### Comparing `lg_rez-4.0.8/lg_rez.egg-info/SOURCES.txt` & `lg_rez-4.0.9/lg_rez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lg_rez.egg-info/requires.txt` & `lg_rez-4.0.9/lg_rez.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/__main__.py` & `lg_rez-4.0.9/lgrez/__main__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/__init__.py` & `lg_rez-4.0.9/lgrez/bdd/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/base.py` & `lg_rez-4.0.9/lgrez/bdd/base.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/enums.py` & `lg_rez-4.0.9/lgrez/bdd/enums.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/model_actions.py` & `lg_rez-4.0.9/lgrez/bdd/model_actions.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/model_ia.py` & `lg_rez-4.0.9/lgrez/bdd/model_ia.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/model_jeu.py` & `lg_rez-4.0.9/lgrez/bdd/model_jeu.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bdd/model_joueurs.py` & `lg_rez-4.0.9/lgrez/bdd/model_joueurs.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/__init__.py` & `lg_rez-4.0.9/lgrez/blocs/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/console.py` & `lg_rez-4.0.9/lgrez/blocs/console.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/env.py` & `lg_rez-4.0.9/lgrez/blocs/env.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/gsheets.py` & `lg_rez-4.0.9/lgrez/blocs/gsheets.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/journey.py` & `lg_rez-4.0.9/lgrez/blocs/journey.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/realshell.py` & `lg_rez-4.0.9/lgrez/blocs/realshell.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/structure.py` & `lg_rez-4.0.9/lgrez/blocs/structure.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/blocs/tools.py` & `lg_rez-4.0.9/lgrez/blocs/tools.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/bot.py` & `lg_rez-4.0.9/lgrez/bot.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/commands.py` & `lg_rez-4.0.9/lgrez/commands.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/config.py` & `lg_rez-4.0.9/lgrez/config.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/__init__.py` & `lg_rez-4.0.9/lgrez/features/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/actions_publiques.py` & `lg_rez-4.0.9/lgrez/features/actions_publiques.py`

 * *Files 11% similar despite different names*

```diff
@@ -281,8 +281,94 @@
     )
 
     haro = CandidHaro(joueur=joueur, type=CandidHaroType.haro, message_id=haro_message.id)
     
     if journey.channel != config.Channel.haros:
         await journey.send(f"Allez, c'est parti ! ({config.Channel.haros.mention})")
 
+@app_commands.command()
+@tools.mjs_only
+@journey_command
+async def haroparmj(journey: DiscordJourney, *, accusé: app_commands.Transform[Joueur, tools.VivantTransformer], accusant:app_commands.Transform[Joueur, tools.VivantTransformer]):
+    """Lance publiquement un haro contre la personne visée par la deuxième personne. (COMMANDE MJ)
+
+    Args:
+        joueur: Le joueur ou la joueuse à accuser de tous les maux.
+
+    Cette commande n'est utilisable que lorsqu'un vote pour le condamné est en cours.
+    """
+    await _haroparmj(journey, joueur=accusé, moi=accusant)
+
+
+
+async def _haroparmj(journey: DiscordJourney, joueur: Joueur, moi: Joueur):
+    try:
+        vaction = joueur.action_vote(Vote.cond)
+    except RuntimeError:
+        await journey.send(":x: Minute papillon, le jeu n'est pas encore lancé !")
+        return
+
+    if not vaction.is_open:
+        await journey.send(":x: Pas de vote pour le condamné du jour en cours !")
+        return
+
+    (motif,) = await journey.modal(
+        f"Haro contre {joueur.nom}",
+        discord.ui.TextInput(label="Quelle est la raison de cette haine ?", style=discord.TextStyle.paragraph),
+    )
+
+    emb = discord.Embed(
+        title=(f"**{config.Emoji.ha}{config.Emoji.ro} contre {joueur.nom} !**"),
+        description=f"**« {motif} »\n**",
+        color=0xFF0000,
+    )
+    emb.set_author(name=f"{moi.nom} en a gros 😡😡")
+    emb.set_thumbnail(url=config.Emoji.bucher.url)
+
+    await journey.ok_cancel("C'est tout bon ?", embed=emb)
+
+    class _HaroView(discord.ui.View):
+        @discord.ui.button(
+            label=f"Voter contre {joueur.nom}"[:80], style=discord.ButtonStyle.primary, emoji=config.Emoji.bucher
+        )
+        async def vote(self, vote_interaction: discord.Interaction, button: discord.ui.Button):
+            async with DiscordJourney(vote_interaction, ephemeral=True) as vote_journey:
+                try:
+                    votant = Joueur.from_member(vote_journey.member)
+                except ValueError:
+                    await vote_journey.send(":x: Tu n'as pas le droit de vote, toi")
+                    return
+                await do_vote(vote_journey, Vote.cond, votant=votant, cible=joueur)
+
+        @discord.ui.button(label=f"Voter contre {moi.nom}", style=discord.ButtonStyle.danger, emoji=config.Emoji.ha)
+        async def vote2(self, vote2_interaction: discord.Interaction, button: discord.ui.Button):
+            async with DiscordJourney(vote2_interaction, ephemeral=True) as vote2_journey:
+                try:
+                    votant = Joueur.from_member(vote2_journey.member)
+                except ValueError:
+                    await vote_journey.send(":x: Tu n'as pas le droit de vote, toi")
+                    return
+                await do_vote(vote2_journey, Vote.cond, votant=votant, cible=moi)
+
+        async def on_error(self, _interaction: discord.Interaction, error: Exception, _item: discord.ui.Item) -> None:
+            raise error
+
+    haro_message = await config.Channel.haros.send(
+        f"(Psst, {joueur.member.mention} :3)", embed=emb, view=_HaroView(timeout=None)
+    )
+    await config.Channel.debats.send(
+        f"{config.Emoji.ha}{config.Emoji.ro} de {moi.member.mention} sur {joueur.member.mention} ! "
+        f"Vous en pensez quoi vous? (détails sur {config.Channel.haros.mention})"
+    )
+
+    haro = CandidHaro(joueur=joueur, type=CandidHaroType.haro, message_id=haro_message.id)
+    contre_haro = CandidHaro(joueur=moi, type=CandidHaroType.haro)
+    CandidHaro.add(haro, contre_haro)
+
+    if journey.channel != config.Channel.haros:
+        await journey.send(f"Allez, c'est parti ! ({config.Channel.haros.mention})")
+
+
+
+
+
```

### Comparing `lg_rez-4.0.8/lgrez/features/annexe.py` & `lg_rez-4.0.9/lgrez/features/annexe.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/chans.py` & `lg_rez-4.0.9/lgrez/features/chans.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/communication.py` & `lg_rez-4.0.9/lgrez/features/communication.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/gestion_actions.py` & `lg_rez-4.0.9/lgrez/features/gestion_actions.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/gestion_ia.py` & `lg_rez-4.0.9/lgrez/features/gestion_ia.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/informations.py` & `lg_rez-4.0.9/lgrez/features/informations.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/inscription.py` & `lg_rez-4.0.9/lgrez/features/inscription.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/open_close.py` & `lg_rez-4.0.9/lgrez/features/open_close.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/special.py` & `lg_rez-4.0.9/lgrez/features/special.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/sync.py` & `lg_rez-4.0.9/lgrez/features/sync.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/taches.py` & `lg_rez-4.0.9/lgrez/features/taches.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/features/voter_agir.py` & `lg_rez-4.0.9/lgrez/features/voter_agir.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/lgrez/server_structure.json` & `lg_rez-4.0.9/lgrez/server_structure.json`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.8/setup.py` & `lg_rez-4.0.9/setup.py`

 * *Files identical despite different names*

