# Comparing `tmp/textLSP-0.3.0.tar.gz` & `tmp/textlsp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textLSP-0.3.0.tar", last modified: Sat Mar  9 18:53:25 2024, max compression
+gzip compressed data, was "textlsp-0.3.1.tar", last modified: Mon May  6 06:09:00 2024, max compression
```

## Comparing `textLSP-0.3.0.tar` & `textlsp-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.427013 textLSP-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-09 18:45:39.000000 textLSP-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-09 18:53:25.427013 textLSP-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-03-09 18:45:39.000000 textLSP-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 18:53:25.427013 textLSP-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-09 18:45:39.000000 textLSP-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.419013 textLSP-0.3.0/textLSP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.419013 textLSP-0.3.0/textLSP/analysers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21669 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/analyser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/gramformer/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/gramformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/gramformer/gramformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/grammarbot/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/grammarbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/grammarbot/grammarbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/hf_checker/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/hf_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/hf_checker/hf_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/hf_completion/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/hf_completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/hf_completion/hf_completion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/hf_instruction_checker/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/hf_instruction_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/hf_instruction_checker/hf_instruction_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/languagetool/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/languagetool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/languagetool/languagetool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/analysers/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/analysers/openai/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/documents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42712 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/documents/latex/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/latex/latex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/documents/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/markdown/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/documents/org/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/org/org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP/documents/txt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/txt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/documents/txt/txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/nn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-09 18:45:39.000000 textLSP-0.3.0/textLSP/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:53:25.423013 textLSP-0.3.0/textLSP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-09 18:53:25.000000 textLSP-0.3.0/textLSP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-09 18:53:25.000000 textLSP-0.3.0/textLSP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 18:53:25.000000 textLSP-0.3.0/textLSP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-09 18:53:25.000000 textLSP-0.3.0/textLSP.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-09 18:53:25.000000 textLSP-0.3.0/textLSP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-09 18:53:25.000000 textLSP-0.3.0/textLSP.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.544007 textlsp-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 06:00:47.000000 textlsp-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-06 06:09:00.544007 textlsp-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-06 06:00:47.000000 textlsp-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:09:00.544007 textlsp-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 06:00:47.000000 textlsp-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.536007 textlsp-0.3.1/textLSP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21669 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/analyser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/gramformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/gramformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/gramformer/gramformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/grammarbot/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/grammarbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/grammarbot/grammarbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/hf_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/hf_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/hf_checker/hf_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/hf_completion/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/hf_completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/hf_completion/hf_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/hf_instruction_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/hf_instruction_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/hf_instruction_checker/hf_instruction_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/languagetool/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/languagetool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/languagetool/languagetool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/analysers/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/analysers/openai/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.540007 textlsp-0.3.1/textLSP/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44990 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.544007 textlsp-0.3.1/textLSP/documents/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/latex/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.544007 textlsp-0.3.1/textLSP/documents/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/markdown/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.544007 textlsp-0.3.1/textLSP/documents/org/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/org/org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.544007 textlsp-0.3.1/textLSP/documents/txt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/documents/txt/txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/nn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-06 06:00:47.000000 textlsp-0.3.1/textLSP/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:09:00.544007 textlsp-0.3.1/textLSP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-06 06:09:00.000000 textlsp-0.3.1/textLSP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-06 06:09:00.000000 textlsp-0.3.1/textLSP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:09:00.000000 textlsp-0.3.1/textLSP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 06:09:00.000000 textlsp-0.3.1/textLSP.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-06 06:09:00.000000 textlsp-0.3.1/textLSP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 06:09:00.000000 textlsp-0.3.1/textLSP.egg-info/top_level.txt
```

### Comparing `textLSP-0.3.0/LICENSE` & `textlsp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/PKG-INFO` & `textlsp-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: textLSP
-Version: 0.3.0
+Version: 0.3.1
 Summary: Language server for text spell and grammar check with various tools.
 Home-page: https://github.com/hangyav/textLSP
 Author: Viktor Hangya
 Author-email: hangyav@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pygls==1.3.0
