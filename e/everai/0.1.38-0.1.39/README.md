# Comparing `tmp/everai-0.1.38-py3-none-any.whl.zip` & `tmp/everai-0.1.39-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 435401 bytes, number of entries: 417
+Zip file size: 436111 bytes, number of entries: 419
 -rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 07:43 everai/__init__.py
 -rw-r--r--  2.0 unx     1214 b- defN 24-Apr-28 08:33 everai/constants.py
--rw-r--r--  2.0 unx       23 b- defN 24-Apr-29 10:55 everai/version.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-06 07:04 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
 -rw-r--r--  2.0 unx    15076 b- defN 24-Apr-25 09:03 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
 -rw-r--r--  2.0 unx     3667 b- defN 24-Apr-23 15:20 everai/app/app.py
 -rw-r--r--  2.0 unx    12187 b- defN 24-Apr-28 08:34 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1791 b- defN 24-Apr-24 07:37 everai/app/app_runner.py
 -rw-r--r--  2.0 unx     3223 b- defN 24-Apr-24 05:08 everai/app/app_runtime.py
@@ -20,15 +20,15 @@
 -rw-r--r--  2.0 unx      291 b- defN 24-Apr-23 15:51 everai/autoscaling/autoscaling_policy.py
 -rw-r--r--  2.0 unx      184 b- defN 24-Apr-23 13:29 everai/autoscaling/autoscaling_policy.pyi
 -rw-r--r--  2.0 unx     2003 b- defN 24-Apr-25 09:05 everai/autoscaling/factors.py
 -rw-r--r--  2.0 unx      698 b- defN 24-Apr-16 13:43 everai/autoscaling/session_autoscaling.py
 -rw-r--r--  2.0 unx     4845 b- defN 24-Apr-25 09:05 everai/autoscaling/simple_autoscaling.py
 -rw-r--r--  2.0 unx       64 b- defN 24-Mar-29 07:34 everai/autoscaling/wellknown.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 06:48 everai/commands/__init__.py
--rw-r--r--  2.0 unx     1683 b- defN 24-Apr-23 14:04 everai/commands/everai_cli.py
+-rw-r--r--  2.0 unx     1758 b- defN 24-May-06 07:03 everai/commands/everai_cli.py
 -rw-r--r--  2.0 unx      163 b- defN 24-Apr-23 04:14 everai/commands/app/__init__.py
 -rw-r--r--  2.0 unx     1315 b- defN 24-Apr-29 10:54 everai/commands/app/app.py
 -rw-r--r--  2.0 unx     1407 b- defN 24-Apr-23 07:57 everai/commands/app/create.py
 -rw-r--r--  2.0 unx      676 b- defN 24-Apr-23 07:57 everai/commands/app/deploy.py
 -rw-r--r--  2.0 unx      765 b- defN 24-Apr-23 07:57 everai/commands/app/get.py
 -rw-r--r--  2.0 unx      791 b- defN 24-Apr-24 06:22 everai/commands/app/list.py
 -rw-r--r--  2.0 unx      773 b- defN 24-Apr-23 07:57 everai/commands/app/pause.py
@@ -63,14 +63,16 @@
 -rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/secret/__init__.py
 -rw-r--r--  2.0 unx     1833 b- defN 24-Apr-24 10:42 everai/commands/secret/create.py
 -rw-r--r--  2.0 unx      668 b- defN 24-Apr-24 10:41 everai/commands/secret/delete.py
 -rw-r--r--  2.0 unx      783 b- defN 24-Apr-24 10:43 everai/commands/secret/get.py
 -rw-r--r--  2.0 unx      765 b- defN 24-Apr-24 10:41 everai/commands/secret/list.py
 -rw-r--r--  2.0 unx     1248 b- defN 24-Apr-25 10:15 everai/commands/secret/secret.py
 -rw-r--r--  2.0 unx     1921 b- defN 24-Apr-24 10:40 everai/commands/secret/update.py
