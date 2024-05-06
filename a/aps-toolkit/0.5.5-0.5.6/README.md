# Comparing `tmp/aps-toolkit-0.5.5.tar.gz` & `tmp/aps-toolkit-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.5.5.tar", last modified: Mon May  6 02:16:23 2024, max compression
+gzip compressed data, was "aps-toolkit-0.5.6.tar", last modified: Mon May  6 06:41:49 2024, max compression
```

## Comparing `aps-toolkit-0.5.5.tar` & `aps-toolkit-0.5.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:16:23.189521 aps-toolkit-0.5.5/
--rw-rw-rw-   0        0        0     1990 2024-05-06 02:16:23.188521 aps-toolkit-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-06 02:16:23.189521 aps-toolkit-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      902 2024-05-06 02:16:13.000000 aps-toolkit-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:16:23.125520 aps-toolkit-0.5.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 02:16:23.152520 aps-toolkit-0.5.5/src/aps_toolkit/
--rw-rw-rw-   0        0        0     6070 2024-05-06 02:13:40.000000 aps-toolkit-0.5.5/src/aps_toolkit/Auth.py
--rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.5.5/src/aps_toolkit/BIM360.py
--rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.5.5/src/aps_toolkit/Bucket.py
--rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.5.5/src/aps_toolkit/DbReader.py
--rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.5.5/src/aps_toolkit/Derivative.py
--rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.5.5/src/aps_toolkit/Fragments.py
--rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/InputStream.py
--rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/ManifestItem.py
--rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/MaterialProperties.py
--rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/Materials.py
--rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/PackFileReader.py
--rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/PathInfo.py
--rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/ProDbReaderCad.py
--rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.5.5/src/aps_toolkit/ProDbReaderNavis.py
--rw-rw-rw-   0        0        0    13855 2024-03-19 23:58:05.000000 aps-toolkit-0.5.5/src/aps_toolkit/ProDbReaderRevit.py
--rw-rw-rw-   0        0        0    13418 2024-03-27 07:23:53.000000 aps-toolkit-0.5.5/src/aps_toolkit/PropReader.py
--rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.5.5/src/aps_toolkit/Resource.py
--rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFContent.py
--rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFGeometries.py
--rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFImage.py
--rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFLines.py
--rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFManifestType.py
--rw-rw-rw-   0        0        0      910 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterialGroup.py
--rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterialMap.py
--rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterialMapScale.py
--rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterials.py
--rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFMesh.py
--rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFMetadata.py
--rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFPoints.py
--rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFReader.py
--rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFTransform.py
--rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.5.5/src/aps_toolkit/SVFUVMap.py
--rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.5.5/src/aps_toolkit/Token.py
--rw-rw-rw-   0        0        0      721 2024-04-01 02:00:06.000000 aps-toolkit-0.5.5/src/aps_toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:16:23.155520 aps-toolkit-0.5.5/src/aps_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-06 02:16:22.000000 aps-toolkit-0.5.5/src/aps_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2024-05-06 02:16:22.000000 aps-toolkit-0.5.5/src/aps_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:16:22.000000 aps-toolkit-0.5.5/src/aps_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 02:16:22.000000 aps-toolkit-0.5.5/src/aps_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-06 02:16:22.000000 aps-toolkit-0.5.5/src/aps_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 02:16:23.187521 aps-toolkit-0.5.5/src/test/
--rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.5.5/src/test/__init__.py
--rw-rw-rw-   0        0        0      974 2024-04-01 02:00:06.000000 aps-toolkit-0.5.5/src/test/context.py
--rw-rw-rw-   0        0        0     1367 2024-05-06 02:12:24.000000 aps-toolkit-0.5.5/src/test/test_auth.py
--rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.5.5/src/test/test_bim360.py
--rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.5.5/src/test/test_bucket.py
--rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.5.5/src/test/test_db_reader.py
--rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.5.5/src/test/test_derivative.py
--rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.5.5/src/test/test_fragment.py
--rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.5.5/src/test/test_geometries.py
--rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/test/test_image.py
--rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.5.5/src/test/test_material.py
--rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.5.5/src/test/test_mesh.py
--rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/test/test_metadata.py
--rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.5.5/src/test/test_prop_reader.py
--rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/test/test_prop_reader_cad.py
--rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.5.5/src/test/test_prop_reader_navis.py
--rw-rw-rw-   0        0        0     3472 2024-03-15 07:18:51.000000 aps-toolkit-0.5.5/src/test/test_prop_reader_revit.py
--rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.5.5/src/test/test_svf_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:41:49.760596 aps-toolkit-0.5.6/
+-rw-rw-rw-   0        0        0     1990 2024-05-06 06:41:49.758631 aps-toolkit-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:41:49.761598 aps-toolkit-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      902 2024-05-06 06:41:25.000000 aps-toolkit-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:41:48.051911 aps-toolkit-0.5.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 06:41:49.385593 aps-toolkit-0.5.6/src/aps_toolkit/
+-rw-rw-rw-   0        0        0    11183 2024-05-06 05:27:02.000000 aps-toolkit-0.5.6/src/aps_toolkit/Auth.py
+-rw-rw-rw-   0        0        0    10333 2024-03-27 07:53:22.000000 aps-toolkit-0.5.6/src/aps_toolkit/BIM360.py
+-rw-rw-rw-   0        0        0     9081 2024-04-01 02:00:06.000000 aps-toolkit-0.5.6/src/aps_toolkit/Bucket.py
+-rw-rw-rw-   0        0        0     2512 2024-03-22 08:01:52.000000 aps-toolkit-0.5.6/src/aps_toolkit/DbReader.py
+-rw-rw-rw-   0        0        0    12931 2024-03-22 07:28:19.000000 aps-toolkit-0.5.6/src/aps_toolkit/Derivative.py
+-rw-rw-rw-   0        0        0     3949 2024-03-22 07:10:58.000000 aps-toolkit-0.5.6/src/aps_toolkit/Fragments.py
+-rw-rw-rw-   0        0        0     2401 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/InputStream.py
+-rw-rw-rw-   0        0        0      905 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/ManifestItem.py
+-rw-rw-rw-   0        0        0     1164 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/MaterialProperties.py
+-rw-rw-rw-   0        0        0     1769 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/Materials.py
+-rw-rw-rw-   0        0        0     3792 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/PackFileReader.py
+-rw-rw-rw-   0        0        0      950 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/PathInfo.py
+-rw-rw-rw-   0        0        0     4586 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/ProDbReaderCad.py
+-rw-rw-rw-   0        0        0     3592 2024-03-25 01:46:50.000000 aps-toolkit-0.5.6/src/aps_toolkit/ProDbReaderNavis.py
+-rw-rw-rw-   0        0        0    13855 2024-03-19 23:58:05.000000 aps-toolkit-0.5.6/src/aps_toolkit/ProDbReaderRevit.py
+-rw-rw-rw-   0        0        0    13418 2024-03-27 07:23:53.000000 aps-toolkit-0.5.6/src/aps_toolkit/PropReader.py
+-rw-rw-rw-   0        0        0     1410 2024-03-22 05:35:45.000000 aps-toolkit-0.5.6/src/aps_toolkit/Resource.py
+-rw-rw-rw-   0        0        0     1095 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFContent.py
+-rw-rw-rw-   0        0        0     3414 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFGeometries.py
+-rw-rw-rw-   0        0        0     1190 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFImage.py
+-rw-rw-rw-   0        0        0     1063 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFLines.py
+-rw-rw-rw-   0        0        0      851 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFManifestType.py
+-rw-rw-rw-   0        0        0      910 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterialGroup.py
+-rw-rw-rw-   0        0        0      793 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterialMap.py
+-rw-rw-rw-   0        0        0      854 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-rw-rw-   0        0        0     7744 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterials.py
+-rw-rw-rw-   0        0        0     9990 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFMesh.py
+-rw-rw-rw-   0        0        0      882 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFMetadata.py
+-rw-rw-rw-   0        0        0      959 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFPoints.py
+-rw-rw-rw-   0        0        0     6840 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFReader.py
+-rw-rw-rw-   0        0        0      844 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFTransform.py
+-rw-rw-rw-   0        0        0      819 2024-03-18 03:16:28.000000 aps-toolkit-0.5.6/src/aps_toolkit/SVFUVMap.py
+-rw-rw-rw-   0        0        0     1010 2024-04-01 02:00:06.000000 aps-toolkit-0.5.6/src/aps_toolkit/Token.py
+-rw-rw-rw-   0        0        0      721 2024-04-01 02:00:06.000000 aps-toolkit-0.5.6/src/aps_toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:41:49.392177 aps-toolkit-0.5.6/src/aps_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-06 06:41:47.000000 aps-toolkit-0.5.6/src/aps_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-05-06 06:41:47.000000 aps-toolkit-0.5.6/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:41:47.000000 aps-toolkit-0.5.6/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 06:41:47.000000 aps-toolkit-0.5.6/src/aps_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 06:41:47.000000 aps-toolkit-0.5.6/src/aps_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 06:41:49.756645 aps-toolkit-0.5.6/src/test/
+-rw-rw-rw-   0        0        0        0 2024-03-04 00:25:18.000000 aps-toolkit-0.5.6/src/test/__init__.py
+-rw-rw-rw-   0        0        0      974 2024-04-01 02:00:06.000000 aps-toolkit-0.5.6/src/test/context.py
+-rw-rw-rw-   0        0        0     2006 2024-05-06 06:38:44.000000 aps-toolkit-0.5.6/src/test/test_auth.py
+-rw-rw-rw-   0        0        0     2734 2024-03-27 07:00:24.000000 aps-toolkit-0.5.6/src/test/test_bim360.py
+-rw-rw-rw-   0        0        0     2019 2024-04-01 02:00:06.000000 aps-toolkit-0.5.6/src/test/test_bucket.py
+-rw-rw-rw-   0        0        0      860 2024-03-22 08:37:55.000000 aps-toolkit-0.5.6/src/test/test_db_reader.py
+-rw-rw-rw-   0        0        0     1919 2024-03-26 06:55:19.000000 aps-toolkit-0.5.6/src/test/test_derivative.py
+-rw-rw-rw-   0        0        0     1022 2024-03-15 07:18:51.000000 aps-toolkit-0.5.6/src/test/test_fragment.py
+-rw-rw-rw-   0        0        0      879 2024-03-15 07:18:51.000000 aps-toolkit-0.5.6/src/test/test_geometries.py
+-rw-rw-rw-   0        0        0      786 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/test/test_image.py
+-rw-rw-rw-   0        0        0     1263 2024-03-15 07:18:51.000000 aps-toolkit-0.5.6/src/test/test_material.py
+-rw-rw-rw-   0        0        0      709 2024-03-15 07:18:51.000000 aps-toolkit-0.5.6/src/test/test_mesh.py
+-rw-rw-rw-   0        0        0      509 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/test/test_metadata.py
+-rw-rw-rw-   0        0        0     1891 2024-03-27 07:25:01.000000 aps-toolkit-0.5.6/src/test/test_prop_reader.py
+-rw-rw-rw-   0        0        0     1481 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/test/test_prop_reader_cad.py
+-rw-rw-rw-   0        0        0      799 2024-03-25 01:46:50.000000 aps-toolkit-0.5.6/src/test/test_prop_reader_navis.py
+-rw-rw-rw-   0        0        0     3472 2024-03-15 07:18:51.000000 aps-toolkit-0.5.6/src/test/test_prop_reader_revit.py
+-rw-rw-rw-   0        0        0     2998 2024-03-22 07:12:32.000000 aps-toolkit-0.5.6/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.5.5/PKG-INFO` & `aps-toolkit-0.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.5/setup.py` & `aps-toolkit-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.5.5",
+    version="0.5.6",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.5.6/src/aps_toolkit/BIM360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.5.6/src/aps_toolkit/Bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.5.6/src/aps_toolkit/DbReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.5.6/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.5.6/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.5.6/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.5.6/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.5.6/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/Materials.py` & `aps-toolkit-0.5.6/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.5.6/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.5.6/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.5.6/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.5.6/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.5.6/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.5.6/src/aps_toolkit/PropReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/Resource.py` & `aps-toolkit-0.5.6/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.5.6/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/Token.py` & `aps-toolkit-0.5.6/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit/__init__.py` & `aps-toolkit-0.5.6/src/aps_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.5.6/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.5.5/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.5.6/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/context.py` & `aps-toolkit-0.5.6/src/test/context.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_auth.py` & `aps-toolkit-0.5.6/src/test/test_auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,17 +21,33 @@
         redirect_uri = "http://localhost:8080/api/auth/callback"
         # https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes
         scopes = 'data:read viewables:read'
         token = auth.auth3leg(redirect_uri, scopes)
         print(token.refresh_token)
         self.assertNotEquals(token.access_token, "")
 
