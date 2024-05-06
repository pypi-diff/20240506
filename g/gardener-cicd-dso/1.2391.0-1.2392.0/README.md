# Comparing `tmp/gardener_cicd_dso-1.2391.0.tar.gz` & `tmp/gardener_cicd_dso-1.2392.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_dso-1.2391.0.tar", last modified: Thu May  2 10:06:45 2024, max compression
+gzip compressed data, was "gardener_cicd_dso-1.2392.0.tar", last modified: Mon May  6 09:19:08 2024, max compression
```

## Comparing `gardener_cicd_dso-1.2391.0.tar` & `gardener_cicd_dso-1.2392.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:06:45.234697 gardener_cicd_dso-1.2391.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-05-02 10:06:45.234697 gardener_cicd_dso-1.2391.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:06:45.230697 gardener_cicd_dso-1.2391.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    19358 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:06:45.230697 gardener_cicd_dso-1.2391.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4680 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8574 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     5564 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:06:45.234697 gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2024-05-02 10:06:45.000000 gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2024-05-02 10:06:45.000000 gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 10:06:45.000000 gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-05-02 10:06:45.000000 gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-02 10:06:45.000000 gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:06:45.234697 gardener_cicd_dso-1.2391.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7653 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17319 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    10709 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    29221 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)    10814 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-02 10:06:45.234697 gardener_cicd_dso-1.2391.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-05-02 10:05:25.000000 gardener_cicd_dso-1.2391.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:19:08.971234 gardener_cicd_dso-1.2392.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-06 09:19:08.971234 gardener_cicd_dso-1.2392.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:19:08.967234 gardener_cicd_dso-1.2392.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7945 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:19:08.967234 gardener_cicd_dso-1.2392.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8574 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:19:08.971234 gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-06 09:19:08.000000 gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2024-05-06 09:19:08.000000 gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:19:08.000000 gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-06 09:19:08.000000 gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-06 09:19:08.000000 gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:19:08.971234 gardener_cicd_dso-1.2392.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17319 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    10774 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    29384 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)    15022 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-06 09:19:08.971234 gardener_cicd_dso-1.2392.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-05-06 09:18:00.000000 gardener_cicd_dso-1.2392.0/setup.py
```

### Comparing `gardener_cicd_dso-1.2391.0/LICENSE` & `gardener_cicd_dso-1.2392.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/README.md` & `gardener_cicd_dso-1.2392.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/checkmarx/client.py` & `gardener_cicd_dso-1.2392.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/checkmarx/model.py` & `gardener_cicd_dso-1.2392.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/checkmarx/project.py` & `gardener_cicd_dso-1.2392.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/checkmarx/tablefmt.py` & `gardener_cicd_dso-1.2392.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/checkmarx/util.py` & `gardener_cicd_dso-1.2392.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/client.py` & `gardener_cicd_dso-1.2392.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/cnudie.py` & `gardener_cicd_dso-1.2392.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/model.py` & `gardener_cicd_dso-1.2392.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/report.py` & `gardener_cicd_dso-1.2392.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/routes.py` & `gardener_cicd_dso-1.2392.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/scan.py` & `gardener_cicd_dso-1.2392.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/clamav/util.py` & `gardener_cicd_dso-1.2392.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener_cicd_dso-1.2392.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/protecode/assessments.py` & `gardener_cicd_dso-1.2392.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/protecode/client.py` & `gardener_cicd_dso-1.2392.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/protecode/model.py` & `gardener_cicd_dso-1.2392.0/protecode/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,17 @@
 
     def reason(self):
         return self.raw['reason']
 
     def description(self):
         return self.raw.get('description')
 
+    def user(self) -> dict:
+        return self.raw.get('user')
+
     @property
     def modified(self) -> datetime.datetime:
         return dateutil.parser.isoparse(self.raw.get('modified'))
 
     def applies_to_same_vulnerability_as(self, other) -> bool:
         if not isinstance(other, Triage):
             return False
```

### Comparing `gardener_cicd_dso-1.2391.0/protecode/rescore.py` & `gardener_cicd_dso-1.2392.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/protecode/scanning.py` & `gardener_cicd_dso-1.2392.0/protecode/scanning.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,14 +398,15 @@
         resource_group: tuple[cnudie.iter.ResourceNode],
         processing_mode: pm.ProcessingMode,
         known_scan_results: dict[
             tuple[str, cm.ResourceIdentity, cm.ArtefactType|str],
             tuple[pm.Product],
         ],
         s3_client: 'botocore.client.S3',
+        delivery_client: delivery.client.DeliveryServiceClient=None,
         license_cfg: image_scan.LicenseCfg=None,
         cve_rescoring_rules: tuple[dso.cvss.RescoringRule]=tuple(),
         auto_assess_max_severity: dso.cvss.CVESeverity=dso.cvss.CVESeverity.MEDIUM,
         use_product_cache: bool=True,
         delete_inactive_products_after_seconds: int=None,
     ) -> collections.abc.Generator[dso.model.ArtefactMetadata, None, None]:
         r = resource_group[0].resource
@@ -514,14 +515,15 @@
 
             logger.info(f'post-processing of {scan_result.display_name()} done')
 
             yield from protecode.util.iter_artefact_metadata(
                 scanned_element=scanned_element,
                 scan_result=scan_result,
                 license_cfg=license_cfg,
+                delivery_client=delivery_client,
             )
 
 
 def _package_version_hints(
     component: cm.Component,
     artefact: cm.Artifact,
     result: pm.AnalysisResult,
@@ -714,14 +716,15 @@
             omit_resource_version=True,
         ))) > 1
         return tuple(processor.process(
             resource_group=resource_group,
             processing_mode=processing_mode,
             known_scan_results=known_scan_results,
             s3_client=s3_client,
+            delivery_client=delivery_client,
             license_cfg=license_cfg,
             cve_rescoring_rules=cve_rescoring_rules,
             auto_assess_max_severity=auto_assess_max_severity,
             use_product_cache=use_product_cache,
             delete_inactive_products_after_seconds=delete_inactive_products_after_seconds,
         ))
```

### Comparing `gardener_cicd_dso-1.2391.0/setup.dso.py` & `gardener_cicd_dso-1.2392.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2391.0/setup.py` & `gardener_cicd_dso-1.2392.0/setup.py`

 * *Files identical despite different names*