+-rw-r--r--  2.0 unx       66 b- defN 24-May-06 07:03 everai/commands/version/__init__.py
+-rw-r--r--  2.0 unx      561 b- defN 24-May-06 07:03 everai/commands/version/version.py
 -rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/volume/__init__.py
 -rw-r--r--  2.0 unx      813 b- defN 24-Apr-23 07:08 everai/commands/volume/create.py
 -rw-r--r--  2.0 unx     1679 b- defN 24-Apr-23 07:09 everai/commands/volume/delete.py
 -rw-r--r--  2.0 unx      752 b- defN 24-Apr-23 07:09 everai/commands/volume/get.py
 -rw-r--r--  2.0 unx      747 b- defN 24-Apr-24 06:20 everai/commands/volume/list.py
 -rw-r--r--  2.0 unx     1507 b- defN 24-Apr-23 07:09 everai/commands/volume/pull.py
 -rw-r--r--  2.0 unx      753 b- defN 24-Apr-23 07:09 everai/commands/volume/push.py
@@ -406,14 +408,14 @@
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 10:55 everai-0.1.38.dist-info/LICENSE
--rw-r--r--  2.0 unx     1951 b- defN 24-Apr-29 10:55 everai-0.1.38.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 10:55 everai-0.1.38.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-29 10:55 everai-0.1.38.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-29 10:55 everai-0.1.38.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    41708 b- defN 24-Apr-29 10:55 everai-0.1.38.dist-info/RECORD
-417 files, 1350077 bytes uncompressed, 367461 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 07:04 everai-0.1.39.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1951 b- defN 24-May-06 07:04 everai-0.1.39.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 07:04 everai-0.1.39.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-May-06 07:04 everai-0.1.39.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-06 07:04 everai-0.1.39.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    41888 b- defN 24-May-06 07:04 everai-0.1.39.dist-info/RECORD
+419 files, 1350959 bytes uncompressed, 367881 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -198,14 +198,20 @@
 
 Filename: everai/commands/secret/secret.py
 Comment: 
 
 Filename: everai/commands/secret/update.py
 Comment: 
 
+Filename: everai/commands/version/__init__.py
+Comment: 
+
+Filename: everai/commands/version/version.py
+Comment: 
+
 Filename: everai/commands/volume/__init__.py
 Comment: 
 
 Filename: everai/commands/volume/create.py
 Comment: 
 
 Filename: everai/commands/volume/delete.py
@@ -1227,26 +1233,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.38.dist-info/LICENSE
+Filename: everai-0.1.39.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.38.dist-info/METADATA
+Filename: everai-0.1.39.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.38.dist-info/WHEEL
+Filename: everai-0.1.39.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.38.dist-info/entry_points.txt
+Filename: everai-0.1.39.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.38.dist-info/top_level.txt
+Filename: everai-0.1.39.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.38.dist-info/RECORD
+Filename: everai-0.1.39.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.38"
+__version__ = "0.1.39"
```

## everai/commands/everai_cli.py

```diff
@@ -7,14 +7,15 @@
 from everai.commands.config import ConfigCommand
 from everai.commands.auth import LoginCommand
 from everai.commands.auth import LogoutCommand
 from everai.commands.configmap import ConfigMapCommand
 from everai.commands.run import RunCommand
 from everai.commands.image import ImageCommand
 from everai.commands.secret import SecretCommand
+from everai.commands.version import VersionCommand
 from everai.commands.volume import VolumeCommand
 from everai.commands.autoscaling import AutoscalingCommand
 from everai.commands.worker import WorkerCommand
 from everai.constants import COMMAND_ENTRY
 import everai.utils.verbose as vb
 
 
@@ -40,14 +41,15 @@
         ImageCommand,
         RunCommand,
         AppCommand,
         SecretCommand,
         VolumeCommand,
         AutoscalingCommand,
         ConfigMapCommand,
