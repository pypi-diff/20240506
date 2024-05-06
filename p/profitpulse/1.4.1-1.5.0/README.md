# Comparing `tmp/profitpulse-1.4.1.tar.gz` & `tmp/profitpulse-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-1.4.1.tar", max compression
+gzip compressed data, was "profitpulse-1.5.0.tar", max compression
```

## Comparing `profitpulse-1.4.1.tar` & `profitpulse-1.5.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-1.4.1/LICENSE
--rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-1.4.1/README.md
--rw-r--r--   0        0        0     1816 2024-05-05 20:20:43.114182 profitpulse-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-1.4.1/src/profitpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-1.4.1/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     7410 2024-05-05 20:15:15.188339 profitpulse-1.4.1/src/profitpulse/cli/adapters.py
--rw-r--r--   0        0        0     5198 2024-05-05 19:43:17.612917 profitpulse-1.4.1/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-1.4.1/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     5684 2024-05-05 20:16:40.464175 profitpulse-1.4.1/src/profitpulse/data/accounts.py
--rw-r--r--   0        0        0     2855 2024-05-04 09:07:56.047857 profitpulse-1.4.1/src/profitpulse/data/accounts_test.py
--rw-r--r--   0        0        0     2007 2024-05-05 20:18:18.593519 profitpulse-1.4.1/src/profitpulse/data/transactions.py
--rw-r--r--   0        0        0     6008 2024-05-05 20:19:04.762138 profitpulse-1.4.1/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     6833 2024-05-05 19:43:17.725626 profitpulse-1.4.1/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-1.4.1/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-1.4.1/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-1.4.1/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-1.4.1/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-1.4.1/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-1.4.1/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1832 2024-05-05 19:43:17.382906 profitpulse-1.4.1/src/profitpulse/lib/account.py
--rw-r--r--   0        0        0      549 2024-04-27 17:48:38.578920 profitpulse-1.4.1/src/profitpulse/lib/account_name.py
--rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-1.4.1/src/profitpulse/lib/comment.py
--rw-r--r--   0        0        0      863 2024-05-05 19:54:59.624362 profitpulse-1.4.1/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-1.4.1/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-1.4.1/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-1.4.1/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-1.4.1/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-1.4.1/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1031 2024-05-05 19:29:56.480759 profitpulse-1.4.1/src/profitpulse/services/close_account.py
--rw-r--r--   0        0        0     1693 2024-05-05 19:43:17.172209 profitpulse-1.4.1/src/profitpulse/services/close_account_test.py
--rw-r--r--   0        0        0     1047 2024-05-05 19:29:56.481760 profitpulse-1.4.1/src/profitpulse/services/delete_account.py
--rw-r--r--   0        0        0     1559 2024-05-05 19:43:17.320460 profitpulse-1.4.1/src/profitpulse/services/delete_account_test.py
--rw-r--r--   0        0        0     1432 2024-05-05 19:43:17.249123 profitpulse-1.4.1/src/profitpulse/services/deposit_into_account.py
--rw-r--r--   0        0        0     2848 2024-05-05 19:43:17.334540 profitpulse-1.4.1/src/profitpulse/services/deposit_into_account_test.py
--rw-r--r--   0        0        0      303 2024-05-05 19:29:56.485862 profitpulse-1.4.1/src/profitpulse/services/errors.py
--rw-r--r--   0        0        0     1672 2024-05-05 19:43:17.358387 profitpulse-1.4.1/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     2112 2024-05-05 19:43:17.451850 profitpulse-1.4.1/src/profitpulse/services/import_transactions_test.py
--rw-r--r--   0        0        0     1231 2024-05-05 19:43:17.209744 profitpulse-1.4.1/src/profitpulse/services/open_account.py
--rw-r--r--   0        0        0     1719 2024-05-05 19:43:17.459527 profitpulse-1.4.1/src/profitpulse/services/open_account_test.py
--rw-r--r--   0        0        0     1209 2024-05-05 19:43:17.183351 profitpulse-1.4.1/src/profitpulse/services/snapshot_account.py
--rw-r--r--   0        0        0     1751 2024-05-05 20:16:09.319552 profitpulse-1.4.1/src/profitpulse/services/snapshot_account_test.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-1.4.1/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-1.4.1/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-1.4.1/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4741 2024-05-05 20:12:45.584169 profitpulse-1.4.1/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-1.4.1/src/profitpulse/turbofan.py
--rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 profitpulse-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-1.5.0/README.md
+-rw-r--r--   0        0        0     1816 2024-05-06 20:07:24.907678 profitpulse-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-1.5.0/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-1.5.0/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     8292 2024-05-06 20:00:20.119273 profitpulse-1.5.0/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     5202 2024-05-06 17:27:14.195913 profitpulse-1.5.0/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-1.5.0/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     5989 2024-05-06 20:00:20.120217 profitpulse-1.5.0/src/profitpulse/data/accounts.py
+-rw-r--r--   0        0        0     2855 2024-05-06 19:33:31.689142 profitpulse-1.5.0/src/profitpulse/data/accounts_test.py
+-rw-r--r--   0        0        0     1894 2024-05-06 20:00:20.120854 profitpulse-1.5.0/src/profitpulse/data/pulse_view.py
+-rw-r--r--   0        0        0     1630 2024-05-06 20:00:20.121528 profitpulse-1.5.0/src/profitpulse/data/pulse_view_test.py
+-rw-r--r--   0        0        0     2007 2024-05-05 20:18:18.593519 profitpulse-1.5.0/src/profitpulse/data/transactions.py
+-rw-r--r--   0        0        0     4677 2024-05-06 20:00:20.122106 profitpulse-1.5.0/src/profitpulse/data/views.py
+-rw-r--r--   0        0        0     6833 2024-05-05 19:43:17.725626 profitpulse-1.5.0/src/profitpulse/data/views_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-1.5.0/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-1.5.0/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-1.5.0/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-1.5.0/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-1.5.0/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-1.5.0/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1831 2024-05-06 19:33:31.689548 profitpulse-1.5.0/src/profitpulse/lib/account.py
+-rw-r--r--   0        0        0      549 2024-04-27 17:48:38.578920 profitpulse-1.5.0/src/profitpulse/lib/account_name.py
+-rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-1.5.0/src/profitpulse/lib/comment.py
+-rw-r--r--   0        0        0      863 2024-05-05 19:54:59.624362 profitpulse-1.5.0/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-1.5.0/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      954 2024-05-05 19:49:14.366161 profitpulse-1.5.0/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-1.5.0/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-1.5.0/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-1.5.0/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1031 2024-05-06 19:33:31.690477 profitpulse-1.5.0/src/profitpulse/services/close_account.py
+-rw-r--r--   0        0        0     1693 2024-05-06 19:33:31.691325 profitpulse-1.5.0/src/profitpulse/services/close_account_test.py
+-rw-r--r--   0        0        0     1047 2024-05-06 19:33:31.692391 profitpulse-1.5.0/src/profitpulse/services/delete_account.py
+-rw-r--r--   0        0        0     1559 2024-05-06 19:33:31.693279 profitpulse-1.5.0/src/profitpulse/services/delete_account_test.py
+-rw-r--r--   0        0        0     1432 2024-05-06 19:33:31.694493 profitpulse-1.5.0/src/profitpulse/services/deposit_into_account.py
+-rw-r--r--   0        0        0     2848 2024-05-06 19:33:31.695520 profitpulse-1.5.0/src/profitpulse/services/deposit_into_account_test.py
+-rw-r--r--   0        0        0      303 2024-05-05 19:29:56.485862 profitpulse-1.5.0/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     1672 2024-05-06 19:33:31.696410 profitpulse-1.5.0/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     2112 2024-05-06 19:33:31.697162 profitpulse-1.5.0/src/profitpulse/services/import_transactions_test.py
+-rw-r--r--   0        0        0     1231 2024-05-06 19:33:31.697817 profitpulse-1.5.0/src/profitpulse/services/open_account.py
+-rw-r--r--   0        0        0     1719 2024-05-06 19:33:31.698567 profitpulse-1.5.0/src/profitpulse/services/open_account_test.py
+-rw-r--r--   0        0        0     1203 2024-05-06 19:33:31.699271 profitpulse-1.5.0/src/profitpulse/services/revalue.py
+-rw-r--r--   0        0        0     1731 2024-05-06 19:33:31.700207 profitpulse-1.5.0/src/profitpulse/services/revalue_test.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-1.5.0/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-1.5.0/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-1.5.0/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4748 2024-05-06 19:58:30.761194 profitpulse-1.5.0/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-1.5.0/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 profitpulse-1.5.0/PKG-INFO
```

### Comparing `profitpulse-1.4.1/LICENSE` & `profitpulse-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/README.md` & `profitpulse-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/pyproject.toml` & `profitpulse-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "1.4.1"
+version = "1.5.0"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
```

### Comparing `profitpulse-1.4.1/src/profitpulse/cli/adapters.py` & `profitpulse-1.5.0/src/profitpulse/cli/adapters.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from pathlib import Path
 from typing import Optional
 
 from gogotable import gogotable
 from turbofan.database import Database, Session
 
 from profitpulse.data.accounts import Accounts
