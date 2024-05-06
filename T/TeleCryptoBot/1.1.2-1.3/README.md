# Comparing `tmp/TeleCryptoBot-1.1.2.tar.gz` & `tmp/TeleCryptoBot-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TeleCryptoBot-1.1.2.tar", last modified: Sun Mar 24 13:58:44 2024, max compression
+gzip compressed data, was "TeleCryptoBot-1.3.tar", last modified: Mon May  6 09:12:15 2024, max compression
```

## Comparing `TeleCryptoBot-1.1.2.tar` & `TeleCryptoBot-1.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 13:58:44.071627 TeleCryptoBot-1.1.2/
--rw-rw-rw-   0        0        0       33 2024-03-23 22:08:01.000000 TeleCryptoBot-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1959 2024-03-24 13:58:44.071627 TeleCryptoBot-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1329 2024-03-24 13:58:35.000000 TeleCryptoBot-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 13:58:44.027753 TeleCryptoBot-1.1.2/TeleCryptoBot/
--rw-rw-rw-   0        0        0     8362 2024-03-24 13:41:24.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/__init__.py
--rw-rw-rw-   0        0        0      323 2024-03-23 20:40:45.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/app_stats.py
--rw-rw-rw-   0        0        0      178 2024-03-23 20:40:44.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/balance.py
--rw-rw-rw-   0        0        0      848 2024-03-23 20:38:08.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/base.py
--rw-rw-rw-   0        0        0      342 2024-03-23 21:34:41.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/check.py
--rw-rw-rw-   0        0        0      246 2024-03-23 20:40:42.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/currencies.py
--rw-rw-rw-   0        0        0      383 2024-03-24 13:25:57.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/exchange.py
--rw-rw-rw-   0        0        0     1263 2024-03-23 21:34:15.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/invoice.py
--rw-rw-rw-   0        0        0      135 2024-03-23 20:40:40.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/profile.py
--rw-rw-rw-   0        0        0      177 2024-03-23 20:40:39.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/rates.py
--rw-rw-rw-   0        0        0      884 2024-03-23 20:54:18.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/request.py
--rw-rw-rw-   0        0        0      341 2024-03-23 21:34:20.000000 TeleCryptoBot-1.1.2/TeleCryptoBot/transfer.py
-drwxrwxrwx   0        0        0        0 2024-03-24 13:58:44.066646 TeleCryptoBot-1.1.2/TeleCryptoBot.egg-info/
--rw-rw-rw-   0        0        0     1959 2024-03-24 13:58:43.000000 TeleCryptoBot-1.1.2/TeleCryptoBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-03-24 13:58:43.000000 TeleCryptoBot-1.1.2/TeleCryptoBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 13:58:43.000000 TeleCryptoBot-1.1.2/TeleCryptoBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-24 13:58:43.000000 TeleCryptoBot-1.1.2/TeleCryptoBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 13:58:44.073622 TeleCryptoBot-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      709 2024-03-24 13:58:25.000000 TeleCryptoBot-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:12:15.442111 TeleCryptoBot-1.3/
+-rw-rw-rw-   0        0        0       33 2024-03-23 22:08:01.000000 TeleCryptoBot-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1957 2024-05-06 09:12:15.444110 TeleCryptoBot-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2024-03-24 13:58:35.000000 TeleCryptoBot-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:12:15.327109 TeleCryptoBot-1.3/TeleCryptoBot/
+-rw-rw-rw-   0        0        0    10019 2024-03-29 00:34:29.000000 TeleCryptoBot-1.3/TeleCryptoBot/__init__.py
+-rw-rw-rw-   0        0        0      323 2024-03-23 20:40:45.000000 TeleCryptoBot-1.3/TeleCryptoBot/app_stats.py
+-rw-rw-rw-   0        0        0      178 2024-03-23 20:40:44.000000 TeleCryptoBot-1.3/TeleCryptoBot/balance.py
+-rw-rw-rw-   0        0        0      848 2024-03-23 20:38:08.000000 TeleCryptoBot-1.3/TeleCryptoBot/base.py
+-rw-rw-rw-   0        0        0      342 2024-03-27 18:56:57.000000 TeleCryptoBot-1.3/TeleCryptoBot/check.py
+-rw-rw-rw-   0        0        0      246 2024-03-23 20:40:42.000000 TeleCryptoBot-1.3/TeleCryptoBot/currencies.py
+-rw-rw-rw-   0        0        0      383 2024-03-27 18:56:53.000000 TeleCryptoBot-1.3/TeleCryptoBot/exchange.py
+-rw-rw-rw-   0        0        0     1263 2024-03-27 18:56:49.000000 TeleCryptoBot-1.3/TeleCryptoBot/invoice.py
+-rw-rw-rw-   0        0        0      135 2024-03-23 20:40:40.000000 TeleCryptoBot-1.3/TeleCryptoBot/profile.py
+-rw-rw-rw-   0        0        0      177 2024-03-23 20:40:39.000000 TeleCryptoBot-1.3/TeleCryptoBot/rates.py
+-rw-rw-rw-   0        0        0      590 2024-03-27 18:58:09.000000 TeleCryptoBot-1.3/TeleCryptoBot/request.py
+-rw-rw-rw-   0        0        0      121 2024-03-27 18:56:51.000000 TeleCryptoBot-1.3/TeleCryptoBot/test.py
+-rw-rw-rw-   0        0        0      341 2024-03-27 18:57:08.000000 TeleCryptoBot-1.3/TeleCryptoBot/transfer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:12:15.431113 TeleCryptoBot-1.3/TeleCryptoBot.egg-info/
+-rw-rw-rw-   0        0        0     1957 2024-05-06 09:12:14.000000 TeleCryptoBot-1.3/TeleCryptoBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-05-06 09:12:14.000000 TeleCryptoBot-1.3/TeleCryptoBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:12:14.000000 TeleCryptoBot-1.3/TeleCryptoBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-06 09:12:14.000000 TeleCryptoBot-1.3/TeleCryptoBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-06 09:12:14.000000 TeleCryptoBot-1.3/TeleCryptoBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:12:15.456112 TeleCryptoBot-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      767 2024-05-06 09:12:03.000000 TeleCryptoBot-1.3/setup.py
```

### Comparing `TeleCryptoBot-1.1.2/PKG-INFO` & `TeleCryptoBot-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TeleCryptoBot
-Version: 1.1.2
+Version: 1.3
 Summary: Библиотека для удобного использования API CryptoPay
 Home-page: https://github.com/vh1dz/TeleCryptoBot
 Author: vh1dz
 Author-email: vh1dz@vh1dz.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TeleCryptoBot-1.1.2/README.md` & `TeleCryptoBot-1.3/README.md`

 * *Files identical despite different names*

### Comparing `TeleCryptoBot-1.1.2/TeleCryptoBot/__init__.py` & `TeleCryptoBot-1.3/TeleCryptoBot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .base import (
     Assets,
     PaidButtons,
     InvoiceStatus,
     CurrencyType,
     CheckStatus,
 )
