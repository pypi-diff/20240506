# Comparing `tmp/atsphinx_mini18n-0.3.0.tar.gz` & `tmp/atsphinx_mini18n-0.3.1.tar.gz`

## Comparing `atsphinx_mini18n-0.3.0.tar` & `atsphinx_mini18n-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.age.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.editorconfig
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.python-version
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/CHANGES.rst
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/requirements.lock
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.github/release-body.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.github/workflows/deploy-doc.yml
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/.gitignore
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/.ruff.toml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/Makefile
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/conf.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/make.bat
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/changelogs/index.po
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/usage/configuration.po
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/usage/index.po
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/usage/setup.po
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_static/.gitignore
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/_templates/.gitignore
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/changelogs/0.1.0.rst
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/changelogs/0.2.0.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/changelogs/0.2.1.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/changelogs/index.rst
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/usage/configuration.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/usage/index.rst
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/doc/usage/setup.rst
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/src/atsphinx/mini18n/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/src/atsphinx/mini18n/templates/mini18n/index.html
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/src/atsphinx/mini18n/templates/mini18n/snippets/select-lang.html
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/tests/.ruff.toml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/tests/test_it.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/tests/test-root/conf.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/tests/test-root/index.rst
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/tools/archive_changelog.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/.gitignore
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/LICENSE
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/README.rst
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.age.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.editorconfig
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.python-version
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/CHANGES.rst
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/requirements.lock
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/release-body.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/workflows/deploy-doc.yml
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/.gitignore
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/.ruff.toml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/Makefile
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/conf.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/make.bat
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/changelogs/index.po
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/configuration.po
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/index.po
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/setup.po
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_static/.gitignore
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/_templates/.gitignore
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.1.0.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.2.0.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.2.1.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/0.3.0.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/changelogs/index.rst
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/usage/configuration.rst
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/usage/index.rst
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/doc/usage/setup.rst
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/__init__.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/templates/mini18n/index.html
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/templates/mini18n/snippets/select-lang.html
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/.ruff.toml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/test_it.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/test-root/conf.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tests/test-root/index.rst
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/tools/archive_changelog.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/.gitignore
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/README.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 atsphinx_mini18n-0.3.1/PKG-INFO
```

### Comparing `atsphinx_mini18n-0.3.0/.age.toml` & `atsphinx_mini18n-0.3.1/.age.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-current_version = "0.3.0"
+current_version = "0.3.1"
 
 [[files]]
 path = "pyproject.toml"
 search = "version = \"{{current_version}}\""
 replace = "version = \"{{new_version}}\""
 
 [[files]]
```

### Comparing `atsphinx_mini18n-0.3.0/.editorconfig` & `atsphinx_mini18n-0.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/requirements-dev.lock` & `atsphinx_mini18n-0.3.1/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     # via requests
 click==8.1.7
     # via sphinx-intl
 colorama==0.4.6
     # via sphinx-autobuild
 docutils==0.20.1
     # via sphinx
+    # via sphinx-revealjs
     # via sphinx-tabs
 esbonio==0.16.4
 exceptiongroup==1.2.0
     # via cattrs
     # via pytest
 furo==2024.1.29
 idna==3.6
@@ -52,14 +53,15 @@
 lsprotocol==2023.0.1
     # via pygls
 markupsafe==2.1.5
     # via jinja2
 packaging==24.0
     # via pytest
     # via sphinx
+    # via sphinx-revealjs
 platformdirs==4.2.0
     # via esbonio
 pluggy==1.4.0
     # via pytest
 pygls==1.3.0
     # via esbonio
 pygments==2.17.2
@@ -84,19 +86,21 @@
 sphinx==7.1.2
     # via atsphinx-mini18n
     # via esbonio
     # via furo
     # via sphinx-autobuild
     # via sphinx-basic-ng
     # via sphinx-intl
