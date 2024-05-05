# Comparing `tmp/robotframework-flaui-3.0.3.tar.gz` & `tmp/robotframework_flaui-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-flaui-3.0.3.tar", last modified: Sun Apr  7 17:06:55 2024, max compression
+gzip compressed data, was "robotframework_flaui-3.1.0.tar", last modified: Sun May  5 22:53:36 2024, max compression
```

## Comparing `robotframework-flaui-3.0.3.tar` & `robotframework_flaui-3.1.0.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/
--rw-rw-rw-   0        0        0     1079 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/LICENSE
--rw-rw-rw-   0        0        0       40 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8998 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7921 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/README.md
--rw-rw-rw-   0        0        0       81 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      103 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/
--rw-rw-rw-   0        0        0     8998 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3054 2024-04-07 17:06:55.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-07 17:06:54.000000 robotframework-flaui-3.0.3/robotframework_flaui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1988 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.021331 robotframework-flaui-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/
--rw-rw-rw-   0        0        0     8747 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/
--rw-rw-rw-   0        0        0   256512 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.Core.dll
--rw-rw-rw-   0        0        0    76288 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA2.dll
--rw-rw-rw-   0        0        0   105984 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA3.dll
--rw-rw-rw-   0        0        0   151040 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/
--rw-rw-rw-   0        0        0       46 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/__init__.py
--rw-rw-rw-   0        0        0     5479 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia.py
--rw-rw-rw-   0        0        0     1062 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia2.py
--rw-rw-rw-   0        0        0     1062 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia3.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.052586 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/
--rw-rw-rw-   0        0        0      127 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/__init__.py
--rw-rw-rw-   0        0        0      305 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/interfacetype.py
--rw-rw-rw-   0        0        0      163 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/screenshotmode.py
--rw-rw-rw-   0        0        0      229 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/enum/treeitemaction.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.068210 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/
--rw-rw-rw-   0        0        0       36 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/__init__.py
--rw-rw-rw-   0        0        0     3268 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/flauierror.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.068210 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/
--rw-rw-rw-   0        0        0      158 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/__init__.py
--rw-rw-rw-   0        0        0      737 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/moduleinterface.py
--rw-rw-rw-   0        0        0      248 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/valuecontainer.py
--rw-rw-rw-   0        0        0     1289 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.083830 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/
--rw-rw-rw-   0        0        0      484 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/__init__.py
--rw-rw-rw-   0        0        0    12745 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/application.py
--rw-rw-rw-   0        0        0     2512 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/checkbox.py
--rw-rw-rw-   0        0        0     2146 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/combobox.py
--rw-rw-rw-   0        0        0     2179 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/debug.py
--rw-rw-rw-   0        0        0    18162 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/element.py
--rw-rw-rw-   0        0        0     7948 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/grid.py
--rw-rw-rw-   0        0        0     7598 2024-04-07 17:06:06.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/keyboard.py
--rw-rw-rw-   0        0        0    17116 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/mouse.py
--rw-rw-rw-   0        0        0    18010 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/property.py
--rw-rw-rw-   0        0        0     8595 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/screenshot.py
--rw-rw-rw-   0        0        0     9645 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/selector.py
--rw-rw-rw-   0        0        0     3224 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tab.py
--rw-rw-rw-   0        0        0     2613 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/textbox.py
--rw-rw-rw-   0        0        0     1698 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tooglebutton.py
--rw-rw-rw-   0        0        0     6756 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tree.py
--rw-rw-rw-   0        0        0     1925 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/window.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.083830 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/
--rw-rw-rw-   0        0        0      262 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/__init__.py
--rw-rw-rw-   0        0        0     1183 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationelement.py
--rw-rw-rw-   0        0        0     1103 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationinterfacecontainer.py
--rw-rw-rw-   0        0        0     2101 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/converter.py
--rw-rw-rw-   0        0        0     7532 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/keyboardinputconverter.py
--rw-rw-rw-   0        0        0     5617 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitems.py
--rw-rw-rw-   0        0        0     1825 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitemsparser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.099455 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/
--rw-rw-rw-   0        0        0      668 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0    10568 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/application.py
--rw-rw-rw-   0        0        0     2643 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/checkbox.py
--rw-rw-rw-   0        0        0    10343 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/combobox.py
--rw-rw-rw-   0        0        0     2473 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/debug.py
--rw-rw-rw-   0        0        0    17790 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/element.py
--rw-rw-rw-   0        0        0     6805 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/grid.py
--rw-rw-rw-   0        0        0    10868 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/keyboard.py
--rw-rw-rw-   0        0        0     8242 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/listbox.py
--rw-rw-rw-   0        0        0    22978 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/mouse.py
--rw-rw-rw-   0        0        0    33400 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/property.py
--rw-rw-rw-   0        0        0     2692 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/radiobutton.py
--rw-rw-rw-   0        0        0     4427 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/screenshot.py
--rw-rw-rw-   0        0        0     2532 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tab.py
--rw-rw-rw-   0        0        0     2527 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/textbox.py
--rw-rw-rw-   0        0        0     1505 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/togglebutton.py
--rw-rw-rw-   0        0        0    14122 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tree.py
--rw-rw-rw-   0        0        0     1247 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/uia.py
--rw-rw-rw-   0        0        0     1357 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/window.py
--rw-rw-rw-   0        0        0      838 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/pythonnetwrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-07 17:06:55.115080 robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/robotlog.py
--rw-rw-rw-   0        0        0       18 2024-04-07 17:06:07.000000 robotframework-flaui-3.0.3/src/FlaUILibrary/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.794663 robotframework_flaui-3.1.0/
+-rw-rw-rw-   0        0        0     1079 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0       40 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9070 2024-05-05 22:53:36.794663 robotframework_flaui-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7993 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/README.md
+-rw-rw-rw-   0        0        0       81 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      103 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.794663 robotframework_flaui-3.1.0/robotframework_flaui.egg-info/
+-rw-rw-rw-   0        0        0     9070 2024-05-05 22:53:36.000000 robotframework_flaui-3.1.0/robotframework_flaui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2024-05-05 22:53:36.000000 robotframework_flaui-3.1.0/robotframework_flaui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 22:53:36.000000 robotframework_flaui-3.1.0/robotframework_flaui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-05 22:53:36.000000 robotframework_flaui-3.1.0/robotframework_flaui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 22:53:36.000000 robotframework_flaui-3.1.0/robotframework_flaui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 22:53:36.794663 robotframework_flaui-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1988 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.700937 robotframework_flaui-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.732164 robotframework_flaui-3.1.0/src/FlaUILibrary/
+-rw-rw-rw-   0        0        0     7722 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.732164 robotframework_flaui-3.1.0/src/FlaUILibrary/bin/
+-rw-rw-rw-   0        0        0   256512 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/bin/FlaUI.Core.dll
+-rw-rw-rw-   0        0        0    76288 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/bin/FlaUI.UIA2.dll
+-rw-rw-rw-   0        0        0   105984 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/bin/FlaUI.UIA3.dll
+-rw-rw-rw-   0        0        0   151040 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.732164 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/
+-rw-rw-rw-   0        0        0        0 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.732164 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/
+-rw-rw-rw-   0        0        0       46 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/__init__.py
+-rw-rw-rw-   0        0        0     5479 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/uia.py
+-rw-rw-rw-   0        0        0     1062 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/uia2.py
+-rw-rw-rw-   0        0        0     1062 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/uia3.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.732164 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/enum/
+-rw-rw-rw-   0        0        0       84 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/enum/__init__.py
+-rw-rw-rw-   0        0        0      305 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/enum/interfacetype.py
+-rw-rw-rw-   0        0        0      229 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/enum/treeitemaction.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.747790 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/exception/
+-rw-rw-rw-   0        0        0       36 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/exception/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/exception/flauierror.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.747790 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/
+-rw-rw-rw-   0        0        0      158 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/__init__.py
+-rw-rw-rw-   0        0        0      737 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/moduleinterface.py
+-rw-rw-rw-   0        0        0      248 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/valuecontainer.py
+-rw-rw-rw-   0        0        0     1289 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.763417 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/
+-rw-rw-rw-   0        0        0      484 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/__init__.py
+-rw-rw-rw-   0        0        0    12745 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/application.py
+-rw-rw-rw-   0        0        0     2512 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/checkbox.py
+-rw-rw-rw-   0        0        0     2146 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/combobox.py
+-rw-rw-rw-   0        0        0     2179 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/debug.py
+-rw-rw-rw-   0        0        0    18303 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/element.py
+-rw-rw-rw-   0        0        0     8008 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/grid.py
+-rw-rw-rw-   0        0        0     7570 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/keyboard.py
+-rw-rw-rw-   0        0        0    17141 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/mouse.py
+-rw-rw-rw-   0        0        0    14335 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/property.py
+-rw-rw-rw-   0        0        0     4250 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/screenshot.py
+-rw-rw-rw-   0        0        0     9548 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/selector.py
+-rw-rw-rw-   0        0        0     3224 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/tab.py
+-rw-rw-rw-   0        0        0     2613 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/textbox.py
+-rw-rw-rw-   0        0        0     1698 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/tooglebutton.py
+-rw-rw-rw-   0        0        0     6756 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/tree.py
+-rw-rw-rw-   0        0        0     1925 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/window.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.779040 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/
+-rw-rw-rw-   0        0        0      262 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/__init__.py
+-rw-rw-rw-   0        0        0     1246 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/automationelement.py
+-rw-rw-rw-   0        0        0     1610 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/automationinterfacecontainer.py
+-rw-rw-rw-   0        0        0     2957 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/converter.py
+-rw-rw-rw-   0        0        0     7532 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/keyboardinputconverter.py
+-rw-rw-rw-   0        0        0     5617 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/treeitems.py
+-rw-rw-rw-   0        0        0     1825 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/treeitemsparser.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.794663 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/
+-rw-rw-rw-   0        0        0      668 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0    10568 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/application.py
+-rw-rw-rw-   0        0        0     2643 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    10343 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/combobox.py
+-rw-rw-rw-   0        0        0     2473 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/debug.py
+-rw-rw-rw-   0        0        0    17790 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/element.py
+-rw-rw-rw-   0        0        0     6805 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/grid.py
+-rw-rw-rw-   0        0        0    10863 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/keyboard.py
+-rw-rw-rw-   0        0        0     8242 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/listbox.py
+-rw-rw-rw-   0        0        0    25216 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/mouse.py
+-rw-rw-rw-   0        0        0    33503 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/property.py
+-rw-rw-rw-   0        0        0     2692 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/radiobutton.py
+-rw-rw-rw-   0        0        0     2176 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     2532 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/tab.py
+-rw-rw-rw-   0        0        0     2527 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/textbox.py
+-rw-rw-rw-   0        0        0     1505 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/togglebutton.py
+-rw-rw-rw-   0        0        0    14122 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/tree.py
+-rw-rw-rw-   0        0        0     1239 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/uia.py
+-rw-rw-rw-   0        0        0     1357 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/window.py
+-rw-rw-rw-   0        0        0      838 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/pythonnetwrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:53:36.794663 robotframework_flaui-3.1.0/src/FlaUILibrary/robotframework/
+-rw-rw-rw-   0        0        0        0 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/robotframework/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/robotframework/robotlog.py
+-rw-rw-rw-   0        0        0       18 2024-05-05 22:52:52.000000 robotframework_flaui-3.1.0/src/FlaUILibrary/version.py
```

### Comparing `robotframework-flaui-3.0.3/LICENSE` & `robotframework_flaui-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/PKG-INFO` & `robotframework_flaui-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-flaui
-Version: 3.0.3
+Version: 3.1.0
 Summary: Windows GUI testing library for Robot Framework
 Home-page: https://github.com/GDATASoftwareAG/robotframework-flaui
 Author: G DATA CyberDefense AG
 Author-email: opensource@gdata.de
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
@@ -186,15 +186,17 @@
   * cleanup - Removes all build folders
   * dependency - Install all python dependencies
   * build - Build wheel file
   * install - Install wheel file
   * test - Test robotframework-flaui (UIA2 and UIA3)
   * test_uia2 - Test UIA2 interface usage
   * test_uia3 - Test UIA3 interface usage
