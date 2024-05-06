# Comparing `tmp/tcia_utils-2.1.6.tar.gz` & `tmp/tcia_utils-2.1.7.tar.gz`

## Comparing `tcia_utils-2.1.6.tar` & `tcia_utils-2.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    87454 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/src/tcia_utils/utils.py
--rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/src/tcia_utils/wordpress.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/LICENSE
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tcia_utils-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    92926 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/src/tcia_utils/wordpress.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/LICENSE
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tcia_utils-2.1.7/PKG-INFO
```

### Comparing `tcia_utils-2.1.6/src/tcia_utils/datacite.py` & `tcia_utils-2.1.7/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/src/tcia_utils/nbia.py` & `tcia_utils-2.1.7/src/tcia_utils/nbia.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,15 +85,16 @@
                         "getSOPInstanceUIDs", "getSeriesMetaData", "getContentsByName",
                        "getImage", "getSingleImage", "getPatientByCollectionAndModality",
                        "NewPatientsInCollection", "NewStudiesInPatientCollection",
                        "getSeriesSize", "getUpdatedSeries"]
     advancedEndpoints = ["getModalityValuesAndCounts", "getBodyPartValuesAndCounts",
                          "getDicomTags", "getSeriesMetadata2", "getCollectionOrSeriesForDOI",
                          "getCollectionValuesAndCounts", "getCollectionDescriptions",
-                         "getSimpleSearchWithModalityAndBodyPartPaged", "getManufacturerValuesAndCounts"]
+                         "getSimpleSearchWithModalityAndBodyPartPaged", "getManufacturerValuesAndCounts",
+                         "getAdvancedQCSearch"]
 
     if not endpoint in searchEndpoints and not endpoint in advancedEndpoints:
         _log.error(
             f"Endpoint not supported by tcia_utils: {endpoint}\n"
             f'Valid "Search" endpoints include {searchEndpoints}\n'
             f'Valid "Advanced" endpoints include {advancedEndpoints}'
         )
@@ -321,15 +322,16 @@
             # format the output (optional)
             if format == "df":
                 df = pd.DataFrame(data)
                 return df
             elif format == "csv":
                 df = pd.DataFrame(data)
                 df.to_csv(endpoint + ".csv")
-                _log.info(f"CSV saved to: {endpoint}.csv")
+                df.to_csv(f"{endpoint}_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M')}.csv")
+                _log.info(f"CSV saved to: {endpoint}_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M')}.csv")
                 return df
             else:
                 return data
         else:
             _log.info("No results found.")
 
     # handle errors
@@ -1345,14 +1347,125 @@
     except requests.exceptions.ConnectionError as errc:
         _log.error(errc)
     except requests.exceptions.Timeout as errt:
         _log.error(errt)
     except requests.exceptions.RequestException as err:
         _log.error(err)
 