+    # via sphinx-revealjs
     # via sphinx-tabs
 sphinx-autobuild==2021.3.14
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-intl==2.1.0
+sphinx-revealjs==3.0.2
 sphinx-tabs==3.4.5
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
```

### Comparing `atsphinx_mini18n-0.3.0/requirements.lock` & `atsphinx_mini18n-0.3.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/.github/workflows/deploy-doc.yml` & `atsphinx_mini18n-0.3.1/.github/workflows/deploy-doc.yml`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/.github/workflows/main.yml` & `atsphinx_mini18n-0.3.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/.github/workflows/release.yml` & `atsphinx_mini18n-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/Makefile` & `atsphinx_mini18n-0.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/make.bat` & `atsphinx_mini18n-0.3.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/index.po` & `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/changelogs/index.po` & `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/changelogs/index.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/usage/configuration.po` & `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/configuration.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/usage/index.po` & `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/index.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/_locales/ja/LC_MESSAGES/usage/setup.po` & `atsphinx_mini18n-0.3.1/doc/_locales/ja/LC_MESSAGES/usage/setup.po`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/usage/configuration.rst` & `atsphinx_mini18n-0.3.1/doc/usage/configuration.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/doc/usage/setup.rst` & `atsphinx_mini18n-0.3.1/doc/usage/setup.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/src/atsphinx/mini18n/__init__.py` & `atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from subprocess import PIPE, run
 
 from jinja2 import Template
 from sphinx.application import Sphinx
 from sphinx.builders.dummy import DummyBuilder
 from sphinx.config import Config
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 package_root = Path(__file__).parent.resolve()
 
 
 @dataclass
 class BuildArgs:
-    """Parameter class to build other langage."""
+    """Parameter class to build other language."""
 
     app: Sphinx
     builder: str
     lang: str
 
 
 class Mini18nBuilderBase(DummyBuilder):
@@ -105,19 +105,30 @@
 
 
 def get_template_dir() -> str:  # noqa: D103
     return str(package_root / "templates")
 
 
 def setup(app: Sphinx):  # noqa: D103
-    register_i18n_builders(app)
     app.add_config_value("mini18n_default_language", None, "env")
     app.add_config_value("mini18n_support_languages", [], "env")
     app.add_config_value("mini18n_basepath", "/", "env")
     app.add_config_value("mini18n_select_lang_label", "Language:", "env")
     app.connect("config-inited", autocomplete_config)
+
+    # IMPORTANT!!
+    # This is verty dirty hack to work it for any builders of third-party extensions.
+    _preload_builder = app.preload_builder
+
+    def preload_builder(buildername):
+        """Wrap for :meth:`sphinx.application.Sphinx.preload_builder`."""
+        register_i18n_builders(app)
+        _preload_builder(buildername)
+
+    app.preload_builder = preload_builder
+
     return {
         "version": __version__,
         "env_version": 1,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `atsphinx_mini18n-0.3.0/src/atsphinx/mini18n/templates/mini18n/index.html` & `atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/templates/mini18n/index.html`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/src/atsphinx/mini18n/templates/mini18n/snippets/select-lang.html` & `atsphinx_mini18n-0.3.1/src/atsphinx/mini18n/templates/mini18n/snippets/select-lang.html`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/.gitignore` & `atsphinx_mini18n-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/LICENSE` & `atsphinx_mini18n-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/README.rst` & `atsphinx_mini18n-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_mini18n-0.3.0/pyproject.toml` & `atsphinx_mini18n-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atsphinx-mini18n"
-version = "0.3.0"
+version = "0.3.1"
 description = "Sphinx builder for i18n site on single deployment"
 authors = [{name = "Kazuya Takei", email = "myself@attakei.net"}]
 license = "Apache-2.0"
 requires-python = ">= 3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Sphinx",
@@ -44,14 +44,15 @@
     "pytest ==7.*",
     "esbonio~=0.16.4",
     "sphinx-tabs~=3.4.5",
     "sphinx-autobuild~=2021.3.14",
     "furo~=2024.1.29",
     "beautifulsoup4~=4.12.3",
     "sphinx-intl~=2.1.0",
+    "sphinx-revealjs~=3.0.2",
 ]
 
 [tool.rye.scripts]
 setup = {chain = ["setup:sync", "setup:pre-commit"]}
 "setup:sync" = "rye sync --no-lock --all-features"
 "setup:pre-commit" = "pre-commit install"
 doc = "make -C doc"
```

### Comparing `atsphinx_mini18n-0.3.0/PKG-INFO` & `atsphinx_mini18n-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atsphinx-mini18n
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sphinx builder for i18n site on single deployment
 Project-URL: Repository, https://github.com/atsphinx/mini18n
 Project-URL: Issues, https://github.com/atsphinx/mini18n/issues
 Project-URL: Document, https://atsphinx.github.io/mini18n/
 Author-email: Kazuya Takei <myself@attakei.net>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