+Requires-Dist: pygls==1.3.1
 Requires-Dist: lsprotocol==2023.0.1
-Requires-Dist: language-tool-python==2.7.1
-Requires-Dist: tree_sitter==0.20.4
-Requires-Dist: gitpython==3.1.42
+Requires-Dist: language-tool-python==2.8
+Requires-Dist: tree_sitter==0.21.3
+Requires-Dist: gitpython==3.1.43
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: torch==2.2.1
-Requires-Dist: openai==1.13.3
-Requires-Dist: transformers==4.38.2
+Requires-Dist: torch==2.3.0
+Requires-Dist: openai==1.25.0
+Requires-Dist: transformers==4.40.1
 Requires-Dist: sortedcontainers==2.4.0
-Requires-Dist: bitsandbytes==0.42.0
+Requires-Dist: bitsandbytes==0.43.1
+Requires-Dist: langdetect==1.0.9
 Provides-Extra: dev
-Requires-Dist: pytest==8.0.2; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: python-lsp-jsonrpc==1.1.2; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: coverage-threshold==0.4.4; extra == "dev"
 
 # textLSP
 Language server for text spell and grammar check with various AI tools.
 
 _This tool is in early development._
 
@@ -226,14 +227,19 @@
                 on_open = false,
                 on_save = false,
                 on_change = false,
             }
         },
     },
     documents = {
+        -- the language of the documents, could be set to `auto` of `auto:<fallback>`
+        -- to detect automatically, default: auto:en
+        language = "auto:en",
+        -- do not autodetect documents with fewer characters
+        min_length_language_detect = 20,
         org = {
             org_todo_keywords = {
                 'TODO',
                 'IN_PROGRESS',
                 'DONE'
             },
         },
```

### Comparing `textLSP-0.3.0/README.md` & `textlsp-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -196,14 +196,19 @@
                 on_open = false,
                 on_save = false,
                 on_change = false,
             }
         },
     },
     documents = {
+        -- the language of the documents, could be set to `auto` of `auto:<fallback>`
+        -- to detect automatically, default: auto:en
+        language = "auto:en",
+        -- do not autodetect documents with fewer characters
+        min_length_language_detect = 20,
         org = {
             org_todo_keywords = {
                 'TODO',
                 'IN_PROGRESS',
                 'DONE'
             },
         },
```

### Comparing `textLSP-0.3.0/setup.py` & `textlsp-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Utility function to read the README file.
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="textLSP",
-    version="0.3.0",
+    version="0.3.1",
     author="Viktor Hangya",
     author_email="hangyav@gmail.com",
     description=("Language server for text spell and grammar check with various tools."),
     license="GPLv3",
     url="https://github.com/hangyav/textLSP",
     packages=find_packages(include=['textLSP*']),
     long_description=read('README.md'),
@@ -23,28 +23,29 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': ['textlsp=textLSP.cli:main'],
     },
     install_requires=[
-        'pygls==1.3.0',
+        'pygls==1.3.1',
         'lsprotocol==2023.0.1',
-        'language-tool-python==2.7.1',
-        'tree_sitter==0.20.4',
-        'gitpython==3.1.42',
+        'language-tool-python==2.8',
+        'tree_sitter==0.21.3',
+        'gitpython==3.1.43',
         'appdirs==1.4.4',
-        'torch==2.2.1',
-        'openai==1.13.3',
-        'transformers==4.38.2',
+        'torch==2.3.0',
+        'openai==1.25.0',
+        'transformers==4.40.1',
         'sortedcontainers==2.4.0',
-        'bitsandbytes==0.42.0',
+        'bitsandbytes==0.43.1',
+        'langdetect==1.0.9',
     ],
     extras_require={
         'dev': [
-            'pytest==8.0.2',
+            'pytest==8.2.0',
             'python-lsp-jsonrpc==1.1.2',
-            'pytest-cov==4.1.0',
+            'pytest-cov==5.0.0',
             'coverage-threshold==0.4.4'
         ]
     },
 )
