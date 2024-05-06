# Comparing `tmp/nrtk-0.3.2.tar.gz` & `tmp/nrtk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrtk-0.3.2.tar", max compression
+gzip compressed data, was "nrtk-0.4.0.tar", max compression
```

## Comparing `nrtk-0.3.2.tar` & `nrtk-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10173 2024-05-01 21:45:55.704154 nrtk-0.3.2/LICENSE
--rw-r--r--   0        0        0      554 2024-05-01 21:45:55.704154 nrtk-0.3.2/NOTICE
--rw-r--r--   0        0        0     2006 2024-05-01 21:45:55.704154 nrtk-0.3.2/README.md
--rw-r--r--   0        0        0      246 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
--rw-r--r--   0        0        0     1986 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
--rw-r--r--   0        0        0     3302 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/PIL/__init__.py
--rw-r--r--   0        0        0     4774 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/PIL/enhance.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/cv2/__init__.py
--rw-r--r--   0        0        0     2702 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/cv2/blur.py
--rw-r--r--   0        0        0      706 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/nop_perturber.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/skimage/__init__.py
--rw-r--r--   0        0        0     6560 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/skimage/random_noise.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/__init__.py
--rw-r--r--   0        0        0     3449 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/perturber.py
--rw-r--r--   0        0        0     5051 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/scenario.py
--rw-r--r--   0        0        0     8599 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/sensor.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image_factory/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image_factory/generic/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image_factory/generic/step.py
--rw-r--r--   0        0        0     3160 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image_factory/pybsm.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/score_detections/__init__.py
--rw-r--r--   0        0        0     2661 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
--rw-r--r--   0        0        0     4277 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/coco_scorer.py
--rw-r--r--   0        0        0     1346 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/nop_scorer.py
--rw-r--r--   0        0        0     1617 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/random_scorer.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/interfaces/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/gen_blackbox_response.py
--rw-r--r--   0        0        0     5401 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/gen_classifier_blackbox_response.py
--rw-r--r--   0        0        0     5394 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/gen_object_detector_blackbox_response.py
--rw-r--r--   0        0        0     1121 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/perturb_image.py
--rw-r--r--   0        0        0     2750 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/perturb_image_factory.py
--rw-r--r--   0        0        0     1345 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/score_classifications.py
--rw-r--r--   0        0        0     1572 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/score_detections.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/interop/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/utils/__init__.py
--rw-r--r--   0        0        0     2667 2024-05-01 21:45:55.740154 nrtk-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 nrtk-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-06 20:03:32.927344 nrtk-0.4.0/LICENSE
+-rw-r--r--   0        0        0      554 2024-05-06 20:03:32.927344 nrtk-0.4.0/NOTICE
+-rw-r--r--   0        0        0     2006 2024-05-06 20:03:32.931344 nrtk-0.4.0/README.md
+-rw-r--r--   0        0        0      246 2024-05-06 20:03:32.959344 nrtk-0.4.0/nrtk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
+-rw-r--r--   0        0        0     1986 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
+-rw-r--r--   0        0        0     3302 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/PIL/__init__.py
+-rw-r--r--   0        0        0     4774 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/PIL/enhance.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/cv2/__init__.py
+-rw-r--r--   0        0        0     2702 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/cv2/blur.py
+-rw-r--r--   0        0        0      706 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/nop_perturber.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/skimage/__init__.py
+-rw-r--r--   0        0        0     6560 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/skimage/random_noise.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/__init__.py
+-rw-r--r--   0        0        0     3569 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/perturber.py
+-rw-r--r--   0        0        0     5067 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/scenario.py
+-rw-r--r--   0        0        0     8611 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/sensor.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image_factory/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image_factory/generic/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image_factory/generic/step.py
+-rw-r--r--   0        0        0     3160 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image_factory/pybsm.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/score_detections/__init__.py
+-rw-r--r--   0        0        0     2661 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
+-rw-r--r--   0        0        0     4277 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/coco_scorer.py
+-rw-r--r--   0        0        0     1346 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/nop_scorer.py
+-rw-r--r--   0        0        0     1617 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/random_scorer.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/interfaces/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/gen_blackbox_response.py
+-rw-r--r--   0        0        0     5401 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/gen_classifier_blackbox_response.py
+-rw-r--r--   0        0        0     5394 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/gen_object_detector_blackbox_response.py
+-rw-r--r--   0        0        0     1121 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/perturb_image.py
+-rw-r--r--   0        0        0     2750 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/perturb_image_factory.py
+-rw-r--r--   0        0        0     1345 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/score_classifications.py
+-rw-r--r--   0        0        0     1572 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/score_detections.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/interop/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.491575 nrtk-0.4.0/nrtk/py.typed
+-rw-r--r--   0        0        0        0 2024-05-06 20:11:48.491575 nrtk-0.4.0/nrtk/utils/__init__.py
+-rw-r--r--   0        0        0     2855 2024-05-06 20:03:32.967344 nrtk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 nrtk-0.4.0/PKG-INFO
```

### Comparing `nrtk-0.3.2/LICENSE` & `nrtk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/NOTICE` & `nrtk-0.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/README.md` & `nrtk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py` & `nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py` & `nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/generic/PIL/enhance.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/generic/PIL/enhance.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/generic/cv2/blur.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/generic/cv2/blur.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/generic/nop_perturber.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/generic/nop_perturber.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/generic/skimage/random_noise.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/generic/skimage/random_noise.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/perturber.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/perturber.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 from typing import Any, Dict
 
 import numpy as np
