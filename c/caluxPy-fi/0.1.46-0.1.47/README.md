# Comparing `tmp/caluxpy_fi-0.1.46.tar.gz` & `tmp/caluxpy_fi-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxpy_fi-0.1.46.tar", last modified: Fri May  3 21:09:27 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.47.tar", last modified: Mon May  6 14:58:45 2024, max compression
```

## Comparing `caluxpy_fi-0.1.46.tar` & `caluxpy_fi-0.1.47.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.518279 caluxpy_fi-0.1.46/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.46/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-05-03 21:09:27.518279 caluxpy_fi-0.1.46/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.46/README.md
--rw-rw-rw-   0        0        0      824 2024-05-03 21:05:47.000000 caluxpy_fi-0.1.46/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 21:09:27.518279 caluxpy_fi-0.1.46/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.345389 caluxpy_fi-0.1.46/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.487545 caluxpy_fi-0.1.46/src/caluxPy_fi/
--rw-rw-rw-   0        0        0    16591 2024-05-03 21:05:13.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-04-30 15:52:50.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4225 2024-03-18 22:03:06.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10561 2024-03-19 16:45:38.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    56544 2024-05-02 13:32:57.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5926 2024-03-21 21:15:39.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-03-14 14:13:38.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0     5887 2024-03-14 13:56:00.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/UserInputs.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.46/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:09:27.509772 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 21:09:27.000000 caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.980372 caluxpy_fi-0.1.47/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.47/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-05-06 14:58:45.980372 caluxpy_fi-0.1.47/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.47/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-06 14:52:54.000000 caluxpy_fi-0.1.47/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 14:58:45.996000 caluxpy_fi-0.1.47/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.870025 caluxpy_fi-0.1.47/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.965369 caluxpy_fi-0.1.47/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0     9878 2024-05-06 14:30:18.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.980372 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxpy_fi-0.1.46/LICENSE.txt` & `caluxpy_fi-0.1.47/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.46/PKG-INFO` & `caluxpy_fi-0.1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.46
+Version: 0.1.47
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.46/README.md` & `caluxpy_fi-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.46/pyproject.toml` & `caluxpy_fi-0.1.47/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.46"
+version = "0.1.47"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,14 @@
     def __del__(self):
         # Ensure the logging handlers are properly closed
         handlers = self.logger.handlers[:]
         for handler in handlers:
             handler.close()
             self.logger.removeHandler(handler)         
         
-        
-
     def getResults(self):
 
         return self.importedData
 
     def processTime(self):
 
         return self.tiempo_calculo
```

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import openpyxl, pandas as pd, numpy as np, datetime, sys, time, os, logging
+#import openpyxl, numpy as np, os
+import pandas as pd, datetime, sys, time, logging
 from collections import Counter
 from caluxPy_fi.Support import Support
 
 class ExternalImport:
     
     def __init__(self, file = '', df = '', file_type = '', initial_row = 0, columns = ''):#, repos = False, repos_attributes = [], medida = False):
         self.file = file
```

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/FixedIncome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+#from tkinter import messagebox
 import numpy as np, pandas as pd, math, time, logging
 from datetime import date, datetime
 from dateutil.relativedelta import relativedelta
-from tkinter import messagebox
 from caluxPy_fi.Support import Support
 
 class FixedIncome:
-
-    #counter = 0
     
     def __init__(self, settlement_date, issuance_date, maturity_date, coupon, ytm, face_value, issuer, methodology, periodicity, payment_type, coupon_type, 
                  forward_date, amortization_start_date, amortization_periods, amortization_periodicity, amortizable_percentage, **kwargs):
         
         self.repo_margin = kwargs['repo_margin'] if 'repo_margin' in kwargs else ''
         self.repo_rate = kwargs['repo_rate'] if 'repo_rate' in kwargs else ''
         self.repo_tenure = kwargs['repo_tenure'] if 'repo_tenure' in kwargs else ''
@@ -328,18 +326,15 @@
 
                 except Exception as e:
                     self._logger.error(f'Error calculating flr => {e}')
                     
                 self._logger.info('SUCCESS: Results ready! Preparing the visualization..')
 
                 values = {}