+from profitpulse.data.pulse_view import PulseView
 from profitpulse.data.transactions import Transactions
-from profitpulse.data.views import AccountsView, PulseView, TransactionsView
+from profitpulse.data.views import AccountsView, TransactionsView
 from profitpulse.gateways.cgdfile import GatewayCGDFile  # type: ignore
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
 from profitpulse.services.close_account import (
     CloseAccountRequester,
     CloseAccountService,
@@ -35,30 +36,35 @@
     ImportTransactionsService,
 )
 from profitpulse.services.open_account import (
     AccountAlreadyExistsError,
     OpenAccountRequester,
     OpenAccountService,
 )
-from profitpulse.services.snapshot_account import (
-    SnapshotAccountRequester,
-    SnapshotAccountService,
-)
+from profitpulse.services.revalue import RevalueAccountRequester, RevalueAccountService
 
 logging.basicConfig(level=logging.CRITICAL)
 logger = logging.getLogger(__name__)
 
 database_path = Path.home() / Path("Library/Application Support/Profitpulse")
 
 
 def report(
     seller: Optional[str],
     since: Optional[datetime] = None,
     on: Optional[datetime] = None,
 ) -> None:
+    """
+    Shows a report of all transactions in all accounts given the provided
+     parameters:
+     - seller: The provider or recipient of the value
+     - since: The data from which the transactions should be shown
+     - on: A specific date for which transactions should be shown
+    """
+
     db = Database(database_path)
     with Session(db.engine) as session:
         view = TransactionsView(session, seller, since, on)
 
         transactions, total = view.data
         if seller:
             print(f"Description: '{seller}', Value: {round(total, 2)}")
