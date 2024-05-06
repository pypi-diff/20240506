# Comparing `tmp/redlite-0.1.3-py3-none-any.whl.zip` & `tmp/redlite-0.1.4rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1814365 bytes, number of entries: 103
--rw-rw-r--  2.0 unx      427 b- defN 24-May-01 10:55 redlite/__init__.py
+Zip file size: 1815183 bytes, number of entries: 104
+-rw-rw-r--  2.0 unx      430 b- defN 24-May-06 14:46 redlite/__init__.py
 -rw-rw-r--  2.0 unx     1841 b- defN 24-Apr-30 19:07 redlite/__main__.py
 -rw-rw-r--  2.0 unx     4512 b- defN 24-Apr-30 19:07 redlite/_core.py
 -rw-rw-r--  2.0 unx      277 b- defN 24-Apr-30 19:07 redlite/_dummy_storage.py
 -rw-rw-r--  2.0 unx     1078 b- defN 24-Apr-30 19:07 redlite/_jsonl_storage.py
 -rw-rw-r--  2.0 unx      902 b- defN 24-Apr-30 19:07 redlite/_lock.py
 -rw-rw-r--  2.0 unx     6000 b- defN 24-Apr-30 19:07 redlite/_run.py
 -rw-rw-r--  2.0 unx     7207 b- defN 24-Apr-30 19:07 redlite/_util.py
@@ -21,17 +21,18 @@
 -rw-rw-r--  2.0 unx     1186 b- defN 24-Apr-30 19:07 redlite/metric/util.py
 -rw-rw-r--  2.0 unx     1672 b- defN 24-Apr-30 19:07 redlite/metric/bleu/__init__.py
 -rw-rw-r--  2.0 unx     1187 b- defN 24-Apr-30 19:07 redlite/metric/f1/__init__.py
 -rw-rw-r--  2.0 unx     1970 b- defN 24-Apr-30 19:07 redlite/metric/rouge/__init__.py
 -rw-rw-r--  2.0 unx      208 b- defN 24-Apr-30 19:07 redlite/model/__init__.py
 -rw-rw-r--  2.0 unx      690 b- defN 24-Apr-30 19:07 redlite/model/_dummy.py
 -rw-rw-r--  2.0 unx     2515 b- defN 24-Apr-30 19:07 redlite/model/_ignore_system.py
--rw-rw-r--  2.0 unx     1388 b- defN 24-May-01 10:57 redlite/model/anthropic_model.py
+-rw-rw-r--  2.0 unx     1388 b- defN 24-May-01 10:59 redlite/model/anthropic_model.py
 -rw-rw-r--  2.0 unx     4411 b- defN 24-Apr-30 19:07 redlite/model/aws_bedrock_model.py
 -rw-rw-r--  2.0 unx     3909 b- defN 24-Apr-30 19:08 redlite/model/hf_model.py
+-rw-rw-r--  2.0 unx     1236 b- defN 24-May-06 14:45 redlite/model/hf_model_pipeline.py
 -rw-rw-r--  2.0 unx      966 b- defN 24-Apr-30 19:07 redlite/model/openai_model.py
 -rw-rw-r--  2.0 unx      296 b- defN 24-Apr-30 19:07 redlite/server/__init__.py
 -rw-rw-r--  2.0 unx     3992 b- defN 24-Apr-30 19:07 redlite/server/_app.py
 -rw-rw-r--  2.0 unx    14557 b- defN 24-Apr-30 19:07 redlite/server/resources/default/3rdpartylicenses.txt
 -rw-rw-r--  2.0 unx    10355 b- defN 24-Apr-30 19:07 redlite/server/resources/default/color.dae87a04d07ca92b.png
 -rw-rw-r--  2.0 unx     5430 b- defN 24-Apr-30 19:07 redlite/server/resources/default/favicon.ico
 -rw-rw-r--  2.0 unx   165742 b- defN 24-Apr-30 19:07 redlite/server/resources/default/fontawesome-webfont.2b13baa7dd4f54c9.eot
