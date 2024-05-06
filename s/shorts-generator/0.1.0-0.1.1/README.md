# Comparing `tmp/shorts_generator-0.1.0.tar.gz` & `tmp/shorts_generator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shorts_generator-0.1.0.tar", max compression
+gzip compressed data, was "shorts_generator-0.1.1.tar", max compression
```

## Comparing `shorts_generator-0.1.0.tar` & `shorts_generator-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1068 2024-05-03 11:39:30.017093 shorts_generator-0.1.0/LICENSE
--rw-r--r--   0        0        0      194 2024-05-06 05:11:25.315546 shorts_generator-0.1.0/README.md
--rw-r--r--   0        0        0      714 2024-05-06 05:16:13.688589 shorts_generator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1518 2024-05-06 05:06:54.931154 shorts_generator-0.1.0/scripts/generate_shorts.py
--rw-r--r--   0        0        0        0 2024-05-03 14:16:25.111236 shorts_generator-0.1.0/shorts_generator/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 12:50:39.438344 shorts_generator-0.1.0/shorts_generator/configs/__init__.py
--rw-r--r--   0        0        0      699 2024-05-05 05:46:26.768359 shorts_generator-0.1.0/shorts_generator/configs/actor.py
--rw-r--r--   0        0        0      293 2024-05-05 05:32:14.311637 shorts_generator-0.1.0/shorts_generator/configs/voice.py
--rw-r--r--   0        0        0     2197 2024-05-06 05:04:08.702661 shorts_generator-0.1.0/shorts_generator/generator.py
--rw-r--r--   0        0        0      371 2024-05-05 13:13:59.371612 shorts_generator-0.1.0/shorts_generator/generators/__init__.py
--rw-r--r--   0        0        0      327 2024-05-05 05:32:28.964131 shorts_generator-0.1.0/shorts_generator/generators/audio.py
--rw-r--r--   0        0        0      648 2024-05-06 05:04:08.702730 shorts_generator-0.1.0/shorts_generator/generators/image.py
--rw-r--r--   0        0        0     2035 2024-05-05 05:47:17.724704 shorts_generator-0.1.0/shorts_generator/generators/script.py
--rw-r--r--   0        0        0     2478 2024-05-06 02:49:16.221952 shorts_generator-0.1.0/shorts_generator/generators/video.py
--rw-r--r--   0        0        0     1573 2024-05-06 05:04:08.702789 shorts_generator-0.1.0/shorts_generator/workspace.py
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 shorts_generator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 11:39:30.017093 shorts_generator-0.1.1/LICENSE
+-rw-r--r--   0        0        0      577 2024-05-06 05:40:35.574806 shorts_generator-0.1.1/README.md
+-rw-r--r--   0        0        0      732 2024-05-06 05:42:00.865420 shorts_generator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1518 2024-05-06 05:06:54.931154 shorts_generator-0.1.1/scripts/generate_shorts.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:16:25.111236 shorts_generator-0.1.1/shorts_generator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 12:50:39.438344 shorts_generator-0.1.1/shorts_generator/configs/__init__.py
+-rw-r--r--   0        0        0      699 2024-05-05 05:46:26.768359 shorts_generator-0.1.1/shorts_generator/configs/actor.py
+-rw-r--r--   0        0        0      293 2024-05-05 05:32:14.311637 shorts_generator-0.1.1/shorts_generator/configs/voice.py
+-rw-r--r--   0        0        0     2197 2024-05-06 05:04:08.702661 shorts_generator-0.1.1/shorts_generator/generator.py
+-rw-r--r--   0        0        0      371 2024-05-05 13:13:59.371612 shorts_generator-0.1.1/shorts_generator/generators/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-05 05:32:28.964131 shorts_generator-0.1.1/shorts_generator/generators/audio.py
+-rw-r--r--   0        0        0      648 2024-05-06 05:04:08.702730 shorts_generator-0.1.1/shorts_generator/generators/image.py
+-rw-r--r--   0        0        0     2035 2024-05-05 05:47:17.724704 shorts_generator-0.1.1/shorts_generator/generators/script.py
+-rw-r--r--   0        0        0     2478 2024-05-06 02:49:16.221952 shorts_generator-0.1.1/shorts_generator/generators/video.py
+-rw-r--r--   0        0        0     1573 2024-05-06 05:04:08.702789 shorts_generator-0.1.1/shorts_generator/workspace.py
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 shorts_generator-0.1.1/PKG-INFO
```

### Comparing `shorts_generator-0.1.0/LICENSE` & `shorts_generator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/pyproject.toml` & `shorts_generator-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shorts-generator"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Jingun Hong <jingun.hong@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/python-poetry/poetry"
 packages = [
     { include = "shorts_generator" },
@@ -13,14 +13,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 openai = "^1.25.1"
 requests = "^2.31.0"
 moviepy = "^1.0.3"
 argparse = "^1.4.0"
+pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 requests-mock = "^1.12.1"
```

### Comparing `shorts_generator-0.1.0/scripts/generate_shorts.py` & `shorts_generator-0.1.1/scripts/generate_shorts.py`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/shorts_generator/configs/actor.py` & `shorts_generator-0.1.1/shorts_generator/configs/actor.py`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/shorts_generator/generator.py` & `shorts_generator-0.1.1/shorts_generator/generator.py`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/shorts_generator/generators/image.py` & `shorts_generator-0.1.1/shorts_generator/generators/image.py`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/shorts_generator/generators/script.py` & `shorts_generator-0.1.1/shorts_generator/generators/script.py`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/shorts_generator/generators/video.py` & `shorts_generator-0.1.1/shorts_generator/generators/video.py`

 * *Files identical despite different names*

### Comparing `shorts_generator-0.1.0/shorts_generator/workspace.py` & `shorts_generator-0.1.1/shorts_generator/workspace.py`

 * *Files identical despite different names*

