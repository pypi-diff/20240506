# Comparing `tmp/halper-1.0.2.tar.gz` & `tmp/halper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halper-1.0.2.tar", max compression
+gzip compressed data, was "halper-1.0.3.tar", max compression
```

## Comparing `halper-1.0.2.tar` & `halper-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0    34523 2024-02-13 23:27:20.777938 halper-1.0.2/LICENSE
--rw-r--r--   0        0        0     6747 2024-02-13 23:27:20.777938 halper-1.0.2/README.md
--rw-r--r--   0        0        0    10189 2024-02-13 23:27:20.777938 halper-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       20 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/__init__.py
--rw-r--r--   0        0        0       43 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/__version__.py
--rw-r--r--   0        0        0     8897 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/cli.py
--rw-r--r--   0        0        0      591 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/commands/__init__.py
--rw-r--r--   0        0        0     1858 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/commands/categorize_command.py
--rw-r--r--   0        0        0     2185 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/commands/category_display.py
--rw-r--r--   0        0        0     3828 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/commands/command_display.py
--rw-r--r--   0        0        0     1123 2024-02-13 23:27:20.777938 halper-1.0.2/src/halper/commands/edit_description.py
--rw-r--r--   0        0        0     2437 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/commands/hidden_commands.py
--rw-r--r--   0        0        0     1406 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/commands/search.py
--rw-r--r--   0        0        0      120 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/config/__init__.py
--rw-r--r--   0        0        0     1248 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/config/config.py
--rw-r--r--   0        0        0      839 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/constants.py
--rw-r--r--   0        0        0     1178 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/default_config.toml
--rw-r--r--   0        0        0      513 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/models/__init__.py
--rw-r--r--   0        0        0    10678 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/models/database.py
--rw-r--r--   0        0        0    14068 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/models/indexer.py
--rw-r--r--   0        0        0     4726 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/models/parser.py
--rw-r--r--   0        0        0      553 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/__init__.py
--rw-r--r--   0        0        0       91 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/console.py
--rw-r--r--   0        0        0     2933 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/errors.py
--rw-r--r--   0        0        0     3372 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/helpers.py
--rw-r--r--   0        0        0     4220 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/logging.py
--rw-r--r--   0        0        0     2140 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/mankier.py
--rw-r--r--   0        0        0     8648 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/utils/text_parsers.py
--rw-r--r--   0        0        0      182 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/views/__init__.py
--rw-r--r--   0        0        0     4668 2024-02-13 23:27:20.781938 halper-1.0.2/src/halper/views/views.py
--rw-r--r--   0        0        0     7909 1970-01-01 00:00:00.000000 halper-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-06 17:27:38.695808 halper-1.0.3/LICENSE
+-rw-r--r--   0        0        0     6747 2024-05-06 17:27:38.695808 halper-1.0.3/README.md
+-rw-r--r--   0        0        0     9390 2024-05-06 17:27:38.695808 halper-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/__init__.py
+-rw-r--r--   0        0        0     8854 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/cli.py
+-rw-r--r--   0        0        0      591 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/__init__.py
+-rw-r--r--   0        0        0     1858 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/categorize_command.py
+-rw-r--r--   0        0        0     2185 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/category_display.py
+-rw-r--r--   0        0        0     3828 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/command_display.py
+-rw-r--r--   0        0        0     1212 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/edit_description.py
+-rw-r--r--   0        0        0     2437 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/hidden_commands.py
+-rw-r--r--   0        0        0     1406 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/commands/search.py
+-rw-r--r--   0        0        0      120 2024-05-06 17:27:38.695808 halper-1.0.3/src/halper/config/__init__.py
+-rw-r--r--   0        0        0     1248 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/config/config.py
+-rw-r--r--   0        0        0      857 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/constants.py
+-rw-r--r--   0        0        0     1178 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/default_config.toml
+-rw-r--r--   0        0        0      513 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/models/__init__.py
+-rw-r--r--   0        0        0    10824 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/models/database.py
+-rw-r--r--   0        0        0    14068 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/models/indexer.py
+-rw-r--r--   0        0        0     4726 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/models/parser.py
+-rw-r--r--   0        0        0      553 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/console.py
+-rw-r--r--   0        0        0     2933 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/errors.py
+-rw-r--r--   0        0        0     3372 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/helpers.py
+-rw-r--r--   0        0        0     4220 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/logging.py
+-rw-r--r--   0        0        0     2108 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/mankier.py
+-rw-r--r--   0        0        0     8648 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/utils/text_parsers.py
+-rw-r--r--   0        0        0      182 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/views/__init__.py
+-rw-r--r--   0        0        0     4669 2024-05-06 17:27:38.699808 halper-1.0.3/src/halper/views/views.py
+-rw-r--r--   0        0        0     7905 1970-01-01 00:00:00.000000 halper-1.0.3/PKG-INFO
```

### Comparing `halper-1.0.2/LICENSE` & `halper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/README.md` & `halper-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/pyproject.toml` & `halper-1.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,65 +7,63 @@
     description = "One stop shop for command line help."
     homepage    = "https://github.com/natelandau/halp"
     keywords    = ["bash", "cli", "dotfiles", "shell", "zsh"]
     license     = "AGPL-3.0-or-later"
     name        = "halper"
     readme      = "README.md"
     repository  = "https://github.com/natelandau/halp"