```

### Comparing `textLSP-0.3.0/textLSP/analysers/analyser.py` & `textlsp-0.3.1/textLSP/analysers/analyser.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/gramformer/gramformer.py` & `textlsp-0.3.1/textLSP/analysers/gramformer/gramformer.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/grammarbot/grammarbot.py` & `textlsp-0.3.1/textLSP/analysers/grammarbot/grammarbot.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/handler.py` & `textlsp-0.3.1/textLSP/analysers/handler.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/hf_checker/hf_checker.py` & `textlsp-0.3.1/textLSP/analysers/hf_checker/hf_checker.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/hf_completion/hf_completion.py` & `textlsp-0.3.1/textLSP/analysers/hf_completion/hf_completion.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/hf_instruction_checker/hf_instruction_checker.py` & `textlsp-0.3.1/textLSP/analysers/hf_instruction_checker/hf_instruction_checker.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/analysers/languagetool/languagetool.py` & `textlsp-0.3.1/textLSP/analysers/languagetool/languagetool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import logging
 
 from typing import List, Tuple
-from collections import defaultdict
 from language_tool_python import LanguageTool
 from lsprotocol.types import (
         Diagnostic,
         Range,
         Position,
         TextEdit,
         CodeAction,
+        MessageType,
 )
 from pygls.server import LanguageServer
 
 from ..analyser import Analyser
 from ...types import Interval
 from ...documents.document import BaseDocument
 
 
 logger = logging.getLogger(__name__)
 
 
-LANGUAGE_MAP = defaultdict(lambda: 'en-US')
+LANGUAGE_MAP = dict()
 LANGUAGE_MAP['en'] = 'en-US'
-LANGUAGE_MAP['en-US'] = 'en-US'
+
+DEFAULT_LANGUAGE = 'en'
 
 
 class LanguageToolAnalyser(Analyser):
     def __init__(self, language_server: LanguageServer, config: dict, name: str):
         super().__init__(language_server, config, name)
         self.tools = dict()
+        self._tool_backoff = dict()
 
     def _analyse(self, text, doc, offset=0) -> Tuple[List[Diagnostic], List[CodeAction]]:
         diagnostics = list()
         code_actions = list()
         matches = self._get_tool_for_language(doc.language).check(text)
 
         for match in matches:
@@ -159,30 +161,56 @@
         doc_langs = {
             document.language
             for _, document in workspace.documents.items()
         }
         tool_langs = set(self.tools.keys())
 
         for lang in tool_langs - doc_langs:
-            self.tools[lang].close()
-            del self.tools[lang]
+            if any(
+                lang2 in doc_langs
+                for lang2, backoff in self._tool_backoff.items()
+                if backoff == lang
+            ):
+                # do not close a language that is still used by other languages as backoff
+                # XXX: not the most efficient but assuming there's not a lot of backed-off
+                # languages around, this should be fast
+                continue
+
+
+            if lang in self.tools:
+                self.tools[lang].close()
+                del self.tools[lang]
 
     def close(self):
         for lang, tool in self.tools.items():
             tool.close()
         self.tool = dict()
 
     def __del__(self):
         self.close()
 
     def _get_mapped_language(self, language):
-        return LANGUAGE_MAP[language]
+        return LANGUAGE_MAP.get(language, language)
 
     def _get_tool_for_language(self, language):
         lang = self._get_mapped_language(language)
         if lang in self.tools:
             return self.tools[lang]
+        if lang in self._tool_backoff and self._tool_backoff[lang] in self.tools:
+            return self.tools[self._tool_backoff[lang]]
+
+        try:
+            tool = LanguageTool(lang)
+            self.tools[lang] = tool
+        except ValueError:
+            self.language_server.show_message(
+                f'{self.name}: unsupported language: {lang}! Using {DEFAULT_LANGUAGE}',
+                MessageType.Error,
+            )
+
+            if lang == DEFAULT_LANGUAGE:
+                return ValueError("We shouldn't get here")
 
-        tool = LanguageTool(lang)
-        self.tools[lang] = tool
+            tool = self._get_tool_for_language(DEFAULT_LANGUAGE)
+            self._tool_backoff[lang] = DEFAULT_LANGUAGE
 
         return tool