-                est_flujos_exp = []
-                flujos_exp = []
-                present_values_export = []
-                accumulated_days_export = []
+                est_flujos_exp, flujos_exp, present_values_export, accumulated_days_export = [], [], [], []
 
                 days = 0
                 for i in range(len(self.flow_num)):
                     days += self.coupon_days[i]
                     accumulated_days_export.append(days)
                     if i < self.current_coupon:
                         est_flujos_exp.append('Vencido' if self._lang == 'esp' else 'Matured')
@@ -368,34 +363,14 @@
             self._logger.error('Título Vencido..' if self._lang == 'esp' else 'Matured Security..')
             self.results['status'] = 'Vencido' if self._lang == 'esp' else 'Matured'
             self._logger.error('Process cancelled because of an error')
         finally:
             self._logger.removeHandler(_fileHandler)
             _fileHandler.close()
     
-    def amortizationDateValidation(self, coupon_dates, amortization_start_date, maturity_date, amortization_periods, amortization_periodicity):
-        
-        if (amortization_start_date in coupon_dates) == False:
-            oldDate = amortization_start_date
-            amortization_start_date = Support.closestDate(coupon_dates, amortization_start_date)
-            prompt = '\n*ERROR! \nLa fecha de inicio de amortizaciones indicada no existe en los flujos de cupones, el programa procederá a buscar el cupon vigente más cercano.. ' + \
-            '\n-Fecha Original: ' + str(oldDate.day) + '/' + str(oldDate.month) + '/' + str(oldDate.year) + \
-            '\n-Fecha Nueva: ' + str(amortization_start_date.day) + '/' + str(amortization_start_date.month) + '/' + str(amortization_start_date.year)
-            print(prompt , file = self.log)
-            messagebox.showwarning('ValueError', prompt)
-        fechaTest = amortization_start_date + relativedelta(months =+ ((amortization_periods - 1) * amortization_periodicity))
-        if fechaTest > maturity_date:
-            prompt = '\n*ERROR! \nLa fecha estimada de última amortización supera la fecha de vencimiento!' + \
-                 '\n-Fecha de Vencimiento: ' + str(maturity_date.day) + '/' + str(maturity_date.month) + '/' + str(maturity_date.year) + \
-                 '\n-Fecha estimada: ' + str(fechaTest.day) + '/' + str(fechaTest.month) + '/' + str(fechaTest.year)
-            print(prompt, file = self.log)
-            messagebox.showerror('ValueError', prompt)
-            return amortization_start_date, False
-        else: return amortization_start_date, True
-
     def expectedMaturity(self, maturity_date, issuance_date, years_to_maturity, nper):
         def check_months(maturity, issuance, nper):
             if maturity.month - issuance.month < 0:
                 return maturity.month - issuance.month + nper
             elif maturity.month - issuance.month > 0:
                 return maturity.month - issuance.month - nper
         #Determination of the expected maturity date
@@ -477,62 +452,22 @@
         return days_to_maturity
 
     def calculationBasis(self, methodology, nper, coupon_dates): 
         #Determination of the calculation basis
         calculation_basis = []
         i = 0
         while i <= nper:
-            if (methodology == 'actual/365'):
-                calculation_basis.append(365)
-            elif (methodology in ['actual/360', 'isma-30-360']):
-                calculation_basis.append(360)
-            else:
-                calculation_basis.append((coupon_dates[i] - (coupon_dates[i] - relativedelta(months=+12))).days)
+            if (methodology == 'actual/365'): calculation_basis.append(365)
+            elif (methodology in ['actual/360', 'isma-30-360']): calculation_basis.append(360)
+            else: calculation_basis.append((coupon_dates[i] - (coupon_dates[i] - relativedelta(months=+12))).days)
             i += 1
         return calculation_basis
 
-    #This module executes all calculations related to amortization including validations (should be included more validations and user inputs through streamlit)
     def amortizationModule(self, payment_type, amortization_start_date, maturity_date, amortization_periods, amortization_periodicity, amortizable_percentage, 
                            settlement_date, face_value, coupon_dates, current_coupon, nper, periodicity):
