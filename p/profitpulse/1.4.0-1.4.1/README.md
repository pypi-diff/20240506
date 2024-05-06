# Comparing `tmp/profitpulse-1.4.0.tar.gz` & `tmp/profitpulse-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-1.4.0.tar", max compression
+gzip compressed data, was "profitpulse-1.4.1.tar", max compression
```

## Comparing `profitpulse-1.4.0.tar` & `profitpulse-1.4.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-1.4.0/LICENSE
--rw-r--r--   0        0        0     1016 2024-04-27 17:48:38.569723 profitpulse-1.4.0/README.md
--rw-r--r--   0        0        0     1450 2024-05-04 09:35:32.280155 profitpulse-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-1.4.0/src/profitpulse/__init__.py
--rw-r--r--   0        0        0       90 2024-04-27 17:48:38.575122 profitpulse-1.4.0/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     6188 2024-05-04 09:11:34.927431 profitpulse-1.4.0/src/profitpulse/cli/cli_adapters.py
--rw-r--r--   0        0        0      321 2024-04-27 17:48:38.575816 profitpulse-1.4.0/src/profitpulse/cli/console.py
--rw-r--r--   0        0        0      649 2024-04-27 17:48:38.576038 profitpulse-1.4.0/src/profitpulse/cli/console_test.py
--rw-r--r--   0        0        0     4407 2024-05-03 15:10:38.922872 profitpulse-1.4.0/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-05-03 15:10:38.923184 profitpulse-1.4.0/src/profitpulse/cli/scenario.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-1.4.0/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     4643 2024-05-04 09:24:03.704854 profitpulse-1.4.0/src/profitpulse/data/accounts.py
--rw-r--r--   0        0        0     2855 2024-05-04 09:07:56.047857 profitpulse-1.4.0/src/profitpulse/data/accounts_test.py
--rw-r--r--   0        0        0     1273 2024-04-27 17:48:38.581281 profitpulse-1.4.0/src/profitpulse/data/transactions.py
--rw-r--r--   0        0        0     3917 2024-05-04 09:11:38.300706 profitpulse-1.4.0/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     6813 2024-05-04 09:11:38.338755 profitpulse-1.4.0/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-1.4.0/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3049 2024-04-27 17:48:38.577257 profitpulse-1.4.0/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2024-04-27 17:48:38.577500 profitpulse-1.4.0/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-1.4.0/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-1.4.0/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-1.4.0/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1755 2024-05-04 07:36:07.378041 profitpulse-1.4.0/src/profitpulse/lib/account.py
--rw-r--r--   0        0        0      549 2024-04-27 17:48:38.578920 profitpulse-1.4.0/src/profitpulse/lib/account_name.py
--rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-1.4.0/src/profitpulse/lib/comment.py
--rw-r--r--   0        0        0      767 2024-05-03 04:50:08.234943 profitpulse-1.4.0/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      194 2024-04-27 17:48:38.579669 profitpulse-1.4.0/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      952 2024-05-04 09:13:33.128368 profitpulse-1.4.0/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-1.4.0/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-1.4.0/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-1.4.0/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1162 2024-05-03 05:02:17.240148 profitpulse-1.4.0/src/profitpulse/services/close_account.py
--rw-r--r--   0        0        0     1741 2024-04-27 17:48:38.582198 profitpulse-1.4.0/src/profitpulse/services/close_account_test.py
--rw-r--r--   0        0        0     1214 2024-05-03 05:02:17.262995 profitpulse-1.4.0/src/profitpulse/services/delete_account.py
--rw-r--r--   0        0        0     1559 2024-04-27 17:48:38.582602 profitpulse-1.4.0/src/profitpulse/services/delete_account_test.py
--rw-r--r--   0        0        0     1396 2024-05-03 05:02:17.184938 profitpulse-1.4.0/src/profitpulse/services/deposit_into_account.py
--rw-r--r--   0        0        0     2889 2024-04-27 17:48:38.583202 profitpulse-1.4.0/src/profitpulse/services/deposit_into_account_test.py
--rw-r--r--   0        0        0     1624 2024-05-03 05:02:17.253307 profitpulse-1.4.0/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     2067 2024-04-27 17:48:38.583985 profitpulse-1.4.0/src/profitpulse/services/import_transactions_test.py
--rw-r--r--   0        0        0     1215 2024-05-03 05:02:17.409661 profitpulse-1.4.0/src/profitpulse/services/open_account.py
--rw-r--r--   0        0        0     1657 2024-04-27 17:48:38.584718 profitpulse-1.4.0/src/profitpulse/services/open_account_test.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-1.4.0/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-1.4.0/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-1.4.0/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4441 2024-05-03 15:10:38.943221 profitpulse-1.4.0/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 profitpulse-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-1.4.1/README.md
+-rw-r--r--   0        0        0     1816 2024-05-05 20:20:43.114182 profitpulse-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-1.4.1/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-1.4.1/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     7410 2024-05-05 20:15:15.188339 profitpulse-1.4.1/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     5198 2024-05-05 19:43:17.612917 profitpulse-1.4.1/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-1.4.1/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     5684 2024-05-05 20:16:40.464175 profitpulse-1.4.1/src/profitpulse/data/accounts.py
+-rw-r--r--   0        0        0     2855 2024-05-04 09:07:56.047857 profitpulse-1.4.1/src/profitpulse/data/accounts_test.py
+-rw-r--r--   0        0        0     2007 2024-05-05 20:18:18.593519 profitpulse-1.4.1/src/profitpulse/data/transactions.py
+-rw-r--r--   0        0        0     6008 2024-05-05 20:19:04.762138 profitpulse-1.4.1/src/profitpulse/data/views.py
+-rw-r--r--   0        0        0     6833 2024-05-05 19:43:17.725626 profitpulse-1.4.1/src/profitpulse/data/views_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-1.4.1/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-1.4.1/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-1.4.1/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-1.4.1/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-1.4.1/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-1.4.1/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1832 2024-05-05 19:43:17.382906 profitpulse-1.4.1/src/profitpulse/lib/account.py
+-rw-r--r--   0        0        0      549 2024-04-27 17:48:38.578920 profitpulse-1.4.1/src/profitpulse/lib/account_name.py
+-rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-1.4.1/src/profitpulse/lib/comment.py
+-rw-r--r--   0        0        0      863 2024-05-05 19:54:59.624362 profitpulse-1.4.1/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-1.4.1/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-1.4.1/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-1.4.1/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-1.4.1/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-1.4.1/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1031 2024-05-05 19:29:56.480759 profitpulse-1.4.1/src/profitpulse/services/close_account.py
+-rw-r--r--   0        0        0     1693 2024-05-05 19:43:17.172209 profitpulse-1.4.1/src/profitpulse/services/close_account_test.py
+-rw-r--r--   0        0        0     1047 2024-05-05 19:29:56.481760 profitpulse-1.4.1/src/profitpulse/services/delete_account.py
+-rw-r--r--   0        0        0     1559 2024-05-05 19:43:17.320460 profitpulse-1.4.1/src/profitpulse/services/delete_account_test.py
+-rw-r--r--   0        0        0     1432 2024-05-05 19:43:17.249123 profitpulse-1.4.1/src/profitpulse/services/deposit_into_account.py
+-rw-r--r--   0        0        0     2848 2024-05-05 19:43:17.334540 profitpulse-1.4.1/src/profitpulse/services/deposit_into_account_test.py
+-rw-r--r--   0        0        0      303 2024-05-05 19:29:56.485862 profitpulse-1.4.1/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     1672 2024-05-05 19:43:17.358387 profitpulse-1.4.1/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     2112 2024-05-05 19:43:17.451850 profitpulse-1.4.1/src/profitpulse/services/import_transactions_test.py
+-rw-r--r--   0        0        0     1231 2024-05-05 19:43:17.209744 profitpulse-1.4.1/src/profitpulse/services/open_account.py
+-rw-r--r--   0        0        0     1719 2024-05-05 19:43:17.459527 profitpulse-1.4.1/src/profitpulse/services/open_account_test.py
+-rw-r--r--   0        0        0     1209 2024-05-05 19:43:17.183351 profitpulse-1.4.1/src/profitpulse/services/snapshot_account.py
+-rw-r--r--   0        0        0     1751 2024-05-05 20:16:09.319552 profitpulse-1.4.1/src/profitpulse/services/snapshot_account_test.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-1.4.1/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-1.4.1/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-1.4.1/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4741 2024-05-05 20:12:45.584169 profitpulse-1.4.1/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-1.4.1/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 profitpulse-1.4.1/PKG-INFO
```

### Comparing `profitpulse-1.4.0/LICENSE` & `profitpulse-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.0/README.md` & `profitpulse-1.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Profit Pulse
 
 [![PyPI version](https://badge.fury.io/py/profitpulse.svg)](https://badge.fury.io/py/profitpulse) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/profitpulse)
 
-Profit Pulse: Maximise Earnings Through Smart Wealth Management.
-
-Effortlessly manage your personal finances, supercharge savings, and boost
-profits. Gain depp insights into your money flow, make strategic choices and
-pave your way to financial growth.
+Profit Pulse: Use a Python built CLI application to effortlessly manage your
+personal finances. Increase savings, and boost profits. Gain deep insights into
+your money flow, make strategic choices and pave your way to financial
+independence.
 
 ## How to install ?
 
-### macOS
+Install [pipx](https://github.com/pypa/pipx) using the [official installation instructions](https://pipx.pypa.io/stable/installation/).
+Next, install profitpulse
 
 ```bash
-pip install profitpulse
+pipx install profitpulse
 ```
 
 ## How to use ?
 
 To access the available commands, just execute:
 
 ```bash
@@ -34,9 +34,8 @@
 
 After cloning the repository to your machine, in the project root, just run:
 
 ```bash
 make all
 ```
 
-If everything went smoothly you are now ready to add some contributions. Take a
-look at the CONTRIBUTING.md file for more guidelines (once I write them :).
+If everything went smoothly you are now ready to add some contributions.
```

### Comparing `profitpulse-1.4.0/pyproject.toml` & `profitpulse-1.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "1.4.0"
+version = "1.4.1"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
 
@@ -19,14 +19,26 @@
 [[tool.poetry.packages]]
 include = "profitpulse"
 from = "src"
 
 [tool.mypy]
 disallow_untyped_defs = true
 
+[[tool.mypy.overrides]]
+module  = "gogotable" # error: Skipping analyzing "gogotable": module is installed, but missing library stubs or py.typed marker  [import-untyped]
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module  = "turbofan.database"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module  = "pastperfect"
+ignore_missing_imports = true
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 max-line-length = 120
 target-version = ["py310","py311", "py312"]
```

### Comparing `profitpulse-1.4.0/src/profitpulse/cli/cli_adapters.py` & `profitpulse-1.4.1/src/profitpulse/cli/adapters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,205 +1,246 @@
 """
-Cli adapters bridge the CLI frameworks with the services use cases and print
-data into the screen.
+Adapters bridge the CLI frameworks and the application services by creating the
+service inputs and handling the output for printing.
 """
 
 import logging
+from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 from gogotable import gogotable
 from turbofan.database import Database, Session
 
-from profitpulse.cli import console
 from profitpulse.data.accounts import Accounts
 from profitpulse.data.transactions import Transactions
 from profitpulse.data.views import AccountsView, PulseView, TransactionsView
-from profitpulse.gateways.cgdfile import GatewayCGDFile
+from profitpulse.gateways.cgdfile import GatewayCGDFile  # type: ignore
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
-from profitpulse.services.close_account import CloseAccountService
-from profitpulse.services.delete_account import ServiceDeleteAccount
-from profitpulse.services.deposit_into_account import ServiceDepositIntoAccount
-from profitpulse.services.import_transactions import ServiceImportTransactions
+from profitpulse.services.close_account import (
+    CloseAccountRequester,
+    CloseAccountService,
+)
+from profitpulse.services.delete_account import (
+    DeleteAccountRequester,
+    DeleteAccountService,
+)
+from profitpulse.services.deposit_into_account import (
+    DepositIntoAccountRequester,
+    DepositIntoAccountService,
+)
+from profitpulse.services.import_transactions import (
+    ImportTransactionsRequester,
+    ImportTransactionsService,
+)
 from profitpulse.services.open_account import (
     AccountAlreadyExistsError,
+    OpenAccountRequester,
     OpenAccountService,
 )
+from profitpulse.services.snapshot_account import (
+    SnapshotAccountRequester,
+    SnapshotAccountService,
+)
 
 logging.basicConfig(level=logging.CRITICAL)
 logger = logging.getLogger(__name__)
 
 database_path = Path.home() / Path("Library/Application Support/Profitpulse")
 
 
-def report(seller, since, on):
+def report(
+    seller: Optional[str],
+    since: Optional[datetime] = None,
+    on: Optional[datetime] = None,
+) -> None:
     db = Database(database_path)
     with Session(db.engine) as session:
         view = TransactionsView(session, seller, since, on)
 
         transactions, total = view.data
-        if not seller:
-            if not transactions:
-                print("Could not find any transactions!")
-                return
-
-            for t in transactions:
-                print(f"Description: '{t['description']:>22}', Value: {t['value']:>10}")
+        if seller:
+            print(f"Description: '{seller}', Value: {round(total, 2)}")
             return
 
-        print(f"Description: '{seller}', Value: {round(total, 2)}")
+        for t in transactions:
+            print(f"Description: '{t['description']:>22}', Value: {t['value']:>10}")
 
 
-def pulse():
+def pulse() -> None:
     """
     Read all the events and print the current proofit pulse.
     """
 
     headers = ["Account Name", "Invested", "Current", "Performance"]
 
     db = Database(database_path)
     with Session(db.engine) as session:
         view = PulseView(session)
         lines = gogotable(headers, view.data)
         for line in lines:
             print(line)
 
 
-def reset():
+class SnapshotAccountRequest(SnapshotAccountRequester):
+    def __init__(self, account_name: str, value: int) -> None:
+        self._account_name = account_name
+        self._value = value
+
+    @property
+    def account_name(self) -> AccountName:
+        return AccountName(self._account_name)
+
+    @property
+    def value(self) -> Money:
+        return Money(self._value)
+
+
+def snapshot(cent_amount: int, account_name: str) -> None:
+    db = Database(database_path)
+    with Session(db.engine) as session:
+        request = SnapshotAccountRequest(account_name, cent_amount)
+        accounts = Accounts(session)
+        service = SnapshotAccountService(accounts)
+        service.execute(request)
+        session.commit()
+
+
+def reset() -> None:
     db = Database(database_path)
     db.remove()
 
 
-class RequestImportTransactions:
+class RequestImportTransactions(ImportTransactionsRequester):
     def __init__(self, account_name: str) -> None:
         self._account_name = account_name
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
-def import_file(file_path: Path, account_name):
+def import_file(file_path: Path, account_name: str) -> None:
     db = Database(database_path)
     with Session(db.engine) as session:
         gateway_cgd = GatewayCGDFile(file_path)
         transactions = Transactions(session)
         accounts = Accounts(session)
-        service = ServiceImportTransactions(gateway_cgd, transactions, accounts)
+        service = ImportTransactionsService(gateway_cgd, transactions, accounts)
         request = RequestImportTransactions(account_name)
         service.execute(request)
         session.commit()
 
 
-class DepositRequest:
-    def __init__(self, cent_amount, account_name, comment: Optional[str] = None):
+class DepositRequest(DepositIntoAccountRequester):
+    def __init__(
+        self, cent_amount: int, account_name: str, comment: Optional[str] = None
+    ) -> None:
         self._cent_amount = cent_amount
         self._account_name = account_name
         self._comment = comment
 
     @property
     def amount(self) -> Money:
         return Money(self._cent_amount)
 
     @property
     def comment(self) -> Optional[Comment]:
         return Comment(self._comment) if self._comment else None
 
     @property
     def account_name(self) -> AccountName:
-        return self._account_name
+        return AccountName(self._account_name)
 
 
 def deposit(cent_amount: int, account_name: str, comment: Optional[str] = None) -> None:
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = DepositRequest(cent_amount, account_name, comment)
-        service = ServiceDepositIntoAccount(accounts)
+        service = DepositIntoAccountService(accounts)
         service.execute(request)
 
         session.commit()
 
 
 def transfer(cent_amount: int, from_account_name: str, to_account_name: str) -> None:
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = DepositRequest(cent_amount, from_account_name)
-        service = ServiceDepositIntoAccount(accounts)
+        service = DepositIntoAccountService(accounts)
         service.execute(request)
 
         request = DepositRequest(-cent_amount, to_account_name)
-        service = ServiceDepositIntoAccount(accounts)
+        service = DepositIntoAccountService(accounts)
         service.execute(request)
 
         session.commit()
 
 
-def show_accounts():
+def show_accounts() -> None:
     with Session(Database(database_path).engine) as session:
         data = AccountsView(session).data
         if not data:
             return
 
         headers = ["Name", "Balance", "Status", "Comment"]
         lines = gogotable(headers, data)
         for line in lines:
             print(line)
 
 
-class OpenAccountRequest:
-    def __init__(self, name):
+class OpenAccountRequest(OpenAccountRequester):
+    def __init__(self, name: str) -> None:
         self._name = AccountName(name)
 
     @property
-    def account_name(self):
+    def account_name(self) -> AccountName:
         return self._name
 
 
-def open_account(name):
+def open_account(name: str) -> None:
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = OpenAccountRequest(name)
         try:
             OpenAccountService(accounts).execute(request)
         except AccountAlreadyExistsError as e:
-            msg = console.message(
-                str(e) + " " + ", why don't you try again using a different name ?"
-            )
-            print(msg)
+            print(str(e))
+            return
 
         session.commit()
 
 
-class CloseAccountRequest:
-    def __init__(self, account_name):
+class CloseAccountRequest(CloseAccountRequester):
+    def __init__(self, account_name: str) -> None:
         self._account_name = account_name
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
-def close_account(name):
+def close_account(name: str) -> None:
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = CloseAccountRequest(name)
         CloseAccountService(accounts).execute(request)
         session.commit()
 
 
-class DeleteAccountRequest:
-    def __init__(self, account_name):
+class DeleteAccountRequest(DeleteAccountRequester):
+    def __init__(self, account_name: str) -> None:
         self._account_name = account_name
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
-def delete_account(name):
+def delete_account(name: str) -> None:
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = DeleteAccountRequest(name)
-        ServiceDeleteAccount(accounts).execute(request)
+        DeleteAccountService(accounts).execute(request)
         session.commit()
```

### Comparing `profitpulse-1.4.0/src/profitpulse/data/accounts.py` & `profitpulse-1.4.1/src/profitpulse/data/accounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,71 @@
+import typing
 from enum import Enum
 from typing import Optional
 
 import pastperfect
 from turbofan.database import text
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
+from profitpulse.services.close_account import CloseAccountAccountCollector
+from profitpulse.services.delete_account import DeleteAccountAccountCollector
+from profitpulse.services.deposit_into_account import DepositIntoAccountAccountCollector
+from profitpulse.services.import_transactions import ImportTransactionsAccountCollector
+from profitpulse.services.open_account import OpenAccountAccountCollector
+from profitpulse.services.snapshot_account import SnapshotAccountAccountCollector
 
 OPEN = "O"
 CLOSED = "C"
 
 
 # Once python3.9 and python.3.10 support is dropped, we can use
 # https://docs.python.org/3/library/enum.html#enum.StrEnum
 class StrEnum(str, Enum):
     pass
 
 
 class PulseEvent(StrEnum):
     MONEY_DEPOSIT = "1"
+    TRANSACTION_IMPORTED = "2"
+    ACCOUNT_SNAPSHOT = "3"
 
 
-class Accounts:
+class Accounts(
+    CloseAccountAccountCollector,
+    DeleteAccountAccountCollector,
+    OpenAccountAccountCollector,
+    DepositIntoAccountAccountCollector,
+    ImportTransactionsAccountCollector,
+    SnapshotAccountAccountCollector,
+):
     """
     Accounts implement the AccountsRepository protocol.
     """
 
-    def __init__(self, session):
+    def __init__(self, session: typing.Any) -> None:
         self._session = session
 
-    def __len__(self):
+    def __len__(self) -> None:
         sql_stmt = """
             SELECT COUNT(*) FROM account
         """
         prepared_statement = text(sql_stmt)
         row = self._session.execute(prepared_statement).first()
         return row[0]
 
     def get(self, account_name: AccountName) -> Optional[Account]:
         try:
             return self[account_name]
         except KeyError:
             return None
 
-    def __setitem__(self, account_name: AccountName, account: Account):
+    def __setitem__(self, account_name: AccountName, account: Account) -> None:
 
         is_a_new_account = False
         try:
             self[account_name]
         except KeyError:
             is_a_new_account = True
 
@@ -61,27 +77,33 @@
         prepared_statement = prepared_statement.bindparams(
             name=str(account.name),
             status=CLOSED if account.closed else OPEN,
         )
         self._session.execute(prepared_statement)
 
         sql_stmt = """
-            INSERT INTO balance (account_id, value, description)
-                 VALUES ((SELECT id FROM account WHERE name = :name), :value, :comment)
+            INSERT INTO balance (account_id, description)
+                 VALUES ((SELECT id FROM account WHERE name = :name), :comment)
         """
         prepared_statement = text(sql_stmt)
         prepared_statement = prepared_statement.bindparams(
             name=str(account.name),
-            value=str(account.balance.cents),
             comment=str(account.last_comment) if account.last_comment else None,
         )
         self._session.execute(prepared_statement)
 
         events = pastperfect.Events(self._session)
 
+        events.append(
+            pastperfect.Event(
+                name=PulseEvent.ACCOUNT_SNAPSHOT,
+                data={"name": str(account.name), "balance": account.balance.cents},
+            )
+        )
+
         if is_a_new_account:
             events.append(
                 pastperfect.Event(
                     name=PulseEvent.MONEY_DEPOSIT,
                     data={"name": str(account.name), "balance": account.balance.cents},
                 )
             )
@@ -90,15 +112,15 @@
             events.append(
                 pastperfect.Event(
                     name=PulseEvent.MONEY_DEPOSIT,
                     data={"name": str(account.name), "balance": deposit.cents},
                 )
             )
 
-    def append(self, account: Account):
+    def append(self, account: Account) -> None:
         self[account.name] = account
 
     def __getitem__(self, account_name: AccountName) -> Account:
         sql_stmt = """
             SELECT account.name as name,
                    account.status,
                    balance.description
@@ -111,28 +133,32 @@
         prepared_statement = prepared_statement.bindparams(name=str(account_name))
         row = self._session.execute(prepared_statement).first()
         if not row:
             raise KeyError
 
         events = pastperfect.Events(self._session)
         account_name = row[0]
-        total_balance = Money(0)
+        balance = Money(0)
         for event in events:
-            if not event.data.get("name") == account_name:
+            if (
+                event.name != PulseEvent.ACCOUNT_SNAPSHOT
+                or event.data.get("name") != account_name
+            ):
                 continue
-            total_balance = total_balance + Money(event.data.get("balance"))
+
+            balance = Money(event.data.get("balance"))
 
         return Account(
             AccountName(row[0]),
-            balance=total_balance,
+            balance=balance,
             closed=True if row[1] == CLOSED else False,
             comment=Comment(row[2] if row[2] else ""),
         )
 
-    def __delitem__(self, account_name: AccountName):
+    def __delitem__(self, account_name: AccountName) -> None:
         sql_stmt = """
             DELETE FROM balance
                   WHERE account_id = (SELECT id FROM account WHERE name = :name)
         """
         prepared_statement = text(sql_stmt)
         prepared_statement = prepared_statement.bindparams(name=str(account_name))
         self._session.execute(prepared_statement)
```

### Comparing `profitpulse-1.4.0/src/profitpulse/data/accounts_test.py` & `profitpulse-1.4.1/src/profitpulse/data/accounts_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.0/src/profitpulse/data/views_test.py` & `profitpulse-1.4.1/src/profitpulse/data/views_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Optional
+from datetime import datetime
 
+import pastperfect
 import pytest
 from turbofan.database import text
 
+from profitpulse.data.accounts import PulseEvent
 from profitpulse.data.views import AccountsView, TransactionsView
 from profitpulse.lib.money import Money
 
 
 class TestAccountsView:
     @pytest.mark.integration
     def test_return_no_data_when_no_accounts(self, tmp_db_session):
@@ -36,49 +38,44 @@
             value=value,
             date_of_movement=date_of_movement,
             origin=origin,
             account_id=account_id,
         )
 
         self.session.execute(prepared_statement)
+
+        events = pastperfect.Events(self.session)
+        events.append(
+            pastperfect.Event(
+                name=PulseEvent.TRANSACTION_IMPORTED,
+                data={
+                    "value": value,
+                    "date": date_of_movement,
+                    "description": description,
+                },
+            )
+        )
+
         return self
 
     def open_account(self, name):
         sql_statement = "INSERT INTO account (name)VALUES (:name)"
         prepared_statement = text(sql_statement).bindparams(name=name)
         result = self.session.execute(prepared_statement)
         self.account_id = result.lastrowid
         return self
 
-    def deposit(
-        self,
-        cent_amount: int,
-        account_name: str,
-        comment: Optional[str] = None,
-    ):
-        sql_statement = """
-            INSERT INTO balance (account_id, value, description)
-                 VALUES ((SELECT id FROM account WHERE name = :name), :value, :comment)
-        """
-        prepared_statement = text(sql_statement).bindparams(
-            name=str(account_name),
-            value=str(cent_amount),
-            comment=str(comment) if comment else None,
-        )
-        self.session.execute(prepared_statement)
-
 
 class TestTransactionsView:
-
     @pytest.mark.integration
     def test_shown_no_transactions_on_empty_database(self, tmp_db_session):
         transactions, total = TransactionsView(tmp_db_session).data
 
         assert not transactions  # nosec
-        assert not total  # nosec
+        assert total == "0.00"  # nosec
 
     @pytest.mark.integration
     def test_show_one_transaction_when_one_is_available(self, tmp_db_session):
         """
         Given a database with one transaction
         When the view is executed
         Then the transaction is shown
@@ -86,16 +83,16 @@
 
         scenario = DatabaseScenario(tmp_db_session)
         scenario.open_account("TheAccountName")
         scenario.log_transaction("foo", 1, "2020-01-01", "foo", scenario.account_id)
 
         transactions, total = TransactionsView(tmp_db_session).data
 
-        assert transactions == [{"description": "foo", "value": 1}]  # nosec
-        assert total == 1  # nosec
+        assert transactions == [{"description": "foo", "value": "0.01"}]  # nosec
+        assert total == "0.01"  # nosec
 
     @pytest.mark.integration
     def test_show_multiple_transactions_when_more_than_one_is_available(
         self, tmp_db_session
     ):
         """
         Given a database with multiple transactions
@@ -119,18 +116,18 @@
             "foo",
             scenario.account_id,
         )
 
         transactions, total = TransactionsView(tmp_db_session).data
 
         assert transactions == [  # nosec
-            {"description": "foo", "value": 1},
-            {"description": "bar", "value": 2},
+            {"description": "foo", "value": "0.01"},
+            {"description": "bar", "value": "0.02"},
         ]
-        assert total == 3  # nosec
+        assert total == "0.03"  # nosec
 
     @pytest.mark.integration
     def test_show_transactions_since_a_given_date(self, tmp_db_session):
         """
         Given a database with multiple transactions
         When the view is executed with a since date
         Then the transactions since the given date are shown
@@ -149,18 +146,20 @@
             "bar",
             2,
             "2020-01-02",
             "foo",
             scenario.account_id,
         )
 
-        transactions, total = TransactionsView(tmp_db_session, since="2020-01-02").data
+        transactions, total = TransactionsView(
+            tmp_db_session, since=datetime.strptime("2020-01-02", "%Y-%m-%d")
+        ).data
 
-        assert transactions == [{"description": "bar", "value": 2}]  # nosec
-        assert total == 2  # nosec
+        assert transactions == [{"description": "bar", "value": "0.02"}]  # nosec
+        assert total == "0.02"  # nosec
 
     @pytest.mark.integration
     def test_show_transactions_on_a_given_date(self, tmp_db_session):
         """
         Given a database with multiple transactions
         When the view is executed with a on date
         Then the transactions on the given date are shown
@@ -179,18 +178,21 @@
             "bar",
             2,
             "2020-01-02",
             "foo",
             scenario.account_id,
         )
 
-        transactions, total = TransactionsView(tmp_db_session, on="2020-01-01").data
+        transactions, total = TransactionsView(
+            tmp_db_session,
+            on=datetime.strptime("2020-01-01", "%Y-%m-%d"),
+        ).data
 
-        assert transactions == [{"description": "foo", "value": 1.0}]  # nosec
-        assert total == 1.0  # nosec
+        assert transactions == [{"description": "foo", "value": "0.01"}]  # nosec
+        assert total == "0.01"  # nosec
 
     @pytest.mark.integration
     def test_show_total_for_a_specific_seller(self, tmp_db_session):
         """
         Given a database with multiple transactions
         When the view is executed with a seller
         Then the total for the given seller is shown
```

### Comparing `profitpulse-1.4.0/src/profitpulse/gateways/cgdfile.py` & `profitpulse-1.4.1/src/profitpulse/gateways/cgdfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+# type: ignore
 import csv
 import pathlib
 
 import pendulum
 
 from profitpulse.lib.transaction import Transaction
+from profitpulse.services.import_transactions import ImportTransactionsTransactionGater
 
 
 class RowParser:
     """
     Example of a row list:
         ['01-01-2020', '01-01-2020', 'COMPRAS C DEB FARMACI ', '15,69', '', '2.350,49', '2.350,49', 'COMPRAS ', ''] # noqa
     """
@@ -55,15 +57,15 @@
         raw_date = self.row[0]
         splited_date = raw_date.split("-")
         splited_date.reverse()
         joined_date = "-".join(splited_date)
         return pendulum.parse(joined_date)
 
 
-class GatewayCGDFile:
+class GatewayCGDFile(ImportTransactionsTransactionGater):
     """
     Example of a file:
         Consultar saldos e movimentos � ordem - 09-08-2022
 
         Conta ;1234567890 - EUR - Conta Caderneta
         Data de in�cio ;01-01-2020
         Data de fim ;09-08-2022
```

### Comparing `profitpulse-1.4.0/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-1.4.1/src/profitpulse/gateways/cgdfile_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.0/src/profitpulse/infrastructure/migrations.py` & `profitpulse-1.4.1/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.0/src/profitpulse/lib/account.py` & `profitpulse-1.4.1/src/profitpulse/lib/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
             self._balance = balance
 
         self._deposit_list: List[Money] = []
 
     def __repr__(self) -> str:
         return f"Account({self._account_name})"
 
+    def snapshot(self, value: Money) -> None:
+        self._balance = value
+
     @property
     def name(self) -> AccountName:
         return self._account_name
 
     @property
     def balance(self) -> Money:
         return self._balance
```

### Comparing `profitpulse-1.4.0/src/profitpulse/lib/account_name.py` & `profitpulse-1.4.1/src/profitpulse/lib/account_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.0/src/profitpulse/lib/money.py` & `profitpulse-1.4.1/src/profitpulse/lib/money.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
     def __repr__(self) -> str:
         return f"Money({self._cents})"
 
     def __add__(self, other: Money) -> Money:
         return Money(self._cents + other._cents)
 
+    def __sub__(self, other: Money) -> Money:
+        return Money(self._cents - other._cents)
+
     def __lt__(self, other: Money) -> bool:
         return self._cents < other._cents
 
     def __gt__(self, other: Money) -> bool:
         return self._cents > other._cents
 
     @property
```

### Comparing `profitpulse-1.4.0/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-1.4.1/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     created_at DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,
     updated_at DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,
     PRIMARY KEY (id)
 );
 
 CREATE TABLE IF NOT EXISTS balance (
     id INTEGER NOT NULL,
-    value INTEGER NOT NULL,
+    value INTEGER DEFAULT 0,
     account_id INTEGER NOT NULL,
     description VARCHAR(30) DEFAULT '',
     date_of_movement DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,
     origin VARCHAR(5) NOT NULL DEFAULT '',
     created_at DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,
     updated_at DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,
     FOREIGN KEY (account_id) REFERENCES account(id),
@@ -22,8 +22,8 @@
 
 CREATE TABLE IF NOT EXISTS event (
     id INTEGER PRIMARY KEY,
     name VARCHAR(30) NOT NULL,
     data JSON NOT NULL,
     created_at DATETIME NOT NULL,
     UNIQUE(name, data, created_at)
-)
+);
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/close_account.py` & `profitpulse-1.4.1/src/profitpulse/services/snapshot_account.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 import abc
-import typing
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
+from profitpulse.lib.money import Money
+from profitpulse.services.errors import AccountNotFoundError
 
 
-class AccountNotFoundError(Exception):
-    def __init__(self, account_name: AccountName) -> None:
-        self._account_name = account_name
-
-    def __str__(self) -> str:
-        return f"Could not find an account with name '{self._account_name}'"
-
-
-class CloseAccountRequester(typing.Protocol):
+class SnapshotAccountRequester(abc.ABC):
     @property
     @abc.abstractmethod
     def account_name(self) -> AccountName: ...  # pragma: no cover
 
+    @property
+    @abc.abstractmethod
+    def value(self) -> Money: ...  # pragma: no cover
 
-class Accounts(typing.Protocol):
-    def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
 
-    def append(self, account: Account) -> None: ...  # pragma: no cover
+class SnapshotAccountAccountCollector(abc.ABC):
+    @abc.abstractmethod
+    def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
 
+    @abc.abstractmethod
+    def __setitem__(
+        self, account_name: AccountName, account: Account
+    ) -> None: ...  # pragma: no cover
 
-class CloseAccountService:
-    """
-    Closes an account.
-    """
 
-    def __init__(self, accounts: Accounts) -> None:
+class SnapshotAccountService:
+    def __init__(self, accounts: SnapshotAccountAccountCollector):
         self.accounts = accounts
 
-    def execute(self, request: CloseAccountRequester) -> None:
+    def execute(self, request: SnapshotAccountRequester) -> None:
         try:
             account = self.accounts[request.account_name]
         except KeyError:
             raise AccountNotFoundError(request.account_name)
 
-        account.close()
+        account.snapshot(request.value)
 
-        self.accounts.append(account)
+        self.accounts[request.account_name] = account
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/close_account_test.py` & `profitpulse-1.4.1/src/profitpulse/services/close_account_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import Optional
 
 import pytest
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
-from profitpulse.services.close_account import AccountNotFoundError, CloseAccountService
+from profitpulse.services.close_account import (
+    AccountNotFoundError,
+    CloseAccountAccountCollector,
+    CloseAccountRequester,
+    CloseAccountService,
+)
 
 
-class CloseAccountRequest:
+class CloseAccountRequest(CloseAccountRequester):
     def __init__(self, account_name: str):
         self._account_name = account_name
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
@@ -25,35 +30,30 @@
     with pytest.raises(
         AccountNotFoundError,
         match="Could not find an account with name 'TheAccountName'",
     ):
         service.execute(request)
 
 
-class CloseAccountAccountsRepo:
+class CloseAccountAccountsRepo(CloseAccountAccountCollector):
     def __init__(self, account: Optional[Account] = None) -> None:
         self._account = account
 
-    @property
-    def account_was_closed(self) -> bool:
-        if not self._account:
-            raise Exception("Expected an account, got None")
-        return self._account.closed
-
     def __getitem__(self, account_name: AccountName) -> Account:
         if not self._account:
             raise KeyError
         return self._account
 
     def append(self, account: Account) -> None:
         self._account = account
 
 
 def test_close_account_when_the_account_exists() -> None:
     account_name = "TheAccountName"
-    accounts = CloseAccountAccountsRepo(Account(AccountName(account_name)))
+    account = Account(AccountName(account_name))
+    accounts = CloseAccountAccountsRepo(account)
     request = CloseAccountRequest(account_name)
     service = CloseAccountService(accounts)
 
     service.execute(request)
 
-    assert accounts.account_was_closed  # nosec
+    assert account.closed  # nosec
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/delete_account.py` & `profitpulse-1.4.1/src/profitpulse/services/deposit_into_account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import abc
+from typing import Optional
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
+from profitpulse.lib.comment import Comment
+from profitpulse.lib.money import Money
+from profitpulse.services.errors import AccountNotFoundError
 
 
-class AccountNotFoundError(Exception):
-    def __init__(self, account_name: AccountName) -> None:
-        self._account_name = account_name
-
-    def __str__(self) -> str:
-        return f"Could not find an account with name '{self._account_name}'"
+class DepositIntoAccountRequester(abc.ABC):
+    @property
+    @abc.abstractmethod
+    def account_name(self) -> AccountName: ...  # pragma: no cover
 
+    @property
+    @abc.abstractmethod
+    def comment(self) -> Optional[Comment]: ...  # pragma: no cover
 
-class DeleteAccountRequester(abc.ABC):
     @property
     @abc.abstractmethod
-    def account_name(self) -> AccountName: ...  # pragma: no cover
+    def amount(self) -> Money: ...  # pragma: no cover
 
 
-class AccountsRepository(abc.ABC):
+class DepositIntoAccountAccountCollector(abc.ABC):
     @abc.abstractmethod
     def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
 
     @abc.abstractmethod
-    def __delitem__(self, account_name: AccountName) -> None: ...  # pragma: no cover
+    def __setitem__(
+        self, account_name: AccountName, account: Account
+    ) -> None: ...  # pragma: no cover
 
 
-class ServiceDeleteAccount:
-    def __init__(self, accounts: AccountsRepository) -> None:
+class DepositIntoAccountService:
+    def __init__(self, accounts: DepositIntoAccountAccountCollector):
         self._accounts = accounts
 
-    def execute(self, request: DeleteAccountRequester) -> None:
+    def execute(self, request: DepositIntoAccountRequester) -> None:
         try:
             account = self._accounts[request.account_name]
         except KeyError:
-            raise AccountNotFoundError(account_name=request.account_name)
+            raise AccountNotFoundError(request.account_name)
 
-        account.prepare_deletion()
+        account.deposit(request.amount, comment=request.comment)
 
-        del self._accounts[request.account_name]
+        self._accounts[request.account_name] = account
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/delete_account_test.py` & `profitpulse-1.4.1/src/profitpulse/services/delete_account_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 
 from profitpulse.lib.account import Account, AccountCantBeDeletedError
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.money import Money
 from profitpulse.services.delete_account import (
     AccountNotFoundError,
     DeleteAccountRequester,
-    ServiceDeleteAccount,
+    DeleteAccountService,
 )
 
 
 class DeleteAccountRequest(DeleteAccountRequester):
     @property
     def account_name(self) -> AccountName:
         return AccountName("TheAccountName")
 
 
 def test_raise_error_when_account_does_not_exist() -> None:
     request = DeleteAccountRequest()
-    service = ServiceDeleteAccount({})  # type: ignore
+    service = DeleteAccountService({})  # type: ignore
     with pytest.raises(
         AccountNotFoundError,
         match=f"Could not find an account with name '{request.account_name}'",
     ):
         service.execute(request)
 
 
 def test_raise_error_when_account_cant_be_deleted() -> None:
     request = DeleteAccountRequest()
     account = Account(account_name=request.account_name, balance=Money(10))
     accounts = {request.account_name: account}
 
-    service = ServiceDeleteAccount(accounts)  # type: ignore
+    service = DeleteAccountService(accounts)  # type: ignore
     with pytest.raises(
         AccountCantBeDeletedError,
         match="Account can't be deleted",
     ):
         service.execute(request)
 
 
 def test_delete_account_when_exists() -> None:
     request = DeleteAccountRequest()
     account = Account(account_name=request.account_name, balance=Money(0))
     accounts = {request.account_name: account}
 
-    service = ServiceDeleteAccount(accounts)  # type: ignore
+    service = DeleteAccountService(accounts)  # type: ignore
     service.execute(request)
 
     assert len(accounts) == 0  # nosec
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/deposit_into_account.py` & `profitpulse-1.4.1/src/profitpulse/services/close_account.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 import abc
-import typing
-from typing import Optional
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
-from profitpulse.lib.comment import Comment
-from profitpulse.lib.money import Money
+from profitpulse.services.errors import AccountNotFoundError
 
 
-class AccountDoesNotExistError(Exception):
-    def __str__(self) -> str:
-        return "Account does not exist"
-
-
-class Accounts(typing.Protocol):
-    def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
-
-    def __setitem__(
-        self, account_name: AccountName, account: Account
-    ) -> None: ...  # pragma: no cover
-
-
-class DepositIntoAccountRequest(typing.Protocol):
+class CloseAccountRequester(abc.ABC):
     @property
     @abc.abstractmethod
     def account_name(self) -> AccountName: ...  # pragma: no cover
 
-    @property
+
+class CloseAccountAccountCollector(abc.ABC):
     @abc.abstractmethod
-    def comment(self) -> Optional[Comment]: ...  # pragma: no cover
+    def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
 
-    @property
     @abc.abstractmethod
-    def amount(self) -> Money: ...  # pragma: no cover
+    def append(self, account: Account) -> None: ...  # pragma: no cover
+
 
+class CloseAccountService:
+    """
+    Closes an account.
+    """
 
-class ServiceDepositIntoAccount:
-    def __init__(self, accounts: Accounts):
-        self._accounts = accounts
+    def __init__(self, accounts: CloseAccountAccountCollector) -> None:
+        self.accounts = accounts
 
-    def execute(self, request: DepositIntoAccountRequest) -> None:
+    def execute(self, request: CloseAccountRequester) -> None:
         try:
-            account = self._accounts[request.account_name]
+            account = self.accounts[request.account_name]
         except KeyError:
-            raise AccountDoesNotExistError()
+            raise AccountNotFoundError(request.account_name)
 
-        account.deposit(request.amount, comment=request.comment)
+        account.close()
 
-        self._accounts[request.account_name] = account
+        self.accounts.append(account)
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/deposit_into_account_test.py` & `profitpulse-1.4.1/src/profitpulse/services/deposit_into_account_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import Any
-
 import pytest
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
 from profitpulse.services.deposit_into_account import (
-    AccountDoesNotExistError,
-    ServiceDepositIntoAccount,
+    AccountNotFoundError,
+    DepositIntoAccountAccountCollector,
+    DepositIntoAccountRequester,
+    DepositIntoAccountService,
 )
+from profitpulse.turbofan import assert_string_equals
 
 
-class AccountsNoAccount:
+class AccountsNoAccount(DepositIntoAccountAccountCollector):
     def __getitem__(self, account_name: AccountName) -> Account:
         raise KeyError
 
     def __setitem__(self, account_name: AccountName, account: Account) -> None:
         pass
 
 
-class DepositInAccountRequest:
+class DepositInAccountRequest(DepositIntoAccountRequester):
     @property
     def account_name(self) -> AccountName:
         return AccountName("TheAccountName")
 
     @property
     def comment(self) -> None:
         return None
@@ -34,20 +35,23 @@
         return Money(100)
 
 
 def test_raise_error_if_account_does_not_exist() -> None:
     request = DepositInAccountRequest()
     accounts = AccountsNoAccount()
 
-    service = ServiceDepositIntoAccount(accounts)
-    with pytest.raises(AccountDoesNotExistError, match="Account does not exist"):
+    service = DepositIntoAccountService(accounts)
+    with pytest.raises(
+        AccountNotFoundError,
+        match="Could not find an account with name 'TheAccountName'",
+    ):
         service.execute(request)
 
 
-class Accounts:
+class AccountsStub(DepositIntoAccountAccountCollector):
     def __init__(self, account: Account) -> None:
         self._account = account
         self.account_added = False
 
     def __getitem__(self, account_name: AccountName) -> Account:
         return self._account
 
@@ -55,25 +59,25 @@
         self.account_added = True
         self._account = account
 
 
 def test_save_deposit_into_account() -> None:
     request = DepositInAccountRequest()
     account = Account(AccountName("TheAccountName"))
-    accounts = Accounts(account)
+    accounts = AccountsStub(account)
 
-    service = ServiceDepositIntoAccount(accounts)
+    service = DepositIntoAccountService(accounts)
 
     service.execute(request)
 
     assert accounts.account_added  # nosec
     assert account.last_comment is None  # nosec
 
 
-class DepositInAccountWithCommentRequest:
+class DepositInAccountWithCommentRequest(DepositIntoAccountRequester):
     @property
     def account_name(self) -> AccountName:
         return AccountName("TheAccountName")
 
     @property
     def comment(self) -> Comment:
         return Comment("A comment")
@@ -82,25 +86,15 @@
     def amount(self) -> Money:
         return Money(100)
 
 
 def test_inject_the_comment_into_the_account_deposit_when_one_is_defined() -> None:
     request = DepositInAccountWithCommentRequest()
     account = Account(AccountName("TheAccountName"))
-    accounts = Accounts(account)
+    accounts = AccountsStub(account)
 
-    service = ServiceDepositIntoAccount(accounts)
+    service = DepositIntoAccountService(accounts)
 
     service.execute(request)
 
     assert accounts.account_added  # nosec
     assert_string_equals("A comment", account.last_comment)
-
-
-# TODO: move to toolcat
-def assert_string_equals(expected: str, got: Any) -> None:
-    """
-    Compares an object objects in its string value and raises an AssertionError
-    if it's not equal to the expected value.
-    """
-    __tracebackhide__ = True
-    assert str(got) == expected, f"Expected {expected}, got {got}"  # nosec
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/import_transactions.py` & `profitpulse-1.4.1/src/profitpulse/services/import_transactions_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,83 @@
 # type: ignore
-import abc
-import typing
+import pytest
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
-from profitpulse.lib.transaction import Transaction
-from profitpulse.services.deposit_into_account import AccountDoesNotExistError
+from profitpulse.services.deposit_into_account import AccountNotFoundError
+from profitpulse.services.import_transactions import ImportTransactionsService
 
 
-class GatewayTransactions(typing.Protocol):
-    """
-    Gateway to transactions.
-    """
+class AccountsStub:
+    def __getitem__(self, account_name: AccountName) -> Account:
+        return Account(account_name)
 
-    def __iter__(self) -> None:
-        pass  # pragma: no cover
 
-
-class RepositoryTransactions(typing.Protocol):
-    """
-    Repository to transactions.
-    """
-
-    def append(self, transaction: Transaction, account_name: AccountName) -> None:
-        pass  # pragma: no cover
-
-
-class ImportTransactionsRequest(abc.ABC):
+class RequestStub:
     @property
-    @abc.abstractmethod
-    def account_name(self) -> AccountName: ...  # pragma: no cover
-
-
-class Accounts(typing.Protocol):
-    def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
-
+    def account_name(self) -> AccountName:
+        return AccountName("TheAccountName")
 
-class ServiceImportTransactions:
-    """
-    Imports transactions from a source.
-    """
-
-    def __init__(
-        self,
-        transactions_gateway: GatewayTransactions,
-        transactions: RepositoryTransactions,
-        accounts: Accounts,
-    ) -> None:
-        self.transactions = transactions_gateway
-        self._transactions = transactions
-        self._accounts = accounts
-
-    def execute(self, request: ImportTransactionsRequest) -> None:
-        try:
-            _ = self._accounts[request.account_name]
-        except KeyError:
-            raise AccountDoesNotExistError
 
-        for transaction in self.transactions:
-            self._transactions.append(transaction, request.account_name)
+def test_append_zero_transactions_when_no_transactions_to_append() -> None:
+    request = RequestStub()
+    accounts = AccountsStub()
+    source_transactions = []
+    transactions = []
+    service = ImportTransactionsService(
+        source_transactions,
+        transactions,
+        accounts,
+    )
+
+    service.execute(request)
+
+    assert len(transactions) == 0  # nosec
+
+
+class TransactionsStub:
+    def __init__(self) -> None:
+        self._transactions = []  # type: ignore
+
+    def append(self, transaction, account_name: AccountName):
+        self._transactions.append(transaction)
+
+    def __len__(self):
+        return len(self._transactions)
+
+
+def test_append_one_transaction_when_one_transaction_available_in_source():
+    request = RequestStub()
+    accounts = AccountsStub()
+    source_transactions = [{}]
+    transactions = TransactionsStub()
+    service = ImportTransactionsService(
+        source_transactions,
+        transactions,
+        accounts,
+    )
+
+    service.execute(request)
+
+    assert len(transactions) == 1  # nosec
+
+
+class AccountNotFounStub:
+    def __getitem__(self, _):
+        raise KeyError
+
+
+def test_raise_error_if_account_not_found() -> None:
+    request = RequestStub()
+    accounts = AccountNotFounStub()
+    transactions = []
+    source_transactions = [{}]
+    service = ImportTransactionsService(
+        source_transactions,
+        transactions,
+        accounts,
+    )
+    with pytest.raises(
+        AccountNotFoundError,
+        match="Could not find an account with name 'TheAccountName'",
+    ):
+        service.execute(request)
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/open_account.py` & `profitpulse-1.4.1/src/profitpulse/services/open_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import abc
-import typing
 from typing import Optional
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
 
 
 class AccountAlreadyExistsError(Exception):
     def __str__(self) -> str:
         return "An account with the same name already exists"
 
 
-class Accounts(typing.Protocol):
+class OpenAccountRequester(abc.ABC):
+    @property
+    @abc.abstractmethod
+    def account_name(self) -> AccountName: ...  # pragma: no cover
+
+
+class OpenAccountAccountCollector(abc.ABC):
     def get(
         self, account_name: AccountName
     ) -> Optional[Account]: ...  # pragma: no cover
 
     def __setitem__(
         self, account_name: AccountName, account: Account
     ) -> None: ...  # pragma: no cover
 
 
-class OpenAccountRequester(abc.ABC):
-    @property
-    @abc.abstractmethod
-    def account_name(self) -> AccountName: ...  # pragma: no cover
-
-
 class OpenAccountService:
-    def __init__(self, accounts: Accounts):
+    def __init__(self, accounts: OpenAccountAccountCollector):
         self.accounts = accounts
 
     def execute(self, request: OpenAccountRequester) -> None:
         if self.accounts.get(request.account_name):
             raise AccountAlreadyExistsError()
 
         account = Account(request.account_name)
```

### Comparing `profitpulse-1.4.0/src/profitpulse/services/open_account_test.py` & `profitpulse-1.4.1/src/profitpulse/services/open_account_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import pytest
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
 from profitpulse.services.open_account import (
     AccountAlreadyExistsError,
+    OpenAccountAccountCollector,
     OpenAccountRequester,
     OpenAccountService,
 )
 
 
-class AccountsStub:
+class AccountsStub(OpenAccountAccountCollector):
     def __init__(self) -> None:
         self._accounts: Dict[AccountName, Account] = dict()
 
     def get(self, account_name: AccountName) -> Optional[Account]:
         try:
             return self._accounts[account_name]
         except KeyError:
```

### Comparing `profitpulse-1.4.0/src/profitpulse/testrig/fixtures.py` & `profitpulse-1.4.1/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.0/src/profitpulse/testrig/scenario.py` & `profitpulse-1.4.1/src/profitpulse/testrig/scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # type: ignore
 from typing import Optional
 
 from typer.testing import CliRunner
 
-from profitpulse.cli.main import app
+from profitpulse.cli.main import profitpulse_app
 
 runner = CliRunner(mix_stderr=False)
 
 
 class CLIScenario:
     """
     Builds scenarios up on the tests can be run.
     """
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}"
 
     def __init__(self, *_, **__) -> None:
-        self._app = app
+        self._app = profitpulse_app
 
     # Account management -----------------------------------------------------------------------------------------------
 
     def show_accounts(self):
         """
         Shows all the accounts and their current balance.
         """
@@ -88,14 +88,21 @@
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     # Reports ----------------------------------------------------------------------------------------------------------
 
+    def snapshot(self, amount: int, account_name: str):
+        result = runner.invoke(
+            self._app, ["snapshot", str(amount), account_name], catch_exceptions=False
+        )
+        assert result.exit_code == 0, result.stderr  # nosec
+        return result.stdout
+
     def pulse(self):
         """
         Shows a global view of the user finances.
         """
 
         result = runner.invoke(self._app, ["pulse"], catch_exceptions=False)
```

### Comparing `profitpulse-1.4.0/PKG-INFO` & `profitpulse-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 1.4.0
+Version: 1.4.1
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
@@ -25,26 +25,26 @@
 Project-URL: Repository, https://github.com/luistm/profitpulse
 Description-Content-Type: text/markdown
 
 # Profit Pulse
 
 [![PyPI version](https://badge.fury.io/py/profitpulse.svg)](https://badge.fury.io/py/profitpulse) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/profitpulse)
 
-Profit Pulse: Maximise Earnings Through Smart Wealth Management.
-
-Effortlessly manage your personal finances, supercharge savings, and boost
-profits. Gain depp insights into your money flow, make strategic choices and
-pave your way to financial growth.
+Profit Pulse: Use a Python built CLI application to effortlessly manage your
+personal finances. Increase savings, and boost profits. Gain deep insights into
+your money flow, make strategic choices and pave your way to financial
+independence.
 
 ## How to install ?
 
-### macOS
+Install [pipx](https://github.com/pypa/pipx) using the [official installation instructions](https://pipx.pypa.io/stable/installation/).
+Next, install profitpulse
 
 ```bash
-pip install profitpulse
+pipx install profitpulse
 ```
 
 ## How to use ?
 
 To access the available commands, just execute:
 
 ```bash
@@ -61,10 +61,9 @@
 
 After cloning the repository to your machine, in the project root, just run:
 
 ```bash
 make all
 ```
 
-If everything went smoothly you are now ready to add some contributions. Take a
-look at the CONTRIBUTING.md file for more guidelines (once I write them :).
+If everything went smoothly you are now ready to add some contributions.
```