@@ -66,66 +72,75 @@
 
         for t in transactions:
             print(f"Description: '{t['description']:>22}', Value: {t['value']:>10}")
 
 
 def pulse() -> None:
     """
-    Read all the events and print the current proofit pulse.
+    Shows the current wealth status.
     """
 
-    headers = ["Account Name", "Invested", "Current", "Performance"]
+    headers = ["Account Name", "Status", "Invested", "Current", "Performance"]
 
     db = Database(database_path)
     with Session(db.engine) as session:
         view = PulseView(session)
         lines = gogotable(headers, view.data)
         for line in lines:
             print(line)
 
 
-class SnapshotAccountRequest(SnapshotAccountRequester):
+class RevalueAccountRequest(RevalueAccountRequester):
     def __init__(self, account_name: str, value: int) -> None:
         self._account_name = account_name
         self._value = value
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
     @property
     def value(self) -> Money:
         return Money(self._value)
 
 
-def snapshot(cent_amount: int, account_name: str) -> None:
+def revalue(cent_amount: int, account_name: str) -> None:
+    """
+    Revalues an asset to reflect it's current worth.
+    """
     db = Database(database_path)
     with Session(db.engine) as session:
-        request = SnapshotAccountRequest(account_name, cent_amount)
+        request = RevalueAccountRequest(account_name, cent_amount)
         accounts = Accounts(session)