-        #First this runs validations
-        while True:
-            amortization_start_date, validation = self.amortizationDateValidation(coupon_dates, amortization_start_date, maturity_date, amortization_periods, amortization_periodicity)
-            if validation == False:
-                while True:
-                    seleccion = input('\nQue desea modificar para solucionar el error? ' + 
-                              '\n1-Fecha de Inicio de las Amortizaciones' + 
-                              '\n2-Periodicidad de las Amortizaciones' + 
-                              '\n3-Cantidad de Amortizaciones' + 
-                              '\nRespuesta: ')
-                    if seleccion in ['1','2','3']:
-                        if seleccion == '1': 
-                            amortization_start_date = self.inputFecha('Fecha de Inicio de Amotizaciones')
-                            break
-                        elif seleccion == '2':
-                            while True:
-                                amortization_periodicity = Support.periodicityConversion(self.inputPrompt('periodicidad de amortizaciones', ['mensual','m','1','bimensual','b','2','trimestral','t','3','cuatrimestral','c','4','semestral','s','5','anual','a','6'], 3), mode = 'amortization')
-                                if (amortization_periodicity == 12 / periodicity) or (amortization_periodicity == (12 / periodicity) * 2):
-                                    break
-                                else:
-                                    prompt = 'Valor inválido: la periodicidad de las amortizaciones debe de ser igual o el doble de la periodicidad de pagos de cupones..'
-                                    print(prompt, file = self.log)
-                                    messagebox.showerror('ValueError', prompt)
-                                    amortization_periodicity, 12 / periodicity
-                                    continue
-                            break
-                        elif seleccion == '3':
-                            amortization_periods = self.inputIntegers()
-                            break
-                    else:
-                        prompt = 'Opción inválida, inténtelo de nuevo..'
-                        print(prompt, file = self.log)
-                        messagebox.showerror('InputError', prompt)
-                        continue
-                continue
-            else: break
 
         #Determination of the dates in which the securities amortize
         amortization_amount = 0
         amortization_dates = []
         dates_results = []
         if (payment_type in ['amortized', 'amortizado', 'pik']):
             date_count = 0
@@ -580,33 +515,28 @@
             adjusted_value = np.array(adjusted_value)
 
         return notional_value, amortization_amount, adjusted_value, dates_results
 
     def gainedCoupon(self, methodology, notional_value, coupon, periodicity, coupon_days, current_coupon, accumulated_days, calculation_basis): 
         #Calculates the running coupon or gained interest
         gained_coupon = 0
-        if (methodology in ['icma']):
-            gained_coupon = (notional_value * coupon / periodicity) / coupon_days[current_coupon] * accumulated_days
-        elif (methodology in ['actual/actual', 'actual/365', 'actual/360']):
-            gained_coupon = notional_value * coupon / calculation_basis[current_coupon] * accumulated_days
-        elif (methodology in ['isma-30-360']):
-            gained_coupon = notional_value * coupon / 360 * accumulated_days
+        if (methodology in ['icma']): gained_coupon = (notional_value * coupon / periodicity) / coupon_days[current_coupon] * accumulated_days
+        elif (methodology in ['actual/actual', 'actual/365', 'actual/360']): gained_coupon = notional_value * coupon / calculation_basis[current_coupon] * accumulated_days
+        elif (methodology in ['isma-30-360']): gained_coupon = notional_value * coupon / 360 * accumulated_days
         return gained_coupon
 
     def bulletPaymentType(self, face_value, coupon, periodicity, nper, per, methodology, calculation_basis, coupon_days, current_coupon):
         coupon_flow = []
         i = current_coupon
         while i <= nper:
-            if (methodology in ['icma']):
-                coupon_flow.append((face_value * coupon) / periodicity)
-            elif (methodology in ['isma-30-360']):
-                coupon_flow.append((face_value * coupon) / 12 * per)
-            elif (methodology in ['actual/actual', 'actual/365', 'actual/360']):
-                coupon_flow.append(face_value * coupon / calculation_basis[i] * coupon_days[i])
-            if i == nper:
+            if (methodology in ['icma']): coupon_flow.append((face_value * coupon) / periodicity)
+            elif (methodology in ['isma-30-360']): coupon_flow.append((face_value * coupon) / 12 * per)
+            elif (methodology in ['actual/actual', 'actual/365', 'actual/360']): coupon_flow.append(face_value * coupon / calculation_basis[i] * coupon_days[i])
+            
+            if i == nper: 
                 coupon_flow[int(nper - current_coupon)] = face_value + coupon_flow[int(nper - current_coupon)]
             i += 1
         return coupon_flow
     
     def amortizedPaymentType(self, methodology, current_coupon, dates_results, adjusted_value, coupon, periodicity, amortization_amount, calculation_basis, coupon_days, amortizable_percentage, nper, per):
         i = current_coupon
         coupon_flow = []