-  * pylint - Static code analysis for PEP 8. Generates pylint.html file in results.
+  * pylint - Static code analysis for python code
+  * robocop - Static code analysis for robotframework code
+  * tidy - Formatter for robotframework code
 
 ## Acknowledgements
 
 ### FlaUI
 
 * Thanks to [@Roemer](https://github.com/Roemer) for the passion to create and maintain the FlaUI project.
 * Thanks to [FlaUI](https://github.com/FlaUI/FlaUI) developers and maintainers for this project.
```

### Comparing `robotframework-flaui-3.0.3/README.md` & `robotframework_flaui-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,17 @@
   * cleanup - Removes all build folders
   * dependency - Install all python dependencies
   * build - Build wheel file
   * install - Install wheel file
   * test - Test robotframework-flaui (UIA2 and UIA3)
   * test_uia2 - Test UIA2 interface usage
   * test_uia3 - Test UIA3 interface usage
-  * pylint - Static code analysis for PEP 8. Generates pylint.html file in results.
+  * pylint - Static code analysis for python code
+  * robocop - Static code analysis for robotframework code
+  * tidy - Formatter for robotframework code
 
 ## Acknowledgements
 
 ### FlaUI
 
 * Thanks to [@Roemer](https://github.com/Roemer) for the passion to create and maintain the FlaUI project.
 * Thanks to [FlaUI](https://github.com/FlaUI/FlaUI) developers and maintainers for this project.
```

### Comparing `robotframework-flaui-3.0.3/robotframework_flaui.egg-info/PKG-INFO` & `robotframework_flaui-3.1.0/robotframework_flaui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-flaui
-Version: 3.0.3
+Version: 3.1.0
 Summary: Windows GUI testing library for Robot Framework
 Home-page: https://github.com/GDATASoftwareAG/robotframework-flaui
 Author: G DATA CyberDefense AG
 Author-email: opensource@gdata.de
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
@@ -186,15 +186,17 @@
   * cleanup - Removes all build folders
   * dependency - Install all python dependencies
   * build - Build wheel file
   * install - Install wheel file
   * test - Test robotframework-flaui (UIA2 and UIA3)
   * test_uia2 - Test UIA2 interface usage
   * test_uia3 - Test UIA3 interface usage
-  * pylint - Static code analysis for PEP 8. Generates pylint.html file in results.
+  * pylint - Static code analysis for python code
+  * robocop - Static code analysis for robotframework code
+  * tidy - Formatter for robotframework code
 
 ## Acknowledgements
 
 ### FlaUI
 
 * Thanks to [@Roemer](https://github.com/Roemer) for the passion to create and maintain the FlaUI project.
 * Thanks to [FlaUI](https://github.com/FlaUI/FlaUI) developers and maintainers for this project.
```

### Comparing `robotframework-flaui-3.0.3/robotframework_flaui.egg-info/SOURCES.txt` & `robotframework_flaui-3.1.0/robotframework_flaui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 src/FlaUILibrary/flaui/__init__.py
 src/FlaUILibrary/flaui/automation/__init__.py
 src/FlaUILibrary/flaui/automation/uia.py
 src/FlaUILibrary/flaui/automation/uia2.py
 src/FlaUILibrary/flaui/automation/uia3.py
 src/FlaUILibrary/flaui/enum/__init__.py
 src/FlaUILibrary/flaui/enum/interfacetype.py
-src/FlaUILibrary/flaui/enum/screenshotmode.py
 src/FlaUILibrary/flaui/enum/treeitemaction.py
 src/FlaUILibrary/flaui/exception/__init__.py
 src/FlaUILibrary/flaui/exception/flauierror.py
 src/FlaUILibrary/flaui/interface/__init__.py
 src/FlaUILibrary/flaui/interface/moduleinterface.py
 src/FlaUILibrary/flaui/interface/valuecontainer.py
 src/FlaUILibrary/flaui/interface/windowsautomationinterface.py
```

### Comparing `robotframework-flaui-3.0.3/setup.py` & `robotframework_flaui-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/__init__.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # pylint: disable=invalid-name
 from enum import Enum
 from robot.libraries.BuiltIn import BuiltIn
 from robotlibcore import DynamicCore
 from FlaUILibrary import version, pythonnetwrapper
-from FlaUILibrary.flaui.enum import ScreenshotMode
 from FlaUILibrary.keywords import (ApplicationKeywords,
                                    CheckBoxKeywords,
                                    ComboBoxKeywords,
                                    DebugKeywords,
                                    ElementKeywords,
                                    MouseKeywords,
                                    KeyboardKeywords,
@@ -111,24 +110,23 @@
         ``timeout`` maximum amount of waiting time in ms for an element find action. Default value is 1000ms.
 
         If the given directory does not already exist, it will be created when the first screenshot is taken.
         If the argument is not given, the default location for screenshots is the output directory of the Robot run,
         i.e. the directory where output and log files are generated.
         """
         # FlaUI init
-        self.mode = FlaUILibrary.RobotMode.TEST_NOT_RUNNING
         self.builtin = BuiltIn()
 
         try:
             if timeout == "None" or int(timeout) <= 0:
                 timeout = 0
         except ValueError:
             timeout = 1000
 
-        if uia != "UIA2" and uia != "UIA3":
+        if uia not in ("UIA2", "UIA3"):
             uia = "UIA3"
 
         self.container = AutomationInterfaceContainer(timeout, uia)
 
         self.screenshots = Screenshot(screenshot_dir, screenshot_on_failure == 'True')
 
         self.keyword_modules = {
@@ -154,35 +152,17 @@
 
         # Robot init
         self.ROBOT_LIBRARY_LISTENER = self  # pylint: disable=invalid-name
         self.libraries = list(self.keyword_modules.values())
         DynamicCore.__init__(self, self.libraries)
 
     def _start_test(self, name, attrs):  # pylint: disable=unused-argument
-        self.mode = FlaUILibrary.RobotMode.TEST_RUNNING
-        self.screenshots.name = name.replace(" ", "_").lower()
-        self.screenshots.execute_action(Screenshot.Action.RESET,
-                                        Screenshot.create_value_container())
-
-    def _end_test(self, name, attrs):  # pylint: disable=unused-argument
-        self.mode = FlaUILibrary.RobotMode.TEST_NOT_RUNNING
-        if attrs['status'] == 'PASS' and self.screenshots.is_enabled:
-            if not self.screenshots.execute_action(Screenshot.Action.DELETE_ALL_SCREENSHOTS,
-                                                   Screenshot.create_value_container()):
-                robotlog.log("Not all files were deleted")
+        self.screenshots.set_name(name)
+        self.screenshots.img_counter = 1
 
     def _end_keyword(self, name, attrs):  # pylint: disable=unused-argument
-        if name in self.screenshots.blacklist:
-            # Keyword in blacklist do not screenshot anything
-            return
-
         if attrs['status'] == 'FAIL' \
-                and self.mode == FlaUILibrary.RobotMode.TEST_RUNNING \
-                and self.screenshots.is_enabled:
-
-            mode = ScreenshotMode.TEMP
-
-            if name in self.screenshots.whitelist:
-                mode = ScreenshotMode.PERSIST
+                and self.screenshots.is_enabled \
+                and attrs['libname'] == "FlaUILibrary":
 
             self.screenshots.execute_action(Screenshot.Action.CAPTURE,
-                                            Screenshot.create_value_container(mode))
+                                            Screenshot.create_value_container())
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.Core.dll` & `robotframework_flaui-3.1.0/src/FlaUILibrary/bin/FlaUI.Core.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA2.dll` & `robotframework_flaui-3.1.0/src/FlaUILibrary/bin/FlaUI.UIA2.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/FlaUI.UIA3.dll` & `robotframework_flaui-3.1.0/src/FlaUILibrary/bin/FlaUI.UIA3.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll` & `robotframework_flaui-3.1.0/src/FlaUILibrary/bin/Interop.UIAutomationClient.dll`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/uia.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia2.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/uia2.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/automation/uia3.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/automation/uia3.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/exception/flauierror.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/exception/flauierror.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/moduleinterface.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/moduleinterface.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/interface/windowsautomationinterface.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/application.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/application.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/checkbox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/checkbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/combobox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/combobox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/debug.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/element.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from enum import Enum
-from typing import Optional, Any
+from typing import Optional, Any, Union
 from System import Exception as CSharpException  # pylint: disable=import-error
 from System import InvalidOperationException # pylint: disable=import-error
 from FlaUI.Core import Debug as FlaUIDebug  # pylint: disable=import-error
 from FlaUI.Core.Exceptions import PropertyNotSupportedException  # pylint: disable=import-error
 from FlaUILibrary.flaui.util.converter import Converter
 from FlaUILibrary.flaui.exception import FlaUiError
 from FlaUILibrary.flaui.interface import (ModuleInterface, ValueContainer)
@@ -17,15 +17,15 @@
     Wrapper module executes methods from AutomationElement.cs implementation.
     """
 
     class Container(ValueContainer):
         """
         Value container from element module.
         """
-        xpath: Optional[str]
+        xpath: Union[str, AutomationElement]
         name: Optional[str]
         use_exception: Optional[bool]
         retries: Optional[int]
 
     class Action(Enum):
         """
         Supported actions for execute action implementation.
@@ -42,15 +42,15 @@
         NAME_SHOULD_CONTAINS = "NAME_SHOULD_CONTAINS"
         ELEMENT_SHOULD_EXIST = "ELEMENT_SHOULD_EXIST"
         ELEMENT_SHOULD_NOT_EXIST = "ELEMENT_SHOULD_NOT_EXIST"
         ELEMENT_SHOULD_BE_ENABLED = "ELEMENT_SHOULD_BE_ENABLED"
         ELEMENT_SHOULD_BE_DISABLED = "ELEMENT_SHOULD_BE_DISABLED"
         WAIT_UNTIL_ELEMENT_IS_OFFSCREEN = "WAIT_UNTIL_ELEMENT_IS_OFFSCREEN"
         WAIT_UNTIL_ELEMENT_IS_ENABLED = "WAIT_UNTIL_ELEMENT_IS_ENABLED"
-        WAIT_UNTIl_ELEMENT_EXIST = "WAIT_UNTIl_ELEMENT_EXIST"
+        WAIT_UNTIL_ELEMENT_EXIST = "WAIT_UNTIL_ELEMENT_EXIST"
         WAIT_UNTIL_ELEMENT_DOES_NOT_EXIST = "WAIT_UNTIL_ELEMENT_DOES_NOT_EXIST"
 
     def __init__(self, automation: Any, timeout: int = 1000):
         """
         Element module wrapper for FlaUI usage.
 
         Args:
@@ -67,21 +67,21 @@
         Helper to create container object.
 
         Raises:
             FlaUiError: If creation from container object failed by invalid values.
 
         Args:
             name (String): Name from element
-            xpath (String): Searched element as xpath
+            xpath (String | AutomationElement): Searched element as xpath from string or AutomationElement
             retries (Number): Retry counter to repeat calls as number
             use_exception (Bool) : Indicator to ignore exception handling by Flaui
             msg (String): Optional error message
         """
         return Element.Container(name=Converter.cast_to_string(name),
-                                 xpath=Converter.cast_to_string(xpath),
+                                 xpath=Converter.cast_to_xpath_string(xpath),
                                  use_exception=Converter.cast_to_bool(use_exception),
                                  retries=Converter.cast_to_int(retries, msg))
 
     def execute_action(self, action: Action, values: Container):
         """
         If action is not supported an ActionNotSupported error will be raised.
         """
@@ -116,15 +116,15 @@
                 lambda: self._element_should_not_exist(values["xpath"], values["use_exception"]),
             self.Action.WAIT_UNTIL_ELEMENT_IS_OFFSCREEN:
                 lambda: self._wait_until_element_is_offscreen(values["xpath"], values["retries"]),
             self.Action.WAIT_UNTIL_ELEMENT_IS_ENABLED:
                 lambda: self._wait_until_element_is_enabled(values["xpath"], values["retries"]),
             self.Action.FIND_ALL_ELEMENTS:
                 lambda: self._find_all_elements(values["xpath"]),
-            self.Action.WAIT_UNTIl_ELEMENT_EXIST:
+            self.Action.WAIT_UNTIL_ELEMENT_EXIST:
                 lambda: self._wait_until_element_exist(values["xpath"], values["retries"]),
             self.Action.WAIT_UNTIL_ELEMENT_DOES_NOT_EXIST:
                 lambda: self._wait_until_element_does_not_exist(values["xpath"], values["retries"])
         }
 
         return switcher.get(action, lambda: FlaUiError.raise_fla_ui_error(FlaUiError.ActionNotSupported))()
 
@@ -213,22 +213,27 @@
 
         except CSharpException:
             raise FlaUiError(FlaUiError.XPathNotFound.format(xpath)) from None
 
     def _get_element_by_xpath(self, xpath: str):
         """
         Try to get element from xpath by desktop.
-        Different from self._get_element, it is abstracted from timeout and error handling.
 
         Args:
             xpath (string): XPath identifier from element.
         """
         return self._automation.GetDesktop().FindFirstByXPath(xpath)
 
     def _find_all_elements(self, xpath: str):
+        """
+        Try to find all elements from xpath by desktop.
+
+        Args:
+            xpath (string): XPath identifier from element.
+        """
         values = []
         elements = self._get_all_elements_by_xpath(xpath)
         for element in elements:
             values.append(AutomationElement(
                 self._try_get_automation_id_property(element),
                 self._try_get_name_property(element),
                 self._try_get_classname_property(element),
@@ -468,15 +473,15 @@
             FlaUiError: If the given element is not focusable.
         """
         element = self._get_element(xpath)
         try:
             element.Focus()
         except InvalidOperationException:
             raise FlaUiError(FlaUiError.ElementNotFocusable.format(xpath)) from None
-        
+
     @staticmethod
     def _try_get_automation_id_property(element):
         """
         Try to get automation id property from element. Return empty string if failed.
 
         Args:
             element (UIA): AutomationElement.
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/grid.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,39 +65,41 @@
             action (Action): Action to use.
             values (Object): Specific value for action if needed.
 
         """
 
         switcher = {
             self.Action.GET_ROW_COUNT: lambda: values["element"].RowCount,
-            self.Action.SELECT_ROW_BY_INDEX: lambda: self._select_row_by_index(values["element"], 
-                                                                               values["index"], 
+            self.Action.SELECT_ROW_BY_INDEX: lambda: self._select_row_by_index(values["element"],
+                                                                               values["index"],
                                                                                values["multiselect"]),
             self.Action.SELECT_ROW_BY_NAME: lambda: self._select_row_by_name(values["element"],
                                                                              values["index"],
-                                                                             values["name"], 
+                                                                             values["name"],
                                                                              values["multiselect"]),
             self.Action.GET_SELECTED_ROWS: lambda: self._get_selected_rows(values["element"]),
             self.Action.GET_ALL_DATA: lambda: self._get_all_data(values["element"]),
             self.Action.GET_HEADER: lambda: self._get_header(values["element"]),
         }
 
         return switcher.get(action, lambda: FlaUiError.raise_fla_ui_error(FlaUiError.ActionNotSupported))()
 
     @staticmethod
     def _get_all_data(control: Any):
+        # pylint: disable=C0301
         """
         Try to get all rows as string.
 
         Args:
             control (Object): List view to select items.
 
         Returns:
             String array of header and columns as texts [[header1, header2, ...], [row1column1, row1column2, ...], [row2column1, row2column2, ...] ...] 
         """
+        # pylint: enable=C0301
         values = []
         data = []
 
         for column in control.Header.Columns:
             data.append(column.Text)
 
         values.append(data)
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/keyboard.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/keyboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,37 +121,38 @@
         Args:
             key_shortcuts (VirtualKeyShort array): Array from VirtualKeyShort usage to execute keyboard actions.
         """
         for key in key_shorts:
             FlaUIKeyboard.Release(key)
 
     @staticmethod
-    def _type_key_combination(key_combination: Any, delay_in_ms: Any, 
+    def _type_key_combination(key_combination: Any, delay_in_ms: Any,
                               press_only: bool, release_only: bool):
         """
         Execution of key control. 
         press_only and release_only supports keys only, not text.
 
         Args:
             key_combination (String): Array from String to execute keyboard actions or send input data.
             delay_in_ms (Number): Delay in ms to wait until key was pressed
             press_only (Bool): Press key only without releasing
             release_only (Bool): Release key only without pressing
         """
         if isinstance(key_combination, list):
             raise FlaUiError(FlaUiError.ArgumentShouldNotBeList)
         try:
-            (action, converting_result) = KeyboardInputConverter.convert_key_combination(key_combination)
+            action, converting_result = KeyboardInputConverter.convert_key_combination(key_combination)
+
             if action == KeyboardInputConverter.InputType.TEXT:
                 if press_only or release_only:
                     raise FlaUiError(
                         FlaUiError.PatternNotSupported.format(" s'SOMEKEY' ") + \
                             " for key press_only and release_only events")
-                else:
-                    Keyboard._type_text(converting_result)
+
+                Keyboard._type_text(converting_result)
             elif action == KeyboardInputConverter.InputType.SHORTCUT:
                 if press_only:
                     Keyboard._press_keys(converting_result)
                 elif release_only:
                     Keyboard._release_keys(converting_result)
                 else:
                     Keyboard._type_keys(converting_result)
@@ -175,12 +176,12 @@
             release_only (Bool): Release key only without pressing
         """
         if not isinstance(keys_combination, list):
             raise FlaUiError(FlaUiError.ArgumentShouldBeList)
         try:
             for key_combination in keys_combination:
                 Keyboard._type_key_combination(key_combination, delay_in_ms,
-                                               press_only=press_only, 
+                                               press_only=press_only,
                                                release_only=release_only
                                                )
         except Exception as ex:
             raise FlaUiError.raise_fla_ui_error(str(ex))
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/mouse.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/mouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,28 +56,30 @@
         DRAG_AND_DROP = "DRAG_AND_DROP"
 
     @staticmethod
     def create_value_container(element=None, second_element=None, timeout_in_ms=None, max_repeat=None,
                                click_element_xpath=None, goal_element_xpath=None,
                                focus_element_xpath_before=None, focus_element_xpath_after=None,
                                ignore_if=None):
+        # pylint: disable=C0301
         """
         Helper to create container object.
 
         Args:
             element (Object): Element to click
             second_element (Object): To Element from drag and drop
             timeout_in_ms: Total time of hold in Click Hold, Timeout in between waiting loops between clicking and existance profing of Click Open/ Click Close
             max_repeat: Maximum number of repeats of clicking and wating in Click Open/ Click Close
             click_element_xpath: The element to be clicked in Click Open/ Click Close
             goal_element_xpath: Close element from Click Close/ open element from Click Open
             focus_element_xpath_before: Focus element before clicking in Click Open/ Click Close
             focus_element_xpath_after: Focus element after clicking in Click Open/ Click Close
             ignore_if: The execution will be ignored if the clicking element exist in Click Open / does not exist in Click Close
         """
+        # pylint: enable=C0301
         return Mouse.Container(element=element, second_element=second_element, timeout_in_ms=timeout_in_ms,
                                max_repeat=max_repeat,
                                click_element_xpath=click_element_xpath, goal_element_xpath=goal_element_xpath,
                                focus_element_xpath_before=focus_element_xpath_before,
                                focus_element_xpath_after=focus_element_xpath_after,
                                ignore_if=ignore_if)
 
@@ -159,15 +161,15 @@
                 if self._element_module.execute_action(Element.Action.GET_ELEMENT_BY_XPATH, container):
                     return True
 
             if focus_element_xpath_before_click:
                 container = Element.create_value_container(xpath=focus_element_xpath_before_click)
                 self._element_module.execute_action(Element.Action.FOCUS_ELEMENT, container)
             _click_element_found = False
-            for i in range(max_repeat):
+            for _ in range(max_repeat):
                 container = Element.create_value_container(xpath=click_element_xpath)
                 click_element = self._element_module.execute_action(Element.Action.GET_ELEMENT_BY_XPATH, container)
 
                 if click_element:
                     _click_element_found = True
                     click_type(click_element)
                     container = Element.create_value_container(xpath=open_element_xpath)
@@ -176,15 +178,15 @@
                     if open_element:
                         if focus_element_xpath_after_open:
                             container = Element.create_value_container(xpath=focus_element_xpath_after_open)
                             self._element_module.execute_action(Element.Action.FOCUS_ELEMENT, container)
                         return True
 
                 time.sleep(float(timeout_between_repeats) / 1000)
-            
+
             if not _click_element_found:
                 raise FlaUiError(FlaUiError.ElementNotExists.format(click_element_xpath))
             raise FlaUiError(FlaUiError.ElementNotOpened.format(open_element_xpath, click_element_xpath))
         except NoClickablePointException:
             raise FlaUiError(FlaUiError.ElementNotClickable) from None
 
     def _click_close(self, click_type, click_element_xpath: str, close_element_xpath: str,
@@ -203,17 +205,17 @@
                 container = Element.create_value_container(xpath=close_element_xpath)
                 if not self._element_module.execute_action(Element.Action.GET_ELEMENT_BY_XPATH, container):
                     return True
 
             if focus_element_xpath_before_click:
                 container = Element.create_value_container(xpath=focus_element_xpath_before_click)
                 self._element_module.execute_action(Element.Action.FOCUS_ELEMENT, container)
-            
+
             _click_element_found = False
-            for i in range(max_repeat):
+            for _ in range(max_repeat):
                 container = Element.create_value_container(xpath=click_element_xpath)
                 click_element = self._element_module.execute_action(Element.Action.GET_ELEMENT_BY_XPATH, container)
 
                 if click_element:
                     _click_element_found = True
                     click_type(click_element)
 
@@ -223,15 +225,15 @@
                     if not open_element:
                         if focus_element_xpath_after_close:
                             container = Element.create_value_container(xpath=focus_element_xpath_after_close)
                             self._element_module.execute_action(Element.Action.FOCUS_ELEMENT, container)
                         return True
 
                 time.sleep(float(timeout_between_repeats) / 1000)
-                
+
             if not _click_element_found:
                 raise FlaUiError(FlaUiError.ElementNotExists.format(click_element_xpath))
             raise FlaUiError(FlaUiError.ElementNotClosed.format(close_element_xpath, click_element_xpath))
         except NoClickablePointException:
             raise FlaUiError(FlaUiError.ElementNotClickable) from None
 
     @staticmethod
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/property.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/property.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,112 +42,27 @@
         IS_VALUE_PATTERN_SUPPORTED = "IS_VALUE_PATTERN_SUPPORTED"
         VALUE = "VALUE"
         IS_EXPAND_COLLAPSE_PATTERN_SUPPORTED = "IS_EXPAND_COLLAPSE_PATTERN_SUPPORTED"
         EXPAND_COLLAPSE_STATE = "EXPAND_COLLAPSE_STATE"
         IS_SELECTION_ITEM_PATTERN_SUPPORTED = "IS_SELECTION_ITEM_PATTERN_SUPPORTED"
         IS_SELECTED = "IS_SELECTED"
         STAGE_FOR_COMBOBOX_SELECTIONITEM = "STAGE_FOR_COMBOBOX_SELECTIONITEM"
-            
+
     @staticmethod
     def create_value_container(element: Any = None, uia: str = None) -> Container:
         """
         Helper to create container object.
 
         Args:
             element (Object): Element to grab property.
             uia (string): User interface identifier
         """
         return Property.Container(element=element, uia=uia)
 
     def execute_action(self, action: Action, values: Container):
-        """If action is not supported an ActionNotSupported error will be raised.
-
-        Supported action usages are:
-
-          *  Action.FOREGROUND_COLOR
-            * Values ["element", "uia"] : Element to get foreground color property from uia2 or uia3.
-            * Returns : Foreground color as (a,r,g,b) tuple.
-
-         *  Action.BACKGROUND_COLOR
-            * Values ["element", "uia"] : Element to get background color property from uia2 or uia3.
-            * Returns : Foreground color as (a,r,g,b) tuple.
-
-         *  Action.FONT_SIZE
-            * Values ["element", "uia"] : Element to get font size property from uia2 or uia3.
-            * Returns : Font size as floating point value
-
-         *  Action.FONT_NAME
-            * Values ["element", "uia"] : Element to get font name property from uia2 or uia3.
-            * Returns : String name from font
-
-         *  Action.FONT_WEIGHT
-            * Values ["element", "uia"] : Element to get font weight property from uia2 or uia3.
-            * Returns : Font weight as floating point value
-
-         *  Action.CULTURE
-            * Values ["element", "uia"] : Element to get culture property from uia2 or uia3.
-            * Returns : Culture property as string
-
-         *  Action.IS_HIDDEN
-            * Values ["element", "uia"] : Element to get culture property from uia2 or uia3.
-            * Returns : Bool if element is hidden.
-
-         *  Action.WINDOW_VISUAL_STATE
-            * Values ["element"] : Element to get window visual state property from window.
-            * Returns : String from visual state.
-
-         *  Action.WINDOW_INTERACTION_STATE
-            * Values ["element"] : Element to get window visual state property from window.
-            * Returns : String from window interaction state.
-
-         *  Action.TOGGLE_STATE
-            * Values ["element", "uia"] : Element to get toggle state property from uia2 or uia3 element.
-            * Returns : String from toggle state like ON, OFF, Intermediate as string.
-
-         *  Action.MAXIMIZE_WINDOW
-            * Values ["element"] : Maximize window
-            * Returns : None
-
-         *  Action.MINIMIZE_WINDOW
-            * Values ["element"] : Minimize window
-            * Returns : None
-
-         *  Action.NORMALIZE_WINDOW
-            * Values ["element"] : Normalize window
-            * Returns : None
-
-         *  Action.CAN_WINDOW_MINIMIZE
-            * Values ["element"] : Verification if window can be minimized.
-            * Returns : Return True if supported otherwise False
-
-         *  Action.CAN_WINDOW_MAXIMIZE
-            * Values ["element"] : Verification if window can be maximized.
-            * Returns : Return True if supported otherwise False
-
-         *  Action.IS_READ_ONLY
-            * Values ["element"] : Verification if element is read only.
-            * Returns : Return True/False otherwise Pattern not supported exception
-
-         *  Action.IS_WINDOW_PATTERN_SUPPORTED, IS_TEXT_PATTERN_SUPPORTED, IS_TOGGLE_PATTERN_SUPPORTED, IS_VALUE_PATTERN_SUPPORTED,
-                   IS_SELECTION_ITEM_PATTERN_SUPPORTED
-            * Values ["element"] : Verification if pattern is supported to element.
-            * Returns : Return True if supported otherwise False
-         
-         *  Action.IS_SELECTED
-            * Values ["element"] : Verification if element is read only.
-            * Returns : Return True/False otherwise Pattern not supported exception
-
-        Raises:
-            FlaUiError: If action is not supported.
-
-        Args:
-            action (Action): Action to use.
-            values (Object): See supported action definitions for value usage.
-        """
-
         switcher = {
             self.Action.FOREGROUND_COLOR: lambda: self._get_foreground_color(values["element"], values["uia"]),
             self.Action.BACKGROUND_COLOR: lambda: self._get_background_color(values["element"], values["uia"]),
             self.Action.FONT_SIZE: lambda: self._get_font_size(values["element"], values["uia"]),
             self.Action.FONT_NAME: lambda: self._get_font_name(values["element"], values["uia"]),
             self.Action.FONT_WEIGHT: lambda: self._get_font_weight(values["element"], values["uia"]),
             self.Action.CULTURE: lambda: self._get_culture(values["element"], values["uia"]),
@@ -168,17 +83,19 @@
             self.Action.IS_TEXT_PATTERN_SUPPORTED: lambda: self._is_text_pattern_supported(values["element"]),
             self.Action.IS_TOGGLE_PATTERN_SUPPORTED: lambda: self._is_toggle_pattern_supported(values["element"]),
             self.Action.IS_VALUE_PATTERN_SUPPORTED: lambda: self._is_value_pattern_supported(values["element"]),
             self.Action.VALUE: lambda: self._get_value_from_value_pattern(values["element"]),
             self.Action.IS_EXPAND_COLLAPSE_PATTERN_SUPPORTED: lambda: self._is_expand_collapse_pattern_supported(
                 values["element"]),
             self.Action.EXPAND_COLLAPSE_STATE: lambda: self._get_expand_collapse_pattern_state(values["element"]),
-            self.Action.IS_SELECTION_ITEM_PATTERN_SUPPORTED: lambda: self._is_selection_item_pattern_supported(values["element"]),
+            self.Action.IS_SELECTION_ITEM_PATTERN_SUPPORTED: lambda: self._is_selection_item_pattern_supported(
+                values["element"]),
             self.Action.IS_SELECTED: lambda: self._is_selected(values["element"]),
-            self.Action.STAGE_FOR_COMBOBOX_SELECTIONITEM: lambda: self._stage_for_combobox_selectionitem(values["element"]),
+            self.Action.STAGE_FOR_COMBOBOX_SELECTIONITEM: lambda: self._stage_for_combobox_selectionitem(
+                values["element"]),
         }
 
         return switcher.get(action, lambda: FlaUiError.raise_fla_ui_error(FlaUiError.ActionNotSupported))()
 
     @staticmethod
     def _get_window_visual_state(element: Any) -> str:
         pattern = Property._get_window_pattern_from_element(element)
@@ -317,19 +234,19 @@
     @staticmethod
     def _is_value_pattern_supported(element: Any) -> bool:
         return Property._prop_to_bool(element.Patterns.Value.IsSupported)
 
     @staticmethod
     def _is_expand_collapse_pattern_supported(element: Any) -> bool:
         return Property._prop_to_bool(element.Patterns.ExpandCollapse.IsSupported)
-    
+
     @staticmethod
     def _is_selection_item_pattern_supported(element: Any) -> bool:
         return Property._prop_to_bool(element.Patterns.SelectionItem.IsSupported)
-    
+
     @staticmethod
     def _int_to_rgba(argb_int: int) -> (int, int, int, int):
         blue = argb_int & 255
         green = (argb_int >> 8) & 255
         red = (argb_int >> 16) & 255
         alpha = (argb_int >> 24) & 255
         return red, green, blue, alpha
@@ -338,24 +255,24 @@
     def _prop_to_bool(prop: Any) -> bool:
 
         if isinstance(prop, bool):
             return bool(prop)
 
         # Should be from type FlaUI.Core.AutomationProperty[Boolean]
         return bool(prop.Value)
-    
+
     @staticmethod
     def _get_expand_collapse_pattern_from_element(element) -> Any:
         if Property._is_expand_collapse_pattern_supported(element):
             pattern = element.Patterns.ExpandCollapse.Pattern
             if pattern is not None:
                 return pattern
 
         raise FlaUiError(FlaUiError.PatternNotSupported.format("ExpandCollapse"))
-    
+
     @staticmethod
     def _get_expand_collapse_pattern_state(element: Any) -> str:
         pattern = Property._get_expand_collapse_pattern_from_element(element)
         return str(pattern.ExpandCollapseState)
 
     @staticmethod
     def _get_value_pattern_from_element(element) -> Any:
@@ -375,20 +292,20 @@
     def _get_selection_item_pattern_from_element(element) -> Any:
         if Property._is_selection_item_pattern_supported(element):
             pattern = element.Patterns.SelectionItem.Pattern
             if pattern is not None:
                 return pattern
 
         raise FlaUiError(FlaUiError.PatternNotSupported.format("SelectionItem"))
-    
+
     @staticmethod
     def _is_selected(element: Any) -> str:
         pattern = Property._get_selection_item_pattern_from_element(element)
         return Property._prop_to_bool(pattern.IsSelected)
-    
+
     @staticmethod
     def _stage_for_combobox_selectionitem(element):
         state = Property._get_expand_collapse_pattern_state(element)
         if state == "Expanded":
             element.Collapse()
         if state == "Collapsed":
-            element.Expand()
+            element.Expand()
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/selector.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,21 @@
             control (Object): Selector object to use (Combobox, Listbox).
             name (String): Name or Text from selector item which should exist.
 
         Returns:
             True if name from combobox item exists otherwise False.
         """
         is_contain = False
-        
+
         for item in control.Items:
             if name in (item.Name, item.Text):
                 is_contain = True
-                
+
         Selector._restore_for_expand_collapse_pattern(control)
-            
+
         if not is_contain:
             raise FlaUiError(FlaUiError.ControlDoesNotContainItem.format(name))
 
     @staticmethod
     def _should_not_contain(control: Any, name: str):
         """
         Checks if selector does not contain a given item by name or text.
@@ -156,21 +156,21 @@
             control (Object): Selector object to use (Combobox, Listbox).
             name (String): Name or Text from selector item which should exist.
 
         Returns:
             True if name from combobox item does not exist otherwise False.
         """
         is_contain = False
-        
+
         for item in control.Items:
             if name in (item.Name, item.Text):
                 is_contain = True
-                
+
         Selector._restore_for_expand_collapse_pattern(control)
-            
+
         if is_contain:
             raise FlaUiError(FlaUiError.ControlContainsItem.format(name))
 
     @staticmethod
     def _should_have_selected_item(control: Any, item: Any):
         """
         Verification if specific items are selected.
@@ -187,15 +187,15 @@
             raise FlaUiError(FlaUiError.ItemNotSelected.format(item))
 
     @staticmethod
     def _get_items_count(control: Any):
         count = control.Items.Length
         Selector._restore_for_expand_collapse_pattern(control)
         return count
-        
+
     @staticmethod
     def _get_all_selected_names(control: Any):
         """
         Get all selected names.
 
         Args:
             control (Object): Selector object to use (Combobox, Listbox).
@@ -241,15 +241,15 @@
             List from all names from list control if exists otherwise empty list.
         """
         names = []
         for item in control.Items:
             names.append(item.Name)
 
         Selector._restore_for_expand_collapse_pattern(control)
-        
+
         return names
 
     @staticmethod
     def _get_all_texts(control: Any):
         """
         Get all texts from selector.
 
@@ -261,19 +261,19 @@
         """
         texts = []
 
         for item in control.Items:
             texts.append(item.Text)
 
         Selector._restore_for_expand_collapse_pattern(control)
-        
+
         return texts
 
     @staticmethod
     def _restore_for_expand_collapse_pattern(control: Any):
         is_supported = control.Patterns.ExpandCollapse.IsSupported
         is_supported = bool(is_supported) if isinstance(is_supported, bool) else bool(is_supported.Value)
         if is_supported:
             pattern = control.Patterns.ExpandCollapse.Pattern
             state = str(pattern.ExpandCollapseState)
             if state == "Expanded":
-                control.Collapse() 
+                control.Collapse()
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tab.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/tab.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/textbox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/textbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tooglebutton.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/tooglebutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/tree.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/tree.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/module/window.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/module/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/automationelement.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/automationelement.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,28 @@
         """
             Creates Automation Element entity.
             ``automation_id`` Automation ID if set by element.
             ``name`` Name if set by element.
             ``class_name`` Class Name from element.
             ``xpath`` Xpath from element.
         """
+        # pylint: disable=C0103
         self.Xpath = xpath
         self.AutomationId = ""
         self.Name = ""
         self.ClassName = ""
 
         if automation_id:
             self.AutomationId = self._get_argument_in_xpath(self.Xpath, "[@AutomationId=\"" + automation_id + "\"]")
 
         if name:
             self.Name = self._get_argument_in_xpath(self.Xpath, "[@Name=\"" + name + "\"]")
 
         if class_name:
             self.ClassName = self._get_argument_in_xpath(self.Xpath, "[@ClassName=\"" + class_name + "\"]")
+        # pylint: enable=C0103
 
     @staticmethod
     def _get_argument_in_xpath(xpath, argument) -> str:
         xpaths = xpath.split("/")
         xpaths[-1] = re.sub(r"\[\d+]", argument, xpaths[-1])
         return "/".join(xpaths)
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/converter.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import re
-from typing import Any
+from typing import Any, Union
 from System import TimeSpan  # pylint: disable=import-error
 from FlaUILibrary.flaui.exception import FlaUiError
+from FlaUILibrary.flaui.util.automationelement import AutomationElement
 
 
 class Converter:
     """
     Helper class to convert specific values.
     """
 
     @staticmethod
     def cast_to_timespan(value: int):
+        """
+        Helper to cast value to timespan. If value is null, None will be returned.
+
+        Args:
+            value (int): Value to convert as timespan
+        """
         if value is None:
             return None
 
         return TimeSpan.FromMilliseconds(value)
 
     @staticmethod
     def cast_to_int(value: Any, error_msg=None):
@@ -50,14 +57,28 @@
         """
         if value is None:
             return ""
 
         return str(value)
 
     @staticmethod
+    def cast_to_xpath_string(value: Union[str, AutomationElement]):
+        """
+        Helper to cast value as xpath string.
+        If value is None empty string will be returned.
+
+        Args:
+            value (Object): Value to convert
+        """
+        if isinstance(value, AutomationElement):
+            return Converter.cast_to_string(value.Xpath)
+
+        return Converter.cast_to_string(value)
+
+    @staticmethod
     def cast_to_bool(value: Any):
         """
         Helper to cast value as bool.
         If value is None False will be returned.
 
         Args:
             value (Object): Value to convert
@@ -65,14 +86,20 @@
         if value is None:
             return False
 
         return bool(value)
 
     @staticmethod
     def get_combobox_xpath_from_combobox_selectionitem_xpath(xpath: str) -> str:
-        is_combobox_selectionitem = True if "ComboBox" in xpath and "ComboBox" not in xpath.split("/")[-1] else False
+        """
+        Try to find first combobox from xpath. If found xpath will be returned otherwise empty string.
+
+        Args:
+            xpath (String): XPath find combobox element.
+        """
+        is_combobox_selectionitem = "ComboBox" in xpath and "ComboBox" not in xpath.split("/")[-1]
         if is_combobox_selectionitem:
             matches = re.findall(r"/ComboBox.*?/", xpath)
-            s = matches[0] if matches is not [] else ""
+            s = "" if not matches else matches[0]
             result = f"{xpath.split(s)[0]}{s}"[:-1] if s else ""
             return result
         return ""
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/keyboardinputconverter.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/keyboardinputconverter.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitems.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/treeitems.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/flaui/util/treeitemsparser.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/flaui/util/treeitemsparser.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/__init__.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/application.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/application.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/checkbox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/combobox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/combobox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/debug.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/element.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         | msg        | string | Custom error message                                                   |
 
         Example:
         | Wait Until Element Exist  <XPATH>  <RETRIES=10> |
         | Wait Until Element Exist  <XPATH>  <RETRIES=10>  <MSG> |
         """
         module = self._container.create_or_get_module()
-        module.action(Element.Action.WAIT_UNTIl_ELEMENT_EXIST,
+        module.action(Element.Action.WAIT_UNTIL_ELEMENT_EXIST,
                       Element.create_value_container(xpath=identifier, retries=retries),
                       msg)
 
     @keyword
     def wait_until_element_does_not_exist(self, identifier, retries=10, msg=None):
         """
         Waits until element does not exist or timeout was reached. If timeout was reached an FlaUIError occurred.
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/grid.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/grid.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/keyboard.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/keyboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         Constructor for element keywords.
 
         ``container`` User automation container to handle element interaction.
         """
         self._container = container
 
     @keyword
-    def press_key(self, key_combination, identifier=None, delay_in_ms=None, 
+    def press_key(self, key_combination, identifier=None, delay_in_ms=None,
                   msg=None, press_only=False, release_only=False):
         """
         Keyboard control to execute a user defined one shortcut or text.
         press_only and release_only supports key shortcut only, not text.
 
         Arguments:
         | Argument         | Type                                  | Description                                |
@@ -103,17 +103,17 @@
         module = self._container.create_or_get_module()
         if identifier is not None:
             module.action(Element.Action.FOCUS_ELEMENT,
                           Element.create_value_container(xpath=identifier, retries=None, name=None),
                           msg)
 
         module.action(Keyboard.Action.KEY_COMBINATION,
-                      Keyboard.create_value_container(shortcut=key_combination, 
+                      Keyboard.create_value_container(shortcut=key_combination,
                                                       delay_in_ms=delay_in_ms,
-                                                      press_only=press_only, 
+                                                      press_only=press_only,
                                                       release_only=release_only),
                       msg)
 
     @keyword
     def press_keys(self, keys_combinations, identifier=None, delay_in_ms=None,
                    msg=None, press_only=False, release_only=False):
         """
@@ -156,12 +156,12 @@
         module = self._container.create_or_get_module()
         if identifier is not None:
             module.action(Element.Action.FOCUS_ELEMENT,
                           Element.create_value_container(xpath=identifier, retries=None, name=None),
                           msg)
 
         module.action(Keyboard.Action.KEYS_COMBINATIONS,
-                      Keyboard.create_value_container(shortcuts=keys_combinations, 
+                      Keyboard.create_value_container(shortcuts=keys_combinations,
                                                       delay_in_ms=delay_in_ms,
-                                                      press_only=press_only, 
+                                                      press_only=press_only,
                                                       release_only=release_only),
                       msg)
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/listbox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/listbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/mouse.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/mouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,17 +210,23 @@
         start_element = module.get_element(start_identifier, msg=msg)
         end_element = module.get_element(end_identifier, msg=msg)
         module.action(Mouse.Action.DRAG_AND_DROP,
                       Mouse.create_value_container(element=start_element, second_element=end_element),
                       msg)
 
     @keyword
-    def click_open(self, click_element_identifier: str, open_element_identifier: str, 
-                    focus_element_identifier_before_click: str = None, focus_element_identifier_after_open: str = None , 
-                    max_repeat: int = 5, timeout_between_repeates: int = 1000, ignore_if_already_open: bool = True, msg=None):
+    def click_open(self, click_element_identifier: str,
+                   open_element_identifier: str,
+                   focus_element_identifier_before_click: str = None,
+                   focus_element_identifier_after_open: str = None,
+                   max_repeat: int = 5,
+                   timeout_between_repeates: int = 1000,
+                   ignore_if_already_open: bool = True,
+                   msg=None):
+        # pylint: disable=C0301
         """
         Left clicks to element by an XPath and excepts an element to be opened.
         It repeats the act of clicking until the excepted element is there by waiting for given seconds each time.
         Maximum repeating time could also be changed
 
         XPaths syntax is explained in `XPath locator`.
 
@@ -237,25 +243,36 @@
         | ignore_if_already_open | bool | the keyword will not be executed if excepted element is already open |
         | msg | string | Custom error message |
 
         Examples:
         | Click Open  <XPATH>  <XPATH>  |
 
         """
+        # pylint: enable=C0301
         module = self._container.create_or_get_module()
         module.action(Mouse.Action.LEFT_CLICK_OPEN,
-                      Mouse.create_value_container(click_element_xpath=click_element_identifier, goal_element_xpath=open_element_identifier, 
-                                                   focus_element_xpath_before=focus_element_identifier_before_click, focus_element_xpath_after=focus_element_identifier_after_open,
-                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates, ignore_if=ignore_if_already_open),
+                      Mouse.create_value_container(click_element_xpath=click_element_identifier,
+                                                   goal_element_xpath=open_element_identifier,
+                                                   focus_element_xpath_before=focus_element_identifier_before_click,
+                                                   focus_element_xpath_after=focus_element_identifier_after_open,
+                                                   max_repeat=max_repeat,
+                                                   timeout_in_ms=timeout_between_repeates,
+                                                   ignore_if=ignore_if_already_open),
                       msg)
 
     @keyword
-    def double_click_open(self, click_element_identifier: str, open_element_identifier: str, 
-                    focus_element_identifier_before_click: str = None, focus_element_identifier_after_open: str = None , 
-                    max_repeat: int = 5, timeout_between_repeates: int = 1000, ignore_if_already_open: bool = True, msg=None):
+    def double_click_open(self, click_element_identifier: str,
+                          open_element_identifier: str,
+                          focus_element_identifier_before_click: str = None,
+                          focus_element_identifier_after_open: str = None,
+                          max_repeat: int = 5,
+                          timeout_between_repeates: int = 1000,
+                          ignore_if_already_open: bool = True,
+                          msg=None):
+        # pylint: disable=C0301
         """
         Double clicks to element by an XPath and excepts an element to be opened.
         It repeats the act of double clicking until the excepted element is there by waiting for given seconds each time.
         Maximum repeating time could also be changed
 
         XPaths syntax is explained in `XPath locator`.
 
@@ -272,25 +289,34 @@
         | ignore_if_already_open | bool | the keyword will not be executed if excepted element is already open |
         | msg | string | Custom error message |
 
         Examples:
         | Double Click Open  <XPATH>  <XPATH>  |
 
         """
+        # pylint: enable=C0301
         module = self._container.create_or_get_module()
         module.action(Mouse.Action.DOUBLE_CLICK_OPEN,
-                      Mouse.create_value_container(click_element_xpath=click_element_identifier, goal_element_xpath=open_element_identifier, 
-                                                   focus_element_xpath_before=focus_element_identifier_before_click, focus_element_xpath_after=focus_element_identifier_after_open,
-                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates, ignore_if=ignore_if_already_open),
-                      msg)
+                      Mouse.create_value_container(click_element_xpath=click_element_identifier,
+                                                   goal_element_xpath=open_element_identifier,
+                                                   focus_element_xpath_before=focus_element_identifier_before_click,
+                                                   focus_element_xpath_after=focus_element_identifier_after_open,
+                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates,
+                                                   ignore_if=ignore_if_already_open), msg)
 
     @keyword
-    def right_click_open(self, click_element_identifier: str, open_element_identifier: str, 
-                    focus_element_identifier_before_click: str = None, focus_element_identifier_after_open: str = None , 
-                    max_repeat: int = 5, timeout_between_repeates: int = 1000, ignore_if_already_open: bool = True, msg=None):
+    def right_click_open(self, click_element_identifier: str,
+                         open_element_identifier: str,
+                         focus_element_identifier_before_click: str = None,
+                         focus_element_identifier_after_open: str = None,
+                         max_repeat: int = 5,
+                         timeout_between_repeates: int = 1000,
+                         ignore_if_already_open: bool = True,
+                         msg=None):
+        # pylint: disable=C0301
         """
         Right clicks to element by an XPath and excepts an element to be opened.
         It repeats the act of right clicking until the excepted element is there by waiting for given seconds each time.
         Maximum repeating time could also be changed
 
         XPaths syntax is explained in `XPath locator`.
 
@@ -307,25 +333,35 @@
         | ignore_if_already_open | bool | the keyword will not be executed if excepted element is already open |
         | msg | string | Custom error message |
 
         Examples:
         | Right Click Open  <XPATH>  <XPATH>  |
 
         """
+        # pylint: enable=C0301
         module = self._container.create_or_get_module()
         module.action(Mouse.Action.RIGHT_CLICK_OPEN,
-                      Mouse.create_value_container(click_element_xpath=click_element_identifier, goal_element_xpath=open_element_identifier, 
-                                                   focus_element_xpath_before=focus_element_identifier_before_click, focus_element_xpath_after=focus_element_identifier_after_open,
-                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates, ignore_if=ignore_if_already_open),
-                      msg)
+                      Mouse.create_value_container(click_element_xpath=click_element_identifier,
+                                                   goal_element_xpath=open_element_identifier,
+                                                   focus_element_xpath_before=focus_element_identifier_before_click,
+                                                   focus_element_xpath_after=focus_element_identifier_after_open,
+                                                   max_repeat=max_repeat,
+                                                   timeout_in_ms=timeout_between_repeates,
+                                                   ignore_if=ignore_if_already_open), msg)
 
     @keyword
-    def click_close(self, click_element_identifier: str, close_element_identifier: str = None, 
-                    focus_element_identifier_before_click: str = None, focus_element_identifier_after_close: str = None , 
-                    max_repeat: int = 5, timeout_between_repeates: int = 1, ignore_if_already_close: bool = True, msg=None):
+    def click_close(self, click_element_identifier: str,
+                    close_element_identifier: str = None,
+                    focus_element_identifier_before_click: str = None,
+                    focus_element_identifier_after_close: str = None,
+                    max_repeat: int = 5,
+                    timeout_between_repeates: int = 1,
+                    ignore_if_already_close: bool = True,
+                    msg=None):
+        # pylint: disable=C0301
         """
         Left clicks an element by an XPath and excepts an element to be closed.
         It repeats the act of clicking until the excepted element is closed by waiting for given seconds each time.
         Maximum repeating time could also be changed
 
         XPaths syntax is explained in `XPath locator`.
 
@@ -344,27 +380,37 @@
 
         Examples:
         | Click Close  <XPATH>  <XPATH>  |
         or
         | Click Close  <XPATH>  |
 
         """
+        # pylint: enable=C0301
         if not close_element_identifier:
             close_element_identifier = click_element_identifier
         module = self._container.create_or_get_module()
         module.action(Mouse.Action.LEFT_CLICK_CLOSE,
-                      Mouse.create_value_container(click_element_xpath=click_element_identifier, goal_element_xpath=close_element_identifier, 
-                                                   focus_element_xpath_before=focus_element_identifier_before_click, focus_element_xpath_after=focus_element_identifier_after_close,
-                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates, ignore_if=ignore_if_already_close),
-                      msg)
+                      Mouse.create_value_container(click_element_xpath=click_element_identifier,
+                                                   goal_element_xpath=close_element_identifier,
+                                                   focus_element_xpath_before=focus_element_identifier_before_click,
+                                                   focus_element_xpath_after=focus_element_identifier_after_close,
+                                                   max_repeat=max_repeat,
+                                                   timeout_in_ms=timeout_between_repeates,
+                                                   ignore_if=ignore_if_already_close), msg)
 
     @keyword
-    def double_click_close(self, click_element_identifier: str, close_element_identifier: str = None, 
-                    focus_element_identifier_before_click: str = None, focus_element_identifier_after_close: str = None , 
-                    max_repeat: int = 5, timeout_between_repeates: int = 1, ignore_if_already_close: bool = True, msg=None):
+    def double_click_close(self, click_element_identifier: str,
+                           close_element_identifier: str = None,
+                           focus_element_identifier_before_click: str = None,
+                           focus_element_identifier_after_close: str = None,
+                           max_repeat: int = 5,
+                           timeout_between_repeates: int = 1,
+                           ignore_if_already_close: bool = True,
+                           msg=None):
+        # pylint: disable=C0301
         """
         Double clicks an element by an XPath and excepts an element to be closed.
         It repeats the act of double clicking until the excepted element is closed by waiting for given seconds each time.
         Maximum repeating time could also be changed
 
         XPaths syntax is explained in `XPath locator`.
 
@@ -383,27 +429,37 @@
 
         Examples:
         | Double Click Close  <XPATH>  <XPATH>  |
         or
         | Double Click Close  <XPATH>  |
 
         """
+        # pylint: enable=C0301
         if not close_element_identifier:
             close_element_identifier = click_element_identifier
         module = self._container.create_or_get_module()
         module.action(Mouse.Action.DOUBLE_CLICK_CLOSE,
-                      Mouse.create_value_container(click_element_xpath=click_element_identifier, goal_element_xpath=close_element_identifier, 
-                                                   focus_element_xpath_before=focus_element_identifier_before_click, focus_element_xpath_after=focus_element_identifier_after_close,
-                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates, ignore_if=ignore_if_already_close),
-                      msg)
+                      Mouse.create_value_container(click_element_xpath=click_element_identifier,
+                                                   goal_element_xpath=close_element_identifier,
+                                                   focus_element_xpath_before=focus_element_identifier_before_click,
+                                                   focus_element_xpath_after=focus_element_identifier_after_close,
+                                                   max_repeat=max_repeat,
+                                                   timeout_in_ms=timeout_between_repeates,
+                                                   ignore_if=ignore_if_already_close), msg)
 
     @keyword
-    def right_click_close(self, click_element_identifier: str, close_element_identifier: str = None, 
-                    focus_element_identifier_before_click: str = None, focus_element_identifier_after_close: str = None , 
-                    max_repeat: int = 5, timeout_between_repeates: int = 1, ignore_if_already_close: bool = True, msg=None):
+    def right_click_close(self, click_element_identifier: str,
+                          close_element_identifier: str = None,
+                          focus_element_identifier_before_click: str = None,
+                          focus_element_identifier_after_close: str = None,
+                          max_repeat: int = 5,
+                          timeout_between_repeates: int = 1,
+                          ignore_if_already_close: bool = True,
+                          msg=None):
+        # pylint: disable=C0301
         """
         Right clicks an element by an XPath and excepts an element to be closed.
         It repeats the act of right clicking until the excepted element is closed by waiting for given seconds each time.
         Maximum repeating time could also be changed
 
         XPaths syntax is explained in `XPath locator`.
 
@@ -422,15 +478,19 @@
 
         Examples:
         | Right Click Close  <XPATH>  <XPATH>  |
         or
         | Right Click Close  <XPATH>  |
 
         """
+        # pylint: enable=C0301
         if not close_element_identifier:
             close_element_identifier = click_element_identifier
         module = self._container.create_or_get_module()
         module.action(Mouse.Action.RIGHT_CLICK_CLOSE,
-                      Mouse.create_value_container(click_element_xpath=click_element_identifier, goal_element_xpath=close_element_identifier, 
-                                                   focus_element_xpath_before=focus_element_identifier_before_click, focus_element_xpath_after=focus_element_identifier_after_close,
-                                                   max_repeat=max_repeat, timeout_in_ms=timeout_between_repeates, ignore_if=ignore_if_already_close),
-                      msg)
+                      Mouse.create_value_container(click_element_xpath=click_element_identifier,
+                                                   goal_element_xpath=close_element_identifier,
+                                                   focus_element_xpath_before=focus_element_identifier_before_click,
+                                                   focus_element_xpath_after=focus_element_identifier_after_close,
+                                                   max_repeat=max_repeat,
+                                                   timeout_in_ms=timeout_between_repeates,
+                                                   ignore_if=ignore_if_already_close), msg)
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/property.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,45 +64,50 @@
         | msg        | string | Custom error message          |
 
         Examples:
         | ${value}       Get Property From Element  <XPATH>  <PROPERTY> |
 
         """
         # pylint: enable=line-too-long
-        
+
         action_value = ""
         try:
             action_value = Property.Action[action.upper()]
-        except KeyError or action_value in [Property.Action.MAXIMIZE_WINDOW, Property.Action.MINIMIZE_WINDOW, Property.Action.NORMALIZE_WINDOW]:
+        except KeyError:
+            FlaUiError.raise_fla_ui_error(FlaUiError.InvalidPropertyArgument)
+
+        if action_value in [Property.Action.MAXIMIZE_WINDOW,
+                            Property.Action.MINIMIZE_WINDOW,
+                            Property.Action.NORMALIZE_WINDOW]:
             FlaUiError.raise_fla_ui_error(FlaUiError.InvalidPropertyArgument)
-        
+
         module = self._container.create_or_get_module()
-        
+
         if action_value is Property.Action.IS_SELECTED:
             # need expand parent ComboBox before to get ComboBox SelectionItem element
             combobox_xpath = Converter.get_combobox_xpath_from_combobox_selectionitem_xpath(identifier)
             if combobox_xpath:
                 combobox_element = module.get_element(combobox_xpath, InterfaceType.COMBOBOX, msg)
                 module.action(Property.Action.STAGE_FOR_COMBOBOX_SELECTIONITEM,
                             Property.create_value_container(element=combobox_element, uia=module.identifier()),
                             msg)
 
         element = module.get_element(identifier, msg=msg)
         property_value = module.action(action_value,
-                            Property.create_value_container(element=element, uia=module.identifier()), 
+                            Property.create_value_container(element=element, uia=module.identifier()),
                             msg)
-        
+
         if action_value is Property.Action.IS_SELECTED:
             combobox_xpath = Converter.get_combobox_xpath_from_combobox_selectionitem_xpath(identifier)
             if combobox_xpath:
                 combobox_element = module.get_element(combobox_xpath, InterfaceType.COMBOBOX, msg)
                 module.action(Property.Action.STAGE_FOR_COMBOBOX_SELECTIONITEM,
                             Property.create_value_container(element=combobox_element, uia=module.identifier()),
                             msg)
-        
+
         return property_value
 
     @keyword
     def get_background_color(self, identifier, msg=None):
         """
         Returns background color as ARGB Tuple (int, int, int, int) from element if background color pattern is
         supported.
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/radiobutton.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/radiobutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tab.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/tab.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/textbox.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/textbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/togglebutton.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/togglebutton.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/tree.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/tree.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/uia.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/uia.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,13 +30,12 @@
         | uia        | string | 'UIA2' or 'UIA3'                        |
 
         Example:
         | Switch UIA To  UIA2           |
         | Switch UIA To  UIA3           |
 
         """
-        if uia == "UIA2" or uia == "UIA3":
+        if uia in ("UIA2", "UIA3"):
             self._container.set_identifier(uia)
             return
 
         raise FlaUiError(FlaUiError.ActionNotSupported) from None
-
```

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/keywords/window.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/keywords/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/pythonnetwrapper.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/pythonnetwrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-flaui-3.0.3/src/FlaUILibrary/robotframework/robotlog.py` & `robotframework_flaui-3.1.0/src/FlaUILibrary/robotframework/robotlog.py`

 * *Files identical despite different names*