@@ -92,14 +93,14 @@
 -rw-rw-r--  2.0 unx     2115 b- defN 24-Apr-30 19:07 redlite/server/resources/legacy/_app/immutable/nodes/5.CNhJU3OA.js
 -rw-rw-r--  2.0 unx     2672 b- defN 24-Apr-30 19:07 redlite/server/resources/legacy/_app/immutable/nodes/6.BA5ucq1q.js
 -rw-rw-r--  2.0 unx     5744 b- defN 24-Apr-30 19:07 redlite/server/resources/legacy/_app/immutable/nodes/7.z3N0foJ1.js
 -rw-rw-r--  2.0 unx     2132 b- defN 24-Apr-30 19:07 redlite/server/resources/legacy/_app/immutable/nodes/8.DkMbLct2.js
 -rw-rw-r--  2.0 unx      487 b- defN 24-Apr-30 19:07 redlite/server/resources/legacy/_app/immutable/nodes/9.ZOpqgAss.js
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 19:07 redlite/zeno/__init__.py
 -rw-rw-r--  2.0 unx     4152 b- defN 24-Apr-30 19:07 redlite/zeno/upload.py
--rw-rw-r--  2.0 unx     1071 b- defN 24-May-01 10:58 redlite-0.1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5631 b- defN 24-May-01 10:58 redlite-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-01 10:58 redlite-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 24-May-01 10:58 redlite-0.1.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-May-01 10:58 redlite-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11061 b- defN 24-May-01 10:58 redlite-0.1.3.dist-info/RECORD
-103 files, 5313167 bytes uncompressed, 1796011 bytes compressed:  66.2%
+-rw-rw-r--  2.0 unx     1071 b- defN 24-May-06 14:46 redlite-0.1.4rc0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5634 b- defN 24-May-06 14:46 redlite-0.1.4rc0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-06 14:46 redlite-0.1.4rc0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 24-May-06 14:46 redlite-0.1.4rc0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-06 14:46 redlite-0.1.4rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11170 b- defN 24-May-06 14:46 redlite-0.1.4rc0.dist-info/RECORD
+104 files, 5314518 bytes uncompressed, 1796649 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -81,14 +81,17 @@
 
 Filename: redlite/model/aws_bedrock_model.py
 Comment: 
 
 Filename: redlite/model/hf_model.py
 Comment: 
 
+Filename: redlite/model/hf_model_pipeline.py
+Comment: 
+
 Filename: redlite/model/openai_model.py
 Comment: 
 
 Filename: redlite/server/__init__.py
 Comment: 
 
 Filename: redlite/server/_app.py
@@ -285,26 +288,26 @@
 
 Filename: redlite/zeno/__init__.py
 Comment: 
 
 Filename: redlite/zeno/upload.py
 Comment: 
 
-Filename: redlite-0.1.3.dist-info/LICENSE
+Filename: redlite-0.1.4rc0.dist-info/LICENSE
 Comment: 
 
-Filename: redlite-0.1.3.dist-info/METADATA
+Filename: redlite-0.1.4rc0.dist-info/METADATA
 Comment: 
 
-Filename: redlite-0.1.3.dist-info/WHEEL
+Filename: redlite-0.1.4rc0.dist-info/WHEEL
 Comment: 
 
-Filename: redlite-0.1.3.dist-info/entry_points.txt
+Filename: redlite-0.1.4rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: redlite-0.1.3.dist-info/top_level.txt
+Filename: redlite-0.1.4rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: redlite-0.1.3.dist-info/RECORD
+Filename: redlite-0.1.4rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## redlite/__init__.py

```diff
@@ -6,15 +6,15 @@
     NamedMetric,
     Run,
     MissingDependencyError,
 )
 from ._run import run, rescore
 from .dataset._load import load_dataset
 
-__version__ = "0.1.3"
+__version__ = "0.1.4rc0"
 __all__ = [
     "run",
     "rescore",
     "load_dataset",
     "NamedModel",
     "NamedDataset",
     "NamedMetric",
```