+
+def getAdvancedQCSearch(criteria_values, api_url = "", format = "", input_type = {}):
+    """
+    This function allows TCIA data curators to perform an advanced QC search.  
+    This function will not work for end users of TCIA.
+
+    Parameters:
+    - criteria_values (list of tuples): A list of tuples where each tuple contains a criteria type and its corresponding value.
+        - For example, [("patientID", "12345"), ("studyUID", "67890")].
+        - The criteria type can be one of the following: "collection", "qcstatus", "released", "batchnumber", "complete", "patientID", "submissiondate", "studyUID", "seriesUID", "studyDate", "seriesDesc", "modality", "manufacturer".
+        - The value depends on the criteria type and the input type. For "list" input type, it can be a single value or multiple values separated by commas. For "commaSeperatedList" input type, it should be a list of exact matches. For "contains" input type, it should be a substring to search for. For "dateRange" input type, it should be a date or a range of dates in the format "MM/DD/YYYY".
+    - api_url (str, optional): The base URL for the API. Defaults to an empty string.
+    - format (str, optional): The format of the response. Defaults to an empty string.
+    - override_input_type (dict, optional): A dictionary where keys are criteria types and values are the new input types. This allows the user to override the default input type for certain criteria types. Defaults to an empty dictionary.
+        - For example, {"patientID": "contains", "studyUID": "contains"}.
+
+    Returns:
+    - data: The response from the API call.
+    
+    Examples:
+    
+    1. Searching for all patient IDs that contain “LIDC”, have a modality of “CR” or “DX”, 
+    and a submission date between Feb 25, 2020 and Jan 1, 2023. Uses input_type to override
+    the default for patientID (comma separated list) to return anything that contains "LIDC".
+    
+        criteria_values = [("patientID", "LIDC"),
+                            ("modality", "CR,DX"), 
+                            ("submissiondate", "2/25/2020"), 
+                            ("submissiondate", "1/1/2023")]
+
+        input_type = {"patientID": "contains"}
+
+        getAdvancedQCSearch(criteria_values, input_type=input_type)
+
+    2. Searching for all data with collection “APOLLO-5-KIRP//UVA-Limited” or “APOLLO-5-LIHC//UVA-Limited” 
+    and qcstatus is either “Not Visible” or “Visible” with results formatted as a dataframe.
+    
+        criteria_values = [("collection", "APOLLO-5-KIRP//UVA-Limited"),
+                            ("collection", "APOLLO-5-LIHC//UVA-Limited"),
+                            ("qcstatus", "Not Visible"),
+                            ("qcstatus", "Visible")]
+
+        getAdvancedQCSearch(criteria_values, format = "df")
+
+    3. Searching for a list of UIDs with results formatted as a dataframe and saved to a CSV file.
+    
+        criteria_values = [("seriesUID", "1.3.6.1.4.1.14519.5.2.1.6279.6001.709632090821449989953075380984,1.3.6.1.4.1.14519.5.2.1.6279.6001.109097931021726413867023009234")]
+
+        getAdvancedQCSearch(criteria_values, format = "csv")
+    """
+    # Mapping between criteriaType and inputType
+    input_type_map = {
+        "qcstatus": "list",
+        "released": "list",
+        "batchnumber": "list",
+        "complete": "list",
+        "patientID": "commaSeperatedList",
+        "submissiondate": "dateRange",
+        "studyUID": "commaSeperatedList",
+        "seriesUID": "commaSeperatedList",
+        "studyDate": "dateRange",
+        "seriesDesc": "contains",
+        "modality": "list",
+        "manufacturer": "list"
+    }
+    
+    endpoint = "getAdvancedQCSearch"
+
+    # set base_url and headers
+    base_url = setApiUrl(endpoint, api_url)
+
+    params = {}
+    for i, (criteria, value) in enumerate(criteria_values):
+        params[f"criteriaType{i}"] = criteria
+        # Check if the criteria has an override input type
+        if criteria in input_type:
+            params[f"inputType{i}"] = input_type[criteria]
+        else:
+            params[f"inputType{i}"] = input_type_map[criteria]
+        params[f"boolean{i}"] = "AND"
+        params[f"value{i}"] = value
+    
+    # full url
+    url = base_url + endpoint
+    _log.info(f'Calling... {url}')
+    data = requests.post(url, headers=api_call_headers, data=params)
+
+    if data.status_code == 200:
+        # check for empty results and format output
+        if data.text != "":
+            data = data.json()
+            # format the output (optional)
+            if format == "df":
+                df = pd.DataFrame(data)
+                return df
+            elif format == "csv":
+                df = pd.DataFrame(data)
+                df.to_csv(endpoint + ".csv")
+                df.to_csv(f"{endpoint}_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M')}.csv")
+                _log.info(f"CSV saved to: {endpoint}_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M')}.csv")
+                return df
+            else:
+                return data
+        else:
+            _log.info("No results found.")
+    else:
+        _log.error(f"Request failed with status code {data.status_code}")
+        raise Exception(f"Request failed with status code {data.status_code}")
+
+
+        
 ##########################
 ##########################
 # Reports
 
 
 def formatSeriesInput(series_data, input_type, api_url):
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tcia_utils-2.1.6/src/tcia_utils/pathdb.py` & `tcia_utils-2.1.7/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/src/tcia_utils/utils.py` & `tcia_utils-2.1.7/src/tcia_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/src/tcia_utils/wordpress.py` & `tcia_utils-2.1.7/src/tcia_utils/wordpress.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/.gitignore` & `tcia_utils-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/LICENSE` & `tcia_utils-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/README.md` & `tcia_utils-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.6/pyproject.toml` & `tcia_utils-2.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "2.1.6"
+version = "2.1.7"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-2.1.6/PKG-INFO` & `tcia_utils-2.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tcia_utils
-Version: 2.1.6
+Version: 2.1.7
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