@@ -669,15 +599,15 @@
                 else:
                     coupon_flow.append(coupon_flow[x - 1] * coupon / calculation_basis[i] * coupon_days[i])
             x += 1
             i += 1
         return coupon_flow
 
     def presentValue(self, current_coupon, nper, w_coupon, discrepancy, coupon_type, maturity_date, expected_maturity, coupon_days, ytm, periodicity, 
-                             coupon_flow, payment_type, issuer, notional_value, gained_coupon): 
+                     coupon_flow, payment_type, issuer, notional_value, gained_coupon): 
         #Calculation of the present value of the coupon payments
         fraction, factor = 0, 0
         preliminar_present_value, final_present_value = 0, 0
         clean_price, dirty_price, purchase_value = 0, 0, 0
         present_values, present_values_factor, values_cvx = [], [], []
         i = current_coupon
         while i <= nper:
@@ -727,38 +657,24 @@
         modified_duration = duration / (1 + (ytm / periodicity))
         dv01 = dirty_price * (modified_duration / 100) * notional_value / 100
         convexity = np.sum(values_cvx) / (1 + (ytm / periodicity)) ** 2 / preliminar_present_value / periodicity ** 2
         return final_present_value, dirty_price, purchase_value, clean_price, duration, modified_duration, dv01, convexity, preliminar_present_value, present_values
 
     def Repos(self, margin, repo_rate, repo_tenure):
         count = -1
-        gained_coupon = 0
         flow_dates = {}
-        error = 0
-        
         settlement_date = self.settlement_date
-        one_way_value, return_value = 0, 0
-        if self._lang == 'eng':
-            try:
-                if self.multiple:
-                    present_value = self.results['Preliminar Present Value']
-                else:
-                    present_value = self.results['preliminar_present_value']
-            except Exception:
-                error += 1
-                
-        elif self._lang == 'esp':
-            try:
-                if self.multiple:
-                    present_value = self.results['Valor Presente Preliminar']
-                else:
-                    present_value = self.results['valor_presente_preliminar']
-            except Exception:
-                error += 1
-
+        gained_coupon, one_way_value, return_value, error = 0, 0, 0, 0
+        
+        try:
+            if self.multiple: present_value = self.results['Preliminar Present Value' if self._lang == 'eng' else 'Valor Presente Preliminar']
+            else: present_value = self.results['preliminar_present_value' if self._lang == 'eng' else 'valor_presente_preliminar']
+        except Exception:
+            error += 1
+                
         if error > 0: return None, None
         
         coupon_dates = self.coupon_dates
         coupon_flows = self.coupon_flow
         repo_maturity = settlement_date + relativedelta(days =+ repo_tenure)
         if repo_maturity >= self.maturity_date:
             prompt = 'ERROR: Security matures before the repo..'
@@ -766,20 +682,18 @@
 
         for date in coupon_dates:
             if date > settlement_date:
                 count += 1
                 flow_dates[date] = coupon_flows[count]
 
         for key, value in flow_dates.items():
-            if key == repo_maturity:
-                flow_dates[key] = value - self.notional_value
+            if key == repo_maturity: flow_dates[key] = value - self.notional_value
         
         for date in coupon_dates:
-            if date > settlement_date and date < repo_maturity:
-                gained_coupon += flow_dates[date]
+            if date > settlement_date and date < repo_maturity: gained_coupon += flow_dates[date]
 
         adjusted_present_value = present_value - gained_coupon
         one_way_value = adjusted_present_value * ( 1 - margin)
         return_value = one_way_value * (1 + repo_rate / 365 * repo_tenure)
 
         return one_way_value, return_value
 
@@ -894,15 +808,14 @@
 Valor Presente Preliminar: {self.results['valor_presente_preliminar']}\n \
 Tiempo de Cálculo: {self.results['tiempo_calculo']}\n')
                 else:
                     return f'Título vencido por: {self.maturity_date - self.settlement_date} días'
         except Exception:
             return f'Security error!'
 