-import pybsm
+from pybsm.simulation import RefImage, simulate_image
 
 from nrtk.impls.perturb_image.pybsm.sensor import PybsmSensor
 from nrtk.impls.perturb_image.pybsm.scenario import PybsmScenario
 from nrtk.interfaces.perturb_image import PerturbImage
 
 
 class PybsmPerturber(PerturbImage):
@@ -31,16 +31,14 @@
 
         for k in kwargs:
             if hasattr(self.sensor, k):
                 setattr(self.sensor, k, kwargs[k])
             elif hasattr(self.scenario, k):
                 setattr(self.scenario, k, kwargs[k])
 
-        self.metrics = pybsm.niirs(self.sensor, self.scenario)
-
         if reflectance_range.shape[0] != 2:
             raise ValueError(f"Reflectance range array must have length of 2, got {reflectance_range.shape[0]}")
         if reflectance_range[0] >= reflectance_range[1]:
             raise ValueError(f"Reflectance range array values must be strictly ascending, got {reflectance_range}")
         self.reflectance_range = reflectance_range
 
         # this is key:value record of the thetas use for perturbing
@@ -57,20 +55,24 @@
             ) -> np.ndarray:
         """
         :raises: ValueError if 'img_gsd' not present in additional_params
         """
         if 'img_gsd' not in additional_params:
             raise ValueError("'img_gsd' must be present in image metadata for this perturber")
 
-        perturbed = pybsm.metrics2image(
-                    self.metrics,
+        ref_img = RefImage(
                     image,
                     additional_params['img_gsd'],
                     np.array([image.min(), image.max()]),
-                    self.reflectance_range)[-1]
+                    self.reflectance_range)
+
+        perturbed = simulate_image(
+                    ref_img,
+                    self.sensor(),
+                    self.scenario())[-1]
 
         min = perturbed.min()
         den = perturbed.max()-min
         perturbed -= min
         perturbed /= den
         perturbed *= 255
 
@@ -83,18 +85,18 @@
             ) -> np.ndarray:
         """
         Alias for :meth:`.NIIRS.apply`.
         """
         return self.perturb(image, additional_params)
 
     def __str__(self) -> str:
-        return self.metrics.name
+        return self.sensor.name + " " + self.scenario.name
 
     def __repr__(self) -> str:
-        return self.metrics.name
+        return self.sensor.name + " " + self.scenario.name
 
     def get_config(self) -> Dict[str, Any]:
         config = {
             'sensor': self.sensor.get_config(),
             'scenario': self.scenario.get_config(),
             'reflectance_range': self.reflectance_range
         }
```

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/scenario.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/scenario.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 from typing import Dict, Optional
 
-import pybsm
+from pybsm.simulation.scenario import Scenario
 from smqtk_core import Plugfigurable
 
 
 class PybsmScenario(Plugfigurable):
     """
     Wrapper for pybsm.scenario.
 
@@ -90,28 +90,28 @@
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
 
-    def create_scenario(self) -> pybsm.scenario:
-        S = pybsm.scenario(self.name, self.ihaze, self.altitude, self.groundRange)
+    def create_scenario(self) -> Scenario:
+        S = Scenario(self.name, self.ihaze, self.altitude, self.groundRange)
         S.aircraftSpeed = self.aircraftSpeed
         S.targetReflectance = self.targetReflectance
         S.targetTemperature = self.targetTemperature
         S.backgroundReflectance = self.backgroundReflectance
         S.backgroundTemperature = self.backgroundTemperature
         S.haWindspeed = self.haWindspeed
         S.cn2at1m = self.cn2at1m
         return S
 
     def __call__(
         self
-    ) -> pybsm.scenario:
+    ) -> Scenario:
         """
         Alias for :meth:`.StoreScenario.create_scenario`.
         """
         return self.create_scenario()
 
     def get_config(self) -> Dict[str, Any]:
         return {
```

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/sensor.py` & `nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from typing import Any
 from typing import Dict, Optional
 
 import numpy as np