+        VersionCommand,
     ])
 
     argcomplete.autocomplete(parser)
 
     args = parser.parse_args()
     if not hasattr(args, "func"):
         parser.print_help()
```

## Comparing `everai-0.1.38.dist-info/METADATA` & `everai-0.1.39.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.38
+Version: 0.1.39
 Summary: Client library to manage everai infrastructure
 Author-email: mc <mc@expvent.com>
 Maintainer-email: mc <mc@expvent.com>
 Project-URL: Homepage, https://everai.expvent.com
 Project-URL: Documentation, https://everai.expvent.com
 Project-URL: Repository, https://github.com/expvent/everai
 Project-URL: Issues, https://github.com/expvent/everai/issues
```

## Comparing `everai-0.1.38.dist-info/RECORD` & `everai-0.1.39.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 everai/__init__.py,sha256=AbgR3tVRy6TETgwXyJITEnET1TSFpEAEqQJJqzReYqQ,66
 everai/constants.py,sha256=6tvPKHYvL1H5ippD2YkwCerLhKftIiOg-SVtFLtVYN4,1214
-everai/version.py,sha256=iqMsqiw28paXOQhpmbrJrO6OnNN9YpR83VgJimFDq8k,23
+everai/version.py,sha256=sfc5YqMhonehojmfXWQszjknUHF_Q-G6tt4E1pfsXOY,23
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
 everai/api/api.py,sha256=FH47WVqBWaHrVCtYOzVYQLXW5w4cQZTJhC2fY2gSAqM,15076
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
 everai/app/app.py,sha256=fweD6GNTR0vCCFvYDXSzZOIcphOEhM5nOlcXDA_kB3M,3667
 everai/app/app_manager.py,sha256=3hR5S8ZvQRc-4C1LpeHVNZd0ztANdqgKbjj6cfI6u70,12187
 everai/app/app_runner.py,sha256=HVlOLweFX-C2kBbgyVwuDz4vfGzQ6uzHpNVzikQhRfA,1791
 everai/app/app_runtime.py,sha256=zyj63A6VfM1P3WL7LVW_mcy9xmMwKueKzTcJduGMwSo,3223
@@ -19,15 +19,15 @@
 everai/autoscaling/autoscaling_policy.py,sha256=i-znbnCG3w1ovmInhFlEwDdC54MFQ3Q9qhvK86jboIE,291
 everai/autoscaling/autoscaling_policy.pyi,sha256=u_OuXVbYDdu09a-ej0j3eURTMeKfJuqvEOHGB8kifG8,184
 everai/autoscaling/factors.py,sha256=w6KurrVSqWGmrqNkbIKD7vj-6kZyJYvYyAFc0Tyi-T0,2003
 everai/autoscaling/session_autoscaling.py,sha256=tnNs91zBLFfWA7kuvlJEs5eQ_MHUUa6R0UAXhxOBEc0,698
 everai/autoscaling/simple_autoscaling.py,sha256=3aDlkLtpTvhPHZOiK2mmPzn9gj3mrldhJV01dNioibo,4845
 everai/autoscaling/wellknown.py,sha256=kUa7XlknGph-XR_qjI2PpEAcNYANXtlXctvHi-OsxVM,64
 everai/commands/__init__.py,sha256=o1tcmQ2Hds3eW_8ybbs39rlUWh5uu0dQ4DkgdEnoMGI,55