-
 class Letras:
     def __init__(self, settlement_date, maturity_date, ytm, face_value, repo_margin = '', repo_rate = '', repo_tenure = '', date_format = '', multiple = False) -> None:
         self.settlement_date = settlement_date
         self.maturity_date = maturity_date
         self.ytm = ytm
         self.face_value = face_value
         self.repo_margin = repo_margin
@@ -910,8 +823,122 @@
         self.repo_tenure = repo_tenure
         self.date_format = date_format
         self.multiple = multiple
 
         self.days_to_maturity = self.maturity_date - self.settlement_date
         self.price = 360 / (360 + self.ytm * self.days_to_maturity)
         self.purchase_value = self.face_value * self.price
-        self.discount = self.face_value - self.purchase_value
+        self.discount = self.face_value - self.purchase_value
+
+class FiBackup:
+    pass
+
+    '''def amortizationDateValidation(self, coupon_dates, amortization_start_date, maturity_date, amortization_periods, amortization_periodicity):
+        
+        if (amortization_start_date in coupon_dates) == False:
+            oldDate = amortization_start_date
+            amortization_start_date = Support.closestDate(coupon_dates, amortization_start_date)
+            prompt = '\n*ERROR! \nLa fecha de inicio de amortizaciones indicada no existe en los flujos de cupones, el programa procederá a buscar el cupon vigente más cercano.. ' + \
+            '\n-Fecha Original: ' + str(oldDate.day) + '/' + str(oldDate.month) + '/' + str(oldDate.year) + \
+            '\n-Fecha Nueva: ' + str(amortization_start_date.day) + '/' + str(amortization_start_date.month) + '/' + str(amortization_start_date.year)
+            print(prompt , file = self.log)
+            messagebox.showwarning('ValueError', prompt)
+        fechaTest = amortization_start_date + relativedelta(months =+ ((amortization_periods - 1) * amortization_periodicity))
+        if fechaTest > maturity_date:
+            prompt = '\n*ERROR! \nLa fecha estimada de última amortización supera la fecha de vencimiento!' + \
+                 '\n-Fecha de Vencimiento: ' + str(maturity_date.day) + '/' + str(maturity_date.month) + '/' + str(maturity_date.year) + \
+                 '\n-Fecha estimada: ' + str(fechaTest.day) + '/' + str(fechaTest.month) + '/' + str(fechaTest.year)
+            print(prompt, file = self.log)
+            messagebox.showerror('ValueError', prompt)
+            return amortization_start_date, False
+        else: return amortization_start_date, True'''
+        
+    '''#This module executes all calculations related to amortization including validations (should be included more validations and user inputs through streamlit)
+    def amortizationModule(self, payment_type, amortization_start_date, maturity_date, amortization_periods, amortization_periodicity, amortizable_percentage, 
+                           settlement_date, face_value, coupon_dates, current_coupon, nper, periodicity):
+        #First this runs validations
+        while True:
+            amortization_start_date, validation = self.amortizationDateValidation(coupon_dates, amortization_start_date, maturity_date, amortization_periods, amortization_periodicity)
+            if validation == False:
+                while True:
+                    seleccion = input('\nQue desea modificar para solucionar el error? ' + 
+                              '\n1-Fecha de Inicio de las Amortizaciones' + 
+                              '\n2-Periodicidad de las Amortizaciones' + 
+                              '\n3-Cantidad de Amortizaciones' + 
+                              '\nRespuesta: ')
+                    if seleccion in ['1','2','3']:
+                        if seleccion == '1': 
+                            amortization_start_date = self.inputFecha('Fecha de Inicio de Amotizaciones')
+                            break
+                        elif seleccion == '2':
+                            while True:
+                                amortization_periodicity = Support.periodicityConversion(self.inputPrompt('periodicidad de amortizaciones', ['mensual','m','1','bimensual','b','2','trimestral','t','3','cuatrimestral','c','4','semestral','s','5','anual','a','6'], 3), mode = 'amortization')
+                                if (amortization_periodicity == 12 / periodicity) or (amortization_periodicity == (12 / periodicity) * 2):
+                                    break
+                                else:
+                                    prompt = 'Valor inválido: la periodicidad de las amortizaciones debe de ser igual o el doble de la periodicidad de pagos de cupones..'
+                                    print(prompt, file = self.log)
+                                    messagebox.showerror('ValueError', prompt)
+                                    amortization_periodicity, 12 / periodicity
+                                    continue
+                            break
+                        elif seleccion == '3':
+                            amortization_periods = self.inputIntegers()
+                            break
+                    else:
+                        prompt = 'Opción inválida, inténtelo de nuevo..'
+                        print(prompt, file = self.log)
+                        messagebox.showerror('InputError', prompt)
+                        continue
+                continue
+            else: break
+
+        #Determination of the dates in which the securities amortize
+        amortization_amount = 0
+        amortization_dates = []
+        dates_results = []
+        if (payment_type in ['amortized', 'amortizado', 'pik']):
+            date_count = 0
+            if amortization_start_date < settlement_date:
+                date_count = 1
+            i = 0
+            while i <= int(amortization_periods) - 1:
+                if i == 0:
+                    amortization_dates.append(amortization_start_date)
+                else:
+                    amortization_dates.append(amortization_dates[i - 1] + relativedelta(months=+amortization_periodicity))
+                    if amortization_dates[i] <= settlement_date:
+                        date_count += 1
+                i += 1
+            amortization_dates = np.array(amortization_dates)
+            i = 0
+            posicion = 0
+            while i <= np.count_nonzero(amortization_dates) - 1:
+                posicion = np.where(coupon_dates == amortization_dates[i])[0]
+                if posicion != 0: dates_results.append(posicion)
+                i += 1
+            amortization_amount = (face_value * amortizable_percentage) / amortization_periods
+            dates_results = np.array(dates_results)
+        #Calculating the Notional Value and the Adjusted Amounts
+        previously_amortized = 0
+        notional_value = 0
+        adjusted_value = []
+        if (payment_type in ['amortized', 'amortizado']):
+            if amortization_periods > 0:
+                if np.count_nonzero(dates_results) != date_count:
+                    previously_amortized = amortization_amount * date_count
+                notional_value = face_value - previously_amortized
+            count = 0
+            i = current_coupon
+            while i <= nper:
+                if np.where(dates_results == i)[0].size > 0:
+                    count += 1
+                    if count <= (amortization_periods - (amortization_periods - np.count_nonzero(dates_results))):
+                        adjusted_value.append(notional_value - (amortization_amount * (count - 1)))
+                    else:
+                        adjusted_value.append(face_value)
+                else:
+                    adjusted_value.append(notional_value - (amortization_amount * count))
+                i += 1
+            adjusted_value = np.array(adjusted_value)
+
+        return notional_value, amortization_amount, adjusted_value, dates_results'''
```

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/Multiple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pandas as pd, time, os, logging, sys
-from pathlib import Path
+#import sys, os
+#from pathlib import Path
 #sys.path.append(str(Path(__file__).resolve().parent.parent))
+import pandas as pd, time, logging
 from caluxPy_fi.FixedIncome import FixedIncome
 from caluxPy_fi.Support import Support
 
 class Multiple:
 
     def __init__(self, data: pd.DataFrame, additional_ops: dict = {}, lang = 'eng'):
 
@@ -76,27 +77,21 @@
                                       repo_rate = repo_rate,
                                       repo_tenure = repo_tenure,
                                       flr_rules = rules,
                                       flr_ratio = ratio,
                                       lang = lang)
             calculador_results = fi_instance.get_results()
             self.mResults.append(calculador_results)
-            if lang == 'eng':
-                _logger.info(f'Calculated - {i + 1} of {len(data)}')
-            elif lang == 'esp':
-                _logger.info(f'Calculados - {i + 1} de {len(data)}')
+            _logger.info(f'Calculated - {i + 1} of {len(data)}' if lang == 'eng' else f'Calculados - {i + 1} de {len(data)}')
             i += 1
 
         self.df_resultados_multiples = pd.DataFrame(self.mResults)
         self.end_time = time.perf_counter()
         self.process_time = self.end_time - self.start_time
-        if lang == 'eng':
-            _logger.info(f'{self.process_time} segs')
-        elif lang == 'esp':
-            _logger.info(f'{self.process_time} secs')
+        _logger.info(f'{self.process_time} {'secs' if lang == 'eng' else 'segs'}')
         _logger.removeHandler(fileHandler)
         fileHandler.close()
 
     def get_results(self):
 
         return self.mResults
```

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.47/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.46/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.46
+Version: 0.1.47
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