```

### Comparing `textLSP-0.3.0/textLSP/analysers/openai/openai.py` & `textlsp-0.3.1/textLSP/analysers/openai/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,37 +81,46 @@
     def _edit(self, text) -> List[TokenDiff]:
         res = self._chat_endpoint(
             system_msg=self.config.get(self.CONFIGURATION_EDIT_INSTRUCTION, self.SETTINGS_DEFAULT_EDIT_INSTRUCTION),
             user_msg=text,
             model=self.config.get(self.CONFIGURATION_MODEL, self.SETTINGS_DEFAULT_MODEL),
             temperature=self.config.get(self.CONFIGURATION_TEMPERATURE, self.SETTINGS_DEFAULT_TEMPERATURE),
         )
+        logger.debug(f"Response: {res}")
+
         if len(res.choices) > 0:
-            return TokenDiff.token_level_diff(text, res.choices[0].message.content.strip())
+            # the API escapes special characters such as newlines
+            res_text = res.choices[0].message.content.strip().encode().decode("unicode_escape")
+            return TokenDiff.token_level_diff(text, res_text)
 
         return []
 
     def _generate(self, text) -> Optional[str]:
         res = self._chat_endpoint(
             system_msg=text,
             user_msg=None,
             model=self.config.get(self.CONFIGURATION_MODEL, self.SETTINGS_DEFAULT_MODEL),
             temperature=self.config.get(self.CONFIGURATION_TEMPERATURE, self.SETTINGS_DEFAULT_TEMPERATURE),
             max_tokens=self.config.get(self.CONFIGURATION_MAX_TOKEN, self.SETTINGS_DEFAULT_MAX_TOKEN),
         )
+        logger.debug(f"Response: {res}")
 
         if len(res.choices) > 0:
-            return res.choices[0].message.content.strip()
+            # the API escapes special characters such as newlines
+            return res.choices[0].message.content.strip().encode().decode("unicode_escape")
 
         return None
 
     def _analyse(self, text, doc, offset=0) -> Tuple[List[Diagnostic], List[CodeAction]]:
         diagnostics = list()
         code_actions = list()
 
+        # we don not want trailing whitespace
+        text = text.rstrip()
+
         try:
             edits = self._edit(text)
         except APIError as e:
             self.language_server.show_message(
                 str(e),
                 MessageType.Error,
             )
```

### Comparing `textLSP-0.3.0/textLSP/cli.py` & `textlsp-0.3.1/textLSP/cli.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/documents/document.py` & `textlsp-0.3.1/textLSP/documents/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,100 @@
+import copy
 import logging
-import tempfile
 import sys
-import copy
-
-from typing import Optional, Generator, List, Dict
+import tempfile
 from dataclasses import dataclass
 from itertools import chain
+from typing import Dict, Generator, List, Optional
 
+import langdetect
 from lsprotocol.types import (
-    Range,
     Position,
+    Range,
     TextDocumentContentChangeEvent,
     TextDocumentContentChangeEvent_Type1,
     TextDocumentContentChangeEvent_Type2,
 )
 from pygls.workspace import TextDocument
 from pygls.workspace.position_codec import PositionCodec
-from tree_sitter import Language, Parser, Tree, Node
+from tree_sitter import Language, Node, Parser, Tree
 
-from ..utils import get_class, synchronized, git_clone, get_user_cache
-from ..types import (
-    OffsetPositionInterval,
-    OffsetPositionIntervalList,
-    Interval
-)
 from .. import documents
+from ..types import Interval, OffsetPositionInterval, OffsetPositionIntervalList
+from ..utils import get_class, get_user_cache, git_clone, synchronized
 
 logger = logging.getLogger(__name__)
 _codec = PositionCodec()
+langdetect.DetectorFactory.seed = 42
 
 
 class BaseDocument(TextDocument):
+    AUTO_LANG = 'auto'
+
+    CONFIGURATION_LANGUAGE = 'language'
+    CONFIGURATION_MIN_LANG_DETECT = 'min_length_language_detect'
+
+    DEFAULT_LANGUAGE = 'auto:en'
+    DEFAULT_NATURAL_LANGUAGE = 'en'
+    DEFAULT_MIN_LANG_DETECT = 20
+
     def __init__(self, *args, config: Dict = None, **kwargs):
         super().__init__(*args, **kwargs)
         if config is None:
             self.config = dict()
         else:
             self.config = config
 