+    def test_auth3legPkce(self):
+        auth = Auth()
+        redirect_uri = "http://localhost:8080/api/auth/callback"
+        # https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes
+        scopes = 'data:read viewables:read'
+        client_id = os.environ['APS_CLIENT_PKCE_ID']
+        token = auth.auth3legPkce(client_id, redirect_uri, scopes)
+        print(token.refresh_token)
+        self.assertNotEquals(token.access_token, "")
+
     def test_refresh_token(self):
         auth = Auth()
         token = auth.auth3leg()
         self.assertNotEquals(token.access_token, "")
         print("Refresh token: ", token.refresh_token)
         print("Start refresh token")
         new_token = auth.refresh_new_token(token.refresh_token)
         print("New Fresh Token", new_token.refresh_token)
         self.assertNotEquals(token.access_token, "")
         self.assertNotEquals(token.refresh_token, "")
+
+    def test_get_user_info(self):
+        auth = Auth()
+        token = auth.auth3leg()
+        user_info = auth.get_user_info()
+        self.assertNotEquals(user_info, "")
```

### Comparing `aps-toolkit-0.5.5/src/test/test_bim360.py` & `aps-toolkit-0.5.6/src/test/test_bim360.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_bucket.py` & `aps-toolkit-0.5.6/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_db_reader.py` & `aps-toolkit-0.5.6/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_derivative.py` & `aps-toolkit-0.5.6/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_fragment.py` & `aps-toolkit-0.5.6/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_geometries.py` & `aps-toolkit-0.5.6/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_image.py` & `aps-toolkit-0.5.6/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_material.py` & `aps-toolkit-0.5.6/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_mesh.py` & `aps-toolkit-0.5.6/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_prop_reader.py` & `aps-toolkit-0.5.6/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.5.6/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.5.6/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.5.6/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.5.5/src/test/test_svf_reader.py` & `aps-toolkit-0.5.6/src/test/test_svf_reader.py`

 * *Files identical despite different names*