-    version     = "1.0.2"
+    version     = "1.0.3"
 
     [tool.poetry.scripts] # https://python-poetry.org/docs/pyproject/#scripts
         halp = "halper.cli:app"
 
     [tool.poetry.dependencies]
         confz       = "^2.0.1"
-        inflect     = "^7.0.0"
+        inflect     = "^7.2.1"
         loguru      = "^0.7.2"
-        markdownify = "^0.11.6"
+        markdownify = "^0.12.1"
         parsy       = "^2.1"
-        peewee      = "^3.17.0"
+        peewee      = "^3.17.3"
         python      = "^3.10"
         requests    = "^2.31.0"
-        rich        = "^13.7.0"
+        rich        = "^13.7.1"
         semver      = "^3.0.2"
         sh          = "^2.0.6"
         tomli       = "^2.0.1"
-        typer       = { extras = ["all"], version = "^0.9.0" }
+        typer       = "^0.12.3"
 
     [tool.poetry.group.test.dependencies]
         pytest                 = "^7.4.3"
         pytest-asyncio         = "^0.21.1"
         pytest-clarity         = "^1.0.1"
         pytest-env             = "^1.1.1"
         pytest-mock            = "^3.12.0"
         pytest-pretty-terminal = "^1.1.0"
         pytest-sugar           = "^0.9.7"
         pytest-xdist           = "^3.3.1"
 
     [tool.poetry.group.dev.dependencies]
-        commitizen     = "^3.12.0"
-        coverage       = "^7.3.1"
-        mypy           = "^1.8.0"
-        pdoc           = "^14.0.0"
-        poethepoet     = "^0.24.2"
-        pre-commit     = "^3.5.0"
-        ruff           = "^0.2.0"
-        sh             = "^2.0.4"
+        commitizen     = "^3.24.0"
+        coverage       = "^7.5.0"
+        mypy           = "^1.10.0"
+        pdoc           = "^14.4.0"
+        poethepoet     = "^0.26.0"
+        pre-commit     = "^3.7.0"
+        ruff           = "^0.4.3"
         shellcheck-py  = "^0.9.0.5"
         types-requests = "^2.31.0.20240106"
-        typos          = "^1.17.1"
-        vulture        = "^2.10"
+        typos          = "^1.20.10"
 
 [tool.commitizen]
     bump_message               = "bump(release): v$current_version → v$new_version"
     changelog_merge_prerelease = true
     tag_format                 = "v$version"
     update_changelog_on_bump   = true