+        self._language = None
+
+    @property
+    def language(self) -> str:
+        if self._language is None:
+            self._update_langauge(
+                self.config.get(
+                    BaseDocument.CONFIGURATION_LANGUAGE, BaseDocument.DEFAULT_LANGUAGE
+                )
+            )
+            logger.debug(f"Language ({self.uri}): {self._language}")
+
+        return self._language
+
+    def _update_langauge(self, lang: str):
+        """
+        Parameters:
+            lang: str -- Language code or `auto` for automatic language detection.
+                         Optionally: `auto:<default>` such as `auto:en`, to set fallback
+                         language in case the content is too short.
+        """
+        lang = lang.split(':')
+        default_lang = BaseDocument.DEFAULT_NATURAL_LANGUAGE
+
+        if len(lang) > 1:
+            default_lang = lang[1]
+        lang = lang[0]
+
+        if lang == BaseDocument.AUTO_LANG:
+            if len(self.cleaned_source) >= self.config.get(
+                BaseDocument.CONFIGURATION_MIN_LANG_DETECT, BaseDocument.DEFAULT_MIN_LANG_DETECT
+            ):
+                lang = langdetect.detect(self.cleaned_source)
+            else:
+                lang = default_lang
+
+        self._language = lang
+
+
     @property
     def cleaned_source(self) -> str:
         return self.source
 
     @property
     def cleaned_lines(self):
         return self.cleaned_source.splitlines(True)
 