## Comparing `redlite-0.1.3.dist-info/LICENSE` & `redlite-0.1.4rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `redlite-0.1.3.dist-info/METADATA` & `redlite-0.1.4rc0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redlite
-Version: 0.1.3
+Version: 0.1.4rc0
 Summary: LLM testing on steroids
 Author-email: Mike Kroutikov <mkroutikov@innodata.com>, David Nadeau <dnadeau@innodata.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/innodatalabs/redlite
 Project-URL: Documentation, https://innodatalabs.github.io/redlite
 Project-URL: Repository, https://github.com/innodatalabs/redlite.git
 Project-URL: Issues, https://github.com/innodatalabs/redlite/issues
```

## Comparing `redlite-0.1.3.dist-info/RECORD` & `redlite-0.1.4rc0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-redlite/__init__.py,sha256=B9XXJBgnnvcSRfmP5OBNJz3bNB7hQxc_cuXixwM-EMY,427
+redlite/__init__.py,sha256=siakRtWiz0BVoPDdIzIDALd2WDL7_n6z6qSayolX2pI,430
 redlite/__main__.py,sha256=PujE49yrqh7VxmPbCeDQHOyy76FIXLvlYg8F96Arluk,1841
 redlite/_core.py,sha256=JPT0gqvdgLPPuHVAWJx8r5wX2Blv5ugIdoe5zywEm9U,4512
 redlite/_dummy_storage.py,sha256=1iowZG3-eNs1B3kWCXiy4xGOiMrmNceqU0BZG5NjCqg,277
 redlite/_jsonl_storage.py,sha256=DQQYjRkx40nk87nlAsOB6vIDaGvzFh2QZNgIaVadhA4,1078
 redlite/_lock.py,sha256=rDP0jaITUxsQvb7c4nCu0KzQDt5HBHPKLBwFWQnWPHI,902
 redlite/_run.py,sha256=6iFiV4cWauNP9BmA06nCYpOs2XlCCKve8I776wHmXV4,6000
 redlite/_util.py,sha256=ETdg75k3BH6sFuUmrOxYuUpDFp7-Itcp0ID0gJ24naY,7207
@@ -23,14 +23,15 @@
 redlite/metric/rouge/__init__.py,sha256=cIlSzqPwpxzRUmJT3S9q-l7dua_XSuB0Sb2SIfe5E-I,1970
 redlite/model/__init__.py,sha256=ZTiL4K73g-nlK0eJZbh1pZjL2lGpGWbRWaCOThRYGRU,208
 redlite/model/_dummy.py,sha256=lGDMdF_EmTMZZwCWKj4mqqjotuZaWyzdLBl4tvf-g7w,690
 redlite/model/_ignore_system.py,sha256=JpJpzOZTUGhcd9Q8Vm2xVGkpuS_LXW2QvIy6sUj8iYQ,2515
 redlite/model/anthropic_model.py,sha256=zHj7UhoNo2Ji-FmYUWI1AcsfA9WqC7MuCnsdLSC8IpM,1388
 redlite/model/aws_bedrock_model.py,sha256=SPT5BGEpJB_1kN_1kx07Pay_ACFbliFe509qgoohX9k,4411
 redlite/model/hf_model.py,sha256=bywbM3yLAswuA2uK8YjpNrH2ipQH6MNU0PTLls0BUKA,3909