-
+from loguru import logger
 from .profile import Profile
 from .balance import Balance
 from .rates import ExchangeRate
 from .currencies import Currency
 from .invoice import Invoice
 from .transfer import Transfer
 from .check import Check
@@ -22,15 +22,19 @@
 class TeleCryptoBot:
 
     def __init__(self,key) -> None:
         self.apikey = key
 
     def getMe(self) -> Profile:
         response = RequestBody.req(self, key=self.apikey, method="getMe")
-        return Profile(**response["result"])
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return Profile(**response["result"])
 
     def createInvoice(
         self,
         amount: Union[int, float],
         asset: Optional[Union[Assets, str]] = None,
         description: Optional[str] = None,
         hidden_message: Optional[str] = None,
@@ -59,22 +63,30 @@
                 "allow_anonymous": allow_anonymous,
                 "expires_in": expires_in,
                 "fiat": fiat,
                 "currency_type": currency_type,
                 "accepted_assets": accepted_assets,
             }
             response = RequestBody.req(self, key=self.apikey, method="createInvoice", data=params)
-            return Invoice(**response["result"])
+            if isinstance(response, str):
+                logger.error(response)
+                return False
+            else:
+                return Invoice(**response["result"])
 
     def deleteInvoice(self,invoice_id: int) -> bool:
         params = {
             "invoice_id": invoice_id
         }
         response = RequestBody.req(self, key=self.apikey, method="deleteInvoice", data=params)
