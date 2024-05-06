# Comparing `tmp/mkdocs_macros_adr_summary-0.1.0.tar.gz` & `tmp/mkdocs_macros_adr_summary-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_macros_adr_summary-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_macros_adr_summary-1.0.0.tar", max compression
```

## Comparing `mkdocs_macros_adr_summary-0.1.0.tar` & `mkdocs_macros_adr_summary-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1073 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/LICENSE
--rw-r--r--   0        0        0     5377 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/README.md
--rw-r--r--   0        0        0      341 2024-01-26 18:09:36.079975 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/__init__.py
--rw-r--r--   0        0        0      459 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/factory.py
--rw-r--r--   0        0        0      643 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/interfaces.py
--rw-r--r--   0        0        0       64 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/parser/__init__.py
--rw-r--r--   0        0        0     2835 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/parser/base.py
--rw-r--r--   0        0        0      218 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/parser/exceptions.py
--rw-r--r--   0        0        0     1974 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/parser/madr3.py
--rw-r--r--   0        0        0     2523 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/parser/nygard.py
--rw-r--r--   0        0        0       99 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/parser/types.py
--rw-r--r--   0        0        0      887 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/plugin.py
--rw-r--r--   0        0        0        0 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/py.typed
--rw-r--r--   0        0        0      885 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/renderer.py
--rw-r--r--   0        0        0      309 2024-01-26 18:09:20.799908 mkdocs_macros_adr_summary-0.1.0/mkdocs_macros_adr_summary/template.jinja
--rw-r--r--   0        0        0     2953 2024-01-26 18:09:36.075976 mkdocs_macros_adr_summary-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7037 1970-01-01 00:00:00.000000 mkdocs_macros_adr_summary-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-06 09:36:56.240038 mkdocs_macros_adr_summary-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5425 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/README.md
+-rw-r--r--   0        0        0     1496 2024-05-06 09:37:06.528055 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/__init__.py
+-rw-r--r--   0        0        0     1653 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/factory.py
+-rw-r--r--   0        0        0     1836 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/interfaces.py
+-rw-r--r--   0        0        0     1707 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/__init__.py
+-rw-r--r--   0        0        0     4975 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/base.py
+-rw-r--r--   0        0        0     1373 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/exceptions.py
+-rw-r--r--   0        0        0     3804 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/madr2.py
+-rw-r--r--   0        0        0     3129 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/madr3.py
+-rw-r--r--   0        0        0     3167 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/nygard.py
+-rw-r--r--   0        0        0     1254 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/parser/types.py
+-rw-r--r--   0        0        0     2042 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/py.typed
+-rw-r--r--   0        0        0     2040 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/renderer.py
+-rw-r--r--   0        0        0      238 2024-05-06 09:36:56.244038 mkdocs_macros_adr_summary-1.0.0/mkdocs_macros_adr_summary/template.jinja
+-rw-r--r--   0        0        0     3458 2024-05-06 09:37:06.528055 mkdocs_macros_adr_summary-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7085 1970-01-01 00:00:00.000000 mkdocs_macros_adr_summary-1.0.0/PKG-INFO
```

### Comparing `mkdocs_macros_adr_summary-0.1.0/LICENSE` & `mkdocs_macros_adr_summary-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_macros_adr_summary-0.1.0/README.md` & `mkdocs_macros_adr_summary-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # mkdocs-macros-adr-summary
 ![Static Badge](https://img.shields.io/badge/Python-3.8_%7C_3.9_%7C_3.10_%7C_3.11_%7C_3.12-blue?logo=python&logoColor=white)
 [![Stable Version](https://img.shields.io/pypi/v/mkdocs-macros-adr-summary?color=blue)](https://pypi.org/project/mkdocs-macros-adr-summary/)
 [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta)
 
 [![Python tests](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-tests.yml/badge.svg?branch=main)](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-tests.yml)
-[![Bandit checks](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-bandit.yml/badge.svg?branch=main)](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-bandit.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/5631f62f6dcd3a34d7ae/maintainability)](https://codeclimate.com/github/febus982/mkdocs-macros-adr-summary/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/5631f62f6dcd3a34d7ae/test_coverage)](https://codeclimate.com/github/febus982/mkdocs-macros-adr-summary/test_coverage)
 
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 This is a macro plugin to generates summaries from a list of a ADR documents in a directory.
 
+The single ADR documents file names have to respect this format: `0000-my-decision-title.md`
+
+* start with 4 digits followed by the character `-`
+* the rest of the file name can contain only letters, numbers, dashes and underscores (`[A-Za-z0-9_-]` regex)
+* end with the `.md` extension
+
 Examples and documentation can be found [here](https://febus982.github.io/mkdocs-macros-adr-summary)
 
 The package should be stable enough for daily use. I'll release 1.0.0, and switch to semantic version,
 as soon as support for MADR version 2 has been implemented. Until that breaking changes can be introduced
 and will be documented in the GitHub release description.
 
 ## Quick start
 
 Enable the plugin in `mkdocs.yml`
 
 ```yaml
 plugins:
   - macros:
-        module_name: mkdocs_macros_adr_summary
+      modules:
+        - mkdocs_macros_adr_summary
 ```
 
 Create a markdown page in your mkdocs website and use the `adr_summary` macro providing
 the path containing your ADR files relative to the `mkdocs.yml` file.
 
 ```markdown
 {{ adr_summary(adr_path="docs/adr", adr_style="nygard") }}
@@ -42,79 +48,70 @@
 
 ## More customization
 
 The page output is generated using a jinja template, but you can provide a custom one. The file path
 must still be relative to the `mkdocs.yml` file.
 
 ```markdown
-{{ adr_summary(adr_path="docs/adr", adr_style="MADR3", template_file="other.jinja") }}
+{{ adr_summary(adr_path="docs/adr", adr_style="MADR3",m) }}
 ```
 
 The default template is:
 
 ```markdown
-## Document list
-
-{% for d in documents %}
-* [{{ d.title }}]({{ d.filename }})
-    * `{{ d.date.strftime('%d-%m-%Y') }}`
-    * `{{ d.file_path }}`
-    {% if d.statuses %}
-    * Statuses:
-        {% for status in d.statuses %}
-        * {{ status }}
-        {% endfor %}
-    {% endif %}
+| ID | Date | Decision | Status |
+|----|------|----------|--------|
+{% for d in documents %}| {{ d.document_id }} | {{ d.date.strftime('%d-%m-%Y') if d.date else "-"}} | [{{ d.title }}]({{ d.file_path }}) | {{ d.status }}  |
 {% endfor %}
 ```
 
 The `documents` variable in the jinja template is a Sequence of `ADRDocument` models:
 
 ```python
 @dataclass
 class ADRDocument:
     file_path: str
+    document_id: Optional[int] = None
     title: Optional[str] = None
     date: Optional[date] = None
-    stasdetus: Optional[str] = None
+    status: Optional[str] = None
     statuses: Sequence[str] = tuple()
     deciders: Optional[str] = None
     consulted: Optional[str] = None
     informed: Optional[str] = None
 ```
 
 There are some differences in what metadata is available when using different formats:
 
 |           | Nygard | MADR3 | MADR2 |
 |-----------|--------|-------|-------|
 | file_path | ✅︎     | ✅︎    | ✅︎    |
 | title     | ✅︎     | ✅︎    | ✅︎    |
-| date      | ✅︎     | ✅︎    | TODO  |
-| status    | ⚠      | ✅︎    | TODO  |
-| statuses  | ✅︎     | ⚠     | TODO  |
-| deciders  | ❌      | ✅︎    | TODO  |
-| consulted | ❌      | ✅︎    | TODO  |
-| informed  | ❌      | ✅︎    | TODO  |
+| date      | ✅︎     | ✅︎    | ✅︎    |
+| status    | ⚠      | ✅︎    | ✅︎    |
+| statuses  | ✅︎     | ⚠     | ⚠     |
+| deciders  | ❌      | ✅︎    | ✅︎    |
+| consulted | ❌      | ✅︎    | ❌     |
+| informed  | ❌      | ✅︎    | ❌     |
 
 * **Nygard format**
-  * `status` is the last item `statuses`. (I don't believe we should use multiple
-    statuses, however `adr-tools` allows it)
-  * `deciders`, `consulted` and `informed` are not supported by the format
-* **MADR3**
-  * I wasn't able to find an automated tool supporting superseding documents.
-    By looking at the template it looks like there's a single status.
-    `statuses` will return a list with a single status.
+    * `status` is the last item `statuses`. (I don't believe we should use multiple
+      statuses, however `adr-tools` allows it)
+    * `deciders`, `consulted` and `informed` are not supported by the format
+* **MADR2** and **MADR3**
+    * I wasn't able to find an automated tool supporting superseding documents.
+      By looking at the template it looks like there's a single status.
+      `statuses` will return a list with a single status.
 
 ## Supported ADR formats
 
 The supported ADR formats are:
 * `nygard` format, it is recommended to use [adr-tools](https://github.com/npryce/adr-tools) to manage the directory
 * `MADR` [version 3](https://github.com/adr/madr/blob/3.0.0/template/adr-template.md)
-
-Support for [MADR](https://adr.github.io/madr/) version 2 will be added in a future version.
+* `MADR` [version 2](https://github.com/adr/madr/blob/2.1.2/template/template.md)
 
 ## Commands for development
 
 All the common commands used during development can be run using make targets:
 
 * `make dev-dependencies`: Install dev requirements
 * `make update-dependencies`: Update dev requirements
```

### Comparing `mkdocs_macros_adr_summary-0.1.0/pyproject.toml` & `mkdocs_macros_adr_summary-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-macros-adr-summary"
-version = "0.1.0"
+version = "1.0.0"
 description = "A plugin to generate a summary of a ADR directory"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/mkdocs-macros-adr-summary"
 homepage = "https://febus982.github.io/mkdocs-macros-adr-summary"
 readme = "README.md"
 packages = [{include = "mkdocs_macros_adr_summary"}]
@@ -54,68 +54,91 @@
 python = ">=3.8,<3.13"
 pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-coverage = ">=6.5.0"
-bandit = ">=1.7.6"
-black = ">=22.10.0"
-mkdocs-awesome-pages-plugin = "^2.9.2"
-mkdocs-material = ">=9.1.16"
-mike = ">=2.0.0"
-mypy = ">=0.990"
-pymdown-extensions = ">=10.0.1"
-pytest = ">=7.2.0"
-pytest-asyncio = ">=0.20.3"
-pytest-cov = ">=4.0.0"
-pytest-factoryboy = ">=2.5.0"
-pytest-xdist = ">=3.0.2"
-ruff = ">=0.0.263"
+coverage = "*"
+mkdocs-awesome-pages-plugin = "*"
+mkdocs-material = "*"
+mike = "*"
+mypy = "*"
+pymdown-extensions = "*"
+pytest = "*"
+pytest-cov = "*"
+pytest-factoryboy = "*"
+pytest-xdist = "*"
+ruff = "*"
 types-pyyaml = "^6.0.12.12"
 
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
-minversion = "6.0"
-addopts = "-n auto --cov-report=term-missing"
-testpaths = [
-    "tests",
-]
-
-[tool.mypy]
-files = "mkdocs_macros_adr_summary"
-
-[[tool.mypy.overrides]]
-module = [
-    "mkdocs_macros.*",
-]
-ignore_missing_imports = true
+############################
+### Tools configuration  ###
+############################
 
 [tool.coverage.run]
 branch = true
 source = ["mkdocs_macros_adr_summary"]
-concurrency = ["multiprocessing"]
-parallel = true
+# It's not necessary to configure concurrency here
+# because pytest-cov takes care of that
 
 [tool.coverage.report]
+fail_under = 100
 exclude_also = [
     "pragma: no cover",
     "pass",
     "\\.\\.\\.",
     ]
 
+[tool.mypy]
+files = "mkdocs_macros_adr_summary"
+
+[[tool.mypy.overrides]]
+module = [
+    "mkdocs_macros.*",
+]
+ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+minversion = "6.0"
+addopts = "-n auto --cov-report=term-missing"
+testpaths = [
+    "tests",
+]
 
 [tool.ruff]
-select = ["E", "F", "I"]
-extend-exclude = ["docs"]
+extend-exclude = ["docs", ".tox"]
+target-version = "py38"
 
-[tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]
+[tool.ruff.lint]
+select = [
+    "E",  # pycodestyle
+    "W",  # pycodestyle
+    "F",  # pyflakes
+    "I",  # isort
+    "N",  # pep8-naming
+    "S",  # flake8-bandit
+    "RUF",  # ruff-specific-rules
+]
+# Ignoring rules problematic with formatter
+# https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
+ignore = [
+    "W191",
+    "E111",
+    "E114",
+    "E117",
+    "D206",
+    "D300",
+    "Q000",
+    "Q001",
+    "Q002",
+    "Q003",
+    "COM812",
+    "COM819",
+    "ISC001",
+    "ISC002",
+]
 
-[tool.black]
-target-version = ["py38", "py39", "py310", "py311", "py312"]
-extend-exclude = '''
-(
-  /docs
-)
-'''
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401"]  # Ignore unused imports on init files
+"tests/**/*.py" = ["S101"]  # Allow assert usage on tests
```

### Comparing `mkdocs_macros_adr_summary-0.1.0/PKG-INFO` & `mkdocs_macros_adr_summary-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-adr-summary
-Version: 0.1.0
+Version: 1.0.0
 Summary: A plugin to generate a summary of a ADR directory
 Home-page: https://febus982.github.io/mkdocs-macros-adr-summary
 License: MIT
 Keywords: adr,architecture-decision-records,mkdocs,mkdocs-plugin,mkdocs-macro,mkdocs-macro-plugin,nygard
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.13
@@ -37,39 +37,45 @@
 
 # mkdocs-macros-adr-summary
 ![Static Badge](https://img.shields.io/badge/Python-3.8_%7C_3.9_%7C_3.10_%7C_3.11_%7C_3.12-blue?logo=python&logoColor=white)
 [![Stable Version](https://img.shields.io/pypi/v/mkdocs-macros-adr-summary?color=blue)](https://pypi.org/project/mkdocs-macros-adr-summary/)
 [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta)
 
 [![Python tests](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-tests.yml/badge.svg?branch=main)](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-tests.yml)
-[![Bandit checks](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-bandit.yml/badge.svg?branch=main)](https://github.com/febus982/mkdocs-macros-adr-summary/actions/workflows/python-bandit.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/5631f62f6dcd3a34d7ae/maintainability)](https://codeclimate.com/github/febus982/mkdocs-macros-adr-summary/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/5631f62f6dcd3a34d7ae/test_coverage)](https://codeclimate.com/github/febus982/mkdocs-macros-adr-summary/test_coverage)
 
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 This is a macro plugin to generates summaries from a list of a ADR documents in a directory.
 
+The single ADR documents file names have to respect this format: `0000-my-decision-title.md`
+
+* start with 4 digits followed by the character `-`
+* the rest of the file name can contain only letters, numbers, dashes and underscores (`[A-Za-z0-9_-]` regex)
+* end with the `.md` extension
+
 Examples and documentation can be found [here](https://febus982.github.io/mkdocs-macros-adr-summary)
 
 The package should be stable enough for daily use. I'll release 1.0.0, and switch to semantic version,
 as soon as support for MADR version 2 has been implemented. Until that breaking changes can be introduced
 and will be documented in the GitHub release description.
 
 ## Quick start
 
 Enable the plugin in `mkdocs.yml`
 
 ```yaml
 plugins:
   - macros:
-        module_name: mkdocs_macros_adr_summary
+      modules:
+        - mkdocs_macros_adr_summary
 ```
 
 Create a markdown page in your mkdocs website and use the `adr_summary` macro providing
 the path containing your ADR files relative to the `mkdocs.yml` file.
 
 ```markdown
 {{ adr_summary(adr_path="docs/adr", adr_style="nygard") }}
@@ -79,79 +85,70 @@
 
 ## More customization
 
 The page output is generated using a jinja template, but you can provide a custom one. The file path
 must still be relative to the `mkdocs.yml` file.
 
 ```markdown
-{{ adr_summary(adr_path="docs/adr", adr_style="MADR3", template_file="other.jinja") }}
+{{ adr_summary(adr_path="docs/adr", adr_style="MADR3",m) }}
 ```
 
 The default template is:
 
 ```markdown
-## Document list
-
-{% for d in documents %}
-* [{{ d.title }}]({{ d.filename }})
-    * `{{ d.date.strftime('%d-%m-%Y') }}`
-    * `{{ d.file_path }}`
-    {% if d.statuses %}
-    * Statuses:
-        {% for status in d.statuses %}
-        * {{ status }}
-        {% endfor %}
-    {% endif %}
+| ID | Date | Decision | Status |
+|----|------|----------|--------|
+{% for d in documents %}| {{ d.document_id }} | {{ d.date.strftime('%d-%m-%Y') if d.date else "-"}} | [{{ d.title }}]({{ d.file_path }}) | {{ d.status }}  |
 {% endfor %}
 ```
 
 The `documents` variable in the jinja template is a Sequence of `ADRDocument` models:
 
 ```python
 @dataclass
 class ADRDocument:
     file_path: str
+    document_id: Optional[int] = None
     title: Optional[str] = None
     date: Optional[date] = None
-    stasdetus: Optional[str] = None
+    status: Optional[str] = None
     statuses: Sequence[str] = tuple()
     deciders: Optional[str] = None
     consulted: Optional[str] = None
     informed: Optional[str] = None
 ```
 
 There are some differences in what metadata is available when using different formats:
 
 |           | Nygard | MADR3 | MADR2 |
 |-----------|--------|-------|-------|
 | file_path | ✅︎     | ✅︎    | ✅︎    |
 | title     | ✅︎     | ✅︎    | ✅︎    |
-| date      | ✅︎     | ✅︎    | TODO  |
-| status    | ⚠      | ✅︎    | TODO  |
-| statuses  | ✅︎     | ⚠     | TODO  |
-| deciders  | ❌      | ✅︎    | TODO  |
-| consulted | ❌      | ✅︎    | TODO  |
-| informed  | ❌      | ✅︎    | TODO  |
+| date      | ✅︎     | ✅︎    | ✅︎    |
+| status    | ⚠      | ✅︎    | ✅︎    |
+| statuses  | ✅︎     | ⚠     | ⚠     |
+| deciders  | ❌      | ✅︎    | ✅︎    |
+| consulted | ❌      | ✅︎    | ❌     |
+| informed  | ❌      | ✅︎    | ❌     |
 
 * **Nygard format**
-  * `status` is the last item `statuses`. (I don't believe we should use multiple
-    statuses, however `adr-tools` allows it)
-  * `deciders`, `consulted` and `informed` are not supported by the format
-* **MADR3**
-  * I wasn't able to find an automated tool supporting superseding documents.
-    By looking at the template it looks like there's a single status.
-    `statuses` will return a list with a single status.
+    * `status` is the last item `statuses`. (I don't believe we should use multiple
+      statuses, however `adr-tools` allows it)
+    * `deciders`, `consulted` and `informed` are not supported by the format
+* **MADR2** and **MADR3**
+    * I wasn't able to find an automated tool supporting superseding documents.
+      By looking at the template it looks like there's a single status.
+      `statuses` will return a list with a single status.
 
 ## Supported ADR formats
 
 The supported ADR formats are:
 * `nygard` format, it is recommended to use [adr-tools](https://github.com/npryce/adr-tools) to manage the directory
 * `MADR` [version 3](https://github.com/adr/madr/blob/3.0.0/template/adr-template.md)
-
-Support for [MADR](https://adr.github.io/madr/) version 2 will be added in a future version.
+* `MADR` [version 2](https://github.com/adr/madr/blob/2.1.2/template/template.md)
 
 ## Commands for development
 
 All the common commands used during development can be run using make targets:
 
 * `make dev-dependencies`: Install dev requirements
 * `make update-dependencies`: Update dev requirements
```

