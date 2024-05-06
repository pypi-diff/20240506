# Comparing `tmp/pyoscar-0.6.4.tar.gz` & `tmp/pyoscar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyoscar-0.6.4.tar", last modified: Tue Sep 19 14:14:03 2023, max compression
+gzip compressed data, was "pyoscar-0.7.0.tar", last modified: Mon May  6 00:16:06 2024, max compression
```

## Comparing `pyoscar-0.6.4.tar` & `pyoscar-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-09-19 14:14:03.000000 pyoscar-0.6.4/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1069 2023-09-14 10:23:29.000000 pyoscar-0.6.4/LICENSE
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       43 2023-09-14 10:23:29.000000 pyoscar-0.6.4/MANIFEST.in
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     6818 2023-09-19 14:14:03.000000 pyoscar-0.6.4/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4481 2023-09-19 13:53:30.000000 pyoscar-0.6.4/README.md
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)    22062 2023-09-19 14:13:08.000000 pyoscar-0.6.4/pyoscar/__init__.py
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     1794 2023-09-14 10:23:29.000000 pyoscar-0.6.4/pyoscar/cli_options.py
-drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     6818 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/PKG-INFO
--rw-rw-r--   0 tomkralidis   (501) staff       (20)      286 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/SOURCES.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/dependency_links.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       41 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/entry_points.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       35 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/requires.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)        8 2023-09-19 14:14:03.000000 pyoscar-0.6.4/pyoscar.egg-info/top_level.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       35 2023-09-14 10:37:57.000000 pyoscar-0.6.4/requirements.txt
--rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2023-09-19 14:14:03.000000 pyoscar-0.6.4/setup.cfg
--rw-rw-r--   0 tomkralidis   (501) staff       (20)     4155 2023-09-14 10:23:29.000000 pyoscar-0.6.4/setup.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-05-06 00:16:06.159232 pyoscar-0.7.0/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1069 2023-09-14 10:23:29.000000 pyoscar-0.7.0/LICENSE
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       43 2023-09-14 10:23:29.000000 pyoscar-0.7.0/MANIFEST.in
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     5314 2024-05-06 00:16:06.158811 pyoscar-0.7.0/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4503 2024-02-12 01:19:42.000000 pyoscar-0.7.0/README.md
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-05-06 00:16:06.154190 pyoscar-0.7.0/pyoscar/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)    21562 2024-05-06 00:14:39.000000 pyoscar-0.7.0/pyoscar/__init__.py
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     1794 2023-09-14 10:23:29.000000 pyoscar-0.7.0/pyoscar/cli_options.py
+drwxrwxr-x   0 tomkralidis   (501) staff       (20)        0 2024-05-06 00:16:06.158048 pyoscar-0.7.0/pyoscar.egg-info/
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     5314 2024-05-06 00:16:05.000000 pyoscar-0.7.0/pyoscar.egg-info/PKG-INFO
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)      286 2024-05-06 00:16:06.000000 pyoscar-0.7.0/pyoscar.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        1 2024-05-06 00:16:05.000000 pyoscar-0.7.0/pyoscar.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       40 2024-05-06 00:16:05.000000 pyoscar-0.7.0/pyoscar.egg-info/entry_points.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       35 2024-05-06 00:16:05.000000 pyoscar-0.7.0/pyoscar.egg-info/requires.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)        8 2024-05-06 00:16:05.000000 pyoscar-0.7.0/pyoscar.egg-info/top_level.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       35 2023-09-14 10:37:57.000000 pyoscar-0.7.0/requirements.txt
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)       38 2024-05-06 00:16:06.159361 pyoscar-0.7.0/setup.cfg
+-rw-rw-r--   0 tomkralidis   (501) staff       (20)     4155 2023-09-14 10:23:29.000000 pyoscar-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyoscar-0.6.4/LICENSE` & `pyoscar-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoscar-0.6.4/README.md` & `pyoscar-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,17 @@
 python3 setup.py test
 
 # measure code coverage
 coverage run --source pyoscar setup.py test
 coverage report -m
 ```
 
-# create release (x.y.z is the release version)
+# Releasing
+```bash
+create release (x.y.z is the release version)
 vi pyoscar/__init__.py  # update __version__
 git commit -am 'update release version x.y.z'
 git push origin master
 git tag -a x.y.z -m 'tagging release version x.y.z'
 git push --tags
 
 # upload to PyPI
@@ -175,14 +177,15 @@
 
 # publish release on GitHub (https://github.com/wmo-cop/pyoscar/releases/new)
 
 # bump version back to dev
 vi pyoscar/__init__.py  # update __version__
 git commit -am 'back to dev'
 git push origin master
+```
 
 ### Code Conventions
 
 * [PEP8](https://www.python.org/dev/peps/pep-0008)
 
 ### Bugs and Issues
```

### Comparing `pyoscar-0.6.4/pyoscar/__init__.py` & `pyoscar-0.7.0/pyoscar/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # =================================================================
 #
 # Authors: Tom Kralidis <tomkralidis@gmail.com>
 #
-# Copyright (c) 2023 Tom Kralidis
+# Copyright (c) 2024 Tom Kralidis
 #
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation
 # files (the "Software"), to deal in the Software without
 # restriction, including without limitation the rights to use,
 # copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the