-        service = SnapshotAccountService(accounts)
+        service = RevalueAccountService(accounts)
         service.execute(request)
         session.commit()
 
 
 def reset() -> None:
+    """
+    Resets the application by removing the database.
+    """
     db = Database(database_path)
     db.remove()
 
 
 class RequestImportTransactions(ImportTransactionsRequester):
     def __init__(self, account_name: str) -> None:
         self._account_name = account_name
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
 def import_file(file_path: Path, account_name: str) -> None:
+    """
+    Imports a file with all the transactions for a specific asset.
+    """
     db = Database(database_path)
     with Session(db.engine) as session:
         gateway_cgd = GatewayCGDFile(file_path)
         transactions = Transactions(session)
         accounts = Accounts(session)
         service = ImportTransactionsService(gateway_cgd, transactions, accounts)
         request = RequestImportTransactions(account_name)
@@ -151,38 +166,47 @@
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
 def deposit(cent_amount: int, account_name: str, comment: Optional[str] = None) -> None:
+    """
+    Appreciate an asset by increasing it's value.
+    """
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = DepositRequest(cent_amount, account_name, comment)
         service = DepositIntoAccountService(accounts)
         service.execute(request)
 
         session.commit()
 
 
 def transfer(cent_amount: int, from_account_name: str, to_account_name: str) -> None:
+    """
+    Transfers value from an asset to another asset.
+    """
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = DepositRequest(cent_amount, from_account_name)
         service = DepositIntoAccountService(accounts)
         service.execute(request)
 
         request = DepositRequest(-cent_amount, to_account_name)
         service = DepositIntoAccountService(accounts)
         service.execute(request)
 
         session.commit()
 
 
 def show_accounts() -> None:
+    """
+    Shows all assets and their current value.
+    """
     with Session(Database(database_path).engine) as session:
         data = AccountsView(session).data
         if not data:
             return
 
         headers = ["Name", "Balance", "Status", "Comment"]
         lines = gogotable(headers, data)
@@ -196,14 +220,17 @@
 
     @property
     def account_name(self) -> AccountName:
         return self._name
 
 
 def open_account(name: str) -> None:
+    """
+    Creates a new asset.
+    """
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = OpenAccountRequest(name)
         try:
             OpenAccountService(accounts).execute(request)
         except AccountAlreadyExistsError as e:
             print(str(e))
@@ -218,14 +245,17 @@
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
 def close_account(name: str) -> None:
+    """
+    Divests an asset from your wealth but the keeping it's history.
+    """
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = CloseAccountRequest(name)
         CloseAccountService(accounts).execute(request)
         session.commit()
 
 
@@ -235,12 +265,15 @@
 
     @property
     def account_name(self) -> AccountName:
         return AccountName(self._account_name)
 
 
 def delete_account(name: str) -> None:
+    """
+    Completely deletes an asset.
+    """
     with Session(Database(database_path).engine) as session:
         accounts = Accounts(session)
         request = DeleteAccountRequest(name)
         DeleteAccountService(accounts).execute(request)
         session.commit()
```

### Comparing `profitpulse-1.4.1/src/profitpulse/cli/main.py` & `profitpulse-1.5.0/src/profitpulse/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     delete_account,
     deposit,
     import_file,
     open_account,
     pulse,
     report,
     reset,
+    revalue,
     show_accounts,
