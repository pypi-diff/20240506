# Comparing `tmp/pyzill-0.0.1.tar.gz` & `tmp/pyzill-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzill-0.0.1.tar", last modified: Tue Apr 23 20:33:51 2024, max compression
+gzip compressed data, was "pyzill-0.0.2.tar", last modified: Mon May  6 08:10:30 2024, max compression
```

## Comparing `pyzill-0.0.1.tar` & `pyzill-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 20:33:51.551705 pyzill-0.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1060 2024-04-23 19:18:55.000000 pyzill-0.0.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1980 2024-04-23 20:33:51.551705 pyzill-0.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1655 2024-04-23 20:30:30.000000 pyzill-0.0.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      423 2024-04-23 20:32:41.000000 pyzill-0.0.1/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-23 20:33:51.551705 pyzill-0.0.1/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 20:33:51.547705 pyzill-0.0.1/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 20:33:51.551705 pyzill-0.0.1/src/pyzill/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2024-04-23 19:40:04.000000 pyzill-0.0.1/src/pyzill/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1486 2024-04-23 19:53:02.000000 pyzill-0.0.1/src/pyzill/details.py
--rw-rw-r--   0 user      (1000) user      (1000)      641 2024-04-23 19:53:57.000000 pyzill-0.0.1/src/pyzill/parse.py
--rw-rw-r--   0 user      (1000) user      (1000)     2733 2024-04-23 20:27:07.000000 pyzill-0.0.1/src/pyzill/search.py
--rw-rw-r--   0 user      (1000) user      (1000)      921 2024-04-23 17:44:18.000000 pyzill-0.0.1/src/pyzill/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 20:33:51.551705 pyzill-0.0.1/src/pyzill.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1980 2024-04-23 20:33:51.000000 pyzill-0.0.1/src/pyzill.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      307 2024-04-23 20:33:51.000000 pyzill-0.0.1/src/pyzill.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-23 20:33:51.000000 pyzill-0.0.1/src/pyzill.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-23 20:33:51.000000 pyzill-0.0.1/src/pyzill.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-23 20:33:51.000000 pyzill-0.0.1/src/pyzill.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:30.928476 pyzill-0.0.2/
+-rw-rw-rw-   0        0        0     1080 2024-05-06 05:00:25.000000 pyzill-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2597 2024-05-06 08:10:30.927475 pyzill-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2024-05-06 08:09:09.000000 pyzill-0.0.2/README.md
+-rw-rw-rw-   0        0        0      451 2024-05-06 07:43:47.000000 pyzill-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:10:30.928476 pyzill-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:30.912474 pyzill-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:30.916474 pyzill-0.0.2/src/pyzill/
+-rw-rw-rw-   0        0        0      122 2024-05-06 07:39:01.000000 pyzill-0.0.2/src/pyzill/__init__.py
+-rw-rw-rw-   0        0        0     2588 2024-05-06 07:35:12.000000 pyzill-0.0.2/src/pyzill/details.py
+-rw-rw-rw-   0        0        0     1042 2024-05-06 07:59:08.000000 pyzill-0.0.2/src/pyzill/parse.py
+-rw-rw-rw-   0        0        0     8054 2024-05-06 07:29:19.000000 pyzill-0.0.2/src/pyzill/search.py
+-rw-rw-rw-   0        0        0      653 2024-05-06 07:30:37.000000 pyzill-0.0.2/src/pyzill/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:30.927475 pyzill-0.0.2/src/pyzill.egg-info/
+-rw-rw-rw-   0        0        0     2597 2024-05-06 08:10:30.000000 pyzill-0.0.2/src/pyzill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-06 08:10:30.000000 pyzill-0.0.2/src/pyzill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:10:30.000000 pyzill-0.0.2/src/pyzill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 08:10:30.000000 pyzill-0.0.2/src/pyzill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 08:10:30.000000 pyzill-0.0.2/src/pyzill.egg-info/top_level.txt
```

### Comparing `pyzill-0.0.1/PKG-INFO` & `pyzill-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,69 @@
-Metadata-Version: 2.1
-Name: pyzill
-Version: 0.0.1
-Summary: Zillow scraper in Python
-Author-email: John Balvin <johnchristian@hotmail.es>
-License: MIT
-Project-URL: Homepage, https://github.com/johnbalvin/pyzill
-Keywords: zillow,scraper,crawler
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: bs4
-
-# Zillow scraper in Python
-
-## Overview
-This project is an open-source tool developed in Python for extracting product information from Zillow. It's designed to be easy to use, making it an ideal solution for developers looking for Zillow product data.
-
-## Features
-- Full search support
-- Extracts detailed product information from Zillow
-- Implemented in Python just because it's popular
-- Easy to integrate with existing Python projects
-
-### Install
-
-```bash
-$ pip install pyzill
-```
-## Examples
-
-```Python
-import pyzill
-import json
-ne_lat = 47.76725314073866
-ne_long = -122.15539952490977
-sw_lat = 47.67128302452179
-sw_long =-122.3442270395582
-zoom_value = 2
-results = pyzill.Search_all(ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
-details_data = []
-progress = 1
-jsondata = json.dumps(results)
-f = open("results.json", "w")
-f.write(jsondata)
-f.close()
-for result in results[:3]:
-    data = pyzill.Get_from_property_id(result["zpid"],"")
-    details_data.append(data)
-    print("len results: ",progress, len(results))
-    progress=progress+1
-    
-details_data_json = json.dumps(details_data)
-f = open("details_data.json", "w")
-f.write(details_data_json)
-f.close()
-```
-
-```Python
-import pyzill
-import json
-property_url="https://www.zillow.com/homedetails/858-Shady-Grove-Ln-Harrah-OK-73045/339897685_zpid/"
-data = pyzill.Get_from_property_url(property_url,"")
-jsondata = json.dumps(data)
-f = open("details.json", "w")
-f.write(jsondata)
-f.close()
-```
-
-```Python
-import pyzill
-import json
-property_id=2056016566
-data = pyzill.Get_from_property_url(property_id,"")
-jsondata = json.dumps(data)
-f = open("details.json", "w")
-f.write(jsondata)
-f.close()
-```
+# Zillow scraper in Python
+
+## Overview
+This project is an open-source tool developed in Python for extracting product information from Zillow. It's designed to be easy to use, making it an ideal solution for developers looking for Zillow product data.
+
+## Features
+- Full search support
+- Extracts detailed product information from Zillow
+- Implemented in Python just because it's popular
+- Easy to integrate with existing Python projects
+
+### Install
+
+```bash
+$ pip install pyzill
+```
+## Examples
+
+```Python
+import pyzill
+import json
+ne_lat = 47.76725314073866
+ne_long = -122.15539952490977
+sw_lat = 47.67128302452179
+sw_long =-122.3442270395582
+zoom_value = 2
+#pagination is for the list that you see at the right when searching it's not required
+#you iterate over all the pages because zillow sends the whole data on the mapresults at once on the first page
+#however the maximum result zillow returns is 500, so if mapResults is 500
+#try playing with the zoom or moving the coordinates, pagination won't help because you will always get at maximum 500 results
+pagination = 1 
+results_sold = pyzill.sold(pagination, ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
+results_sale = pyzill.for_sale(pagination, ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
+results_rent = pyzill.for_rent(pagination, ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
+jsondata_sold = json.dumps(results_sold)
+jsondata_sale = json.dumps(results_sale)
+jsondata_rent = json.dumps(results_rent)
+f = open("./jsondata_sold.json", "w")
+f.write(jsondata_sold)
+f.close()
+f = open("./jsondata_sale.json", "w")
+f.write(jsondata_sale)
+f.close()
+f = open("./jsondata_rent.json", "w")
+f.write(jsondata_rent)
+f.close()
+```
+
+```Python
+import pyzill
+import json
+property_url="https://www.zillow.com/homedetails/858-Shady-Grove-Ln-Harrah-OK-73045/339897685_zpid/"
+data = pyzill.Get_from_property_url(property_url,"")
+jsondata = json.dumps(data)
+f = open("details.json", "w")
+f.write(jsondata)
+f.close()
+```
+
+```Python
+import pyzill
+import json
+property_id=2056016566
+data = pyzill.Get_from_property_url(property_id,"")
+jsondata = json.dumps(data)
+f = open("details.json", "w")
+f.write(jsondata)
+f.close()
+```
```

### Comparing `pyzill-0.0.1/src/pyzill.egg-info/PKG-INFO` & `pyzill-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,82 @@
-Metadata-Version: 2.1
-Name: pyzill
-Version: 0.0.1
-Summary: Zillow scraper in Python
-Author-email: John Balvin <johnchristian@hotmail.es>
-License: MIT
-Project-URL: Homepage, https://github.com/johnbalvin/pyzill
-Keywords: zillow,scraper,crawler
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: bs4
-
-# Zillow scraper in Python
-
-## Overview
-This project is an open-source tool developed in Python for extracting product information from Zillow. It's designed to be easy to use, making it an ideal solution for developers looking for Zillow product data.
-
-## Features
-- Full search support
-- Extracts detailed product information from Zillow
-- Implemented in Python just because it's popular
-- Easy to integrate with existing Python projects
-
-### Install
-
-```bash
-$ pip install pyzill
-```
-## Examples
-
-```Python
-import pyzill
-import json
-ne_lat = 47.76725314073866
-ne_long = -122.15539952490977
-sw_lat = 47.67128302452179
-sw_long =-122.3442270395582
-zoom_value = 2
-results = pyzill.Search_all(ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
-details_data = []
-progress = 1
-jsondata = json.dumps(results)
-f = open("results.json", "w")
-f.write(jsondata)
-f.close()
-for result in results[:3]:
-    data = pyzill.Get_from_property_id(result["zpid"],"")
-    details_data.append(data)
-    print("len results: ",progress, len(results))
-    progress=progress+1
-    
-details_data_json = json.dumps(details_data)
-f = open("details_data.json", "w")
-f.write(details_data_json)
-f.close()
-```
-
-```Python
-import pyzill
-import json
-property_url="https://www.zillow.com/homedetails/858-Shady-Grove-Ln-Harrah-OK-73045/339897685_zpid/"
-data = pyzill.Get_from_property_url(property_url,"")
-jsondata = json.dumps(data)
-f = open("details.json", "w")
-f.write(jsondata)
-f.close()
-```
-
-```Python
-import pyzill
-import json
-property_id=2056016566
-data = pyzill.Get_from_property_url(property_id,"")
-jsondata = json.dumps(data)
-f = open("details.json", "w")
-f.write(jsondata)
-f.close()
-```
+Metadata-Version: 2.1
+Name: pyzill
+Version: 0.0.2
+Summary: Zillow scraper in Python
+Author-email: John Balvin <johnchristian@hotmail.es>
+License: MIT
+Project-URL: Homepage, https://github.com/johnbalvin/pyzill
+Keywords: zillow,scraper,crawler
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: bs4
+Requires-Dist: requests
+
+# Zillow scraper in Python
+
+## Overview
+This project is an open-source tool developed in Python for extracting product information from Zillow. It's designed to be easy to use, making it an ideal solution for developers looking for Zillow product data.
+
+## Features
+- Full search support
+- Extracts detailed product information from Zillow
+- Implemented in Python just because it's popular
+- Easy to integrate with existing Python projects
+
+### Install
+
+```bash
+$ pip install pyzill
+```
+## Examples
+
+```Python
+import pyzill
+import json
+ne_lat = 47.76725314073866
+ne_long = -122.15539952490977
+sw_lat = 47.67128302452179
+sw_long =-122.3442270395582
+zoom_value = 2
+#pagination is for the list that you see at the right when searching it's not required
+#you iterate over all the pages because zillow sends the whole data on the mapresults at once on the first page
+#however the maximum result zillow returns is 500, so if mapResults is 500
+#try playing with the zoom or moving the coordinates, pagination won't help because you will always get at maximum 500 results
+pagination = 1 
+results_sold = pyzill.sold(pagination, ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
+results_sale = pyzill.for_sale(pagination, ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
+results_rent = pyzill.for_rent(pagination, ne_lat,ne_long,sw_lat,sw_long,zoom_value, "")
+jsondata_sold = json.dumps(results_sold)
+jsondata_sale = json.dumps(results_sale)
+jsondata_rent = json.dumps(results_rent)
+f = open("./jsondata_sold.json", "w")
+f.write(jsondata_sold)
+f.close()
+f = open("./jsondata_sale.json", "w")
+f.write(jsondata_sale)
+f.close()
+f = open("./jsondata_rent.json", "w")
+f.write(jsondata_rent)
+f.close()
+```
+
+```Python
+import pyzill
+import json
+property_url="https://www.zillow.com/homedetails/858-Shady-Grove-Ln-Harrah-OK-73045/339897685_zpid/"
+data = pyzill.Get_from_property_url(property_url,"")
+jsondata = json.dumps(data)
+f = open("details.json", "w")
+f.write(jsondata)
+f.close()
+```
+
+```Python
+import pyzill
+import json
+property_id=2056016566
+data = pyzill.Get_from_property_url(property_id,"")
+jsondata = json.dumps(data)
+f = open("details.json", "w")
+f.write(jsondata)
+f.close()
+```
```

