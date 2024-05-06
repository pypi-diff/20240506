# Comparing `tmp/flowkit_jwt_generator-1.25.0.post0.dev82-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.25.0.post0.dev84-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8543 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-May-03 15:58 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 24-May-03 15:58 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-May-03 15:58 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-May-03 15:58 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-May-03 15:58 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-03 15:58 flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 15:58 flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-May-03 15:58 flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-May-03 15:58 flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 24-May-03 15:58 flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/RECORD
-10 files, 17781 bytes uncompressed, 6845 bytes compressed:  61.5%
+Zip file size: 8539 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-May-06 04:26 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      510 b- defN 24-May-06 04:26 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-May-06 04:26 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-May-06 04:26 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-May-06 04:26 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-06 04:26 flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 04:26 flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-May-06 04:26 flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-May-06 04:26 flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 24-May-06 04:26 flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/RECORD
+10 files, 17781 bytes uncompressed, 6841 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowkit_jwt_generator/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-05-03T15:55:49+0000",
+ "date": "2024-05-06T04:23:18+0000",
  "dirty": false,
  "error": null,
- "full-revisionid": "d2f2a13c271cb2ed91c3bed34b690629e33ed637",
- "version": "1.25.0.post0.dev82"
+ "full-revisionid": "12eb83a59e22ee234d9fd257a704d5ab60c9f2b9",
+ "version": "1.25.0.post0.dev84"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/METADATA` & `flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowkit_jwt_generator
-Version: 1.25.0.post0.dev82
+Version: 1.25.0.post0.dev84
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

## Comparing `flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/RECORD` & `flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 flowkit_jwt_generator/__init__.py,sha256=Vqa2vcGLH7wfO7GXFiSQX2QXctRgwUuM-QG9DJ0HQqk,507
-flowkit_jwt_generator/_version.py,sha256=BuL3nt-AcCPWWELBMdGxIGpoS0S94sCctznXUhKMRQw,510
+flowkit_jwt_generator/_version.py,sha256=O4Vm60tb81CyKFCWB-mS1BZYtDYjT5z3ZEplEhWK47k,510
 flowkit_jwt_generator/cli.py,sha256=hx88rA2O7sqhQ0EHQTCVrZpcdBLW-qssaaodnpXV1DQ,1591
 flowkit_jwt_generator/fixtures.py,sha256=jVDYkagDNtu_m94ns2F6sDtqMmq1kBygS6DBaMqBGoo,3405
 flowkit_jwt_generator/jwt.py,sha256=R_IjXQwtq3eYOmEVcHp7bOCtBgoGUyUpmrJRKsp1MMc,9215
-flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/METADATA,sha256=UFyTUUJw3Z0yMSFcFGFzk5FeSnPRlbbLJBgmN4_jZdc,1334
-flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
-flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
-flowkit_jwt_generator-1.25.0.post0.dev82.dist-info/RECORD,,
+flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/METADATA,sha256=-o-1jK15n2uQDZYn1ObzOOjhwOhDN183fAbgdygyIqs,1334
+flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
+flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
+flowkit_jwt_generator-1.25.0.post0.dev84.dist-info/RECORD,,
```