-    snapshot,
     transfer,
 )
 from profitpulse.infrastructure.migrations import migrate_database  # type: ignore
 
 profitpulse_app = typer.Typer(
     add_completion=False,
     help="Profitpulse helps you manage your personal finances.",
@@ -47,26 +47,26 @@
 @profitpulse_app.command(name="pulse", help="Show's the health of your wealth")
 def pulse_() -> None:
     migrate_database(database_path)
     pulse()
 
 
 @profitpulse_app.command(
-    name="snapshot", help="Save the current balance for an account"
+    name="revalue", help="Revalues an asset to reflect it's current worth"
 )
-def snapshot_(
+def revalue_(
     cent_amount: int = typer.Argument(
         0, help="Amount to deposit in cents", metavar="AMOUNT"
     ),
     account_name: str = typer.Argument(
         "", help="Name of the account", metavar='"ACCOUNT NAME"'
     ),
 ) -> None:
     migrate_database(database_path)
-    snapshot(cent_amount, account_name)
+    revalue(cent_amount, account_name)
 
 
 @profitpulse_app.command(name="import", help="Import transactions for expense tracking")
 def import_(
     file_path: Path,
     account_name: str = typer.Argument(
         "", help="Name of the account", metavar='"ACCOUNT NAME"'
```

### Comparing `profitpulse-1.4.1/src/profitpulse/data/accounts.py` & `profitpulse-1.5.0/src/profitpulse/data/accounts.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,39 +10,52 @@
 from profitpulse.lib.comment import Comment
 from profitpulse.lib.money import Money
 from profitpulse.services.close_account import CloseAccountAccountCollector
 from profitpulse.services.delete_account import DeleteAccountAccountCollector
 from profitpulse.services.deposit_into_account import DepositIntoAccountAccountCollector
 from profitpulse.services.import_transactions import ImportTransactionsAccountCollector
 from profitpulse.services.open_account import OpenAccountAccountCollector
-from profitpulse.services.snapshot_account import SnapshotAccountAccountCollector
+from profitpulse.services.revalue import RevalueAccountAccountCollector
 
-OPEN = "O"
-CLOSED = "C"
+ACTIVE = "O"
+DIVESTED = "C"
+
+
+def status_from_value(status: str) -> str:
+    """
+    Returns the status human readable representation.
+    """
+    # TODO: this should be the presentation layer.
+    if status == "O":
+        return "Active"
+    if status == "C":
+        return "Divested"
+
+    raise Exception(f"Unknown status {status}")
 
 
 # Once python3.9 and python.3.10 support is dropped, we can use
 # https://docs.python.org/3/library/enum.html#enum.StrEnum
 class StrEnum(str, Enum):
     pass
 
 
 class PulseEvent(StrEnum):
     MONEY_DEPOSIT = "1"
     TRANSACTION_IMPORTED = "2"
-    ACCOUNT_SNAPSHOT = "3"
+    ACCOUNT_REVALUE = "3"
 
 
 class Accounts(
     CloseAccountAccountCollector,
     DeleteAccountAccountCollector,
     OpenAccountAccountCollector,
     DepositIntoAccountAccountCollector,
     ImportTransactionsAccountCollector,
-    SnapshotAccountAccountCollector,
+    RevalueAccountAccountCollector,
 ):
     """
     Accounts implement the AccountsRepository protocol.
     """
 
     def __init__(self, session: typing.Any) -> None:
         self._session = session
@@ -72,15 +85,15 @@
         sql_stmt = """
             INSERT OR REPLACE INTO account (name, status)
                  VALUES (:name, :status)
         """
         prepared_statement = text(sql_stmt)
         prepared_statement = prepared_statement.bindparams(
             name=str(account.name),
-            status=CLOSED if account.closed else OPEN,
+            status=DIVESTED if account.closed else ACTIVE,
         )
         self._session.execute(prepared_statement)
 
         sql_stmt = """
             INSERT INTO balance (account_id, description)
                  VALUES ((SELECT id FROM account WHERE name = :name), :comment)
         """
@@ -91,15 +104,15 @@
         )
         self._session.execute(prepared_statement)
 
         events = pastperfect.Events(self._session)
 
         events.append(
             pastperfect.Event(
-                name=PulseEvent.ACCOUNT_SNAPSHOT,
+                name=PulseEvent.ACCOUNT_REVALUE,
                 data={"name": str(account.name), "balance": account.balance.cents},
             )
         )
 
         if is_a_new_account:
             events.append(
                 pastperfect.Event(
@@ -136,25 +149,25 @@
             raise KeyError
 
         events = pastperfect.Events(self._session)
         account_name = row[0]
         balance = Money(0)
         for event in events:
             if (
-                event.name != PulseEvent.ACCOUNT_SNAPSHOT
+                event.name != PulseEvent.ACCOUNT_REVALUE
                 or event.data.get("name") != account_name
             ):
                 continue
 
             balance = Money(event.data.get("balance"))
 
         return Account(
             AccountName(row[0]),
             balance=balance,
-            closed=True if row[1] == CLOSED else False,
+            closed=True if row[1] == DIVESTED else False,
             comment=Comment(row[2] if row[2] else ""),
         )
 
     def __delitem__(self, account_name: AccountName) -> None:
         sql_stmt = """
             DELETE FROM balance
                   WHERE account_id = (SELECT id FROM account WHERE name = :name)
```

### Comparing `profitpulse-1.4.1/src/profitpulse/data/accounts_test.py` & `profitpulse-1.5.0/src/profitpulse/data/accounts_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/data/transactions.py` & `profitpulse-1.5.0/src/profitpulse/data/transactions.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/data/views.py` & `profitpulse-1.5.0/src/profitpulse/data/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -37,76 +37,34 @@
 
         results = []
         for account in accounts:
             account_name = account[0]
             account_details = [
                 account_name,
                 "0.00",
-                "Open" if account[1] == accounts_repository.OPEN else "Closed",
+                "Open" if account[1] == accounts_repository.ACTIVE else "Closed",
                 account[2] if account[2] else "",
             ]
             total_balance = Money(0)
             for event in events:
                 if (
-                    event.name != PulseEvent.ACCOUNT_SNAPSHOT
+                    event.name != PulseEvent.ACCOUNT_REVALUE
                     or event.data.get("name") != account_name
                 ):
                     continue
 
                 total_balance = Money(event.data.get("balance"))
 
             account_details[1] = str(total_balance)
 
             results.append(account_details)
 
         return results
 
 
-class PulseView(View):
-    def __init__(self, session: typing.Any):
-        self._session = session
-
-    @property
-    def data(self) -> typing.Any:
-        sql_stmt = """SELECT account.name as name FROM account ORDER BY id ASC"""
-        accounts = self._session.execute(text(sql_stmt))
-
-        events = pastperfect.Events(self._session)
-
-        results = []
-        for account in accounts:
-            account_name = account[0]
-            account_details = [""] * 4
-            invested = Money(0)
-            current = Money(0)
-
-            for event in events:
-                if (
-                    event.name == PulseEvent.ACCOUNT_SNAPSHOT
-                    and event.data.get("name") == account_name
-                ):
-                    current = Money(event.data.get("balance"))
-                    continue
-
-                if (
-                    event.name == PulseEvent.MONEY_DEPOSIT
-                    and event.data.get("name") == account_name
-                ):
-                    invested = invested + Money(event.data.get("balance"))
-
-            account_details[0] = account_name
-            account_details[1] = str(invested)
-            account_details[2] = str(current)
-            account_details[3] = str(current - invested)
-
-            results.append(account_details)
-
-        return results
-
-
 class TransactionsView(View):
     def __init__(
         self,
         session: typing.Any,
         seller: typing.Optional[str] = None,
         since: typing.Optional[datetime] = None,
         on: typing.Optional[datetime] = None,
```

### Comparing `profitpulse-1.4.1/src/profitpulse/data/views_test.py` & `profitpulse-1.5.0/src/profitpulse/data/views_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/gateways/cgdfile.py` & `profitpulse-1.5.0/src/profitpulse/gateways/cgdfile.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-1.5.0/src/profitpulse/gateways/cgdfile_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/infrastructure/migrations.py` & `profitpulse-1.5.0/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/lib/account.py` & `profitpulse-1.5.0/src/profitpulse/lib/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             self._balance = balance
 
         self._deposit_list: List[Money] = []
 
     def __repr__(self) -> str:
         return f"Account({self._account_name})"
 
-    def snapshot(self, value: Money) -> None:
+    def revalue(self, value: Money) -> None:
         self._balance = value
 
     @property
     def name(self) -> AccountName:
         return self._account_name
 
     @property
```

### Comparing `profitpulse-1.4.1/src/profitpulse/lib/account_name.py` & `profitpulse-1.5.0/src/profitpulse/lib/account_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/lib/money.py` & `profitpulse-1.5.0/src/profitpulse/lib/money.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-1.5.0/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/close_account.py` & `profitpulse-1.5.0/src/profitpulse/services/close_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/close_account_test.py` & `profitpulse-1.5.0/src/profitpulse/services/close_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/delete_account.py` & `profitpulse-1.5.0/src/profitpulse/services/delete_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/delete_account_test.py` & `profitpulse-1.5.0/src/profitpulse/services/delete_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/deposit_into_account.py` & `profitpulse-1.5.0/src/profitpulse/services/deposit_into_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/deposit_into_account_test.py` & `profitpulse-1.5.0/src/profitpulse/services/deposit_into_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/import_transactions.py` & `profitpulse-1.5.0/src/profitpulse/services/import_transactions.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/import_transactions_test.py` & `profitpulse-1.5.0/src/profitpulse/services/import_transactions_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/open_account.py` & `profitpulse-1.5.0/src/profitpulse/services/open_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/open_account_test.py` & `profitpulse-1.5.0/src/profitpulse/services/open_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/services/snapshot_account.py` & `profitpulse-1.5.0/src/profitpulse/services/revalue.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.money import Money
 from profitpulse.services.errors import AccountNotFoundError
 
 
-class SnapshotAccountRequester(abc.ABC):
+class RevalueAccountRequester(abc.ABC):
     @property
     @abc.abstractmethod
     def account_name(self) -> AccountName: ...  # pragma: no cover
 
     @property
     @abc.abstractmethod
     def value(self) -> Money: ...  # pragma: no cover
 
 
-class SnapshotAccountAccountCollector(abc.ABC):
+class RevalueAccountAccountCollector(abc.ABC):
     @abc.abstractmethod
     def __getitem__(self, account_name: AccountName) -> Account: ...  # pragma: no cover
 
     @abc.abstractmethod
     def __setitem__(
         self, account_name: AccountName, account: Account
     ) -> None: ...  # pragma: no cover
 
 
-class SnapshotAccountService:
-    def __init__(self, accounts: SnapshotAccountAccountCollector):
+class RevalueAccountService:
+    def __init__(self, accounts: RevalueAccountAccountCollector):
         self.accounts = accounts
 
-    def execute(self, request: SnapshotAccountRequester) -> None:
+    def execute(self, request: RevalueAccountRequester) -> None:
         try:
             account = self.accounts[request.account_name]
         except KeyError:
             raise AccountNotFoundError(request.account_name)
 
-        account.snapshot(request.value)
+        account.revalue(request.value)
 
         self.accounts[request.account_name] = account
```

### Comparing `profitpulse-1.4.1/src/profitpulse/services/snapshot_account_test.py` & `profitpulse-1.5.0/src/profitpulse/services/revalue_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 import pytest
 
 from profitpulse.lib.account import Account
 from profitpulse.lib.account_name import AccountName
 from profitpulse.lib.money import Money
-from profitpulse.services.snapshot_account import (
+from profitpulse.services.revalue import (
     AccountNotFoundError,
-    SnapshotAccountAccountCollector,
-    SnapshotAccountRequester,
-    SnapshotAccountService,
+    RevalueAccountAccountCollector,
+    RevalueAccountRequester,
+    RevalueAccountService,
 )
 
 
-class SnapshotAccountRequest(SnapshotAccountRequester):
+class RevalueAccountRequest(RevalueAccountRequester):
     def __init__(self, account_name: str, value: int):
         self._account_name = AccountName(account_name)
         self._value = value
 
     @property
     def value(self) -> Money:
         return Money(self._value)
 
     @property
     def account_name(self) -> AccountName:
         return self._account_name
 
 
-class Accounts(SnapshotAccountAccountCollector):
+class Accounts(RevalueAccountAccountCollector):
     def __init__(self, account: Account) -> None:
         self.account = account
 
     def __getitem__(self, account_name: AccountName) -> Account:
         return self.account
 
     def __setitem__(self, account_name: AccountName, account: Account) -> None:
         self.account = account
 
 
 def test_return_error_when_account_does_not_exist() -> None:
     account_name = "TheAccountName"
-    request = SnapshotAccountRequest(account_name, 0)
+    request = RevalueAccountRequest(account_name, 0)
 
-    service = SnapshotAccountService(dict())  # type: ignore
+    service = RevalueAccountService(dict())  # type: ignore
 
     with pytest.raises(
         AccountNotFoundError,
         match=f"Could not find an account with name '{account_name}'",
     ):
         service.execute(request)
 
 
-def test_snapshot_account() -> None:
+def test_revalue_account() -> None:
     account_name = "TheAccountName"
     accounts = Accounts(Account(account_name=AccountName(account_name)))
 
-    request = SnapshotAccountRequest(account_name, 1)
-    service = SnapshotAccountService(accounts)
+    request = RevalueAccountRequest(account_name, 1)
+    service = RevalueAccountService(accounts)
 
     service.execute(request)
 
     assert accounts.account.balance == Money(1)  # nosec
```

### Comparing `profitpulse-1.4.1/src/profitpulse/testrig/fixtures.py` & `profitpulse-1.5.0/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.4.1/src/profitpulse/testrig/scenario.py` & `profitpulse-1.5.0/src/profitpulse/testrig/scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from profitpulse.cli.main import profitpulse_app
 
 runner = CliRunner(mix_stderr=False)
 
 
 class CLIScenario:
     """
-    Builds scenarios up on the tests can be run.
+    Builds scenarios up on the tests can be run and evaluates the result taking
+    the context (CLI) into account.
     """
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}"
 
     def __init__(self, *_, **__) -> None:
         self._app = profitpulse_app
@@ -38,18 +39,15 @@
         """
 
         result = runner.invoke(
             self._app, ["accounts", "open", account_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
 
-    def close_account(self, account_name: str) -> None:
-        """
-        Closes an account.
-        """
+    def divest(self, account_name: str) -> None:
         result = runner.invoke(
             self._app, ["accounts", "close", account_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
         assert result.stdout == "", result.stdout  # nosec
 
     def delete_account(self, account_name: str) -> None:
@@ -88,17 +86,17 @@
             catch_exceptions=False,
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     # Reports ----------------------------------------------------------------------------------------------------------
 
-    def snapshot(self, amount: int, account_name: str):
+    def revalue(self, amount: int, account_name: str):
         result = runner.invoke(
-            self._app, ["snapshot", str(amount), account_name], catch_exceptions=False
+            self._app, ["revalue", str(amount), account_name], catch_exceptions=False
         )
         assert result.exit_code == 0, result.stderr  # nosec
         return result.stdout
 
     def pulse(self):
         """
         Shows a global view of the user finances.
```

### Comparing `profitpulse-1.4.1/PKG-INFO` & `profitpulse-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 1.4.1
+Version: 1.5.0
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
```