-import pybsm
+from pybsm.simulation.sensor import Sensor
 from smqtk_core import Plugfigurable
 
 
 class PybsmSensor(Plugfigurable):
     """
     Wrapper for pybsm.sensor.
 
@@ -177,16 +177,16 @@
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
 
-    def create_sensor(self) -> pybsm.sensor:
-        S = pybsm.sensor(self.name, self.D, self.f, self.px, self.optTransWavelengths)
+    def create_sensor(self) -> Sensor:
+        S = Sensor(self.name, self.D, self.f, self.px, self.optTransWavelengths)
         S.opticsTransmission = self.opticsTransmission
         S.eta = self.eta
         S.py = self.py
         S.wx = self.wx
         S.wy = self.wy
         S.intTime = self.intTime
         S.darkCurrent = self.darkCurrent
@@ -196,15 +196,15 @@
         S.bitdepth = self.bitdepth
         S.qewavelengths = self.qewavelengths
         S.qe = self.qe
         return S
 
     def __call__(
         self
-    ) -> pybsm.sensor:
+    ) -> Sensor:
         """
         Alias for :meth:`.StoreSensor.sensor`.
         """
         return self.create_sensor()
 
     def get_config(self) -> Dict[str, Any]:
         return {
```

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image_factory/generic/step.py` & `nrtk-0.4.0/nrtk/impls/perturb_image_factory/generic/step.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/perturb_image_factory/pybsm.py` & `nrtk-0.4.0/nrtk/impls/perturb_image_factory/pybsm.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py` & `nrtk-0.4.0/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/score_detections/coco_scorer.py` & `nrtk-0.4.0/nrtk/impls/score_detections/coco_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/score_detections/nop_scorer.py` & `nrtk-0.4.0/nrtk/impls/score_detections/nop_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/impls/score_detections/random_scorer.py` & `nrtk-0.4.0/nrtk/impls/score_detections/random_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/gen_blackbox_response.py` & `nrtk-0.4.0/nrtk/interfaces/gen_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/gen_classifier_blackbox_response.py` & `nrtk-0.4.0/nrtk/interfaces/gen_classifier_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/gen_object_detector_blackbox_response.py` & `nrtk-0.4.0/nrtk/interfaces/gen_object_detector_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/perturb_image.py` & `nrtk-0.4.0/nrtk/interfaces/perturb_image.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/perturb_image_factory.py` & `nrtk-0.4.0/nrtk/interfaces/perturb_image_factory.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/score_classifications.py` & `nrtk-0.4.0/nrtk/interfaces/score_classifications.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/nrtk/interfaces/score_detections.py` & `nrtk-0.4.0/nrtk/interfaces/score_detections.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.2/pyproject.toml` & `nrtk-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 ###############################################################################
 [tool.poetry]
 name = "nrtk"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # This package prefers to use the strict numbering standard when possible.
-version = "0.3.2"
-description = ""
+version = "0.4.0"
+description = "An open source toolkit for evaluating the natural robustness of computer vision algorithms."
 license = "Apache-2.0"
 authors = ["Kitware, Inc. <nrtk@kitware.com>"]
 readme = "README.md"
 packages = [{include = "nrtk"}]
 documentation = "https://nrtk.readthedocs.io/"
 classifiers = [
     'Development Status :: 3 - Alpha',
@@ -27,24 +27,27 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-numpy = ">=1.18"
+numpy = [
+    {version = ">=1.23.1,<1.25", python = ">=3.8,<3.12"},
+    {version = ">=1.26", python = "^3.12"}
+]
 opencv-python = ">=4.6"
 Pillow = ">=10.2.0"
 scikit-image = ">=0.21"
 smqtk-classifier = ">=0.19.0"
 smqtk-core = ">=0.19"
 smqtk-detection = ">=0.19.0"
 smqtk-image-io = ">=0.17.1"
 tqdm = ">=4.64"
-pybsm = "<0.2.0"
+pybsm = ">=0.2.0"
 pycocotools = ">=2.0.6"
 setuptools = ">=65.6.1"
 
 [tool.poetry.extras]
 
 [tool.poetry.group.dev.dependencies]
 # Linting
```

### Comparing `nrtk-0.3.2/PKG-INFO` & `nrtk-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nrtk
-Version: 0.3.2
-Summary: 
+Version: 0.4.0
+Summary: An open source toolkit for evaluating the natural robustness of computer vision algorithms.
 License: Apache-2.0
 Author: Kitware, Inc.
 Author-email: nrtk@kitware.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -15,17 +15,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: Pillow (>=10.2.0)
-Requires-Dist: numpy (>=1.18)
+Requires-Dist: numpy (>=1.23.1,<1.25) ; python_version >= "3.8" and python_version < "3.12"
+Requires-Dist: numpy (>=1.26) ; python_version >= "3.12" and python_version < "4.0"
 Requires-Dist: opencv-python (>=4.6)
-Requires-Dist: pybsm (<0.2.0)
+Requires-Dist: pybsm (>=0.2.0)
 Requires-Dist: pycocotools (>=2.0.6)
 Requires-Dist: scikit-image (>=0.21)
 Requires-Dist: setuptools (>=65.6.1)
 Requires-Dist: smqtk-classifier (>=0.19.0)
 Requires-Dist: smqtk-core (>=0.19)
 Requires-Dist: smqtk-detection (>=0.19.0)
 Requires-Dist: smqtk-image-io (>=0.17.1)
```

