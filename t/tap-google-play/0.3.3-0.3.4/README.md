# Comparing `tmp/tap_google_play-0.3.3.tar.gz` & `tmp/tap_google_play-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_google_play-0.3.3.tar", max compression
+gzip compressed data, was "tap_google_play-0.3.4.tar", max compression
```

## Comparing `tap_google_play-0.3.3.tar` & `tap_google_play-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/LICENSE
--rw-r--r--   0        0        0     3919 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/README.md
--rw-r--r--   0        0        0     2333 2024-02-19 16:38:04.099696 tap_google_play-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       23 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/tap_google_play/__init__.py
--rw-r--r--   0        0        0      142 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/tap_google_play/__main__.py
--rw-r--r--   0        0        0      195 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/tap_google_play/client.py
--rw-r--r--   0        0        0     2479 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/tap_google_play/streams.py
--rw-r--r--   0        0        0     1103 2024-02-19 16:37:47.539723 tap_google_play-0.3.3/tap_google_play/tap.py
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 tap_google_play-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3919 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/README.md
+-rw-r--r--   0        0        0     2353 2024-05-06 14:55:18.738773 tap_google_play-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/tap_google_play/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/tap_google_play/__main__.py
+-rw-r--r--   0        0        0      194 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/tap_google_play/client.py
+-rw-r--r--   0        0        0     2479 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/tap_google_play/streams.py
+-rw-r--r--   0        0        0     1103 2024-05-06 14:55:14.722758 tap_google_play-0.3.4/tap_google_play/tap.py
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 tap_google_play-0.3.4/PKG-INFO
```

### Comparing `tap_google_play-0.3.3/LICENSE` & `tap_google_play-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_google_play-0.3.3/README.md` & `tap_google_play-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `tap_google_play-0.3.3/pyproject.toml` & `tap_google_play-0.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 requires = [
   "poetry-core==1.8",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-google-play"
-version = "0.3.3"
+version = "0.3.4"
 description = "`tap-google-play` is a Singer tap for GooglePlay, built with the Meltano SDK for Singer Taps."
 readme = "README.md"
 authors = [
   "hotglue <hello@hotglue.xyz>",
   "Edgar Ramírez-Mondragón <edgarrmondragon@hey.com>",
 ]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrmondragon@hey.com>"]
 keywords = ["ELT", "GooglePlay", "Meltano", "singer.io"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-singer-sdk = "~=0.35.0"
+singer-sdk = "~=0.37.0"
 google-play-scraper = { version = "==1.2.4", python = "<4" }
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7"
-singer-sdk = { version = "~=0.35.1", extras = ["testing"] }
+singer-sdk = { version = "~=0.37.0", extras = ["testing"] }
 
 [tool.poetry.scripts]
 # CLI declaration
 tap-google-play = 'tap_google_play.tap:TapGooglePlay.cli'
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -58,30 +58,30 @@
   "FIX002", # line-contains-todo
 ]
 select = ["ALL"]
 unfixable = [
   "ERA001", # commented-out-code
 ]
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "noxfile.py" = ["ANN"]
 "tests/*" = [
   "ANN201", # missing-return-type-public-function
   "S101",   # assert
   "SLF001", # private-member-access
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["tap_google_play"]
 required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 addopts = "-vvv"
 filterwarnings = [
   "error",
   "default:No records were available to test:UserWarning",
```

### Comparing `tap_google_play-0.3.3/tap_google_play/streams.py` & `tap_google_play-0.3.4/tap_google_play/streams.py`

 * *Files identical despite different names*

### Comparing `tap_google_play-0.3.3/tap_google_play/tap.py` & `tap_google_play-0.3.4/tap_google_play/tap.py`

 * *Files identical despite different names*

### Comparing `tap_google_play-0.3.3/PKG-INFO` & `tap_google_play-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-google-play
-Version: 0.3.3
+Version: 0.3.4
 Summary: `tap-google-play` is a Singer tap for GooglePlay, built with the Meltano SDK for Singer Taps.
 License: Apache-2.0
 Keywords: ELT,GooglePlay,Meltano,singer.io
 Author: hotglue
 Author-email: hello@hotglue.xyz
 Maintainer: Edgar Ramírez-Mondragón
 Maintainer-email: edgarrmondragon@hey.com
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-play-scraper (==1.2.4) ; python_version < "4"
-Requires-Dist: singer-sdk (>=0.35.0,<0.36.0)
+Requires-Dist: singer-sdk (>=0.37.0,<0.38.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # tap-google-play
 
 <div>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: tap-google-play Version: 0.3.3 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-google-play Version: 0.3.4 Summary: `tap-
 google-play` is a Singer tap for GooglePlay, built with the Meltano SDK for
 Singer Taps. License: Apache-2.0 Keywords: ELT,GooglePlay,Meltano,singer.io
 Author: hotglue Author-email: hello@hotglue.xyz Maintainer: Edgar RamÃ­rez-
 MondragÃ³n Maintainer-email: edgarrmondragon@hey.com Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: google-play-scraper (==1.2.4) ; python_version < "4" Requires-Dist:
-singer-sdk (>=0.35.0,<0.36.0) Description-Content-Type: text/markdown
+singer-sdk (>=0.37.0,<0.38.0) Description-Content-Type: text/markdown
                                # tap-google-play
     _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_R_u_f_f_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 Singer tap for Google Play Reviews. Built with the [Meltano Singer SDK](https:/
    /sdk.meltano.com). Based on [hotglue/tap-google-play](https://gitlab.com/
                            hotglue/tap-google-play).
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` *
 `schema-flattening` * `batch` ## Settings | Setting | Required | Default |
```