-everai/commands/everai_cli.py,sha256=3-FEdOHXG5Tu5Kfm_Z_JnDaJOXn-AbEeowzfBP47PHU,1683
+everai/commands/everai_cli.py,sha256=V-X5cdDbt3sEQORP_unDt5ZK6c_344XzclYIYgdE7S8,1758
 everai/commands/app/__init__.py,sha256=bZsGYyqZz9ewwBfaEknc6dp8H7_z-QmXK5IyuAEfNto,163
 everai/commands/app/app.py,sha256=z1eJvmKtnZDVM2yMTZNhIIUdvlSFjIu0qVgm8ngUtH4,1315
 everai/commands/app/create.py,sha256=KEN7KV0yHCqmwFmEqq2EB8b-gQ-Z8pny4joBBG4xr6A,1407
 everai/commands/app/deploy.py,sha256=o0yF3qHbpqwcMn5TY83UbZkwCPIt4UA8ckmxHQDCl9o,676
 everai/commands/app/get.py,sha256=wXmC_s4e5ed9q1INNFbAiZHhuGccWAYedfMIiGO60_0,765
 everai/commands/app/list.py,sha256=UVx8-T01eBIicX6Xi6BXtnOc6qe3pVqE6GmiL93bgp8,791
 everai/commands/app/pause.py,sha256=LtQrxglQ9kgM0k_h05RaV9ZzRv18kiMY3pn33Xm4B68,773
@@ -62,14 +62,16 @@
 everai/commands/secret/__init__.py,sha256=O4Tj-pg2EGxcF7y_HWLsY0PAxE-cB09iGmyzrvaALiI,63
 everai/commands/secret/create.py,sha256=okYRA3JDdrP7o6l_82C0_CLFruOEEMGaoALHCprBmxk,1833
 everai/commands/secret/delete.py,sha256=Us6aoFymKcq0vkC6pZb9aTvYjvC5W--ZHNHT9UvY3a0,668
 everai/commands/secret/get.py,sha256=bfOUasLLVMAHacfr8xUUs-Ah_2FB_mr8VnIKvFX_oxI,783
 everai/commands/secret/list.py,sha256=1ynwbElHGKldMDheplUx4Q73UGpuByefpyHC0bIYs3k,765
 everai/commands/secret/secret.py,sha256=nk7T_Q9EdQGllSSTNDLFivxPg4qFz1DEcbnY_U0B8NI,1248
 everai/commands/secret/update.py,sha256=Ukp0xzahxKeiEmuYKdEbelvWT20DBGak0FS5blLU-cg,1921
+everai/commands/version/__init__.py,sha256=gTsFsCRNV8TvUgZ0Vbvqi_7RQ6mChgi9Wf5o-EBBdUo,66
+everai/commands/version/version.py,sha256=Y98SgjQ21-wwve8wZVhDZDtfwaQfpp3n5X0cM72_S7g,561
 everai/commands/volume/__init__.py,sha256=UlxXpx7spko6zt5QASgQf3FvKMFWVDs0z6kc9ET_Z3M,63
 everai/commands/volume/create.py,sha256=zX4Jnx81NQjK82tZsatl-ZCtQKKf5mcMz2TTRmg4Szo,813
 everai/commands/volume/delete.py,sha256=OzKZ9AN4tHQO9orWhUeIxgVxfhHgGDKWF2PG95yHgC8,1679
 everai/commands/volume/get.py,sha256=ruLx6zRKnmUZdpXhxHF2C1XIVgGaa1zLlnfU-nX0bfE,752
 everai/commands/volume/list.py,sha256=YmjnCWIl3pyDxE-F7rOmhDZu2PrlGFsR6MacnJlOFmY,747
 everai/commands/volume/pull.py,sha256=sJKByR1qWxCreb6BMj3kfbhM7w2UuO5eKySDMPtp7lQ,1507
 everai/commands/volume/push.py,sha256=lH_EB0joXOKGY4lPalWkmAPnCesDiytfhzfW_0E4jQA,753
@@ -405,13 +407,13 @@
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.38.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.38.dist-info/METADATA,sha256=UmTffTe5PYIord7htaTuzIazt2ufvB0efsQ6wUtleHk,1951
-everai-0.1.38.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.38.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.38.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.38.dist-info/RECORD,,
+everai-0.1.39.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.39.dist-info/METADATA,sha256=zvRvZ5gBt71KVRHvTyuJQ1OiQkw-OoZ1XwH-7HqxMfw,1951
+everai-0.1.39.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.39.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.39.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.39.dist-info/RECORD,,
```