-    @property
-    def language(self) -> str:
-        return 'en'
-
     def position_at_offset(self, offset: int, cleaned=False) -> Position:
         pos = 0
         lines = self.cleaned_lines if cleaned else self.lines
         for lidx, line in enumerate(lines):
             line_len = len(line)
             if pos + line_len > offset:
                 return Position(
@@ -340,33 +381,33 @@
     CONFIGURATION_REPARSE_ALL = 'reparse_all'
     DEFAULT_REPARSE_ALL = True
 
     def __init__(self, language_name, grammar_url, branch, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #######################################################################
         # Do not deepcopy these
-        self._language = self.get_language(language_name, grammar_url, branch)
-        self._parser = self.get_parser(
+        self._ts_language = self.get_language(language_name, grammar_url, branch)
+        self._ts_parser = self.get_parser(
             language_name,
             grammar_url,
             branch,
-            self._language
+            self._ts_language
         )
         self._tree = None
         self._query = self._build_query()
         #######################################################################
 
         self._text_intervals = None
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
-            if k not in {'_language', '_parser', '_tree', '_query'}:
+            if k not in {'_ts_language', '_ts_parser', '_tree', '_query'}:
                 setattr(result, k, copy.deepcopy(v, memo))
             else:
                 setattr(result, k, v)
         return result
 
     @classmethod
     def build_library(cls, name, url, branch=None) -> None:
@@ -401,15 +442,15 @@
         parser.set_language(language)
         return parser
 
     def _build_query(self):
         raise NotImplementedError()
 
     def _parse_source(self):
-        return self._parser.parse(bytes(self.source, 'utf-8'))
+        return self._ts_parser.parse(bytes(self.source, 'utf-8'))
 
     @property
     def tree(self) -> Tree:
         if self._tree is None:
             self._tree = self._parse_source()
         return self._tree
 
@@ -909,15 +950,15 @@
             new_end_byte=new_end_byte,
             start_point=start_point,
             old_end_point=old_end_point,
             new_end_point=new_end_point,
         )
         super()._apply_incremental_change(change)
         new_source = bytes(self.source, 'utf-8')
-        self._tree = self._parser.parse(
+        self._tree = self._ts_parser.parse(
             new_source,
             tree
         )
 
         if old_tree_first_node is not None:
             old_tree_first_node.edit(
                 start_byte=start_byte,
@@ -1082,34 +1123,52 @@
         doc_uri: str,
         config: Dict,
         source: Optional[str] = None,
         version: Optional[int] = None,
         language_id: Optional[str] = None,
         sync_kind=None,
     ) -> TextDocument:
+        lang = config.get(BaseDocument.CONFIGURATION_LANGUAGE)
+        min_len = config.get(BaseDocument.CONFIGURATION_MIN_LANG_DETECT)
         try:
             type = DocumentTypeFactory.get_file_type(language_id)
             cls = get_class(
                 '{}.{}'.format(
                     documents.__name__,
                     type,
                 ),
                 BaseDocument,
             )
+
+            config = config.get(type, dict())
+            if lang is not None and BaseDocument.CONFIGURATION_LANGUAGE not in config:
+                config[BaseDocument.CONFIGURATION_LANGUAGE] = lang
+            if (
+                min_len is not None
+                and BaseDocument.CONFIGURATION_MIN_LANG_DETECT not in config
+            ):
+                config[BaseDocument.CONFIGURATION_MIN_LANG_DETECT] = min_len
+
             return cls(
-                config=config.get(type, dict()),
+                config=config,
                 uri=doc_uri,
                 source=source,
                 version=version,
                 language_id=language_id,
                 sync_kind=sync_kind
             )
         except ImportError:
+            config = dict()
+            if lang is not None:
+                config[BaseDocument.CONFIGURATION_LANGUAGE] = lang
+            if min_len is not None:
+                config[BaseDocument.CONFIGURATION_MIN_LANG_DETECT] = min_len
+
             return BaseDocument(
-                config=dict(),
+                config=config,
                 uri=doc_uri,
                 source=source,
                 version=version,
                 language_id=language_id,
                 sync_kind=sync_kind
             )
```

### Comparing `textLSP-0.3.0/textLSP/documents/latex/latex.py` & `textlsp-0.3.1/textLSP/documents/latex/latex.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             query_str += f'({root} ({self.TEXT} ({self.WORD}) @{self.NODE_CONTENT}))\n'
 
         for root in self.NEWLINE_BEFORE_AFTER_CURLY_PARENT:
             query_str += f'({root} ({self.CURLY_GROUP}) @{self.NODE_NEWLINE_BEFORE_AFTER})\n'
         for root in self.NEWLINE_BEFORE_AFTER:
             query_str += f'({root}) @{self.NODE_NEWLINE_BEFORE_AFTER}\n'
 
-        return self._language.query(query_str)
+        return self._ts_language.query(query_str)
 
     def _iterate_text_nodes(
             self,
             tree: Tree,
             start_point,
             end_point,
     ) -> Generator[TextNode, None, None]:
```

### Comparing `textLSP-0.3.0/textLSP/documents/markdown/markdown.py` & `textlsp-0.3.1/textLSP/documents/markdown/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         for root in self.NEWLINE_AFTER_ONE:
             query_str += f'({root}) @{self.NODE_NEWLINE_AFTER_ONE}\n'
 
         for root in self.NEWLINE_AFTER_TWO:
             query_str += f'({root}) @{self.NODE_NEWLINE_AFTER_TWO}\n'
 
-        return self._language.query(query_str)
+        return self._ts_language.query(query_str)
 
     def _iterate_text_nodes(
             self,
             tree: Tree,
             start_point,
             end_point,
     ) -> Generator[TextNode, None, None]:
```

### Comparing `textLSP-0.3.0/textLSP/documents/org/org.py` & `textlsp-0.3.1/textLSP/documents/org/org.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         for root in self.NEWLINE_AFTER_ONE:
             query_str += f'({root}) @{self.NODE_NEWLINE_AFTER_ONE}\n'
 
         for root in self.NEWLINE_AFTER_TWO:
             query_str += f'({root}) @{self.NODE_NEWLINE_AFTER_TWO}\n'
 
-        return self._language.query(query_str)
+        return self._ts_language.query(query_str)
 
     def _iterate_text_nodes(
             self,
             tree: Tree,
             start_point,
             end_point,
     ) -> Generator[TextNode, None, None]:
```

### Comparing `textLSP-0.3.0/textLSP/documents/txt/txt.py` & `textlsp-0.3.1/textLSP/documents/txt/txt.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/nn_utils.py` & `textlsp-0.3.1/textLSP/nn_utils.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/server.py` & `textlsp-0.3.1/textLSP/server.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/types.py` & `textlsp-0.3.1/textLSP/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,26 +314,30 @@
     type: str
     old_token: str
     new_token: str
     offset: int
     length: int
 
     @staticmethod
+    def _split(text):
+        return [item for item in re.split("(\s)", text) if item != ""]
+
+    @staticmethod
     def token_level_diff(text1, text2) -> List:
-        tokens1 = text1.split()
-        tokens2 = text2.split()
+        tokens1 = TokenDiff._split(text1)
+        tokens2 = TokenDiff._split(text2)
         diff = difflib.SequenceMatcher(None, tokens1, tokens2)
 
         return [
             TokenDiff(
                 type=item[0],
-                old_token=' '.join(tokens1[item[1]:item[2]]),
-                new_token=' '.join(tokens2[item[3]:item[4]]),
-                offset=0 if item[1] == 0 else len(' '.join(tokens1[:item[1]]))+1,
-                length=len(' '.join(tokens1[item[1]:item[2]])),
+                old_token=''.join(tokens1[item[1]:item[2]]),
+                new_token=''.join(tokens2[item[3]:item[4]]),
+                offset=0 if item[1] == 0 else len(''.join(tokens1[:item[1]])),
+                length=len(''.join(tokens1[item[1]:item[2]])),
             )
             for item in diff.get_opcodes()
             if item[0] != 'equal'
         ]
 
     def __str__(self):
         return (
```

### Comparing `textLSP-0.3.0/textLSP/utils.py` & `textlsp-0.3.1/textLSP/utils.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP/workspace.py` & `textlsp-0.3.1/textLSP/workspace.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.3.0/textLSP.egg-info/PKG-INFO` & `textlsp-0.3.1/textLSP.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: textLSP
-Version: 0.3.0
+Version: 0.3.1
 Summary: Language server for text spell and grammar check with various tools.
 Home-page: https://github.com/hangyav/textLSP
 Author: Viktor Hangya
 Author-email: hangyav@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pygls==1.3.0
+Requires-Dist: pygls==1.3.1
 Requires-Dist: lsprotocol==2023.0.1
-Requires-Dist: language-tool-python==2.7.1
-Requires-Dist: tree_sitter==0.20.4
-Requires-Dist: gitpython==3.1.42
+Requires-Dist: language-tool-python==2.8
+Requires-Dist: tree_sitter==0.21.3
+Requires-Dist: gitpython==3.1.43
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: torch==2.2.1
-Requires-Dist: openai==1.13.3
-Requires-Dist: transformers==4.38.2
+Requires-Dist: torch==2.3.0
+Requires-Dist: openai==1.25.0
+Requires-Dist: transformers==4.40.1
 Requires-Dist: sortedcontainers==2.4.0
-Requires-Dist: bitsandbytes==0.42.0
+Requires-Dist: bitsandbytes==0.43.1
+Requires-Dist: langdetect==1.0.9
 Provides-Extra: dev
-Requires-Dist: pytest==8.0.2; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: python-lsp-jsonrpc==1.1.2; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: coverage-threshold==0.4.4; extra == "dev"
 
 # textLSP
 Language server for text spell and grammar check with various AI tools.
 
 _This tool is in early development._
 
@@ -226,14 +227,19 @@
                 on_open = false,
                 on_save = false,
                 on_change = false,
             }
         },
     },
     documents = {
+        -- the language of the documents, could be set to `auto` of `auto:<fallback>`
+        -- to detect automatically, default: auto:en
+        language = "auto:en",
+        -- do not autodetect documents with fewer characters
+        min_length_language_detect = 20,
         org = {
             org_todo_keywords = {
                 'TODO',
                 'IN_PROGRESS',
                 'DONE'
             },
         },
```

### Comparing `textLSP-0.3.0/textLSP.egg-info/SOURCES.txt` & `textlsp-0.3.1/textLSP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