@@ -23,15 +23,15 @@
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
-__version__ = '0.6.4'
+__version__ = '0.7.0'
 
 from datetime import date
 import json
 import logging
 import os
 import requests
 from typing import Generator, Union
@@ -40,29 +40,14 @@
 import click
 from lxml import etree
 
 from pyoscar import cli_options
 
 LOGGER = logging.getLogger(__name__)
 
-FACILITY_TYPE_LOOKUP = {
-    'seaMobile': 'Sea (mobile)',
-    'underwaterFixed': 'Underwater (fixed)',
-    'underwaterMobile': 'Underwater (mobile)',
-    'airMobile': 'Air (mobile)',
-    'lakeRiverMobile': 'Lake/River (mobile)',
-    'seaOnIce': 'Sea (on ice)',
-    'landMobile': 'Land (mobile)',
-    'landFixed': 'Land (fixed)',
-    'lakeRiverFixed': 'Lake/River (fixed)',
-    'seaFixed': 'Sea (fixed)',
-    'airFixed': 'Air (fixed)',
-    'landOnIce': 'Land (on ice)'
-}
-
 
 class OSCARClient:
     """OSCAR client API"""
 
     def __init__(self, env: str = 'depl', api_token: str = None,
                  timeout: int = 30):
         """
@@ -144,15 +129,15 @@
                 LOGGER.debug(f'Program: {program}')
                 params['programAffiliation'] = program
             if country is not None:
                 LOGGER.debug(f'Country: {program}')
                 params['territoryName'] = country
             if station_type is not None:
                 LOGGER.debug(f'Station type: {station_type}')
-                params['facilityType'] = FACILITY_TYPE_LOOKUP[station_type]
+                params['facilityType'] = station_type
 
         response = requests.get(request, headers=self.headers, params=params)
         LOGGER.debug(f'Request: {response.url}')
         LOGGER.debug(f'Response: {response.status_code}')
 
         return response.json()
 
@@ -205,28 +190,28 @@
         :param summary: whether to provide a summary report (default `False`)
         :param format_: format (JSON [default] or XML)
 
         :returns: `dict` of JSON payload or summary, or `etree.Element` of
                   matching station report WMDR XML
         """
 
-        LOGGER.debug(f'Searching stations for WIGOS ID: {identifier}')
-        response = self.get_stations(wigos_id=identifier)
-        if not response or response['totalCount'] == 0:
-            msg = f'Station {identifier} not found'
-            LOGGER.debug(msg)
-            raise RuntimeError(msg)
-
-        identifier = str(response['stationSearchResults'][0]['id'])
-
-        LOGGER.debug(f'Fetching station report {identifier}')
         if format_ == 'XML':
             LOGGER.debug('Trying WIGOS XML download')
-            request = f'{self.api_url}/wmd/download/{identifier}'
+            request = f'{self.harvest_url}?verb=GetRecord&metadataPrefix=wmdr&identifier={identifier}'  # noqa
         else:
+            LOGGER.debug(f'Searching stations for WIGOS ID: {identifier}')
+            response = self.get_stations(wigos_id=identifier)
+            if not response or response['totalCount'] == 0:
+                msg = f'Station {identifier} not found'
+                LOGGER.debug(msg)
+                raise RuntimeError(msg)
+
+            identifier = str(response['stationSearchResults'][0]['id'])
+
+            LOGGER.debug(f'Fetching station report {identifier}')
             request = f'{self.api_url}/stations/station/{identifier}/stationReport'  # noqa
 
         response = requests.get(request, headers=self.headers)
         LOGGER.debug(f'Request: {response.url}')
         LOGGER.debug(f'Response: {response.status_code}')
 
         response.raise_for_status()
@@ -293,15 +278,15 @@
             if not territory_name:
                 territory_name = None
             else:
                 territory_name = territory_name.split('/')[-1]
 
             summary['station_name'] = station_name
             summary['wigos_station_identifier'] = wigos_station_identifier
-            summary['facility_type'] = FACILITY_TYPE_LOOKUP[facility_type]
+            summary['facility_type'] = facility_type
             summary['wmo_region'] = wmo_region
             summary['territory_name'] = territory_name
 
             geometry = get_xpath(
                 station, '//wmdr:ObservingFacility//wmdr:geoLocation//gml:pos')
 
             if geometry is None:
@@ -559,16 +544,15 @@
 
 @click.command('stations')
 @click.pass_context
 @cli_options.OPTION_COUNTRY
 @cli_options.OPTION_ENV
 @cli_options.OPTION_VERBOSITY
 @click.option('--program', '-p', help='Program Affiliation')
-@click.option('--station-type', '-st', help='Station type',
-              type=click.Choice(FACILITY_TYPE_LOOKUP.keys()))
+@click.option('--station-type', '-st', help='Station type')
 def stations(ctx, env, program=None, country=None, station_type=None,
              verbosity=None):
     """get list of OSCAR stations"""
 
     if verbosity is not None:
         logging.basicConfig(level=getattr(logging, verbosity))
     else:
```

### Comparing `pyoscar-0.6.4/pyoscar/cli_options.py` & `pyoscar-0.7.0/pyoscar/cli_options.py`

 * *Files identical despite different names*

### Comparing `pyoscar-0.6.4/setup.py` & `pyoscar-0.7.0/setup.py`

 * *Files identical despite different names*