-    version                    = "1.0.2"
-    version_files              = ["pyproject.toml:version", "src/halper/__version__.py:__version__"]
+    version_files              = ["pyproject.toml:version", "src/halper/constants.py:VERSION"]
+    version_provider           = "poetry"
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html#report
     exclude_lines = [
         'def __repr__',
         'except [\w\s\._]+ as .*:',
         'log\.critical',
         'log\.debug',
@@ -91,20 +89,14 @@
     command_line = "--module pytest"
     data_file    = "reports/.coverage"
     source       = ["src"]
 
 [tool.coverage.xml]
     output = "reports/coverage.xml"
 
-[tool.interrogate]
-    exclude            = ["build", "docs", "tests"]
-    fail-under         = 90
-    ignore-init-method = true
-    verbose            = 2
-
 [tool.mypy] # https://mypy.readthedocs.io/en/latest/config_file.html
     disallow_any_unimported = false
     disallow_subclassing_any = false
     disallow_untyped_decorators = false
     disallow_untyped_defs = true
     exclude = [
         'tests/', # TOML literal string (single-quotes, regex okay, no escaping necessary)
@@ -162,17 +154,14 @@
     fix            = true
     line-length    = 100
     output-format  = "grouped"
     src            = ["src", "tests"]
     target-version = "py310"
 
     [tool.ruff.lint]
-        # Avoiding flagging (and removing) `V101` from any `# noqa`
-        # directives, despite Ruff's lack of support for `vulture`.
-        external = ["V"]
         ignore = [
             "B006",    # mutable-argument-default
             "B008",    # function-call-in-default-argument
             "D107",    # undocumented-public-init
             "D213",    # multi-line-summary-second-line
             "D215",    # section-underline-not-over-indented
             "D406",    # new-line-after-section-name
@@ -262,24 +251,14 @@
 
 [tool.ruff.format]
     indent-style              = "space"
     line-ending               = "auto"
     quote-style               = "double"
     skip-magic-trailing-comma = false
 
-[tool.vulture] # https://pypi.org/project/vulture/
-    # exclude = ["file*.py", "dir/"]
-    # ignore_decorators = ["@app.route", "@require_*"]
-    ignore_names = ["args", "kwargs", "mock_config", "request", "version"]
-    # make_whitelist = true
-    min_confidence = 80
-    paths          = ["src", "tests"]
-    sort_by_size   = true
-    verbose        = false
-
 [tool.poe.tasks]
 
     [tool.poe.tasks.docs]
         cmd = """
 pdoc
       --docformat google
 --output-directory docs
@@ -302,18 +281,19 @@
         [[tool.poe.tasks.lint.sequence]]
             shell = "mypy --config-file pyproject.toml src/"
 
         [[tool.poe.tasks.lint.sequence]]
             shell = "typos"
 
         [[tool.poe.tasks.lint.sequence]]
-            shell = "vulture src/ tests/ --exclude src/valentina/cogs/test_cog.py"
-
-        [[tool.poe.tasks.lint.sequence]]
-            shell = "yamllint ."
+            cmd = """
+                pre-commit run
+                    --all-files
+                    --color always
+                """
 
 [tool.poe.tasks.test]
     help = "Test this package"
 
     [[tool.poe.tasks.test.sequence]]
         cmd = "coverage run"
```

### Comparing `halper-1.0.2/src/halper/cli.py` & `halper-1.0.3/src/halper/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,28 @@
 from pathlib import Path
 from typing import Annotated, Optional
 
 import peewee
 import typer
 from loguru import logger
 
-from halper.__version__ import __version__
-
 # isort:skip
 from halper.commands import (
     categorize_command,
     category_display,
     command_display,
     command_list,
     edit_command_description,
     hide_commands,
     list_hidden_commands,
     search_commands,
     unhide_commands,
 )
 from halper.config import HalpConfig
-from halper.constants import APP_DIR, DB, SearchType
+from halper.constants import APP_DIR, DB, VERSION, SearchType
 from halper.models import Database, Indexer
 from halper.utils import (
     check_python_version,
     console,
     edit_config,
     instantiate_logger,
     validate_config,
@@ -35,15 +33,15 @@
 app = typer.Typer(add_completion=False, rich_markup_mode="rich")
 typer.rich_utils.STYLE_HELPTEXT = ""
 
 
 def version_callback(value: bool) -> None:
     """Print version and exit."""
     if value:
-        console.print(f"halp version: {__version__}")
+        console.print(f"halp version: {VERSION}")
         raise typer.Exit()
 
 
 @app.command()
 def main(  # noqa: PLR0917, C901
     input_string: Annotated[
         Optional[str],
@@ -225,15 +223,15 @@
         raise typer.Exit(0)
 
     validate_config()
 
     # Instantiate Database
     try:
         db = Database(DB)
-        db.instantiate(current_version=__version__)
+        db.instantiate(current_version=VERSION)
     except peewee.OperationalError as e:
         logger.exception(f"Unable to instantiate database: {e}")
         raise typer.Exit(code=1) from e
 
     if db.is_empty() and (not index and not index_full):
         console.print(
             "No commands found.\nMake sure your configuration file is up to date and run [code]halp --index[/code] to index your commands."
```

### Comparing `halper-1.0.2/src/halper/commands/__init__.py` & `halper-1.0.3/src/halper/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/commands/categorize_command.py` & `halper-1.0.3/src/halper/commands/categorize_command.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/commands/category_display.py` & `halper-1.0.3/src/halper/commands/category_display.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/commands/command_display.py` & `halper-1.0.3/src/halper/commands/command_display.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/commands/edit_description.py` & `halper-1.0.3/src/halper/commands/edit_description.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,22 @@
     """Edit command description by ID."""
     command = Command.get_or_none(Command.id == command_id)
     if not command:
         logger.error(f"No command found with ID {command_id}")
         raise typer.Exit(code=1)
 
     console.print(f"Editing description for command [code]{command.name}[/code]")
-    console.print(f"Current description: [code]{command.description}[/code]")
+    console.print(f"Current description: [code]{command.escaped_desc}[/code]")
     console.rule()
     new_description = Prompt.ask("New description")
 
-    confirm = Prompt.ask(f"Set description to [code]{new_description}[/code]?", choices=["y", "n"])
+    new_description_display = new_description.replace("[", "\\[")
+    confirm = Prompt.ask(
+        f"Set description to [code]{new_description_display}[/code]?", choices=["y", "n"]
+    )
     if confirm.lower() == "n":
         raise typer.Abort()
 
     command.description = new_description
     command.has_custom_description = True
     command.save()
```

### Comparing `halper-1.0.2/src/halper/commands/hidden_commands.py` & `halper-1.0.3/src/halper/commands/hidden_commands.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/commands/search.py` & `halper-1.0.3/src/halper/commands/search.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/config/config.py` & `halper-1.0.3/src/halper/config/config.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/constants.py` & `halper-1.0.3/src/halper/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,7 +41,8 @@
     NAME = "name"
 
 
 APP_DIR = Path(typer.get_app_dir("halp"))
 CONFIG_PATH = APP_DIR / "config.toml"
 DB_PATH = APP_DIR / "halp.sqlite"
 DB = SqliteDatabase(DB_PATH)
+VERSION = "0.1.0"
```

### Comparing `halper-1.0.2/src/halper/default_config.toml` & `halper-1.0.3/src/halper/default_config.toml`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/models/__init__.py` & `halper-1.0.3/src/halper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/models/database.py` & `halper-1.0.3/src/halper/models/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Database models for the HALP app."""
+
 import os
 import re
 
 from loguru import logger
 from peewee import BooleanField, ForeignKeyField, Model, PeeweeException, SqliteDatabase, TextField
 from rich.syntax import Syntax
 from rich.table import Table
@@ -78,14 +79,19 @@
     def __str__(self) -> str:
         """Return string representation of command."""
         return (
             f"{self.name=}\n{self.description=}\n{self.command_type=}\n{self.code=}\n{self.file=}\n"
         )
 
     @property
+    def escaped_desc(self) -> str:
+        """Return escaped description."""
+        return self.description.replace("[", "\\[")
+
+    @property
     def category_names(self) -> list[str]:
         """Return a list of category names associated with this command.
 
         Retrieves the names of categories linked to the current command instance
         from the database, ordered alphabetically by category name.
 
         Returns:
@@ -118,15 +124,15 @@
         """
         grid = Table.grid(expand=False, padding=(0, 1))
         grid.add_column(style="bold")
         grid.add_column()
         grid.add_row("Command:", f"[bold]{self.name}[/bold]")
         if show_id:
             grid.add_row("ID:", f"[cyan]{self.id!s}[/cyan]")
-        grid.add_row("Description:", self.description)
+        grid.add_row("Description:", self.escaped_desc)
         grid.add_row("Categories:", ", ".join(self.category_names))
         grid.add_row("Type:", self.command_type.title())
         grid.add_row("File:", f"[dim]{self.file.path}[/dim]")
         if found_in_tldr:
             grid.add_row("TLDR:", f"View TLDR entry with [code]tldr {self.name}[/code]")
         if full_output:
             grid.add_row("Code:", self.code_syntax(padding=True))
```

### Comparing `halper-1.0.2/src/halper/models/indexer.py` & `halper-1.0.3/src/halper/models/indexer.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/models/parser.py` & `halper-1.0.3/src/halper/models/parser.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/utils/__init__.py` & `halper-1.0.3/src/halper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/utils/errors.py` & `halper-1.0.3/src/halper/utils/errors.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/utils/helpers.py` & `halper-1.0.3/src/halper/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/utils/logging.py` & `halper-1.0.3/src/halper/utils/logging.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/utils/mankier.py` & `halper-1.0.3/src/halper/utils/mankier.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def get_mankier_description(input_string: str) -> str:
     """Query mankier.com for a command's description."""
     # Get the command description as markdown
     url = f"https://www.mankier.com/api/v2/mans/{input_string.split(' ')[0]}.1/sections/Description"
 
     try:
         response = requests.get(url, timeout=15)
-    except Exception as e:  # noqa: BLE001
+    except Exception as e:
         raise typer.Exit(1) from e
 
     if response.status_code != 200:  # noqa: PLR2004
         logger.error(f"Error contacting mankier.com: {response.status_code} {response.reason}")
         raise typer.Exit(1)
 
     if "html" not in response.json():
@@ -50,15 +50,15 @@
 def get_mankier_explanation(input_string: str) -> str:
     """Query mankier.com for a command's explanation."""
     url = "https://www.mankier.com/api/explain/"
     params = {"q": input_string}
 
     try:
         response = requests.get(url, params=params, timeout=15)
-    except Exception as e:  # noqa: BLE001
+    except Exception as e:
         raise typer.Exit(1) from e
 
     if response.status_code != 200:  # noqa: PLR2004
         logger.error(f"Error contacting mankier.com: {response.status_code} {response.reason}")
         raise typer.Exit(1)
 
     return strip_last_two_lines(response.text)
```

### Comparing `halper-1.0.2/src/halper/utils/text_parsers.py` & `halper-1.0.3/src/halper/utils/text_parsers.py`

 * *Files identical despite different names*

### Comparing `halper-1.0.2/src/halper/views/views.py` & `halper-1.0.3/src/halper/views/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     for c in commands_to_display:
         if only_exports and c.command_type != CommandType.EXPORT.name:
             continue
         if not only_exports and not full_output and c.command_type == CommandType.EXPORT.name:
             continue
 
         description = (
-            c.description
+            c.escaped_desc
             if c.description
             else c.code_syntax()
             if c.command_type in {CommandType.ALIAS.name, CommandType.EXPORT.name}
             else ""
         )
         row_values = [
             c.name,
```

### Comparing `halper-1.0.2/PKG-INFO` & `halper-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: halper
-Version: 1.0.2
+Version: 1.0.3
 Summary: One stop shop for command line help.
 Home-page: https://github.com/natelandau/halp
 License: AGPL-3.0-or-later
 Keywords: bash,cli,dotfiles,shell,zsh
 Author: Nate Landau
 Author-email: github@natenate.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: confz (>=2.0.1,<3.0.0)
-Requires-Dist: inflect (>=7.0.0,<8.0.0)
+Requires-Dist: inflect (>=7.2.1,<8.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: markdownify (>=0.11.6,<0.12.0)
+Requires-Dist: markdownify (>=0.12.1,<0.13.0)
 Requires-Dist: parsy (>=2.1,<3.0)
-Requires-Dist: peewee (>=3.17.0,<4.0.0)
+Requires-Dist: peewee (>=3.17.3,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: semver (>=3.0.2,<4.0.0)
 Requires-Dist: sh (>=2.0.6,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/natelandau/halp
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/halper.svg)](https://badge.fury.io/py/halper) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/halper) [![Python Code Checker](https://github.com/natelandau/halp/actions/workflows/automated-tests.yml/badge.svg)](https://github.com/natelandau/halp/actions/workflows/automated-tests.yml) [![codecov](https://codecov.io/gh/natelandau/halp/graph/badge.svg?token=GQ0UO3YCJO)](https://codecov.io/gh/natelandau/halp)
 
 # Halp
```

