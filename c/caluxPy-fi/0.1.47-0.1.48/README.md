# Comparing `tmp/caluxpy_fi-0.1.47.tar.gz` & `tmp/caluxpy_fi-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxpy_fi-0.1.47.tar", last modified: Mon May  6 14:58:45 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.48.tar", last modified: Mon May  6 18:24:50 2024, max compression
```

## Comparing `caluxpy_fi-0.1.47.tar` & `caluxpy_fi-0.1.48.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.980372 caluxpy_fi-0.1.47/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.47/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-05-06 14:58:45.980372 caluxpy_fi-0.1.47/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.47/README.md
--rw-rw-rw-   0        0        0      824 2024-05-06 14:52:54.000000 caluxpy_fi-0.1.47/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 14:58:45.996000 caluxpy_fi-0.1.47/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.870025 caluxpy_fi-0.1.47/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.965369 caluxpy_fi-0.1.47/src/caluxPy_fi/
--rw-rw-rw-   0        0        0     9878 2024-05-06 14:30:18.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.47/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:58:45.980372 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 14:58:45.000000 caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 18:24:50.834071 caluxpy_fi-0.1.48/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.48/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-05-06 18:24:50.819068 caluxpy_fi-0.1.48/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.48/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-06 18:22:23.000000 caluxpy_fi-0.1.48/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:24:50.834071 caluxpy_fi-0.1.48/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 18:24:50.771753 caluxpy_fi-0.1.48/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 18:24:50.819068 caluxpy_fi-0.1.48/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0     9865 2024-05-06 18:22:18.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.48/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:24:50.819068 caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-05-06 18:24:50.000000 caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-05-06 18:24:50.000000 caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:24:50.000000 caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-06 18:24:50.000000 caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 18:24:50.000000 caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxpy_fi-0.1.47/LICENSE.txt` & `caluxpy_fi-0.1.48/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/PKG-INFO` & `caluxpy_fi-0.1.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.47
+Version: 0.1.48
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.47/README.md` & `caluxpy_fi-0.1.48/README.md`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/pyproject.toml` & `caluxpy_fi-0.1.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.47"
+version = "0.1.48"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/Convexity.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/Convexity.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,37 +57,37 @@
                                              periodicity = periodicity, 
                                              coupon_flow = coupon_flow, 
                                              payment_type = payment_type, 
                                              issuer = issuer, 
                                              notional_value = notional_value, 
                                              gained_coupon = gained_coupon)
             # Creating lists lists for the table
-            listPBS.append(y) #list of basis points
-            listDirtyPrice.append(resValuation[1] * 100) # list of dirty prices
-            y += 1 # marginal increase
+            listPBS.append(y) # List of basis points
+            listDirtyPrice.append(resValuation[1] * 100) # List of dirty prices
+            y += 1 # Marginal increase
         
-        # conversion of lists into numpy arrays for ease of use
+        # Conversion of lists into numpy arrays for ease of use
         listPBS = np.array(listPBS)
         listDirtyPrice = np.array(listDirtyPrice)
         
         # Creation of DataFrame
         self.df_convex = pd.DataFrame({'pbs': listPBS, 'Price': listDirtyPrice})
         
         # Treatment of the negatives in the df
         negatives = self.df_convex[self.df_convex['pbs'] <= 0].copy() # Copy the DataFrame for ease of use
         negatives.sort_values(by = 'pbs', ascending = False, inplace = True) # Sort descending
-        negatives['dv01'] = negatives['Precio Sucio'].diff().fillna(0) * 10000 # Calculate the difference and fill first with 0
+        negatives['dv01'] = negatives['Price'].diff().fillna(0) * 10000 # Calculate the difference and fill first with 0
         negatives['accum'] = negatives['dv01'].cumsum() # Perform Cummulative Sum
         negatives.sort_values(by = 'pbs', ascending = True, inplace = True) # Sort Ascending
         first_neg = negatives.iloc[-2]['dv01'] # Get the first negative (the one after 0)
         
         # Treatment of the positives in the df
         positives = self.df_convex[self.df_convex['pbs'] >= 0].copy() # Copy the DataFrame for ease of use
         positives.sort_values(by = 'pbs', ascending = True, inplace = True) # Sort Ascending
-        positives['dv01'] = positives['Precio Sucio'].diff().fillna(0) * -10000 # Calculate the difference and fill first with 0
+        positives['dv01'] = positives['Price'].diff().fillna(0) * -10000 # Calculate the difference and fill first with 0
         positives['accum'] = positives['dv01'].cumsum() # Perform Cummulative Sum
         first_pos = positives.iloc[1]['dv01'] # Get the first positive (the one after 0)
         
         # Getting the average
         self.avg_dv01 = (first_neg + first_pos) / 2 # Get an averaged dv01 with the first occurrence of a marginal increase, because it can go both ways
         
         #Concatenating the dfs to form the complete one
```

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/ExternalImport.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/ExternalImport2.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/FixedIncome.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/Multiple.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.48/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.47/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.48/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.47
+Version: 0.1.48
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

