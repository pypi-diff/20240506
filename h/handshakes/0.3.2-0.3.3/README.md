# Comparing `tmp/handshakes-0.3.2.tar.gz` & `tmp/handshakes-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handshakes-0.3.2.tar", max compression
+gzip compressed data, was "handshakes-0.3.3.tar", max compression
```

## Comparing `handshakes-0.3.2.tar` & `handshakes-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,49 @@
--rw-r--r--   0        0        0       23 2024-03-28 13:40:44.249770 handshakes-0.3.2/handshake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 19:36:05.913478 handshakes-0.3.2/handshake/services/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 19:36:05.880180 handshakes-0.3.2/handshake/services/CommandLine/__init__.py
--rw-r--r--   0        0        0    10245 2024-03-21 18:58:35.713013 handshakes-0.3.2/handshake/services/CommandLine/_init.py
--rw-r--r--   0        0        0     4276 2024-03-17 18:56:17.875233 handshakes-0.3.2/handshake/services/CommandLine/center.py
--rw-r--r--   0        0        0       16 2024-03-21 18:58:35.714109 handshakes-0.3.2/handshake/services/DBService/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-21 18:58:35.716132 handshakes-0.3.2/handshake/services/DBService/lifecycle.py
--rw-r--r--   0        0        0     4356 2024-02-18 16:56:43.494324 handshakes-0.3.2/handshake/services/DBService/migrator.py
--rw-r--r--   0        0        0      599 2024-01-18 18:47:07.797836 handshakes-0.3.2/handshake/services/DBService/models/__init__.py
--rw-r--r--   0        0        0      969 2024-01-18 18:47:07.798848 handshakes-0.3.2/handshake/services/DBService/models/attachmentBase.py
--rw-r--r--   0        0        0     2043 2024-03-13 18:17:40.351615 handshakes-0.3.2/handshake/services/DBService/models/config_base.py
--rw-r--r--   0        0        0     1671 2024-02-12 19:08:51.042688 handshakes-0.3.2/handshake/services/DBService/models/dynamic_base.py
--rw-r--r--   0        0        0     1038 2024-03-13 18:17:40.352991 handshakes-0.3.2/handshake/services/DBService/models/enums.py
--rw-r--r--   0        0        0     6047 2024-03-21 18:58:35.718163 handshakes-0.3.2/handshake/services/DBService/models/result_base.py
--rw-r--r--   0        0        0     1208 2024-01-18 18:47:07.805848 handshakes-0.3.2/handshake/services/DBService/models/static_base.py
--rw-r--r--   0        0        0     2153 2024-03-21 18:58:35.720129 handshakes-0.3.2/handshake/services/DBService/models/types.py
--rw-r--r--   0        0        0       52 2024-01-17 19:36:05.893788 handshakes-0.3.2/handshake/services/DBService/sanic_free_shared.py
--rw-r--r--   0        0        0      462 2024-02-18 08:30:45.354410 handshakes-0.3.2/handshake/services/DBService/scripts/bump-v3.sql
--rw-r--r--   0        0        0     2293 2024-01-18 18:47:07.808459 handshakes-0.3.2/handshake/services/DBService/scripts/bump-v4.sql
--rw-r--r--   0        0        0      227 2024-02-12 19:08:51.047367 handshakes-0.3.2/handshake/services/DBService/scripts/bump-v5.sql
--rw-r--r--   0        0        0      381 2024-03-13 18:17:40.352991 handshakes-0.3.2/handshake/services/DBService/scripts/bump-v6.sql
--rw-r--r--   0        0        0      419 2024-02-07 18:28:47.928557 handshakes-0.3.2/handshake/services/DBService/scripts/revert-v4.sql
--rw-r--r--   0        0        0     1557 2024-01-18 18:47:07.809470 handshakes-0.3.2/handshake/services/DBService/scripts/revert-v5.sql
--rw-r--r--   0        0        0      101 2024-02-12 19:08:51.048386 handshakes-0.3.2/handshake/services/DBService/scripts/revert-v6.sql
--rw-r--r--   0        0        0      463 2024-03-13 18:17:40.354108 handshakes-0.3.2/handshake/services/DBService/scripts/revert-v7.sql
--rw-r--r--   0        0        0      782 2024-02-12 19:08:51.050465 handshakes-0.3.2/handshake/services/DBService/shared.py
--rw-r--r--   0        0        0        0 2024-01-17 19:36:05.898026 handshakes-0.3.2/handshake/services/Endpoints/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 19:36:05.898026 handshakes-0.3.2/handshake/services/Endpoints/blueprints/__init__.py
--rw-r--r--   0        0        0     8071 2024-03-21 18:58:35.722133 handshakes-0.3.2/handshake/services/Endpoints/blueprints/coreEndpoints.py
--rw-r--r--   0        0        0     1492 2024-02-12 19:08:51.057789 handshakes-0.3.2/handshake/services/Endpoints/blueprints/utils.py
--rw-r--r--   0        0        0     1990 2024-02-19 20:32:12.841919 handshakes-0.3.2/handshake/services/Endpoints/blueprints/writeServices.py
--rw-r--r--   0        0        0      445 2024-03-28 13:40:44.252291 handshakes-0.3.2/handshake/services/Endpoints/center.py
--rw-r--r--   0        0        0     1084 2024-03-13 18:17:40.356438 handshakes-0.3.2/handshake/services/Endpoints/core.py
--rw-r--r--   0        0        0      285 2024-01-17 19:36:05.902025 handshakes-0.3.2/handshake/services/Endpoints/errorHandling.py
--rw-r--r--   0        0        0      985 2024-03-21 18:58:35.724131 handshakes-0.3.2/handshake/services/Endpoints/internalEndpoints.py
--rw-r--r--   0        0        0      132 2024-01-17 19:36:05.903026 handshakes-0.3.2/handshake/services/Endpoints/static_server.py
--rw-r--r--   0        0        0        0 2024-01-17 19:36:05.903026 handshakes-0.3.2/handshake/services/SchedularService/__init__.py
--rw-r--r--   0        0        0     3077 2024-03-13 18:17:40.358180 handshakes-0.3.2/handshake/services/SchedularService/center.py
--rw-r--r--   0        0        0     8544 2024-03-21 18:58:35.727122 handshakes-0.3.2/handshake/services/SchedularService/completeTestRun.py
--rw-r--r--   0        0        0      369 2024-01-17 19:36:05.905114 handshakes-0.3.2/handshake/services/SchedularService/constants.py
--rw-r--r--   0        0        0     2103 2024-02-12 19:08:51.073108 handshakes-0.3.2/handshake/services/SchedularService/deleteRuns.py
--rw-r--r--   0        0        0     2374 2024-02-12 19:08:51.076122 handshakes-0.3.2/handshake/services/SchedularService/handlePending.py
--rw-r--r--   0        0        0     2283 2024-03-13 18:17:40.359538 handshakes-0.3.2/handshake/services/SchedularService/handleTestResults.py
--rw-r--r--   0        0        0     1548 2024-02-12 19:08:51.081122 handshakes-0.3.2/handshake/services/SchedularService/lifecycle.py
--rw-r--r--   0        0        0     6499 2024-03-21 18:58:35.729131 handshakes-0.3.2/handshake/services/SchedularService/modifySuites.py
--rw-r--r--   0        0        0     1590 2024-02-12 19:08:51.084124 handshakes-0.3.2/handshake/services/SchedularService/pruneTasks.py
--rw-r--r--   0        0        0      251 2024-01-17 19:36:05.909582 handshakes-0.3.2/handshake/services/SchedularService/refer_types.py
--rw-r--r--   0        0        0     2369 2024-03-13 18:17:40.360547 handshakes-0.3.2/handshake/services/SchedularService/register.py
--rw-r--r--   0        0        0      200 2024-01-17 19:36:05.913478 handshakes-0.3.2/handshake/services/starter.py
--rw-r--r--   0        0        0     1307 2024-03-28 18:14:32.079613 handshakes-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      774 2024-02-12 19:08:50.648368 handshakes-0.3.2/README.md
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      749 2024-05-06 19:29:28.744154 handshakes-0.3.3/README.md
+-rw-r--r--   0        0        0      448 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/.version
+-rw-r--r--   0        0        0       22 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/CommandLine/__init__.py
+-rw-r--r--   0        0        0     8485 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/CommandLine/_init.py
+-rw-r--r--   0        0        0     4326 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/CommandLine/center.py
+-rw-r--r--   0        0        0       15 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/__init__.py
+-rw-r--r--   0        0        0     3107 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/lifecycle.py
+-rw-r--r--   0        0        0     4234 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/migrator.py
+-rw-r--r--   0        0        0      570 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/__init__.py
+-rw-r--r--   0        0        0      939 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/attachmentBase.py
+-rw-r--r--   0        0        0     2034 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/config_base.py
+-rw-r--r--   0        0        0     1618 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/dynamic_base.py
+-rw-r--r--   0        0        0     1010 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/enums.py
+-rw-r--r--   0        0        0     5894 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/result_base.py
+-rw-r--r--   0        0        0     1167 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/static_base.py
+-rw-r--r--   0        0        0     2102 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/types.py
+-rw-r--r--   0        0        0       50 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/sanic_free_shared.py
+-rw-r--r--   0        0        0      221 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/bump-v5.sql
+-rw-r--r--   0        0        0      369 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/bump-v6.sql
+-rw-r--r--   0        0        0      407 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/revert-v4.sql
+-rw-r--r--   0        0        0       99 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/revert-v6.sql
+-rw-r--r--   0        0        0      452 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/revert-v7.sql
+-rw-r--r--   0        0        0      753 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/shared.py
+-rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/__init__.py
+-rw-r--r--   0        0        0     7967 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/coreEndpoints.py
+-rw-r--r--   0        0        0     1434 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/utils.py
+-rw-r--r--   0        0        0     1934 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/writeServices.py
+-rw-r--r--   0        0        0      431 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/center.py
+-rw-r--r--   0        0        0     1055 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/core.py
+-rw-r--r--   0        0        0      278 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/errorHandling.py
+-rw-r--r--   0        0        0      954 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/internalEndpoints.py
+-rw-r--r--   0        0        0      128 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/static_server.py
+-rw-r--r--   0        0        0     2587 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/__init__.py
+-rw-r--r--   0        0        0     9654 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/completeTestRun.py
+-rw-r--r--   0        0        0      591 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/constants.py
+-rw-r--r--   0        0        0     4562 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/handlePending.py
+-rw-r--r--   0        0        0     1635 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/handleTestResults.py
+-rw-r--r--   0        0        0     8216 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/modifySuites.py
+-rw-r--r--   0        0        0     1867 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/pruneTasks.py
+-rw-r--r--   0        0        0      666 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/refer_types.py
+-rw-r--r--   0        0        0     1653 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/register.py
+-rw-r--r--   0        0        0    13922 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/start.py
+-rw-r--r--   0        0        0        0 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/starter.py
+-rw-r--r--   0        0        0     1576 2024-05-06 19:29:28.764154 handshakes-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.3/PKG-INFO
```

### Comparing `handshakes-0.3.2/handshake/services/CommandLine/_init.py` & `handshakes-0.3.3/handshake/services/CommandLine/_init.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,310 +1,282 @@
-import datetime
-import pprint
-from sqlite3 import connect
-from click import (
-    group,
-    argument,
-    secho,
-    version_option,
-    pass_context,
-    Context,
-    Path as C_Path,
-)
-from handshake import __version__
-from handshake.services.DBService.migrator import check_version, migration, DB_VERSION
-from handshake.services.SchedularService.center import start_service
-from handshake.services.SchedularService.lifecycle import start_loop
-from handshake.services.SchedularService.handleTestResults import (
-    moveTestRunsRelatedAttachment,
-    setConfig,
-)
-from functools import partial
-from handshake.services.SchedularService.constants import writtenAttachmentFolderName
-from handshake.services.SchedularService.register import (
-    deleteExportTicket,
-    createExportTicket,
-)
-from os.path import relpath
-from subprocess import call, check_output
-from loguru import logger
-from concurrent.futures import ThreadPoolExecutor
-import json
-from handshake.services.DBService.lifecycle import (
-    config_file,
-)
-from click import option
-from pathlib import Path
-from handshake.services.DBService.shared import db_path
-from handshake.services.DBService.models.config_base import ConfigKeys
-from tortoise import run_async
-from os import getenv
-
-
-@group(
-    name="Handshake",
-    short_help="Handshake command",
-    help=f"""
-
-{'{:*^69}'.format(" Welcome to Handshake's CLI ")}
-
-Handshake simplifies the collection and processing of your test results. The Handshake CLI helps you to interact with 
-the stored results or with the server. so for each command it requires a <path> argument, representing the collection 
-folder, a place where you could have the database or were planning to store the results [not the HTML files].
-
-[ROOT-DIR] >> [COLLECTION_NAME] (*we need this) >> TeStReSuLtS.db & [Attachments] (for getting this).
-
-{'{:*^69}'.format(" Glossary ")}
-""",
-)
-@version_option(f"{__version__}, DB: {DB_VERSION}")
-def handle_cli():
-    pass
-
-
-general_requirement = argument(
-    "COLLECTION_PATH", nargs=1, type=C_Path(exists=True, dir_okay=True), required=True
-)
-general_but_optional_requirement = argument(
-    "COLLECTION_PATH", nargs=1, type=C_Path(dir_okay=True), required=True
-)
-
-
-@general_requirement
-@handle_cli.command()
-def db_version(collection_path):
-    return check_version(db_path(collection_path))
-
-
-@general_requirement
-@handle_cli.command(
-    short_help="Migrates the database to the latest version as per the handshake executable.",
-    help="it's a command to execute the required migration scripts, note; this command would be executed "
-    "automatically whenever we run patch or run-app command",
-)
-def migrate(collection_path: str):
-    return migration(db_path(collection_path))
-
-
-@handle_cli.command(
-    short_help="Processes the collected results",
-    help="runs an async scheduler, thanks to apscheduler, it would process your test results to patch some missing "
-    "values. which are essential while showcasing your test reports",
-)
-@option(
-    "--log-file",
-    "-l",
-    help="give me file name to store the logs for the patch command.",
-    type=C_Path(),
-    default="",
-    required=False,
-)
-@option(
-    "-r",
-    "--reset",
-    default=False,
-    show_default=True,
-    help="re-calculates the values for the test runs",
-    type=bool,
-    is_flag=True,
-)
-@general_requirement
-def patch(collection_path, log_file: str, reset: bool = False):
-    if log_file:
-        logger.add(
-            log_file if log_file.endswith(".log") else f"{log_file}.log",
-            backtrace=True,
-            diagnose=True,
-        )
-
-    if not Path(collection_path).is_dir():
-        raise NotADirectoryError(collection_path)
-    start_service(db_path(collection_path), reset)
-    start_loop()
-
-
-@handle_cli.command(
-    help="Helper command which would assume you have nodejs installed and with the help of Next.js's SSG [Static Site "
-    "Generation] we would generate reports from processed results."
-    " Note: make sure to run this command from the directory where we can access the required npm scope",
-    short_help="Generates the static dashboard from processed results",
-)
-@general_requirement
-@option(
-    "-mr",
-    "--max-runs",
-    type=int,
-    default=100,
-    help="Asks Sanic to set the use max. number of workers",
-)
-@option("--out", type=C_Path(dir_okay=True), required=True)
-@option("--clarity", is_flag=True)
-def export(collection_path, max_runs, out, clarity):
-    saved_db_path = db_path(collection_path)
-    if not saved_db_path.exists():
-        raise FileNotFoundError(f"DB file not in {collection_path}")
-
-    resolved = Path(out).resolve()
-    resolved.mkdir(exist_ok=True)
-
-    logger.debug(
-        "we are currently at: {}. assuming npm in scope, finding dashboard lib.",
-        Path.cwd(),
-    )
-
-    node_modules = check_output(
-        "npm root", shell=True, text=True, cwd=Path.cwd()
-    ).strip()
-
-    logger.info("Found Node modules at: {}", node_modules)
-
-    handshake = Path(node_modules) / "handshake-dashboard"
-    if not handshake.exists():
-        logger.error(
-            "handshake-dashboard was not found in packages located at {}. please try to install the dashboard through "
-            "the command: npm install handshake",
-            handshake,
-        )
-        raise FileNotFoundError(
-            "Please install handshake-dashboard in your project, npm install handshake"
-        )
-
-    logger.debug("Given details are valid, creating a export ticket")
-
-    ticket_i_ds = []
-    runs = []
-    run_async(createExportTicket(max_runs, saved_db_path, ticket_i_ds, runs, clarity))
-
-    if len(ticket_i_ds) == 0:
-        logger.error("Ticket was not created, please report this as a issue.")
-
-    logger.info("Exporting results to {}", relpath(resolved, handshake))
-    logger.debug(
-        "building files, with command:"
-        ' "npx cross-env TICKET_ID={} EXPORT_DIR={}'
-        ' DB_PATH={} npm run export"',
-        ticket_i_ds[0],
-        relpath(resolved, handshake),
-        relpath(saved_db_path, handshake),
-    )
-
-    exported = call(
-        f"npx cross-env TICKET_ID={ticket_i_ds[0]} EXPORT_DIR={relpath(resolved, handshake)}"
-        f" DB_PATH={relpath(saved_db_path, handshake)} CLARITY={getenv('CLARITY')} npm run export",
-        cwd=handshake,
-        shell=True,
-    )
-
-    if ticket_i_ds:
-        run_async(deleteExportTicket(ticket_i_ds[0]))
-
-    attachments = Path(out) / writtenAttachmentFolderName
-    attachments.mkdir(exist_ok=True)
-
-    attachments_from = Path(collection_path) / writtenAttachmentFolderName
-
-    if not (Path(out).exists() and exported == 0 and attachments_from.exists()):
-        return logger.warning("Task for copying attachments was skipped.")
-
-    allocated_work = partial(
-        moveTestRunsRelatedAttachment, copyFrom=attachments_from, copyTo=attachments
-    )
-
-    with ThreadPoolExecutor(max_workers=6) as workers:
-        logger.info("Copying attachments for {} test runs.", len(runs))
-        workers.map(allocated_work, runs)
-
-    logger.info("Done.")
-
-
-@handle_cli.command(
-    short_help="Quick Config for test collection",
-    help="configures few values which is used while processing your reports., ignore the options if not required for "
-    "update",
-)
-@general_but_optional_requirement
-@option(
-    "--max_runs",
-    "-mr",
-    default=-1,
-    help="Max. Number of runs to keep. NOTE: should be >1",
-)
-def config(collection_path, max_runs):
-    saved_db_path = db_path(collection_path)
-
-    set_default_first = not Path(collection_path).exists()
-    if set_default_first:
-        Path(collection_path).mkdir(exist_ok=True)
-
-    feed_from = config_file(saved_db_path)
-    feed = dict() if not feed_from.exists() else json.loads(feed_from.read_text())
-    if max_runs > 1:
-        feed[ConfigKeys.maxRuns] = max_runs
-
-    run_async(setConfig(saved_db_path, feed, set_default_first))
-
-
-@handle_cli.group(
-    name="db",
-    short_help="Commands that will/(try to) fetch mostly asked info. from db",
-    help="you can query using db following the subcommands, which are created to provide mostly asked info. from db",
-)
-@version_option(DB_VERSION, prog_name="handshake-db")
-@general_requirement
-def db(collection_path: str):
-    if not Path(db_path(collection_path)).exists():
-        raise FileNotFoundError(
-            f"db path was not found in the collections: {collection_path}"
-        )
-
-
-@db.command(short_help="fetches the timestamp of the latest run")
-@option(
-    "-p",
-    "--allow-pending",
-    default=False,
-    show_default=True,
-    help="consider runs, whose status are pending",
-    type=bool,
-    is_flag=True,
-)
-@pass_context
-def latest_run(ctx: Context, allow_pending: bool):
-    db_file = db_path(Path(ctx.parent.params["collection_path"]))
-    pipe = connect(db_file)
-    result = pipe.execute(
-        "SELECT ENDED FROM RUNBASE WHERE ENDED <> '' ORDER BY STARTED LIMIT 1"
-        if not allow_pending
-        else "SELECT ENDED FROM RUNBASE ORDER BY STARTED LIMIT 1"
-    ).fetchone()
-
-    secho(
-        "No Test Runs were found"
-        if not result
-        else datetime.datetime.fromisoformat(result[0]).astimezone().strftime("%c %Z"),
-        fg="bright_yellow" if not result else "bright_magenta",
-    )
-
-    pipe.close()
-
-
-@db.command(
-    short_help="fetches the number of yet to patch task",
-    help="returns list of tasks of form: (ticket_id, task_type, dropped_date, is_picked, test_id)",
-)
-@pass_context
-def yet_to_process(ctx: Context):
-    db_file = db_path(Path(ctx.parent.params["collection_path"]))
-    pipe = connect(db_file)
-    result = pipe.execute(
-        "SELECT ticketID, type, STRFTIME('%d/%m/%Y, %H:%M', dropped, 'localtime'), picked, test_id FROM TASKBASE WHERE "
-        "PROCESSED = 0"
-    ).fetchall()
-
-    secho(
-        "No Pending Tasks"
-        if not result
-        else f"pending tasks:\n {pprint.pformat(result)}",
-        fg="bright_green" if not result else "bright_yellow",
-    )
-
-    pipe.close()
+import datetime
+import pprint
+from sqlite3 import connect, sqlite_version_info
+from click import (
+    group,
+    argument,
+    secho,
+    version_option,
+    pass_context,
+    Context,
+    Path as C_Path,
+)
+from handshake import __version__
+from handshake.services.DBService.migrator import check_version, migration, DB_VERSION
+from handshake.services.SchedularService.start import Scheduler
+from handshake.services.SchedularService.handleTestResults import (
+    setConfig,
+)
+from loguru import logger
+import json
+from handshake.services.DBService.lifecycle import config_file, close_connection
+from click import option
+from pathlib import Path
+from handshake.services.DBService.shared import db_path
+from handshake.services.DBService.models.config_base import ConfigKeys
+from tortoise import run_async
+from asyncio import run
+
+
+@group(
+    name="Handshake",
+    short_help="Handshake command",
+    help=f"""
+
+{'{:*^69}'.format(" Welcome to Handshake's CLI ")}
+
+Handshake simplifies the collection and processing of your test results. The Handshake CLI helps you to interact with 
+the stored results or with the server. so for each command it requires a <path> argument, representing the collection 
+folder, a place where you could have the database or were planning to store the results [not the HTML files].
+
+[ROOT-DIR] >> [COLLECTION_NAME] (*we need this) >> TeStReSuLtS.db & [Attachments] (for getting this).
+
+{'{:*^69}'.format(" Glossary ")}
+""",
+)
+@version_option(f"{__version__}, DB: {DB_VERSION}")
+def handle_cli():
+    pass
+
+
+general_requirement = argument(
+    "COLLECTION_PATH", nargs=1, type=C_Path(exists=True, dir_okay=True), required=True
+)
+general_but_optional_requirement = argument(
+    "COLLECTION_PATH", nargs=1, type=C_Path(dir_okay=True), required=True
+)
+observed_version = option(
+    "--version",
+    "-v",
+    default="",
+    type=str,
+    required=False,
+    show_default=True,
+    help="Used Internally with the reporters,"
+    " reporters will pass the version of the expected handshake server if it matches,"
+    " we run the server else we terminate the execution.",
+)
+
+
+def break_if_mismatch(expected: str) -> bool:
+    if expected:
+        assert expected.strip() == __version__, (
+            f"Mismatch between expected version: {expected} "
+            f"and the actual version v{__version__}"
+        )
+    return True
+
+
+@general_requirement
+@handle_cli.command()
+def db_version(collection_path):
+    return check_version(db_path(collection_path))
+
+
+@handle_cli.command(
+    short_help="checks the version of the sqlite3 installed in your system"
+)
+def check_sqlite():
+    assert int(sqlite_version_info[0]) >= 3, "Required version is >= 3."
+    assert (
+        int(sqlite_version_info[1]) >= 38
+    ), "Required Version is >= 3.38,  for supporting our sql scripts, for supporting our sql scripts"
+    logger.info("your sqlite version is fine as per our need")
+
+
+@general_requirement
+@handle_cli.command(
+    short_help="Migrates the database to the latest version as per the handshake executable.",
+    help="it's a command to execute the required migration scripts, note; this command would be executed "
+    "automatically whenever we run patch or run-app command",
+)
+def migrate(collection_path: str):
+    return migration(db_path(collection_path))
+
+
+@handle_cli.command(
+    short_help="Processes the collected results and even could export the test results",
+    help="runs an async loop, schedules some tasks to patch some your test results "
+    "so you can see it in the way we need. you can pass the output directory to generate the report",
+)
+@option(
+    "--log-file",
+    "-l",
+    help="give me file name to store the logs for the patch command.",
+    type=C_Path(),
+    default="",
+    required=False,
+)
+@option(
+    "-r",
+    "--reset",
+    default=False,
+    show_default=True,
+    help="re-calculates the values for the test runs",
+    type=bool,
+    is_flag=True,
+)
+@general_requirement
+# TODO: Support the max runs feature, allows user to only export certain number of test runs
+# @option(
+#     "-mr",
+#     "--max-runs",
+#     type=int,
+#     default=100,
+#     help="Asks Sanic to set the use max. number of workers",
+# )
+@option(
+    "--build",
+    "-b",
+    required=False,
+    help="builds the dashboard output at the build output folder",
+    type=C_Path(exists=True, file_okay=True, readable=True),
+)
+@option(
+    "--include",
+    "-i",
+    required=False,
+    help="generates the Import Data folder inside the test results (used for internal purposes only)",
+    type=bool,
+    is_flag=True,
+    default=False,
+    show_default=True,
+)
+@option("--out", "-o", type=C_Path(dir_okay=True, writable=True), required=False)
+def patch(
+    collection_path,
+    log_file: str,
+    reset: bool = False,
+    build: str = None,
+    out: str = None,
+    include=False,
+):
+    if log_file:
+        logger.add(
+            log_file if log_file.endswith(".log") else f"{log_file}.log",
+            backtrace=True,
+            diagnose=True,
+        )
+
+    if not Path(collection_path).is_dir():
+        raise NotADirectoryError(collection_path)
+
+    scheduler = Scheduler(collection_path, out, reset, build, include)
+    try:
+        run(scheduler.start())
+    except (KeyboardInterrupt, SystemExit):
+        logger.warning("Scheduler terminated explicitly...")
+        run(close_connection())
+
+
+@handle_cli.command(
+    help="returns the version of the handshake", short_help="example: 1.0.0"
+)
+def v():
+    secho(__version__)
+
+
+@handle_cli.command(
+    short_help="Quick Config for test collection",
+    help="configures few values which is used while processing your reports., ignore the options if not required for "
+    "update",
+)
+@general_but_optional_requirement
+@option(
+    "--max_runs",
+    "-mr",
+    default=-1,
+    help="Max. Number of runs to keep. NOTE: should be >1",
+)
+def config(collection_path, max_runs):
+    saved_db_path = db_path(collection_path)
+
+    set_default_first = not Path(collection_path).exists()
+    if set_default_first:
+        Path(collection_path).mkdir(exist_ok=True)
+
+    feed_from = config_file(saved_db_path)
+    feed = dict() if not feed_from.exists() else json.loads(feed_from.read_text())
+    if max_runs > 1:
+        feed[ConfigKeys.maxRunsPerProject] = max_runs
+
+    run_async(setConfig(saved_db_path, feed, set_default_first))
+
+
+@handle_cli.group(
+    name="db",
+    short_help="Commands that will/(try to) fetch mostly asked info. from db",
+    help="you can query using db following the subcommands, which are created to provide mostly asked info. from db",
+)
+@version_option(DB_VERSION, prog_name="handshake-db")
+@general_requirement
+def db(collection_path: str):
+    if not Path(db_path(collection_path)).exists():
+        raise FileNotFoundError(
+            f"db path was not found in the collections: {collection_path}"
+        )
+
+
+@db.command(short_help="fetches the timestamp of the latest run")
+@option(
+    "-p",
+    "--allow-pending",
+    default=False,
+    show_default=True,
+    help="consider runs, whose status are pending",
+    type=bool,
+    is_flag=True,
+)
+@pass_context
+def latest_run(ctx: Context, allow_pending: bool):
+    db_file = db_path(Path(ctx.parent.params["collection_path"]))
+    pipe = connect(db_file)
+    result = pipe.execute(
+        "SELECT PROJECTNAME, ENDED FROM RUNBASE WHERE ENDED <> '' ORDER BY STARTED LIMIT 1"
+        if not allow_pending
+        else "SELECT PROJECTNAME, ENDED FROM RUNBASE ORDER BY STARTED LIMIT 1"
+    ).fetchone()
+
+    secho(
+        "No Test Runs were found"
+        if not result
+        else (
+            result[0],
+            datetime.datetime.fromisoformat(result[1]).astimezone().strftime("%c %Z"),
+        ),
+        fg="bright_yellow" if not result else "bright_magenta",
+    )
+
+    pipe.close()
+
+
+@db.command(
+    short_help="fetches the number of yet to patch task",
+    help="returns list of tasks of form: (ticket_id, task_type, dropped_date, is_picked, test_id)",
+)
+@pass_context
+def yet_to_process(ctx: Context):
+    db_file = db_path(Path(ctx.parent.params["collection_path"]))
+    pipe = connect(db_file)
+    result = pipe.execute(
+        "SELECT ticketID, type, STRFTIME('%d/%m/%Y, %H:%M', dropped, 'localtime'), picked, test_id FROM TASKBASE WHERE "
+        "PROCESSED = 0"
+    ).fetchall()
+
+    secho(
+        "No Pending Tasks"
+        if not result
+        else f"pending tasks:\n {pprint.pformat(result)}",
+        fg="bright_green" if not result else "bright_yellow",
+    )
+
+    pipe.close()
```

### Comparing `handshakes-0.3.2/handshake/services/CommandLine/center.py` & `handshakes-0.3.3/handshake/services/CommandLine/center.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,145 +1,155 @@
-from handshake.services.CommandLine._init import (
-    handle_cli,
-    general_but_optional_requirement,
-)
-from handshake.services.Endpoints.center import service_provider
-from handshake.services.DBService.lifecycle import (
-    init_tortoise_orm,
-    close_connection,
-    create_run,
-)
-from handshake import __version__
-from typing import Union
-from handshake.services.DBService.shared import set_test_id
-from click import argument, option, Path
-from pathlib import Path as P_Path
-from multiprocessing.sharedctypes import Array
-from sanic.worker.loader import AppLoader
-from sanic import Sanic
-from typing import Tuple
-from functools import partial
-from loguru import logger
-from handshake.services.Endpoints.static_server import static_provider
-
-
-def feed_app() -> Sanic:
-    return service_provider
-
-
-def feed_static_provider(export: str) -> Sanic:
-    static_provider.static(
-        "/", str(P_Path(export)), name="export", index=["index.html", "RUNS.html"]
-    )
-    return static_provider
-
-
-def prepare_loader() -> Tuple[Sanic, AppLoader]:
-    loader = AppLoader(factory=feed_app)
-    app = loader.load()
-    return app, loader
-
-
-def setup_app(
-    projectname: str,
-    path: str,
-    port: int = 6969,
-    workers: int = 2,
-):
-    @service_provider.main_process_start
-    async def get_me_started(app, loop):
-        service_provider.shared_ctx.ROOT = Array("c", str.encode(path))
-        await init_tortoise_orm(migrate=True)
-        test_id = await create_run(projectname)
-        service_provider.shared_ctx.TEST_ID = Array("c", str.encode(test_id))
-        set_test_id()
-
-    @service_provider.main_process_stop
-    async def close_things(app, loop):
-        await close_connection()
-
-    _app, loader = prepare_loader()
-    _app.prepare(
-        port=port,
-        workers=max(2, workers),
-        host="127.0.0.1",
-        motd_display=dict(version=__version__),
-    )
-    logger.debug("Serving at port: {}", port)
-    Sanic.serve(primary=_app, app_loader=loader)
-
-
-@handle_cli.command(
-    short_help="Starts the server which would listen for your input",
-    help="""
-Starts the Handshake server to listen for inputs at the specified port on localhost. This command initiates a test run,
-allowing the server to handle a single test run at a time. For multiple test runs, spawn the process separately on different
-ports.
-""",
-)
-@argument("PROJECT_NAME", nargs=1, required=True, type=str)
-@general_but_optional_requirement
-@option(
-    "-p",
-    "--port",
-    default=6969,
-    show_default=True,
-    help="Port for the service to connect to",
-    type=int,
-)
-@option(
-    "-w",
-    "--workers",
-    default=2,
-    show_default=True,
-    help="Number of workers to use",
-    type=int,
-)
-def run_app(
-    collection_path: str,
-    project_name: str,
-    port: int,
-    workers: int,
-):
-    if workers < 2:
-        logger.warning(
-            "we have set default of 2 workers, if it's less than that, server might miss results sent from the runner."
-        )
-
-    P_Path(collection_path).mkdir(exist_ok=True)
-    setup_app(project_name, collection_path, port, workers)
-
-
-@handle_cli.command(
-    help="serves the generated reports. simply serves the static files generated in your directory mentioned "
-    "in static_path",
-    short_help="serves generated report",
-)
-@argument("STATIC_PATH", nargs=1, required=False, type=Path(exists=True, dir_okay=True))
-@option(
-    "-p",
-    "--port",
-    default=8000,
-    show_default=True,
-    help="Port for the service to connect to",
-    type=int,
-)
-def display(static_path: Union[str, P_Path] = "TestReports", port: int = 8000):
-    if static_path:
-        static_path = P_Path(static_path)
-
-        if not static_path.exists():
-            raise NotADirectoryError(f"{static_path} does not exist")
-
-    loader = AppLoader(factory=partial(feed_static_provider, static_path))
-    _app = loader.load()
-    _app.prepare(
-        host="127.0.0.1",
-        port=port,
-        access_log=False,
-        motd_display=dict(version=__version__),
-    )
-    Sanic.serve(primary=_app, app_loader=loader)
-
-
-if __name__ == "__main__":
-    setup_app("sample", "../../../TestResults")
+from handshake.services.CommandLine._init import (
+    handle_cli,
+    general_but_optional_requirement,
+    version_option,
+    observed_version,
+    break_if_mismatch,
+)
+from handshake.services.Endpoints.center import service_provider
+from handshake.services.DBService.lifecycle import (
+    init_tortoise_orm,
+    close_connection,
+    create_run,
+)
+from handshake import __version__
+from typing import Union
+from handshake.services.DBService.shared import set_test_id
+from click import argument, option, Path
+from pathlib import Path as P_Path
+from multiprocessing.sharedctypes import Array
+from sanic.worker.loader import AppLoader
+from sanic import Sanic
+from typing import Tuple
+from functools import partial
+from loguru import logger
+from handshake.services.Endpoints.static_server import static_provider
+
+
+def feed_app() -> Sanic:
+    return service_provider
+
+
+def feed_static_provider(export: str) -> Sanic:
+    static_provider.static(
+        "/", str(P_Path(export)), name="export", index=["index.html", "RUNS.html"]
+    )
+    return static_provider
+
+
+def prepare_loader() -> Tuple[Sanic, AppLoader]:
+    loader = AppLoader(factory=feed_app)
+    app = loader.load()
+    return app, loader
+
+
+def setup_app(
+    projectname: str,
+    path: str,
+    port: int = 6969,
+    workers: int = 2,
+):
+    @service_provider.main_process_start
+    async def get_me_started(app, loop):
+        service_provider.shared_ctx.ROOT = Array("c", str.encode(path))
+        await init_tortoise_orm(migrate=True)
+        test_id = await create_run(projectname)
+        service_provider.shared_ctx.TEST_ID = Array("c", str.encode(test_id))
+        set_test_id()
+
+    @service_provider.main_process_stop
+    async def close_things(app, loop):
+        await close_connection()
+
+    _app, loader = prepare_loader()
+    _app.prepare(
+        port=port,
+        workers=max(2, workers),
+        host="127.0.0.1",
+        motd_display=dict(version=__version__),
+    )
+    logger.debug("Serving at port: {}", port)
+    Sanic.serve(primary=_app, app_loader=loader)
+
+
+@handle_cli.command(
+    short_help="Starts the server which would listen for your input",
+    help="""
+Starts the Handshake server to listen for inputs at the specified port on localhost. This command initiates a test run,
+allowing the server to handle a single test run at a time. For multiple test runs, spawn the process separately on different
+ports.
+""",
+)
+@argument("PROJECT_NAME", nargs=1, required=True, type=str)
+@observed_version
+@general_but_optional_requirement
+@option(
+    "-p",
+    "--port",
+    default=6969,
+    show_default=True,
+    help="Port for the service to connect to",
+    type=int,
+)
+@option(
+    "-w",
+    "--workers",
+    default=2,
+    show_default=True,
+    help="Number of workers to use",
+    type=int,
+)
+def run_app(
+    collection_path: str,
+    project_name: str,
+    version: Union[str, bool],
+    port: int,
+    workers: int,
+):
+    break_if_mismatch(version)
+    if workers < 2:
+        logger.warning(
+            "we have set default of 2 workers, if it's less than that, server might miss results sent from the runner."
+        )
+
+    P_Path(collection_path).mkdir(exist_ok=True)
+    setup_app(project_name, collection_path, port, workers)
+
+
+@handle_cli.command(
+    help="serves the generated reports. simply serves the static files generated in your directory mentioned "
+    "in static_path",
+    short_help="serves generated report",
+)
+@argument("STATIC_PATH", nargs=1, required=False, type=Path(exists=True, dir_okay=True))
+@option(
+    "-p",
+    "--port",
+    default=8000,
+    show_default=True,
+    help="Port for the service to connect to",
+    type=int,
+)
+def display(
+    version: Union[bool, str] = False,
+    static_path: Union[str, P_Path] = "TestReports",
+    port: int = 8000,
+):
+    if static_path:
+        static_path = P_Path(static_path)
+
+        if not static_path.exists():
+            raise NotADirectoryError(f"{static_path} does not exist")
+
+    loader = AppLoader(factory=partial(feed_static_provider, static_path))
+    _app = loader.load()
+    _app.prepare(
+        host="127.0.0.1",
+        port=port,
+        access_log=False,
+        motd_display=dict(version=__version__),
+    )
+    Sanic.serve(primary=_app, app_loader=loader)
+
+
+if __name__ == "__main__":
+    setup_app("sample", "../../../TestResults")
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/lifecycle.py` & `handshakes-0.3.3/handshake/services/DBService/lifecycle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,99 @@
-import json
-from handshake.services.DBService.models.config_base import ConfigBase
-from handshake.services.DBService import DB_VERSION
-from handshake.services.DBService.models.result_base import RunBase
-from handshake.services.DBService.models.enums import ConfigKeys
-from handshake.services.DBService.migrator import migration
-from tortoise import Tortoise, connections
-from handshake.services.DBService.shared import db_path
-from pathlib import Path
-from handshake import __version__
-from typing import Optional, Union
-from loguru import logger
-from handshake.services.SchedularService.constants import writtenAttachmentFolderName
-
-models = ["handshake.services.DBService.models"]
-
-
-def config_file(provided_db_path: Path):
-    return provided_db_path.parent / "config.json"
-
-
-def attachment_folder(provided_db_path: Path):
-    return provided_db_path.parent / writtenAttachmentFolderName
-
-
-async def init_tortoise_orm(
-    force_db_path: Optional[Union[Path, str]] = None, migrate: bool = False
-):
-    chosen = force_db_path if force_db_path else db_path()
-    if migrate:
-        migration(chosen)
-
-    await Tortoise.init(
-        db_url=r"{}".format(f"sqlite://{chosen}"),
-        modules={"models": models},
-    )
-    await Tortoise.generate_schemas()
-    await set_default_config(chosen)
-
-
-async def create_run(projectName: str) -> str:
-    test_id = str((await RunBase.create(projectName=projectName)).testID)
-    return test_id
-
-
-READ_ONLY = (
-    ConfigKeys.version,
-    ConfigKeys.recentlyDeleted,
-    ConfigKeys.reset_test_run,
-    ConfigKeys.py_version,
-)
-ALLOW_WRITE = (ConfigKeys.maxRuns,)
-
-
-async def set_default_config(path: Path):
-    attachment_folder(path).mkdir(exist_ok=True)
-    config_file_provided = config_file(path)
-    config_provided = (
-        json.loads(config_file_provided.read_text())
-        if config_file_provided.exists()
-        else dict()
-    )
-
-    for key, value in [
-        (ConfigKeys.version, DB_VERSION),
-        (ConfigKeys.py_version, __version__),
-        (ConfigKeys.reset_test_run, ""),
-        # below keys can be overridden by the config file
-        *[(_, config_provided.get(_, __)) for _, __ in [(ConfigKeys.maxRuns, "100")]],
-    ]:
-        record = await ConfigBase.filter(key=str(key)).first()
-        if not record:
-            await ConfigBase.create(key=key, value=value)
-
-
-async def close_connection():
-    await connections.close_all()
-    # waiting for the logs to be sent or saved
-    await logger.complete()
+import json
+from handshake.services.DBService.models.config_base import ConfigBase
+from handshake.services.DBService import DB_VERSION
+from handshake.services.DBService.models.result_base import RunBase
+from handshake.services.DBService.models.enums import ConfigKeys
+from handshake.services.DBService.migrator import migration
+from tortoise import Tortoise, connections
+from handshake.services.DBService.shared import db_path
+from pathlib import Path
+from typing import Optional, Union
+from loguru import logger
+from handshake.services.SchedularService.constants import (
+    writtenAttachmentFolderName,
+)
+
+models = ["handshake.services.DBService.models"]
+
+
+def config_file(provided_db_path: Path):
+    return provided_db_path.parent / "config.json"
+
+
+def attachment_folder(provided_db_path: Path):
+    return provided_db_path.parent / writtenAttachmentFolderName
+
+
+async def init_tortoise_orm(
+    force_db_path: Optional[Union[Path, str]] = None, migrate: bool = False
+):
+    chosen = force_db_path if force_db_path else db_path()
+    if migrate:
+        migration(chosen)
+
+    await Tortoise.init(
+        db_url=r"{}".format(f"sqlite://{chosen}"),
+        modules={"models": models},
+    )
+    await Tortoise.generate_schemas()
+    await set_default_config(chosen)
+
+
+async def create_run(projectName: str) -> str:
+    test_id = str((await RunBase.create(projectName=projectName)).testID)
+    return test_id
+
+
+READ_ONLY = (
+    ConfigKeys.version,
+    ConfigKeys.recentlyDeleted,
+    ConfigKeys.reset_test_run,
+)
+ALLOW_WRITE = {
+    ConfigKeys.maxRunsPerProject,
+}
+
+
+async def set_default_config(path: Path):
+    attachment_folder(path).mkdir(exist_ok=True)
+    config_file_provided = config_file(path)
+    config_provided = (
+        json.loads(config_file_provided.read_text())
+        if config_file_provided.exists()
+        else dict()
+    )
+
+    for key, value in [
+        (ConfigKeys.version, DB_VERSION),
+        (ConfigKeys.reset_test_run, ""),
+        (ConfigKeys.maxRunsPerProject, "100")
+        # below keys can be overridden by the config file
+    ]:
+        record = await ConfigBase.filter(key=str(key)).first()
+        if not record:
+            logger.debug(
+                "{} was not found in our table, registering it with value: {}",
+                key,
+                value,
+            )
+            await ConfigBase.create(key=key, value=value)
+        else:
+            if (
+                record.key in ALLOW_WRITE
+                and config_provided.get(record.key, value) != record.value
+            ):
+                logger.debug(
+                    "Found a key: {} already existing in configbase with value: {},"
+                    " but received a request to change it to {}",
+                    record.key,
+                    value,
+                    config_provided.get(record.key, value),
+                )
+                record.value = config_provided.get(record.key, value)
+                await record.save()
+
+
+async def close_connection():
+    await connections.close_all()
+    # waiting for the logs to be sent or saved
+    await logger.complete()
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/migrator.py` & `handshakes-0.3.3/handshake/services/DBService/migrator.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import typing
-from sqlite3 import connect
-from handshake.services.DBService import DB_VERSION
-from handshake.services.DBService.models.enums import ConfigKeys
-from sqlite3.dbapi2 import Connection
-from typing import Optional, Tuple
-from pathlib import Path
-from loguru import logger
-
-
-def check_version(
-    path: Path = None, connection: Optional[Connection] = None
-) -> Tuple[bool, Connection, bool, Optional[int]]:
-    connection = connection if connection else connect(path)
-    query = f"select value from configbase where key = '{ConfigKeys.version}'"
-    result = connection.execute(query).fetchone()
-
-    version_stored = False
-    migration_required = False
-
-    if not result:
-        logger.warning(
-            f"Could not find the version, Please raise this as an issue or re-run after deleting the folder at: {path}."
-        )
-    else:
-        version_stored = result if not result else int(result[0])
-        migration_required = version_stored != DB_VERSION
-
-        logger.log(
-            "INFO" if not migration_required else "WARNING",
-            "Currently at: v{}."
-            if not migration_required
-            else 'Found version: v{}. but required is v{}. Please execute: \n"handshake migrate [COLLECTION_PATH]"',
-            result[0],
-            DB_VERSION,
-        )
-    return (
-        migration_required,
-        connection,
-        version_stored < DB_VERSION,
-        version_stored,
-    )
-
-
-# returns True if it requires further migration
-def migrate(
-    connection: Optional[Connection] = None, db_path: Optional[Path] = None
-) -> typing.Tuple[bool, bool]:  # further migration required, migration was done
-    if not connection:
-        connection = connect(db_path)
-
-    try:
-        is_required, connection, bump_if_required, version_stored = check_version(
-            connection=connection
-        )
-
-        if not is_required:
-            logger.info("Already migrated to required version")
-            return False, False
-
-        if not bump_if_required:
-            logger.error(
-                "You have more recent version of database, v{}. but we can only support: v{}. "
-                "Hence requesting you to update your reporter, to support this version.",
-                # "use your backup database inside the collection_path.",
-                version_stored,
-                DB_VERSION,
-            )
-            return False, False
-
-        script = Path(__file__).parent / "scripts" / f"bump-v{version_stored}.sql"
-        logger.info("Executing {} to migrate from v{}", script.name, version_stored)
-        connection.executescript(script.read_text())
-    finally:
-        if db_path:
-            connection.commit()
-            connection.close()
-
-    return (version_stored + 1) < DB_VERSION, version_stored < DB_VERSION
-
-
-def migration(path: Path):
-    migration_was_conducted = False
-    if not path.exists():
-        logger.info("Migration check is not required, as the db does not exist.")
-        return
-
-    connection = connect(path)
-    try:
-        backup_file = "backup_results.db"
-
-        while True:
-            first_time = not migration_was_conducted
-            further_required, migration_was_conducted = migrate(connection)
-            if migration_was_conducted and first_time:
-                backup_path = path.parent / backup_file
-                backup_path.unlink(missing_ok=True)
-                backup = connect(backup_path)
-                logger.info(
-                    "Before migration, Taking a backup and storing it in {}",
-                    backup_path,
-                )
-                connection.backup(backup)
-                backup.close()
-            if not migration_was_conducted:
-                migration_was_conducted = True
-                break
-
-        if migration_was_conducted:
-            (path.parent / backup_file).unlink(missing_ok=True)
-            connection.commit()
-            logger.info("Migrated to latest version!")
-
-    except Exception as error:
-        logger.error(f"Failed to execute migration script, due to {error}")
-        return True
-    finally:
-        connection.close()
-
-
-if __name__ == "__main__":
-    migration(Path.cwd().parent.parent.parent / "TestResults" / "TeStReSuLtS.db")
+import typing
+from sqlite3 import connect
+from handshake.services.DBService import DB_VERSION
+from handshake.services.DBService.models.enums import ConfigKeys
+from sqlite3.dbapi2 import Connection
+from typing import Optional, Tuple
+from pathlib import Path
+from loguru import logger
+
+
+def check_version(
+    path: Path = None, connection: Optional[Connection] = None
+) -> Tuple[bool, Connection, bool, Optional[int]]:
+    connection = connection if connection else connect(path)
+    query = f"select value from configbase where key = '{ConfigKeys.version}'"
+    result = connection.execute(query).fetchone()
+
+    version_stored = False
+    migration_required = False
+
+    if not result:
+        logger.warning(
+            f"Could not find the version, Please raise this as an issue or re-run after deleting the folder at: {path}."
+        )
+    else:
+        version_stored = result if not result else int(result[0])
+        migration_required = version_stored != DB_VERSION
+
+        logger.log(
+            "INFO" if not migration_required else "WARNING",
+            "Currently at: v{}."
+            if not migration_required
+            else 'Found version: v{}. but required is v{}. Please execute: \n"handshake migrate [COLLECTION_PATH]"',
+            result[0],
+            DB_VERSION,
+        )
+    return (
+        migration_required,
+        connection,
+        version_stored < DB_VERSION,
+        version_stored,
+    )
+
+
+# returns True if it requires further migration
+def migrate(
+    connection: Optional[Connection] = None, db_path: Optional[Path] = None
+) -> typing.Tuple[bool, bool]:  # further migration required, migration was done
+    if not connection:
+        connection = connect(db_path)
+
+    try:
+        is_required, connection, bump_if_required, version_stored = check_version(
+            connection=connection
+        )
+
+        if not is_required:
+            logger.info("Already migrated to required version")
+            return False, False
+
+        if not bump_if_required:
+            logger.error(
+                "You have more recent version of database, v{}. but we can only support: v{}. "
+                "Hence requesting you to update your reporter, to support this version.",
+                # "use your backup database inside the collection_path.",
+                version_stored,
+                DB_VERSION,
+            )
+            return False, False
+
+        script = Path(__file__).parent / "scripts" / f"bump-v{version_stored}.sql"
+        logger.info("Executing {} to migrate from v{}", script.name, version_stored)
+        connection.executescript(script.read_text())
+    finally:
+        if db_path:
+            connection.commit()
+            connection.close()
+
+    return (version_stored + 1) < DB_VERSION, version_stored < DB_VERSION
+
+
+def migration(path: Path):
+    migration_was_conducted = False
+    if not path.exists():
+        logger.info("Migration check is not required, as the db does not exist.")
+        return
+
+    connection = connect(path)
+    try:
+        backup_file = "backup_results.db"
+
+        while True:
+            first_time = not migration_was_conducted
+            further_required, migration_was_conducted = migrate(connection)
+            if migration_was_conducted and first_time:
+                backup_path = path.parent / backup_file
+                backup_path.unlink(missing_ok=True)
+                backup = connect(backup_path)
+                logger.info(
+                    "Before migration, Taking a backup and storing it in {}",
+                    backup_path,
+                )
+                connection.backup(backup)
+                backup.close()
+            if not migration_was_conducted:
+                migration_was_conducted = True
+                break
+
+        if migration_was_conducted:
+            (path.parent / backup_file).unlink(missing_ok=True)
+            connection.commit()
+            logger.info("Migrated to latest version!")
+
+    except Exception as error:
+        logger.error(f"Failed to execute migration script, due to {error}")
+        return True
+    finally:
+        connection.close()
+
+
+if __name__ == "__main__":
+    migration(Path.cwd().parent.parent.parent / "TestResults" / "TeStReSuLtS.db")
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/models/__init__.py` & `handshakes-0.3.3/handshake/services/DBService/models/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from .result_base import (
-    SessionBase,
-    SuiteBase,
-    RunBase,
-    RollupBase,
-    RetriedBase,
-    TestLogBase,
-)
-from .config_base import ConfigBase, ExportBase, TestConfigBase
-from .static_base import AttachmentBase, StaticBase
-from .dynamic_base import TaskBase, PrunedBase
-from .attachmentBase import AssertBase
-
-__all__ = [
-    SessionBase,
-    SuiteBase,
-    RunBase,
-    TestConfigBase,
-    AttachmentBase,
-    TaskBase,
-    PrunedBase,
-    ExportBase,
-    ConfigBase,
-    RollupBase,
-    StaticBase,
-    RetriedBase,
-    AssertBase,
-    TestLogBase,
-]
+from .result_base import (
+    SessionBase,
+    SuiteBase,
+    RunBase,
+    RollupBase,
+    RetriedBase,
+    TestLogBase,
+)
+from .config_base import ConfigBase, ExportBase, TestConfigBase
+from .static_base import AttachmentBase, StaticBase
+from .dynamic_base import TaskBase, PrunedBase
+from .attachmentBase import AssertBase
+
+__all__ = [
+    SessionBase,
+    SuiteBase,
+    RunBase,
+    TestConfigBase,
+    AttachmentBase,
+    TaskBase,
+    PrunedBase,
+    ExportBase,
+    ConfigBase,
+    RollupBase,
+    StaticBase,
+    RetriedBase,
+    AssertBase,
+    TestLogBase,
+]
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/models/attachmentBase.py` & `handshakes-0.3.3/handshake/services/DBService/models/attachmentBase.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from handshake.services.DBService.models.result_base import SuiteBase
-from tortoise.models import Model
-from tortoise.fields import (
-    ForeignKeyField,
-    ForeignKeyRelation,
-    TextField,
-    IntField,
-    BooleanField,
-)
-
-
-class AssertBase(Model):
-    entity: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
-        "models.SuiteBase", related_name="assertion", to_field="suiteID"
-    )
-    passed = BooleanField(
-        default=False, description="Whether the assertion passed or not"
-    )
-    wait = IntField(
-        description="Number of milli-seconds configured to wait for this test",
-        default=-1,
-        null=True,
-    )
-    interval = IntField(
-        description="interval (in milli-seconds) to test this assertion until it passes",
-        default=-1,
-        null=True,
-    )
-    title = TextField(description="Name of the Assertion")
-    message = TextField(description="Message attached to the assertion")
+from handshake.services.DBService.models.result_base import SuiteBase
+from tortoise.models import Model
+from tortoise.fields import (
+    ForeignKeyField,
+    ForeignKeyRelation,
+    TextField,
+    IntField,
+    BooleanField,
+)
+
+
+class AssertBase(Model):
+    entity: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
+        "models.SuiteBase", related_name="assertion", to_field="suiteID"
+    )
+    passed = BooleanField(
+        default=False, description="Whether the assertion passed or not"
+    )
+    wait = IntField(
+        description="Number of milli-seconds configured to wait for this test",
+        default=-1,
+        null=True,
+    )
+    interval = IntField(
+        description="interval (in milli-seconds) to test this assertion until it passes",
+        default=-1,
+        null=True,
+    )
+    title = TextField(description="Name of the Assertion")
+    message = TextField(description="Message attached to the assertion")
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/models/config_base.py` & `handshakes-0.3.3/handshake/services/DBService/models/dynamic_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-from handshake.services.DBService.models.enums import ConfigKeys
-from tortoise.fields import IntField, CharField
-from handshake.services.DBService.models.result_base import RunBase
-from tortoise.models import Model
-from tortoise.fields import (
-    CharEnumField,
-    ForeignKeyField,
-    ForeignKeyRelation,
-    TextField,
-    UUIDField,
-    BooleanField,
-)
-
-
-class ConfigBase(Model):
-    key = CharEnumField(
-        ConfigKeys, pk=True, null=False, description="Type of job we would like to run"
-    )
-    value = TextField(null=False, description="Handling type is upto us")
-
-
-class ExportBase(Model):
-    ticketID = UUIDField(pk=True)
-    maxTestRuns = IntField(
-        null=True,
-        default=10,
-        description="Number of test runs to export [recent ones are picked]",
-    )
-
-
-class TestConfigBase(Model):
-    test: ForeignKeyRelation[RunBase] = ForeignKeyField(
-        "models.RunBase", related_name="config", to_field="testID"
-    )
-    platform = TextField(null=False, description="could be windows or linux")
-    framework = TextField(null=False, description="name of the framework used")
-    maxInstances = IntField(
-        null=True, default=1, description="Max. Number of workers used to run the tests"
-    )
-    exitCode = IntField(
-        null=False, default=0, description="Exit code for the test execution"
-    )
-    fileRetries = IntField(
-        null=False,
-        default=0,
-        description="Number of times it retried to execute a spec file",
-    )
-    avoidParentSuitesInCount = BooleanField(
-        null=False,
-        default=False,
-        description="whether to count the spec file as a suite or not,"
-        " example: in gherkin if in a feature file with one scenario, "
-        "if this value is true then the number of suites is treated as 1 else 2",
-    )
-    bail = IntField(
-        null=False,
-        default=0,
-        description="if > 0 then it means that run would stop if it finds this number of test cases failed",
-    )
+from tortoise.models import Model
+from tortoise.fields import (
+    CharField,
+    DatetimeField,
+    JSONField,
+    CharEnumField,
+    ForeignKeyField,
+    ForeignKeyRelation,
+    BooleanField,
+    TextField,
+)
+from handshake.services.SchedularService.constants import JobType
+from handshake.services.DBService.models.result_base import RunBase
+from handshake.services.DBService.models.enums import PrunedRecords
+
+
+class TaskBase(Model):
+    table = "TaskBase"
+
+    ticketID = CharField(max_length=45, pk=True)
+    type = CharEnumField(JobType, null=False)
+    dropped = DatetimeField(auto_now=True)  # use modified timestamp
+    # this would schedule the parent suites in the later rounds
+    meta = JSONField(
+        null=True,
+        default={},
+        description="Data required to process the task, Not used as of now though",
+    )
+    test: ForeignKeyRelation[RunBase] = ForeignKeyField(
+        "models.RunBase", related_name="test", to_field="testID"
+    )
+    picked = BooleanField(
+        null=True,
+        default=False,
+        description="True if the task is picked by the job else False",
+    )
+    processed = BooleanField(
+        null=True,
+        default=False,
+        description="True if the task is processed or completed",
+    )
+
+
+class PrunedBase:
+    prunedID = CharField(
+        max_length=36, description="possibly uuid of length 36 that was pruned"
+    )
+    reason = TextField(description="Reason for its existence here")
+    details = JSONField(
+        null=True, default={}, description="If any details were required"
+    )
+    type = CharEnumField(PrunedRecords, null=False)
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/models/result_base.py` & `handshakes-0.3.3/handshake/services/DBService/models/result_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,170 @@
-from tortoise.models import Model
-from tortoise.fields import (
-    DatetimeField,
-    IntField,
-    FloatField,
-    JSONField,
-    CharEnumField,
-    UUIDField,
-    CharField,
-    ReverseRelation,
-    ForeignKeyField,
-    BooleanField,
-    ForeignKeyRelation,
-    TextField,
-)
-from tortoise.contrib.pydantic import pydantic_model_creator
-from handshake.services.DBService.models.enums import Status, SuiteType, LogType
-
-
-class CommandReportFields(Model):
-    started = DatetimeField(descrption="Start Datetime field")
-    ended = DatetimeField(null=True, description="End Datetime field")
-    tests = IntField(default=0, null=False, description="No. of the test entries")
-    passed = IntField(default=0, null=False, description="Passed test entities")
-    failed = IntField(default=0, null=False, description="Failed test entities")
-    skipped = IntField(
-        default=0, null=False, description="test entities that were skipped"
-    )
-    duration = FloatField(default=0, null=False, description="duration of test entity")
-    retried = IntField(
-        default=0, null=False, description="number of the retries performed"
-    )
-    suitesConfig = JSONField(description="Dict. of suites", default={})
-
-    class Meta:
-        abstract = True
-
-
-class CommonDetailedFields(CommandReportFields):
-    suitesConfig = JSONField(description="Dict. of suites", default={})  # not used yet.
-
-    class Meta:
-        abstract = True
-
-
-class EntityBaseSpecific:
-    standing = CharEnumField(
-        Status, description="status of the test run", default=Status.PENDING
-    )
-
-    class Meta:
-        abstract = True
-
-
-class RunBase(CommonDetailedFields, EntityBaseSpecific):
-    table = "RunBase"
-    testID = UUIDField(pk=True)
-    sessions = ReverseRelation["SessionBase"]
-    tasks = ReverseRelation["TaskBase"]
-    config = ReverseRelation["TestConfigBase"]
-    started = DatetimeField(null=False, auto_now_add=True)
-    projectName = CharField(
-        max_length=30, null=False, description="Name of the project"
-    )
-    specStructure = JSONField(
-        description="file structure of spec files", default=dict()
-    )
-    suiteSummary = JSONField(
-        description="summary of the suites",
-        default=dict(count=0, passed=0, failed=0, skipped=0),
-    )
-
-
-class SessionBase(CommonDetailedFields):
-    table = "SessionBase"
-    test: ForeignKeyRelation[RunBase] = ForeignKeyField(
-        "models.RunBase", related_name="sessions", to_field="testID"
-    )
-    retried = BooleanField(
-        description="was this session omitted, because there would be one more retried session",
-        default=False,
-        required=False,
-    )
-    suites = ReverseRelation["SuiteBase"]
-    sessionID = UUIDField(pk=True)
-    entityName = CharField(max_length=30, default="")
-    entityVersion = CharField(max_length=20, default="")
-    simplified = TextField(
-        default="", description="browser name & version &/ platform name included"
-    )
-    hooks = IntField(default=0, null=False, description="Number of hooks used")
-
-
-class SuiteBase(EntityBaseSpecific, CommandReportFields):
-    table = "SuiteBase"
-    # https://tortoise.github.io/models.html#the-db-backing-field
-    # so we require session_id instead of sessionID
-    session: ForeignKeyRelation[SessionBase] = ForeignKeyField(
-        "models.SessionBase", related_name="suites", to_field="sessionID"
-    )
-    attachments = ReverseRelation["AttachmentBase"]
-    suiteID = UUIDField(pk=True)
-    suiteType = CharEnumField(
-        SuiteType,
-        description="Specifies whether if it is a test suite or test case",
-        null=False,
-    )
-    title = TextField(max_length=225)
-    file = TextField(max_length=150, null=False, description="path to the spec file")
-    description = TextField(
-        null=True, default="", description="Summary if provided for the test entity"
-    )
-    parent = CharField(max_length=45, description="Parent Suite's ID", default="")
-    tags = JSONField(description="list of all tags", default=[])
-    modified = DatetimeField(
-        auto_now=True, description="Modified timestamp", null=False
-    )
-    errors = JSONField(description="Errors found", default=[], null=True)
-
-
-class RollupBase(Model):
-    tests = IntField(default=0, null=False, description="Rolled up Test Entities")
-    passed = IntField(
-        default=0, null=False, description="Rolled up Passed test entities"
-    )
-    failed = IntField(
-        default=0, null=False, description="Rolled up Failed test entities"
-    )
-    skipped = IntField(
-        default=0, null=False, description="Rolled up test entities that were skipped"
-    )
-    suite: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
-        "models.SuiteBase", related_name="rollup", to_field="suiteID"
-    )
-
-
-class RetriedBase(Model):
-    tests = JSONField(
-        default=[],
-        description="details of all suites which were retried for a particular test case",
-    )
-    suite: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
-        "models.SuiteBase", related_name="retries", to_field="suiteID"
-    )
-
-    length = IntField(
-        description="Just the length of the tests cols", default=1, null=False
-    )
-
-    modified = DatetimeField(
-        auto_now=True, description="Modified timestamp", null=False
-    )
-
-
-class TestLogBase(Model):
-    test: ForeignKeyRelation[RunBase] = ForeignKeyField(
-        "models.RunBase", related_name="log", to_field="testID", pk=True
-    )
-    type = CharEnumField(LogType, description="Log type", null=False)
-    message = TextField(description="Log Message", null=False)
-    feed = JSONField(
-        description="If you want to share any feed here", null=True, default={}
-    )
-    dropped = DatetimeField(auto_now=True, description="timestamp", null=False)
-
-
-RunBasePydanticModel = pydantic_model_creator(RunBase)
-SuiteBasePydanticModel = pydantic_model_creator(SuiteBase)
+from tortoise.models import Model
+from tortoise.fields import (
+    DatetimeField,
+    IntField,
+    FloatField,
+    JSONField,
+    CharEnumField,
+    UUIDField,
+    CharField,
+    ReverseRelation,
+    ForeignKeyField,
+    BooleanField,
+    ForeignKeyRelation,
+    TextField,
+)
+from tortoise.contrib.pydantic import pydantic_model_creator
+from handshake.services.DBService.models.enums import Status, SuiteType, LogType
+
+
+class CommandReportFields(Model):
+    started = DatetimeField(descrption="Start Datetime field")
+    ended = DatetimeField(null=True, description="End Datetime field")
+    tests = IntField(default=0, null=False, description="No. of the test entries")
+    passed = IntField(default=0, null=False, description="Passed test entities")
+    failed = IntField(default=0, null=False, description="Failed test entities")
+    skipped = IntField(
+        default=0, null=False, description="test entities that were skipped"
+    )
+    duration = FloatField(default=0, null=False, description="duration of test entity")
+    retried = IntField(
+        default=0, null=False, description="number of the retries performed"
+    )
+
+    class Meta:
+        abstract = True
+
+
+class CommonDetailedFields(CommandReportFields):
+    class Meta:
+        abstract = True
+
+
+class EntityBaseSpecific:
+    standing = CharEnumField(
+        Status, description="status of the test run", default=Status.PENDING
+    )
+
+    class Meta:
+        abstract = True
+
+
+class RunBase(CommonDetailedFields, EntityBaseSpecific):
+    table = "RunBase"
+    testID = UUIDField(pk=True)
+    sessions = ReverseRelation["SessionBase"]
+    tasks = ReverseRelation["TaskBase"]
+    config = ReverseRelation["TestConfigBase"]
+    started = DatetimeField(null=False, auto_now_add=True)
+    projectName = CharField(
+        max_length=30, null=False, description="Name of the project"
+    )
+    specStructure = JSONField(
+        description="file structure of spec files", default=dict()
+    )
+    suiteSummary = JSONField(
+        description="summary of the suites",
+        default=dict(count=0, passed=0, failed=0, skipped=0),
+    )
+    exitCode = IntField(
+        null=False, default=0, description="Exit code for the test execution"
+    )
+
+
+class SessionBase(CommonDetailedFields):
+    table = "SessionBase"
+    test: ForeignKeyRelation[RunBase] = ForeignKeyField(
+        "models.RunBase", related_name="sessions", to_field="testID"
+    )
+    retried = BooleanField(
+        description="was this session omitted, because there would be one more retried session",
+        default=False,
+        required=False,
+    )
+    suites = ReverseRelation["SuiteBase"]
+    sessionID = UUIDField(pk=True)
+    entityName = CharField(max_length=30, default="")
+    entityVersion = CharField(max_length=20, default="")
+    simplified = TextField(
+        default="", description="browser name & version &/ platform name included"
+    )
+    hooks = IntField(default=0, null=False, description="Number of hooks used")
+
+
+class SuiteBase(EntityBaseSpecific, CommandReportFields):
+    table = "SuiteBase"
+    # https://tortoise.github.io/models.html#the-db-backing-field
+    # so we require session_id instead of sessionID
+    session: ForeignKeyRelation[SessionBase] = ForeignKeyField(
+        "models.SessionBase", related_name="suites", to_field="sessionID"
+    )
+    attachments = ReverseRelation["AttachmentBase"]
+    retries = ReverseRelation["RetriedBase"]
+    rolled_up = ReverseRelation["RollupBase"]
+
+    suiteID = UUIDField(pk=True)
+    suiteType = CharEnumField(
+        SuiteType,
+        description="Specifies whether if it is a test suite or test case",
+        null=False,
+    )
+    title = TextField(max_length=225)
+    file = TextField(max_length=150, null=False, description="path to the spec file")
+    description = TextField(
+        null=True, default="", description="Summary if provided for the test entity"
+    )
+    parent = CharField(max_length=45, description="Parent Suite's ID", default="")
+    tags = JSONField(
+        description="comma separated list of tags used by the framework to filter the suites or spec files",
+        default=[],
+    )
+    modified = DatetimeField(
+        auto_now=True, description="Modified timestamp", null=False
+    )
+    errors = JSONField(description="Errors found", default=[], null=True)
+
+
+class RollupBase(Model):
+    tests = IntField(default=0, null=False, description="Rolled up Test Entities")
+    passed = IntField(
+        default=0, null=False, description="Rolled up Passed test entities"
+    )
+    failed = IntField(
+        default=0, null=False, description="Rolled up Failed test entities"
+    )
+    skipped = IntField(
+        default=0, null=False, description="Rolled up test entities that were skipped"
+    )
+    suite: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
+        "models.SuiteBase", related_name="rollup", to_field="suiteID"
+    )
+
+
+class RetriedBase(Model):
+    tests = JSONField(
+        default=[],
+        description="details of all suites which were retried for a particular test case",
+    )
+    suite: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
+        "models.SuiteBase", related_name="retries", to_field="suiteID"
+    )
+
+    length = IntField(
+        description="Just the length of the tests cols", default=1, null=False
+    )
+
+    modified = DatetimeField(
+        auto_now=True, description="Modified timestamp", null=False
+    )
+
+
+class TestLogBase(Model):
+    test: ForeignKeyRelation[RunBase] = ForeignKeyField(
+        "models.RunBase", related_name="log", to_field="testID", pk=True
+    )
+    type = CharEnumField(LogType, description="Log type", null=False)
+    message = TextField(description="Log Message", null=False)
+    feed = JSONField(
+        description="If you want to share any feed here", null=True, default={}
+    )
+    dropped = DatetimeField(auto_now=True, description="timestamp", null=False)
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/models/static_base.py` & `handshakes-0.3.3/handshake/services/DBService/models/static_base.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from handshake.services.DBService.models.types import AttachmentType
-from handshake.services.DBService.models.result_base import SuiteBase
-from tortoise.models import Model
-from tortoise.fields import (
-    JSONField,
-    CharEnumField,
-    ForeignKeyField,
-    ForeignKeyRelation,
-    TextField,
-    UUIDField,
-)
-
-
-class AttachmentFields(Model):
-    attachmentValue = JSONField(
-        description="An attachment value", default={"value": ""}
-    )
-    description = TextField(
-        null=False, description="Description Field for the attachment"
-    )
-    type = CharEnumField(
-        AttachmentType,
-        description="Type of an attachment, refer the enums to get an idea",
-    )
-
-    class Meta:
-        abstract = True
-
-
-class AttachmentBase(AttachmentFields):
-    table = "AttachmentBase"
-    entity: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
-        "models.SuiteBase", related_name="attachment", to_field="suiteID"
-    )
-
-
-class StaticBase(AttachmentFields):
-    attachmentID = UUIDField(pk=True)
-    entity: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
-        "models.SuiteBase", related_name="staticAttachments", to_field="suiteID"
-    )
+from handshake.services.DBService.models.types import AttachmentType
+from handshake.services.DBService.models.result_base import SuiteBase
+from tortoise.models import Model
+from tortoise.fields import (
+    JSONField,
+    CharEnumField,
+    ForeignKeyField,
+    ForeignKeyRelation,
+    TextField,
+    UUIDField,
+)
+
+
+class AttachmentFields(Model):
+    attachmentValue = JSONField(
+        description="An attachment value", default={"value": ""}
+    )
+    description = TextField(
+        null=False, description="Description Field for the attachment"
+    )
+    type = CharEnumField(
+        AttachmentType,
+        description="Type of an attachment, refer the enums to get an idea",
+    )
+
+    class Meta:
+        abstract = True
+
+
+class AttachmentBase(AttachmentFields):
+    table = "AttachmentBase"
+    entity: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
+        "models.SuiteBase", related_name="attachment", to_field="suiteID"
+    )
+
+
+class StaticBase(AttachmentFields):
+    attachmentID = UUIDField(pk=True)
+    entity: ForeignKeyRelation[SuiteBase] = ForeignKeyField(
+        "models.SuiteBase", related_name="staticAttachments", to_field="suiteID"
+    )
```

### Comparing `handshakes-0.3.2/handshake/services/DBService/models/types.py` & `handshakes-0.3.3/handshake/services/DBService/models/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,100 @@
-import uuid
-from typing import List, Optional, Union
-from handshake.services.DBService.models.enums import Status, SuiteType, AttachmentType
-from pydantic import BaseModel
-from datetime import datetime
-from typing_extensions import TypedDict
-
-# send iso-format for the datetime string
-
-
-class CommonRegisterCols(BaseModel):
-    started: datetime
-
-
-class RegisterSession(CommonRegisterCols):
-    ...
-
-
-class RegisterSuite(CommonRegisterCols):
-    title: str
-    retried: int
-    description: Optional[str] = ""
-    suiteType: SuiteType
-    session_id: uuid.UUID
-    file: str
-    parent: str
-    tags: Optional[List] = []
-
-
-class MarkSession(BaseModel):
-    duration: float
-    skipped: int
-    passed: int
-    failed: int
-    tests: int
-    hooks: int
-    ended: datetime
-    sessionID: uuid.UUID
-    entityName: str
-    entityVersion: str
-    simplified: str
-
-
-class Error(TypedDict):
-    name: str
-    message: str
-    stack: Optional[str]
-
-
-class MarkSuite(BaseModel):
-    duration: float
-    ended: datetime
-    suiteID: uuid.UUID
-    errors: Optional[List[Error]] = []
-    standing: Optional[Status] = Status.SKIPPED
-
-
-class AssertionPayload(TypedDict):
-    passed: bool
-    wait: Optional[int]
-    interval: Optional[int]
-    message: str
-
-
-# this is for all kinds of attachments
-class AddAttachmentForEntity(BaseModel):
-    entityID: uuid.UUID
-    type: AttachmentType
-    description: Optional[str] = ""
-    value: Union[AssertionPayload, str]
-    color: Optional[str] = ""
-    title: Optional[str] = ""
-
-
-class WrittenAttachmentForEntity(BaseModel):
-    entityID: uuid.UUID
-    type: AttachmentType
-    description: Optional[str] = ""
-    title: Optional[str] = ""
-
-
-class ValueForTestRunConfigBase(TypedDict):
-    version: str
-    platformName: str
-
-
-class PydanticModalForTestRunConfigBase(BaseModel):
-    maxInstances: Optional[int] = 1
-    platformName: str
-    framework: str
-    exitCode: int
-    bail: Optional[int] = 0
-    fileRetries: Optional[int] = 0
-    avoidParentSuitesInCount: Optional[bool] = False
-    teamsHook: Optional[str] = ""
+import uuid
+from typing import List, Optional, Union
+from handshake.services.DBService.models.enums import Status, SuiteType, AttachmentType
+from pydantic import BaseModel
+from datetime import datetime
+from typing_extensions import TypedDict
+
+# send iso-format for the datetime string
+
+
+class CommonRegisterCols(BaseModel):
+    started: datetime
+
+
+class Tag(TypedDict):
+    name: str
+    label: str
+
+
+class RegisterSession(CommonRegisterCols):
+    ...
+
+
+class RegisterSuite(CommonRegisterCols):
+    title: str
+    retried: int
+    description: Optional[str] = ""
+    suiteType: SuiteType
+    session_id: uuid.UUID
+    file: str
+    parent: str
+    tags: Optional[List[Tag]] = []
+
+
+class MarkSession(BaseModel):
+    duration: float
+    skipped: int
+    passed: int
+    failed: int
+    tests: int
+    hooks: int
+    ended: datetime
+    sessionID: uuid.UUID
+    entityName: str
+    entityVersion: str
+    simplified: str
+
+
+class Error(TypedDict):
+    name: str
+    message: str
+    stack: Optional[str]
+
+
+class MarkSuite(BaseModel):
+    duration: float
+    ended: datetime
+    suiteID: uuid.UUID
+    errors: Optional[List[Error]] = []
+    standing: Optional[Status] = Status.SKIPPED
+
+
+class AssertionPayload(TypedDict):
+    passed: bool
+    wait: Optional[int]
+    interval: Optional[int]
+    message: str
+
+
+# this is for all kinds of attachments
+class AddAttachmentForEntity(BaseModel):
+    entityID: uuid.UUID
+    type: AttachmentType
+    description: Optional[str] = ""
+    value: Union[AssertionPayload, str]
+    color: Optional[str] = ""
+    title: Optional[str] = ""
+
+
+class WrittenAttachmentForEntity(BaseModel):
+    entityID: uuid.UUID
+    type: AttachmentType
+    description: Optional[str] = ""
+    title: Optional[str] = ""
+
+
+class ValueForTestRunConfigBase(TypedDict):
+    version: str
+    platformName: str
+
+
+class PydanticModalForTestRunConfigBase(BaseModel):
+    maxInstances: Optional[int] = 1
+    platformName: str
+    framework: str
+    exitCode: int
+    bail: Optional[int] = 0
+    fileRetries: Optional[int] = 0
+    avoidParentSuitesInCount: Optional[bool] = False
+    tags: List[Tag]
```

### Comparing `handshakes-0.3.2/handshake/services/Endpoints/blueprints/coreEndpoints.py` & `handshakes-0.3.3/handshake/services/Endpoints/blueprints/coreEndpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,220 @@
-from handshake.services.DBService.models.result_base import SessionBase, SuiteBase
-from handshake.services.DBService.models.types import (
-    RegisterSession,
-    RegisterSuite,
-    MarkSuite,
-    MarkSession,
-    AddAttachmentForEntity,
-    PydanticModalForTestRunConfigBase,
-    WrittenAttachmentForEntity,
-)
-from handshake.services.Endpoints.blueprints.utils import (
-    attachError,
-    extractPayload,
-    attachWarn,
-    extractPydanticErrors,
-)
-from handshake.services.DBService.models.static_base import (
-    AttachmentBase,
-    AttachmentType,
-)
-from handshake.services.DBService.models.config_base import TestConfigBase
-from handshake.services.DBService.models.attachmentBase import AssertBase
-from handshake.services.DBService.models.enums import Status, SuiteType
-from handshake.services.DBService.models.static_base import StaticBase
-from sanic.blueprints import Blueprint
-from sanic.response import JSONResponse, text, HTTPResponse
-from loguru import logger
-from sanic.request import Request
-from handshake.services.DBService.shared import get_test_id
-from handshake.services.SchedularService.register import register_patch_suite
-from pydantic import ValidationError
-from dotenv import load_dotenv
-from handshake.services.DBService.lifecycle import attachment_folder, db_path
-
-load_dotenv()
-
-
-service = Blueprint("DBService", url_prefix="/save")
-
-
-@service.on_response
-async def handle_response(request: Request, response: JSONResponse):
-    if 200 <= response.status < 300:
-        return response
-
-    payload = extractPayload(request, response)
-    await attachError(payload, request.url)
-    return JSONResponse(body=payload, status=response.status)
-
-
-@service.put("/registerSession")
-async def register_session(request: Request) -> HTTPResponse:
-    try:
-        session = RegisterSession.model_validate(request.json)
-        session_record = await SessionBase.create(
-            **session.model_dump(), test_id=get_test_id()
-        )
-        await session_record.save()
-    except Exception as error:
-        logger.error("Failed to create a session due to exception: {}", str(error))
-        return text(str(error), status=404)
-
-    return text(str(session_record.sessionID), status=201)
-
-
-@service.put("/registerSuite")
-async def register_suite(request: Request) -> HTTPResponse:
-    suite = RegisterSuite.model_validate(request.json)
-    suite_record = await SuiteBase.create(**suite.model_dump())
-    await suite_record.save()
-
-    return text(str(suite_record.suiteID), status=201)
-
-
-@service.put("/updateSuite", error_format="json")
-async def updateSuite(request: Request) -> HTTPResponse:
-    suite = MarkSuite.model_validate(request.json)
-
-    suite_record = await SuiteBase.filter(suiteID=suite.suiteID).first()
-    if not suite_record:
-        logger.error("Was not able to found {} suite", str(suite.suiteID))
-        return text(f"Suite {suite.suiteID} was not found", status=404)
-
-    if suite_record.suiteType == SuiteType.SUITE:
-        suite.standing = Status.YET_TO_CALCULATE
-    else:
-        note = {
-            suite.standing.lower(): 1,
-            "tests": 1,
-        }
-        await suite_record.update_from_dict(note)
-        await suite_record.save()
-
-    await suite_record.update_from_dict(suite.model_dump())
-    await suite_record.save()
-
-    if suite_record.suiteType == SuiteType.SUITE:
-        await register_patch_suite(suite_record.suiteID, get_test_id())
-
-    return text(
-        f"Suite: {suite_record.title} - {suite_record.suiteID} was updated", status=201
-    )
-
-
-@service.put("/updateSession", error_format="json")
-async def update_session(request: Request) -> HTTPResponse:
-    session = MarkSession.model_validate(request.json)
-    test_session = await SessionBase.filter(sessionID=session.sessionID).first()
-    if not test_session:
-        logger.error("Expected {} session was not found", str(session.sessionID))
-        return text(f"Session {session.sessionID} was not found", status=404)
-
-    await test_session.update_from_dict(session.model_dump())
-    await test_session.save()
-    return text(f"{session.sessionID} was updated", status=201)
-
-
-@service.put("/addAttachmentsForEntities")
-async def addAttachmentForEntity(request: Request) -> HTTPResponse:
-    attachments = []
-    note = []
-    assertions = []
-
-    for _ in request.json:
-        try:
-            if _["type"] == AttachmentType.ASSERT:
-                value = _.get("value", dict())
-                value["wait"] = value.get("wait", -1)
-                value["interval"] = value.get("interval", -1)
-
-            attachment = AddAttachmentForEntity.model_validate(_)
-        except ValidationError as error:
-            note.append(_.get("entityID", False))
-            url = "/addAttachmentsForEntities"
-            await attachWarn(extractPydanticErrors(url, _, error), url)
-            continue
-
-        match attachment.type:
-            case AttachmentType.ASSERT:
-                assertions.append(
-                    await AssertBase(
-                        **dict(
-                            entity_id=attachment.entityID,
-                            title=attachment.title,
-                            message=attachment.value["message"],
-                            passed=attachment.value["passed"],
-                            interval=attachment.value["interval"],
-                            wait=attachment.value["wait"],
-                        )
-                    )
-                )
-
-            case _:
-                (
-                    attachments.append(
-                        await AttachmentBase(
-                            **dict(
-                                entity_id=attachment.entityID,
-                                description=attachment.description,
-                                type=attachment.type,
-                                attachmentValue=dict(
-                                    color=attachment.color,
-                                    value=attachment.value,
-                                    title=attachment.title,
-                                ),
-                            )
-                        )
-                    )
-                )
-
-    if attachments:
-        await AttachmentBase.bulk_create(attachments)
-    if assertions:
-        await AssertBase.bulk_create(assertions)
-    return text(
-        "Attachments was added successfully", status=201 if not len(note) else 206
-    )
-
-
-@service.put("/currentRun")
-async def update_run_config(request: Request) -> HTTPResponse:
-    run_config = PydanticModalForTestRunConfigBase.model_validate(request.json)
-    config = await TestConfigBase.create(
-        test_id=get_test_id(),
-        platform=run_config.platformName,
-        framework=run_config.framework,
-        maxInstances=run_config.maxInstances,
-        exitCode=run_config.exitCode,
-        fileRetries=run_config.fileRetries,
-        avoidParentSuitesInCount=run_config.avoidParentSuitesInCount,
-        bail=run_config.bail,
-    )
-    await config.save()
-
-    return text("provided config was saved successfully.", status=200)
-
-
-@service.put("/registerAWrittenAttachment", error_format="json")
-async def saveImage(request: Request) -> HTTPResponse:
-    attachment = WrittenAttachmentForEntity.model_validate(request.json)
-    record = await StaticBase.create(
-        entity_id=attachment.entityID,
-        description=attachment.description,
-        type=attachment.type,
-    )
-    file_name = f"{record.attachmentID}.{record.type.lower()}"
-    await record.update_from_dict(
-        dict(
-            attachmentValue=dict(value=file_name, title=attachment.title),
-        )
-    )
-    await record.save()
-    # we can save the file in this request itself, but no. we let the framework's custom reporter cook.
-    return text(
-        str(attachment_folder(db_path()) / get_test_id() / file_name), status=201
-    )
+from handshake.services.DBService.models.result_base import SessionBase, SuiteBase
+from handshake.services.DBService.models.types import (
+    RegisterSession,
+    RegisterSuite,
+    MarkSuite,
+    MarkSession,
+    AddAttachmentForEntity,
+    PydanticModalForTestRunConfigBase,
+    WrittenAttachmentForEntity,
+)
+from handshake.services.Endpoints.blueprints.utils import (
+    attachError,
+    extractPayload,
+    attachWarn,
+    extractPydanticErrors,
+)
+from handshake.services.DBService.models.static_base import (
+    AttachmentBase,
+    AttachmentType,
+)
+from handshake.services.DBService.models.config_base import TestConfigBase
+from handshake.services.DBService.models.attachmentBase import AssertBase
+from handshake.services.DBService.models.enums import Status, SuiteType
+from handshake.services.DBService.models.static_base import StaticBase
+from sanic.blueprints import Blueprint
+from sanic.response import JSONResponse, text, HTTPResponse
+from loguru import logger
+from sanic.request import Request
+from handshake.services.DBService.shared import get_test_id
+from handshake.services.SchedularService.register import register_patch_suite
+from pydantic import ValidationError
+from dotenv import load_dotenv
+from handshake.services.DBService.lifecycle import attachment_folder, db_path
+
+load_dotenv()
+
+
+service = Blueprint("DBService", url_prefix="/save")
+
+
+@service.on_response
+async def handle_response(request: Request, response: JSONResponse):
+    if 200 <= response.status < 300:
+        return response
+
+    payload = extractPayload(request, response)
+    await attachError(payload, request.url)
+    return JSONResponse(body=payload, status=response.status)
+
+
+@service.put("/registerSession")
+async def register_session(request: Request) -> HTTPResponse:
+    try:
+        session = RegisterSession.model_validate(request.json)
+        session_record = await SessionBase.create(
+            **session.model_dump(), test_id=get_test_id()
+        )
+        await session_record.save()
+    except Exception as error:
+        logger.error("Failed to create a session due to exception: {}", str(error))
+        return text(str(error), status=404)
+
+    return text(str(session_record.sessionID), status=201)
+
+
+@service.put("/registerSuite")
+async def register_suite(request: Request) -> HTTPResponse:
+    suite = RegisterSuite.model_validate(request.json)
+    suite_record = await SuiteBase.create(**suite.model_dump())
+    await suite_record.save()
+
+    return text(str(suite_record.suiteID), status=201)
+
+
+@service.put("/updateSuite", error_format="json")
+async def updateSuite(request: Request) -> HTTPResponse:
+    suite = MarkSuite.model_validate(request.json)
+
+    suite_record = await SuiteBase.filter(suiteID=suite.suiteID).first()
+    if not suite_record:
+        logger.error("Was not able to found {} suite", str(suite.suiteID))
+        return text(f"Suite {suite.suiteID} was not found", status=404)
+
+    if suite_record.suiteType == SuiteType.SUITE:
+        suite.standing = Status.YET_TO_CALCULATE
+    else:
+        note = {
+            suite.standing.lower(): 1,
+            "tests": 1,
+        }
+        await suite_record.update_from_dict(note)
+        await suite_record.save()
+
+    await suite_record.update_from_dict(suite.model_dump())
+    await suite_record.save()
+
+    if suite_record.suiteType == SuiteType.SUITE:
+        await register_patch_suite(suite_record.suiteID, get_test_id())
+
+    return text(
+        f"Suite: {suite_record.title} - {suite_record.suiteID} was updated", status=201
+    )
+
+
+@service.put("/updateSession", error_format="json")
+async def update_session(request: Request) -> HTTPResponse:
+    session = MarkSession.model_validate(request.json)
+    test_session = await SessionBase.filter(sessionID=session.sessionID).first()
+    if not test_session:
+        logger.error("Expected {} session was not found", str(session.sessionID))
+        return text(f"Session {session.sessionID} was not found", status=404)
+
+    await test_session.update_from_dict(session.model_dump())
+    await test_session.save()
+    return text(f"{session.sessionID} was updated", status=201)
+
+
+@service.put("/addAttachmentsForEntities")
+async def addAttachmentForEntity(request: Request) -> HTTPResponse:
+    attachments = []
+    note = []
+    assertions = []
+
+    for _ in request.json:
+        try:
+            if _["type"] == AttachmentType.ASSERT:
+                value = _.get("value", dict())
+                value["wait"] = value.get("wait", -1)
+                value["interval"] = value.get("interval", -1)
+
+            attachment = AddAttachmentForEntity.model_validate(_)
+        except ValidationError as error:
+            note.append(_.get("entityID", False))
+            url = "/addAttachmentsForEntities"
+            await attachWarn(extractPydanticErrors(url, _, error), url)
+            continue
+
+        match attachment.type:
+            case AttachmentType.ASSERT:
+                assertions.append(
+                    await AssertBase(
+                        **dict(
+                            entity_id=attachment.entityID,
+                            title=attachment.title,
+                            message=attachment.value["message"],
+                            passed=attachment.value["passed"],
+                            interval=attachment.value["interval"],
+                            wait=attachment.value["wait"],
+                        )
+                    )
+                )
+
+            case _:
+                (
+                    attachments.append(
+                        await AttachmentBase(
+                            **dict(
+                                entity_id=attachment.entityID,
+                                description=attachment.description,
+                                type=attachment.type,
+                                attachmentValue=dict(
+                                    color=attachment.color,
+                                    value=attachment.value,
+                                    title=attachment.title,
+                                ),
+                            )
+                        )
+                    )
+                )
+
+    if attachments:
+        await AttachmentBase.bulk_create(attachments)
+    if assertions:
+        await AssertBase.bulk_create(assertions)
+    return text(
+        "Attachments was added successfully", status=201 if not len(note) else 206
+    )
+
+
+@service.put("/currentRun")
+async def update_run_config(request: Request) -> HTTPResponse:
+    run_config = PydanticModalForTestRunConfigBase.model_validate(request.json)
+    config = await TestConfigBase.create(
+        test_id=get_test_id(),
+        platform=run_config.platformName,
+        framework=run_config.framework,
+        maxInstances=run_config.maxInstances,
+        fileRetries=run_config.fileRetries,
+        avoidParentSuitesInCount=run_config.avoidParentSuitesInCount,
+        bail=run_config.bail,
+        tags=run_config.tags,
+    )
+
+    test = await config.test
+    await test.update_from_dict(dict(exitCode=run_config.exitCode))
+    await test.save()
+    await config.save()
+
+    return text("provided config was saved successfully.", status=200)
+
+
+@service.put("/registerAWrittenAttachment", error_format="json")
+async def saveImage(request: Request) -> HTTPResponse:
+    attachment = WrittenAttachmentForEntity.model_validate(request.json)
+    record = await StaticBase.create(
+        entity_id=attachment.entityID,
+        description=attachment.description,
+        type=attachment.type,
+    )
+    file_name = f"{record.attachmentID}.{record.type.lower()}"
+    await record.update_from_dict(
+        dict(
+            attachmentValue=dict(value=file_name, title=attachment.title),
+        )
+    )
+    await record.save()
+    # we can save the file in this request itself, but no. we let the framework's custom reporter cook.
+    return text(
+        str(attachment_folder(db_path()) / get_test_id() / file_name), status=201
+    )
```

### Comparing `handshakes-0.3.2/handshake/services/Endpoints/blueprints/utils.py` & `handshakes-0.3.3/handshake/services/Endpoints/blueprints/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from handshake.services.DBService.models.result_base import LogType, TestLogBase
-from handshake.services.DBService.shared import get_test_id
-from sanic.request import Request
-from sanic.response import JSONResponse
-from pydantic import ValidationError
-
-
-def extractPayload(request: Request, response: JSONResponse):
-    payload = dict(
-        url=request.url,
-        payload=request.json,
-        status=response.status,
-        reason=response.body.decode(),
-    )
-    return payload
-
-
-def extractPydanticErrors(url, payload, error: ValidationError):
-    payload = dict(
-        url=url,
-        payload=payload,
-        status="ERROR",
-        reason=error.json(),
-    )
-    return payload
-
-
-async def attachLog(payload, attachmentType: LogType, description: str):
-    await TestLogBase.create(
-        test_id=get_test_id(),
-        type=attachmentType,
-        feed=payload,
-        message=description,
-    )
-
-
-async def attachError(payload, url: str):
-    await attachLog(
-        payload,
-        LogType.ERROR,
-        f"Failed to process the request at: {url}, will affect the test run",
-    )
-
-
-async def attachInfo(payload, url: str):
-    await attachLog(
-        payload,
-        LogType.INFO,
-        f"utilizing: {url}",
-    )
-
-
-async def attachWarn(payload, url: str):
-    await attachLog(
-        payload,
-        LogType.WARN,
-        f"Failed to process the request at: {url}, we will miss this attachment",
-    )
+from handshake.services.DBService.models.result_base import LogType, TestLogBase
+from handshake.services.DBService.shared import get_test_id
+from sanic.request import Request
+from sanic.response import JSONResponse
+from pydantic import ValidationError
+
+
+def extractPayload(request: Request, response: JSONResponse):
+    payload = dict(
+        url=request.url,
+        payload=request.json,
+        status=response.status,
+        reason=response.body.decode(),
+    )
+    return payload
+
+
+def extractPydanticErrors(url, payload, error: ValidationError):
+    payload = dict(
+        url=url,
+        payload=payload,
+        status="ERROR",
+        reason=error.json(),
+    )
+    return payload
+
+
+async def attachLog(payload, attachmentType: LogType, description: str):
+    await TestLogBase.create(
+        test_id=get_test_id(),
+        type=attachmentType,
+        feed=payload,
+        message=description,
+    )
+
+
+async def attachError(payload, url: str):
+    await attachLog(
+        payload,
+        LogType.ERROR,
+        f"Failed to process the request at: {url}, will affect the test run",
+    )
+
+
+async def attachInfo(payload, url: str):
+    await attachLog(
+        payload,
+        LogType.INFO,
+        f"utilizing: {url}",
+    )
+
+
+async def attachWarn(payload, url: str):
+    await attachLog(
+        payload,
+        LogType.WARN,
+        f"Failed to process the request at: {url}, we will miss this attachment",
+    )
```

### Comparing `handshakes-0.3.2/handshake/services/Endpoints/core.py` & `handshakes-0.3.3/handshake/services/Endpoints/core.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import os
-from handshake.services.DBService.lifecycle import DB_VERSION
-from handshake.services.Endpoints.internalEndpoints import one_liners
-from handshake.services.DBService.shared import APP_NAME
-from handshake.services.Endpoints.blueprints.coreEndpoints import service
-from handshake.services.Endpoints.blueprints.writeServices import writeServices
-from handshake.services.Endpoints.errorHandling import handle_validation_error
-from sanic import Sanic
-from pydantic import ValidationError
-import sentry_sdk
-from handshake import __version__
-
-dns = os.getenv("SENTRY_SDK")
-if dns:
-    sentry_sdk.init(
-        dsn=os.getenv("SENTRY_SDK"),
-        enable_tracing=True,
-        max_breadcrumbs=10,
-        release=f"{__version__} - {DB_VERSION}",
-        server_name=APP_NAME,
-    )
-
-service_provider = Sanic(APP_NAME)
-service_provider.config.TOUCHUP = False
-service_provider.blueprint(one_liners)
-service_provider.blueprint(service)
-service_provider.blueprint(writeServices)
-
-service_provider.error_handler.add(ValidationError, handle_validation_error)
+import os
+from handshake.services.DBService.lifecycle import DB_VERSION
+from handshake.services.Endpoints.internalEndpoints import one_liners
+from handshake.services.DBService.shared import APP_NAME
+from handshake.services.Endpoints.blueprints.coreEndpoints import service
+from handshake.services.Endpoints.blueprints.writeServices import writeServices
+from handshake.services.Endpoints.errorHandling import handle_validation_error
+from sanic import Sanic
+from pydantic import ValidationError
+import sentry_sdk
+from handshake import __version__
+
+dns = os.getenv("SENTRY_SDK")
+if dns:
+    sentry_sdk.init(
+        dsn=os.getenv("SENTRY_SDK"),
+        enable_tracing=True,
+        max_breadcrumbs=10,
+        release=f"{__version__} - {DB_VERSION}",
+        server_name=APP_NAME,
+    )
+
+service_provider = Sanic(APP_NAME)
+service_provider.config.TOUCHUP = False
+service_provider.blueprint(one_liners)
+service_provider.blueprint(service)
+service_provider.blueprint(writeServices)
+
+service_provider.error_handler.add(ValidationError, handle_validation_error)
```

### Comparing `handshakes-0.3.2/handshake/services/Endpoints/internalEndpoints.py` & `handshakes-0.3.3/handshake/services/Endpoints/internalEndpoints.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from handshake.services.DBService.shared import get_test_id
-from handshake.services.DBService.lifecycle import close_connection
-from sanic.blueprints import Blueprint
-from sanic.response import HTTPResponse, text
-from sanic.request import Request
-from handshake.services.SchedularService.register import register_patch_test_run
-
-one_liners = Blueprint(name="one_liners", url_prefix="/")
-
-
-# Here we will have requests which are very simple but used at crucial points
-
-
-@one_liners.get("/")
-async def health_status(request: Request) -> HTTPResponse:
-    return text("1")
-
-
-@one_liners.put("/done")
-async def set_done(request: Request) -> HTTPResponse:
-    task = await register_patch_test_run(get_test_id())
-    return text(task.ticketID)
-
-
-# bye is core request, so make sure to handle it carefully
-@one_liners.post("/bye")
-async def bye(request: Request) -> HTTPResponse:
-    await close_connection()
-    request.app.m.terminate()
-
-    return text("1")
+from handshake.services.DBService.shared import get_test_id
+from handshake.services.DBService.lifecycle import close_connection
+from sanic.blueprints import Blueprint
+from sanic.response import HTTPResponse, text
+from sanic.request import Request
+from handshake.services.SchedularService.register import register_patch_test_run
+
+one_liners = Blueprint(name="one_liners", url_prefix="/")
+
+
+# Here we will have requests which are very simple but used at crucial points
+
+
+@one_liners.get("/")
+async def health_status(request: Request) -> HTTPResponse:
+    return text("1")
+
+
+@one_liners.put("/done")
+async def set_done(request: Request) -> HTTPResponse:
+    task = await register_patch_test_run(get_test_id())
+    return text(task.ticketID)
+
+
+# bye is core request, so make sure to handle it carefully
+@one_liners.post("/bye")
+async def bye(request: Request) -> HTTPResponse:
+    await close_connection()
+    request.app.m.terminate()
+
+    return text("1")
```

### Comparing `handshakes-0.3.2/handshake/services/SchedularService/completeTestRun.py` & `handshakes-0.3.3/handshake/services/SchedularService/completeTestRun.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,274 @@
-from handshake.services.DBService.models.result_base import (
-    SessionBase,
-    RunBase,
-    SuiteBase,
-)
-from handshake.services.DBService.models.config_base import TestConfigBase
-from uuid import UUID
-from typing import Union
-from traceback import format_exc
-from handshake.services.SchedularService.register import (
-    skip_test_run,
-)
-from handshake.services.DBService.models.dynamic_base import TaskBase
-from handshake.services.DBService.models.types import Status, SuiteType
-from handshake.services.SchedularService.refer_types import PathTree, PathItem
-from handshake.services.SchedularService.modifySuites import fetch_key_from_status
-from tortoise.functions import Sum, Max, Min, Count, Lower
-from datetime import datetime, timezone
-from typing import List
-from pathlib import Path
-from os.path import join
-from loguru import logger
-from tortoise.expressions import Q
-
-
-async def skip_coz_error(test_id: Union[str, UUID], reason: str, **extra) -> False:
-    return await skip_test_run(test_id, reason, **extra)
-
-
-async def mark_test_failure_if_required(test_id: str) -> bool:
-    test_run = await RunBase.filter(testID=test_id).first()
-    if test_run.ended is None:
-        await skip_coz_error(
-            test_id,
-            f"Failed to patch the Test Run: {test_id} of project: {test_run.projectName},"
-            f" because it didn't have a end date",
-            incomplete=test_run.projectName,
-        )
-        return True
-
-    suites = [
-        str(_)
-        for _ in await SuiteBase.filter(session__test_id=test_id)
-        .filter(Q(standing=Status.YET_TO_CALCULATE) | Q(standing=Status.PENDING))
-        .all()
-        .values_list("suiteID", flat=True)
-    ]
-
-    does_it_exist = await TaskBase.exists(ticketID__in=suites)
-    if does_it_exist:
-        # it means there are child tasks ensured to complete the child suites
-        return False
-
-    reason = f"Failed to patch TestRun: {test_id} because of incomplete child suites"
-    await skip_coz_error(test_id, reason, incomplete=suites)
-    return True
-
-
-def simplify_file_paths(paths: List[str]):
-    tree: PathTree = {"<path>": ""}
-    _paths: List[PathItem] = [
-        dict(
-            children=list(reversed(Path(path).parts)),
-            pointer=tree,
-        )
-        for path in paths
-    ]
-
-    # Tree - Builder
-    while _paths:
-        path_to_include = _paths[-1]
-        if not path_to_include["children"]:
-            _paths.pop()
-            continue
-
-        parent_pointer: PathTree = path_to_include["pointer"]
-        possible_parent: str = path_to_include["children"].pop()
-        # that dict will be inside the tree
-
-        pointing_to = parent_pointer.setdefault(
-            possible_parent, {"<path>": join(parent_pointer["<path>"], possible_parent)}
-        )
-        path_to_include["pointer"] = pointing_to
-
-    # Reducer
-    while True:
-        stack = [(_, tree) for _ in tree.keys() if not _.startswith("<")]
-        movements = 0
-
-        while stack:
-            node_key, parent_node = stack.pop()
-            target_node = parent_node[node_key]
-
-            children = set(target_node.keys())
-            children.remove("<path>")
-
-            if len(children) > 1:
-                for child_key in target_node.keys():
-                    if child_key.startswith("<"):
-                        continue
-                    stack.append((child_key, target_node))
-                continue
-
-            if not children:
-                continue
-            child_key = children.pop()
-
-            movements += 1
-            target_popped = parent_node.pop(node_key)
-            new_key = join(node_key, child_key)
-            parent_node[new_key] = target_popped.pop(child_key)
-            new_child = parent_node[new_key]
-            new_child["<path>"] = join(target_popped["<path>"], child_key)
-
-            for child_key in new_child.keys():
-                if child_key.startswith("<"):
-                    continue
-                stack.append((child_key, new_child))
-
-        if not movements:
-            break
-
-    return tree
-
-
-async def patchValues(test_run: RunBase):
-    test_id = test_run.testID
-
-    filtered = SessionBase.filter(Q(test_id=test_id) & Q(retried=False))
-    retried_sessions = await SessionBase.filter(
-        Q(test_id=test_id) & Q(retried=True)
-    ).count()
-
-    actual_start = "actual_start"
-    actual_end = "actual_end"
-
-    test_result = (
-        await filtered.annotate(
-            passed=Sum("passed"),
-            failed=Sum("failed"),
-            skipped=Sum("skipped"),
-            tests=Sum("tests"),
-            actual_end=Max("ended"),
-            actual_start=Min("started"),
-        )
-        .first()
-        .values("passed", "failed", "skipped", "tests", actual_start, actual_end)
-    )
-
-    test_config = await TestConfigBase.filter(test_id=test_id).first()
-
-    refer = SuiteBase
-
-    if test_config:
-        # consider cucumber files
-        # if the feature file has 3 scenarios, then if user sets the avoidParentSuitesInCount
-        # we would get a value of 3 as total scenarios else 4
-        if test_config.avoidParentSuitesInCount:
-            refer = SuiteBase.filter(~Q(parent=""))
-
-    # we want to count the number of suites status
-    summary = dict(passed=0, failed=0, skipped=0)
-    summary.update(
-        await refer.filter(
-            Q(session__test_id=test_id)
-            & Q(suiteType=SuiteType.SUITE)
-            & ~Q(standing=Status.RETRIED)
-        )
-        .annotate(count=Count("suiteID"), status=Lower("standing"))
-        .group_by("standing")
-        .values_list("status", "count")
-    )
-    summary["count"] = sum(summary.values())
-
-    # start date was initially when we start the shipment
-    # now it is when the first session starts
-    started = test_result.get(actual_start, test_run.started) or test_run.started
-    ended = test_result.get(actual_end, datetime.now(timezone.utc)) or datetime.now(
-        timezone.utc
-    )
-    test_result.pop(actual_start) if actual_start in test_result else ...
-    test_result.pop(actual_end) if actual_end in test_result else ...
-
-    await test_run.update_from_dict(
-        dict(
-            **{_: test_result[_] or 0 for _ in test_result.keys()},
-            retried=retried_sessions,
-            started=started,
-            ended=ended,
-            duration=(ended - started).total_seconds() * 1000,
-            specStructure=simplify_file_paths(
-                [
-                    path
-                    for path in await SuiteBase.filter(Q(session__test_id=test_id))
-                    .distinct()
-                    .values_list("file", flat=True)
-                ]
-            ),
-            standing=fetch_key_from_status(
-                summary["passed"], summary["failed"], summary["skipped"]
-            ),
-            suiteSummary=summary,
-        )
-    )
-    return True
-
-
-async def patchTestRun(test_id: str, current_test_id: str):
-    test_run = await RunBase.filter(testID=test_id).first()
-    if not test_run:
-        return True
-
-    task = await TaskBase.filter(ticketID=test_run.testID).first()
-    if not task:
-        return True
-
-    logger.info("Patching up the Test Run: {}", test_id)
-
-    if test_run.standing != Status.PENDING:
-        logger.warning("{} was already processed", test_id)
-        return True
-
-    pending_items = (
-        await SuiteBase.filter(session__test_id=test_id)
-        .filter(Q(standing=Status.YET_TO_CALCULATE) | Q(standing=Status.PENDING))
-        .count()
-    )
-
-    if pending_items > 0:
-        if await mark_test_failure_if_required(test_id):
-            return
-        logger.warning(
-            "Patch Test Run: {} will be picked in the next run, some of its entities are not processed yet.",
-            test_id,
-        )
-        await task.update_from_dict(dict(picked=False))
-        await task.save()  # continue in the next run
-        return False
-
-    to_return = False
-    try:
-        if await patchValues(test_run):
-            logger.info("Completed the patch for test run: {}", test_id)
-            to_return = True
-    except Exception:
-        await skip_coz_error(
-            test_id,
-            f"Failed to patch the test run, error in calculation, {format_exc()}",
-        )
-    finally:
-        await test_run.save()
-
-    return to_return
+from handshake.services.DBService.models.result_base import (
+    SessionBase,
+    RunBase,
+    SuiteBase,
+)
+from handshake.services.DBService.models.config_base import TestConfigBase
+from uuid import UUID
+from typing import Union
+from traceback import format_exc
+from handshake.services.SchedularService.register import (
+    skip_test_run,
+)
+from handshake.services.SchedularService.constants import JobType
+from handshake.services.DBService.models.dynamic_base import TaskBase
+from handshake.services.DBService.models.types import Status, SuiteType
+from handshake.services.SchedularService.refer_types import PathTree, PathItem
+from handshake.services.SchedularService.modifySuites import fetch_key_from_status
+from tortoise.functions import Sum, Max, Min, Count, Lower
+from datetime import datetime, timezone
+from typing import List, Tuple
+from pathlib import Path
+from os.path import join
+from loguru import logger
+from tortoise.expressions import Q
+from typing import Optional
+from asyncio import gather
+
+
+class PatchTestRun:
+    actual_start = "actual_start"
+    actual_end = "actual_end"
+
+    def __init__(self, test_id):
+        self.test: Optional[RunBase] = None
+        self.test_id = test_id
+        self.task: Optional[TaskBase] = None
+
+    async def fetch_records(self):
+        self.test = await RunBase.filter(testID=self.test_id).first()
+        self.task = await TaskBase.filter(ticketID=self.test_id).first()
+
+    async def patch_test(self):
+        await self.fetch_records()
+        if not await self.do_we_need_patch():
+            return False
+        await self.patch_test_values()
+        await self.mark_processed()
+        return True
+
+    async def mark_processed(self):
+        self.task.processed = True
+        await self.task.save()
+
+    async def fetch_suite_summary(self):
+        test_config = await TestConfigBase.filter(test_id=self.test_id).first()
+
+        refer = SuiteBase
+
+        if test_config:
+            # consider cucumber files
+            # if the feature file has 3 scenarios, then if user sets the avoidParentSuitesInCount
+            # we would get a value of 3 as total scenarios else 4
+            if test_config.avoidParentSuitesInCount:
+                refer = SuiteBase.filter(~Q(parent=""))
+
+        # we want to count the number of suites status
+        summary = dict(passed=0, failed=0, skipped=0)
+        summary.update(
+            await refer.filter(
+                Q(session__test_id=self.test_id)
+                & Q(suiteType=SuiteType.SUITE)
+                & ~Q(standing=Status.RETRIED)
+            )
+            .annotate(count=Count("suiteID"), status=Lower("standing"))
+            .group_by("standing")
+            .values_list("status", "count")
+        )
+        summary["count"] = sum(summary.values())
+
+        return summary
+
+    async def fetch_agg_values_of_test(self):
+        filtered = SessionBase.filter(Q(test_id=self.test_id) & Q(retried=False))
+
+        # we get the values of the test run from the non-retried test sessions
+        test_result = (
+            await filtered.annotate(
+                passed=Sum("passed"),
+                failed=Sum("failed"),
+                skipped=Sum("skipped"),
+                tests=Sum("tests"),
+                actual_end=Max("ended"),
+                actual_start=Min("started"),
+            )
+            .first()
+            .values(
+                "passed",
+                "failed",
+                "skipped",
+                "tests",
+                self.actual_start,
+                self.actual_end,
+            )
+        )
+
+        return test_result
+
+    async def patch_test_values(self):
+        (summary, test_result, retried_sessions) = await gather(
+            self.fetch_suite_summary(),
+            self.fetch_agg_values_of_test(),
+            # just to get the count of the retried sessions we had in this run
+            SessionBase.filter(Q(test_id=self.test_id) & Q(retried=True)).count(),
+        )
+
+        # start date was initially when we start the shipment
+        # now it is when the first session starts
+        started = (
+            test_result.get(self.actual_start, self.test.started) or self.test.started
+        )
+        ended = test_result.get(
+            self.actual_end, datetime.now(timezone.utc)
+        ) or datetime.now(timezone.utc)
+        test_result.pop(self.actual_start) if self.actual_start in test_result else ...
+        test_result.pop(self.actual_end) if self.actual_end in test_result else ...
+
+        await self.test.update_from_dict(
+            dict(
+                **{_: test_result[_] or 0 for _ in test_result.keys()},
+                retried=retried_sessions,
+                started=started,
+                ended=ended,
+                duration=(ended - started).total_seconds() * 1000,
+                specStructure=simplify_file_paths(
+                    [
+                        path
+                        for path in await SuiteBase.filter(
+                            Q(session__test_id=self.test_id)
+                            & Q(suiteType=SuiteType.SUITE)
+                            & ~Q(standing=Status.RETRIED)
+                            & Q(parent="")
+                        )
+                        .group_by("file")
+                        .prefetch_related("rollup")
+                        .annotate(tests=Sum("rollup__tests"))
+                        .values_list("file", "tests")
+                    ]
+                ),
+                standing=fetch_key_from_status(
+                    summary["passed"], summary["failed"], summary["skipped"]
+                ),
+                suiteSummary=summary,
+            )
+        )
+        await self.test.save()
+
+    async def pick_it_later(self):
+        self.task.picked = False
+        await self.task.save()
+
+    async def do_we_need_patch(self):
+        # check: 1
+        # to see if the test is not pending
+        if self.test.standing != Status.PENDING:
+            logger.warning("{} was already processed", self.test_id)
+            await self.mark_processed()
+            return False
+
+        # check: 2
+        # check if any child suites are yet to be processed
+        # this should not happen, as we are patching all the related suites before test run
+
+        pending_items = (
+            await SuiteBase.filter(session__test_id=self.test_id)
+            .filter(Q(standing=Status.YET_TO_CALCULATE) | Q(standing=Status.PENDING))
+            .count()
+        )
+
+        if pending_items > 0:
+            await skip_coz_error(
+                self.test_id,
+                f"Failed to patch the Test Run: {self.test_id} of project: {self.test.projectName},"
+                f" because some of the suites were not processed",
+                incomplete=self.test.projectName,
+                pending_suites=pending_items,
+            )
+            return False
+
+        return True
+
+
+async def skip_coz_error(test_id: Union[str, UUID], reason: str, **extra) -> False:
+    return await skip_test_run(test_id, reason, type=JobType.MODIFY_TEST_RUN, **extra)
+
+
+def simplify_file_paths(paths: List[Tuple[str, int]]):
+    tree: PathTree = {"current": "", "paths": {}, "suites": 1}
+    _paths: List[PathItem] = [
+        dict(children=list(reversed(Path(path[0]).parts)), pointer=tree, count=path[1])
+        for path in paths
+    ]
+
+    # Tree - Builder
+    while _paths:
+        path_to_include = _paths[-1]
+        if not path_to_include["children"]:
+            _paths.pop()
+            path_to_include["pointer"]["suites"] = path_to_include["count"]
+            continue
+
+        parent_pointer: PathTree = path_to_include["pointer"]
+        possible_parent: str = path_to_include["children"].pop()
+        # that dict will be inside the tree
+
+        # NOTE: we are not calculating the cumulative count of suites for the folder
+        pointing_to = parent_pointer["paths"].setdefault(
+            possible_parent,
+            {
+                "current": join(parent_pointer["current"], possible_parent),
+                "paths": {},
+                "suites": 1,
+            },
+        )
+        path_to_include["pointer"] = pointing_to
+
+    # Reducer
+    while True:
+        stack = [(_, tree) for _ in tree["paths"].keys()]
+        movements = 0
+
+        while stack:
+            node_key, parent_node = stack.pop()
+            target_node = parent_node["paths"][node_key]
+
+            children = list(target_node["paths"].keys())
+            if len(children) > 1:
+                for child_key in target_node["paths"]:
+                    stack.append((child_key, target_node))
+                continue
+
+            if not children:
+                continue
+            child_key = children.pop()
+
+            movements += 1
+            target_popped = parent_node["paths"].pop(node_key)
+            new_key = join(node_key, child_key)
+            parent_node["paths"][new_key] = target_popped["paths"].pop(child_key)
+            new_child = parent_node["paths"][new_key]
+            new_child["current"] = join(target_popped["current"], child_key)
+
+            for child_key in new_child["paths"]:
+                stack.append((child_key, new_child))
+
+        if not movements:
+            break
+
+    return tree["paths"]
+
+
+async def patchTestRun(test_id: str):
+    patcher = PatchTestRun(test_id)
+    to_return = False
+
+    try:
+        if await patcher.patch_test():
+            logger.info("Completed the patch for test run: {}", test_id)
+            to_return = True
+    except Exception:
+        await skip_coz_error(
+            test_id,
+            f"Failed to patch the test run, error in calculation, {format_exc()}",
+        )
+    return to_return
```

### Comparing `handshakes-0.3.2/handshake/services/SchedularService/register.py` & `handshakes-0.3.3/handshake/services/SchedularService/register.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,48 @@
-from loguru import logger
-from handshake.services.DBService.models.dynamic_base import TaskBase, JobType
-from uuid import uuid4, UUID
-from typing import Union
-from handshake.services.DBService.models.result_base import TestLogBase, LogType
-from handshake.services.DBService.lifecycle import init_tortoise_orm, close_connection
-from handshake.services.DBService.models.config_base import ExportBase
-from handshake.services.DBService.models.result_base import RunBase
-from pathlib import Path
-from typing import List
-from os import getenv
-
-
-async def register_patch_suite(suiteID: str, testID: str) -> TaskBase:
-    return await TaskBase.create(
-        ticketID=suiteID, test_id=testID, type=JobType.MODIFY_SUITE
-    )
-
-
-async def register_patch_test_run(testID: str) -> TaskBase:
-    return await TaskBase.create(
-        type=JobType.MODIFY_TEST_RUN, test_id=testID, ticketID=testID
-    )
-
-
-async def mark_for_prune_task(test_id: str):
-    # someone called this explicitly hence it's a warning
-
-    logger.warning("Requested to prune some tasks")
-    await TaskBase.create(
-        ticketID=str(uuid4()), type=JobType.PRUNE_TASKS, test_id=test_id
-    )
-
-
-async def skip_test_run(test_id: Union[str, UUID], reason: str, **extra) -> False:
-    logger.error(reason)
-    await TestLogBase.create(
-        test_id=str(test_id), message=reason, type=LogType.ERROR, feed=extra
-    )
-    await mark_for_prune_task(test_id)
-    return False
-
-
-async def warn_about_test_run(test_id: Union[str, UUID], about: str, **extra) -> True:
-    logger.warning(about)
-    await TestLogBase.create(
-        test_id=str(test_id), message=about, type=LogType.WARN, feed=extra
-    )
-    return True
-
-
-async def createExportTicket(
-    maxTestRuns: int, path: Path, store: List[str], runs: List[str], clarity
-):
-    await init_tortoise_orm(path)
-    ticket = await ExportBase.create(maxTestRuns=maxTestRuns)
-
-    runs.extend(
-        await RunBase.all()
-        .order_by("-started")
-        .limit(maxTestRuns)
-        .values_list("testID", flat=True)
-    )
-
-    await close_connection()
-    store.append(str(ticket.ticketID))
-
-
-async def deleteExportTicket(ticketID: str):
-    task = await ExportBase.filter(ticketID=ticketID).first()
-    logger.info("Deleting the Export ticket: {}", ticketID)
-    await task.delete()
+from loguru import logger
+from handshake.services.DBService.models.dynamic_base import TaskBase, JobType
+from uuid import uuid4, UUID
+from typing import Union
+from handshake.services.DBService.models.result_base import TestLogBase, LogType
+from handshake.services.DBService.lifecycle import init_tortoise_orm, close_connection
+from handshake.services.DBService.models.config_base import ExportBase
+from handshake.services.DBService.models.result_base import RunBase
+from pathlib import Path
+from typing import List
+
+
+async def register_patch_suite(suiteID: str, testID: str) -> TaskBase:
+    return await TaskBase.create(
+        ticketID=suiteID, test_id=testID, type=JobType.MODIFY_SUITE
+    )
+
+
+async def register_patch_test_run(testID: str) -> TaskBase:
+    return await TaskBase.create(
+        type=JobType.MODIFY_TEST_RUN, test_id=testID, ticketID=testID
+    )
+
+
+async def mark_for_prune_task(test_id: str):
+    # someone called this explicitly hence it's a warning
+
+    logger.warning("Requested to prune some tasks")
+    await TaskBase.create(
+        ticketID=str(uuid4()), type=JobType.PRUNE_TASKS, test_id=test_id
+    )
+
+
+async def skip_test_run(test_id: Union[str, UUID], reason: str, **extra) -> False:
+    logger.error(reason)
+    await TestLogBase.create(
+        test_id=str(test_id), message=reason, type=LogType.ERROR, feed=extra
+    )
+    await mark_for_prune_task(test_id)
+    return False
+
+
+async def warn_about_test_run(test_id: Union[str, UUID], about: str, **extra) -> True:
+    logger.warning(about)
+    await TestLogBase.create(
+        test_id=str(test_id), message=about, type=LogType.WARN, feed=extra
+    )
+    return True
```

### Comparing `handshakes-0.3.2/pyproject.toml` & `handshakes-0.3.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,62 @@
-[tool.poetry]
-name = "handshakes"
-version = "0.3.2"
-description = "A service that's keen to process your test results"
-authors = ["Rahul <saihanumarahul66@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{include = "handshake"}]
-maintainers = [
-    "Rahul <saihanumarahul66@gmail.com>"
-]
-exclude=[ 'handshake/.env', 'handshake/prod.env', 'handshake/test.env' ]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Database :: Front-Ends",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent"
-]
-
-[tool.poetry.dependencies]
-python = "^3.11,<3.13"
-pydantic = "^2.4.2"
-sanic = "^23.6.0"
-tortoise-orm = "^0.20.0"
-click = "^8.1.7"
-APScheduler = "^3.10.4"
-loguru = "^0.7.2"
-httpx = "^0.26.0"
-python-dotenv = "^1.0.1"
-sentry-sdk = {extras = ["sanic"], version = "^1.40.4"}
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.4.2"
-pytest-asyncio = "^0.21.1"
-sanic-testing = "^23.6.0"
-psutil = "^5.9.5"
-black = "^23.9.1"
-virtualenv = "^20.25.1"
-
-[tool.poetry.extras]
-excel-export = ["openpyxl"]
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.scripts]
-handshake = "handshake.services.CommandLine.center:handle_cli"
+[tool.poetry]
+name = "handshakes"
+version = "0.3.3"
+description = "A service that's keen to process your test results"
+authors = ["Rahul <saihanumarahul66@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+packages = [{include = "handshake"}]
+maintainers = [
+    "Rahul <saihanumarahul66@gmail.com>"
+]
+exclude=[ 'handshake/.env', 'handshake/prod.env', 'handshake/test.env']
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Database :: Front-Ends",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent"
+]
+
+[tool.poetry.dependencies]
+python = "^3.11,<3.13"
+pydantic = "^2.4.2"
+sanic = "^23.6.0"
+tortoise-orm = "^0.20.0"
+click = "^8.1.7"
+loguru = "^0.7.2"
+httpx = "^0.26.0"
+python-dotenv = "^1.0.1"
+sentry-sdk = {extras = ["sanic"], version = "^1.40.4"}
+setuptools = "^69.2.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.2"
+pytest-asyncio = "^0.21.1"
+sanic-testing = "^23.6.0"
+psutil = "^5.9.5"
+black = ">=23.9.1,<25.0.0"
+virtualenv = "^20.25.1"
+requests = "^2.31.0"
+
+[tool.poetry.extras]
+excel-export = ["openpyxl"]
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[project.urls]
+"Homepage" = "https://github.com/RahulARanger/handshake"
+"Bug Reports" = "https://github.com/RahulARanger/handshake/issues"
+"Source" = "https://github.com/RahulARanger/handshake"
+
+
+[tool.poetry.scripts]
+handshake = "handshake.services.CommandLine.center:handle_cli"
+
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
```

### Comparing `handshakes-0.3.2/README.md` & `handshakes-0.3.3/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Handshake 🫱🏾‍🫲🏼
-_A Modern Test Reporter_
-
-Processes the data collected from the test execution and then generates a modern Dashboard.
-
-## Getting Started
-
-### WebdriverIO
-
-[WebdriverIO](https://webdriver.io/) is a Next-gen browser and mobile automation test framework for Node.js
-
-1. Install Packages: `npm install wdio-handshake-reporter`
-2. Install Dashboard: `npm install handshake`
-3. Once done you can configure the reporter in your configuration.
-
-## Plans
-below are the things I would like to implement sooner or later.
-
-* [X] Add support for `webdriverio`
-* [ ] Add Reporter for `jest`
-* [ ] Work on documentation
-* [ ] Support for `mocha`
-* [ ] Listen to `cypress` results
-* [ ] Add Support for `playwright`
-
+# Handshake 🫱🏾‍🫲🏼
+_A Modern Test Reporter_
+
+Processes the data collected from the test execution and then generates a modern Dashboard.
+
+## Getting Started
+
+### WebdriverIO
+
+[WebdriverIO](https://webdriver.io/) is a Next-gen browser and mobile automation test framework for Node.js
+
+1. Install Packages: `npm install wdio-handshake-reporter`
+2. Install Dashboard: `npm install handshake`
+3. Once done you can configure the reporter in your configuration.
+
+## Plans
+below are the things I would like to implement sooner or later.
+
+* [X] Add support for `webdriverio`
+* [ ] Add Reporter for `jest`
+* [ ] Work on documentation
+* [ ] Support for `mocha`
+* [ ] Listen to `cypress` results
+* [ ] Add Support for `playwright`
+
 ## Sample Shots
```

### Comparing `handshakes-0.3.2/PKG-INFO` & `handshakes-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handshakes
-Version: 0.3.2
+Version: 0.3.3
 Summary: A service that's keen to process your test results
 License: MIT
 Author: Rahul
 Author-email: saihanumarahul66@gmail.com
 Maintainer: Rahul
 Maintainer-email: saihanumarahul66@gmail.com
 Requires-Python: >=3.11,<3.13
@@ -13,22 +13,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: excel-export
-Requires-Dist: APScheduler (>=3.10.4,<4.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: sanic (>=23.6.0,<24.0.0)
 Requires-Dist: sentry-sdk[sanic] (>=1.40.4,<2.0.0)
+Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Requires-Dist: tortoise-orm (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Handshake 🫱🏾‍🫲🏼
 _A Modern Test Reporter_
 
 Processes the data collected from the test execution and then generates a modern Dashboard.
```