-        return response['result']
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return response['result']
 
     def createCheck(
         self,
         asset: Union[Assets, str],
         amount: Union[int, float],
         pin_to_user_id: Optional[int] = None,
         pin_to_username: Optional[str] = None,
@@ -89,15 +101,19 @@
         return Check(**response["result"])
 
     def deleteCheck(self, check_id: int) -> bool:
         params = {
             "check_id": check_id
         }
         response = RequestBody.req(self, key=self.apikey, method="deleteCheck", data=params)
-        return response["result"]
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return response["result"]
 
     def transfer(
         self,
         user_id: int,
         asset: Union[Assets, str],
         amount: Union[int, float],
         spend_id: Union[str, int],
@@ -109,15 +125,19 @@
             "asset": asset,
             "amount": amount,
             "spend_id": spend_id,
             "comment": comment,
             "disable_send_notification": disable_send_notification,
             }
         response = RequestBody.req(self, key=self.apikey, method="transfer", data=params)
-        return Transfer(**response["result"])
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return Transfer(**response["result"])
 
     def getInvoices(
         self,
         asset: Optional[Union[Assets, str]] = None,
         invoice_ids: Optional[Union[List[int], int]] = None,
         status: Optional[Union[InvoiceStatus, str]] = None,
         offset: Optional[int] = None,
@@ -129,18 +149,22 @@
             "asset": asset,
             "invoice_ids": invoice_ids,
             "status": status,
             "offset": offset,
             "count": count,
             }
         response = RequestBody.req(self, key=self.apikey, method="getInvoices", data=params)
-        if len(response["result"]["items"]) > 0:
-            if invoice_ids and isinstance(invoice_ids, int):
-                return Invoice(**response["result"]["items"][0])
-            return [Invoice(**invoice) for invoice in response["result"]["items"]]
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                if len(response["result"]["items"]) > 0:
+                    if invoice_ids and isinstance(invoice_ids, int):
+                        return Invoice(**response["result"]["items"][0])
+                return [Invoice(**invoice) for invoice in response["result"]["items"]]
 
     def getTransfers(
         self,
         asset: Optional[Union[Assets, str]] = None,
         transfer_ids: Optional[Union[List[int], int]] = None,
         offset: Optional[int] = None,
         count: Optional[int] = None,
@@ -150,18 +174,22 @@
         params = {
             "asset": asset,
             "transfer_ids": transfer_ids,
             "offset": offset,
             "count": count,
             }
         response = RequestBody.req(self, key=self.apikey, method="getTransfers", data=params)
-        if len(response["result"]["items"]) > 0:
-            if transfer_ids and isinstance(transfer_ids, int):
-                return Transfer(**response["result"]["items"][0])
-            return [Transfer(**transfer) for transfer in response["result"]["items"]]
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                if len(response["result"]["items"]) > 0:
+                    if transfer_ids and isinstance(transfer_ids, int):
+                        return Transfer(**response["result"]["items"][0])
+                return [Transfer(**transfer) for transfer in response["result"]["items"]]
 
     def getChecks(
         self,
         asset: Optional[Union[Assets, str]] = None,
         check_ids: Optional[Union[List[int], int]] = None,
         status: Optional[Union[CheckStatus, str]] = None,
         offset: Optional[int] = None,
@@ -173,41 +201,61 @@
             "asset": asset,
             "check_ids": check_ids,
             "status": status,
             "offset": offset,
             "count": count,
         }
         response = RequestBody.req(self, key=self.apikey, method="getChecks", data=params)
-        if len(response["result"]["items"]) > 0:
-            if check_ids and isinstance(check_ids, int):
-                return Check(**response["result"]["items"][0])
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+            if len(response["result"]["items"]) > 0:
+                if check_ids and isinstance(check_ids, int):
+                    return Check(**response["result"]["items"][0])
             return [Check(**check) for check in response["result"]["items"]]
     def getBalance(self)-> List[Balance]:
         response = RequestBody.req(self, key=self.apikey, method="getBalance")
-        return [Balance(**balance) for balance in response["result"]]
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return [Balance(**balance) for balance in response["result"]]
       
     def getExchangeRates(self) -> List[ExchangeRate]:
         response = RequestBody.req(self, key=self.apikey, method="getExchangeRates")
-        return [ExchangeRate(**rate) for rate in response["result"]]
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return [ExchangeRate(**rate) for rate in response["result"]]
 
     def getCurrencies(self) -> List[Currency]:
         response = RequestBody.req(self, key=self.apikey, method="getCurrencies")
-        return [Currency(**currency) for currency in response["result"]]
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return [Currency(**currency) for currency in response["result"]]
 
     def getStats(
         self,
         start_at: Optional[Union[datetime, str]] = None,
         end_at: Optional[Union[datetime, str]] = None,
     ) -> AppStats:
         params = {
             "start_at": start_at,
             "end_at": end_at
         }
         response = RequestBody.req(self, key=self.apikey, method="getStats", data=params)
-        return AppStats(**response["result"])
+        if isinstance(response, str):
+                logger.error(response)
+                return False
+        else:
+                return AppStats(**response["result"])
     def getAmountByFiat(
         self, summ: Union[int, float], asset: Union[Assets, str], target: str
     ) -> Union[int, float]:
         rates = self.getExchangeRates()
         rate = getRate(source=asset, target=target, rates=rates)
         fiatSumm = getRateSumm(summ=summ, rate=rate)
         return fiatSumm
```

### Comparing `TeleCryptoBot-1.1.2/TeleCryptoBot/base.py` & `TeleCryptoBot-1.3/TeleCryptoBot/base.py`

 * *Files identical despite different names*

### Comparing `TeleCryptoBot-1.1.2/TeleCryptoBot/invoice.py` & `TeleCryptoBot-1.3/TeleCryptoBot/invoice.py`

 * *Files identical despite different names*

### Comparing `TeleCryptoBot-1.1.2/TeleCryptoBot.egg-info/PKG-INFO` & `TeleCryptoBot-1.3/TeleCryptoBot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TeleCryptoBot
-Version: 1.1.2
+Version: 1.3
 Summary: Библиотека для удобного использования API CryptoPay
 Home-page: https://github.com/vh1dz/TeleCryptoBot
 Author: vh1dz
 Author-email: vh1dz@vh1dz.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TeleCryptoBot-1.1.2/setup.py` & `TeleCryptoBot-1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 try:
     description=pypandoc.convert('README.md', 'rst')
 except (IOError, ImportError):
     description=open('README.md').read()
 setup(
 	name='TeleCryptoBot',
-	version='1.1.2',
+	version='1.3',
 	author='vh1dz',
 	author_email='vh1dz@vh1dz.ru',
 	description='Библиотека для удобного использования API CryptoPay',
     long_description=description,
 	url='https://github.com/vh1dz/TeleCryptoBot',
 	packages=['TeleCryptoBot'],
+    install_requires=['pypandoc==1.5', 'pydantic>=2.3.0'],
 	include_package_data=True,
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
```