+redlite/model/hf_model_pipeline.py,sha256=OYSdYES3Kz6aTZ4PpdmLi3aeSpSglUKMqrzp4mvWzIA,1236
 redlite/model/openai_model.py,sha256=1PcLyzYYEL8fkp-DF_MBViV2dWXOkRg5pfo6LsaLd5A,966
 redlite/server/__init__.py,sha256=DwXZuEVYlCPgY_yapgP5yHoXhEuBRId_myXxpVpYDzY,296
 redlite/server/_app.py,sha256=YXr1Ft0jsnhoYMAl5BCXAcK9TLJ-KMmljbJTBOTZ2gU,3992
 redlite/server/resources/default/3rdpartylicenses.txt,sha256=tzaVZCL8EQnKnukRP4ApoYfWWn1RMJv6M9ZYGympBl8,14557
 redlite/server/resources/default/color.dae87a04d07ca92b.png,sha256=RzvIymmSMrwAKUVwJRXfhwOVqLuXRIlU11mkRdtFnnw,10355
 redlite/server/resources/default/favicon.ico,sha256=ucy7cQDhOulawYo6ntAIV_MhtjtJjx-3q6tQb8HEDpk,5430
 redlite/server/resources/default/fontawesome-webfont.2b13baa7dd4f54c9.eot,sha256=e_yrbbmdXPvxcFygU23ceFhUMsxfpBu9etDwCQM7KXk,165742
@@ -91,13 +92,13 @@
 redlite/server/resources/legacy/_app/immutable/nodes/5.CNhJU3OA.js,sha256=RTT_qn53DDGtegTDoqzfpzlQtlg-Jo91UTObZ4B-ZPU,2115
 redlite/server/resources/legacy/_app/immutable/nodes/6.BA5ucq1q.js,sha256=i-tB1t0VnQcjtq5h8fv1PuQiUuhUO4J6g-yhLJhbKn0,2672
 redlite/server/resources/legacy/_app/immutable/nodes/7.z3N0foJ1.js,sha256=kml7Q8w7jwiMFAX5j7IIkGc9NXeXqhqsiYpGAP0Ie7g,5744
 redlite/server/resources/legacy/_app/immutable/nodes/8.DkMbLct2.js,sha256=ic66fwCyaJkDx4_n4yQNo3Jr8fASXf1y_H17y9MQSFo,2132
 redlite/server/resources/legacy/_app/immutable/nodes/9.ZOpqgAss.js,sha256=10Ptj8B4QFZ7so7mCTkdU0e8IuA3bMwBjHWB06b2eSk,487
 redlite/zeno/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 redlite/zeno/upload.py,sha256=S-FSyfjm0A-tzL8eq16R-T6hS7rChyFi0sejTOtxP20,4152
-redlite-0.1.3.dist-info/LICENSE,sha256=kZKRsVQHychHYv7Sc7DjcIWxR4h97y7c-kfdo_GiXnQ,1071
-redlite-0.1.3.dist-info/METADATA,sha256=i2GKm5N72dflmxxZH0LHspPqefVDzaqHjlkMUUwHE7c,5631
-redlite-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-redlite-0.1.3.dist-info/entry_points.txt,sha256=F3u0t1T8WflnUv6dQxV99aNHg3TY_R6GIQ_1kucAP8Y,50
-redlite-0.1.3.dist-info/top_level.txt,sha256=fzFhwp7BwhuEW_IwLiIiOXjdgvL07JpsCqEaPCd4YJ0,8
-redlite-0.1.3.dist-info/RECORD,,
+redlite-0.1.4rc0.dist-info/LICENSE,sha256=kZKRsVQHychHYv7Sc7DjcIWxR4h97y7c-kfdo_GiXnQ,1071
+redlite-0.1.4rc0.dist-info/METADATA,sha256=bd30h_p047--fuNFBUJoM0NRzEaPvxkhqt3hOzxRJqI,5634
+redlite-0.1.4rc0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+redlite-0.1.4rc0.dist-info/entry_points.txt,sha256=F3u0t1T8WflnUv6dQxV99aNHg3TY_R6GIQ_1kucAP8Y,50
+redlite-0.1.4rc0.dist-info/top_level.txt,sha256=fzFhwp7BwhuEW_IwLiIiOXjdgvL07JpsCqEaPCd4YJ0,8
+redlite-0.1.4rc0.dist-info/RECORD,,
```

