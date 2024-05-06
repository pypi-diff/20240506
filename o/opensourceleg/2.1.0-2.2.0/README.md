# Comparing `tmp/opensourceleg-2.1.0.tar.gz` & `tmp/opensourceleg-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-2.1.0.tar", max compression
+gzip compressed data, was "opensourceleg-2.2.0.tar", max compression
```

## Comparing `opensourceleg-2.1.0.tar` & `opensourceleg-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    26526 2024-03-11 16:37:38.238392 opensourceleg-2.1.0/LICENSE
--rw-r--r--   0        0        0     4155 2023-10-24 15:09:08.036501 opensourceleg-2.1.0/README.md
--rw-r--r--   0        0        0      415 2023-10-12 15:36:40.401967 opensourceleg-2.1.0/opensourceleg/__init__.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002099 opensourceleg-2.1.0/opensourceleg/control/__init__.py
--rw-r--r--   0        0        0     7309 2024-03-11 17:27:03.438226 opensourceleg-2.1.0/opensourceleg/control/compiled_controller.py
--rw-r--r--   0        0        0    15826 2024-03-11 17:27:03.438733 opensourceleg-2.1.0/opensourceleg/control/state_machine.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002819 opensourceleg-2.1.0/opensourceleg/hardware/__init__.py
--rw-r--r--   0        0        0    32561 2024-03-12 15:25:41.513775 opensourceleg-2.1.0/opensourceleg/hardware/actuators.py
--rw-r--r--   0        0        0    13392 2024-03-11 17:27:03.440004 opensourceleg-2.1.0/opensourceleg/hardware/joints.py
--rw-r--r--   0        0        0    19583 2024-03-11 17:27:03.440657 opensourceleg-2.1.0/opensourceleg/hardware/sensors.py
--rw-r--r--   0        0        0     6501 2024-03-11 17:27:03.441212 opensourceleg-2.1.0/opensourceleg/hardware/thermal.py
--rw-r--r--   0        0        0    13725 2024-03-11 17:27:03.441382 opensourceleg-2.1.0/opensourceleg/osl.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.003682 opensourceleg-2.1.0/opensourceleg/tools/__init__.py
--rw-r--r--   0        0        0     5908 2024-03-11 17:27:03.441623 opensourceleg-2.1.0/opensourceleg/tools/logger.py
--rw-r--r--   0        0        0     4093 2024-03-11 17:27:03.441733 opensourceleg-2.1.0/opensourceleg/tools/units.py
--rw-r--r--   0        0        0    11696 2024-03-12 15:21:54.650251 opensourceleg-2.1.0/opensourceleg/tools/utilities.py
--rw-r--r--   0        0        0     3798 2024-03-12 15:24:24.334650 opensourceleg-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 opensourceleg-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-03-11 16:37:38.238392 opensourceleg-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4158 2024-04-11 18:15:50.369362 opensourceleg-2.2.0/README.md
+-rw-r--r--   0        0        0      415 2023-10-12 15:36:40.401967 opensourceleg-2.2.0/opensourceleg/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002099 opensourceleg-2.2.0/opensourceleg/control/__init__.py
+-rw-r--r--   0        0        0     7309 2024-04-22 16:55:56.739331 opensourceleg-2.2.0/opensourceleg/control/compiled_controller.py
+-rw-r--r--   0        0        0    15826 2024-04-22 16:55:56.739869 opensourceleg-2.2.0/opensourceleg/control/state_machine.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002819 opensourceleg-2.2.0/opensourceleg/hardware/__init__.py
+-rw-r--r--   0        0        0    34576 2024-05-06 17:40:50.560221 opensourceleg-2.2.0/opensourceleg/hardware/actuators.py
+-rw-r--r--   0        0        0    12842 2024-05-06 17:26:49.228964 opensourceleg-2.2.0/opensourceleg/hardware/joints.py
+-rw-r--r--   0        0        0    19890 2024-05-06 17:36:59.460237 opensourceleg-2.2.0/opensourceleg/hardware/sensors.py
+-rw-r--r--   0        0        0     6501 2024-04-22 16:55:56.743110 opensourceleg-2.2.0/opensourceleg/hardware/thermal.py
+-rw-r--r--   0        0        0    14085 2024-05-06 17:36:33.700442 opensourceleg-2.2.0/opensourceleg/osl.py
+-rw-r--r--   0        0        0     6352 2024-05-06 17:36:33.057100 opensourceleg-2.2.0/opensourceleg/safety/sensors.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.003682 opensourceleg-2.2.0/opensourceleg/tools/__init__.py
+-rw-r--r--   0        0        0     5920 2024-05-06 17:18:03.548467 opensourceleg-2.2.0/opensourceleg/tools/logger.py
+-rw-r--r--   0        0        0     4093 2024-04-22 16:55:56.744516 opensourceleg-2.2.0/opensourceleg/tools/units.py
+-rw-r--r--   0        0        0    11696 2024-04-22 16:57:48.693201 opensourceleg-2.2.0/opensourceleg/tools/utilities.py
+-rw-r--r--   0        0        0     3797 2024-05-06 17:39:28.083443 opensourceleg-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 opensourceleg-2.2.0/PKG-INFO
```

### Comparing `opensourceleg-2.1.0/LICENSE` & `opensourceleg-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.1.0/README.md` & `opensourceleg-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 
 </div>
 
 <br>
 
 ## Installation
 
-The easiest and quickest way to install the *opensourceleg* library is via [pip](https://pip.pypa.io/en/stable/):
+The easiest and quickest way to install the _opensourceleg_ library is via [pip](https://pip.pypa.io/en/stable/):
 
 ```bash
 pip install opensourceleg
 ```
 
-> If you plan on installing the *opensourceleg* library on a Raspberry Pi, we recommend using [opensourcelegpi](https://github.com/neurobionics/opensourcelegpi) tool, which is a cloud-based CI tool used to build an up-to-date OS for a [Raspberry Pi](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/) that can be used headless/GUI-less to control autonomous/remote robotic systems. This tool bundles the *opensourceleg* library and its dependencies into a single OS image, which can be flashed onto a microSD card and used to boot a Raspberry Pi. For more information, click [here](https://github.com/neurobionics/opensourcelegpi/blob/main/README.md).
+> If you plan on installing the _opensourceleg_ library on a Raspberry Pi, we recommend using [opensourcelegpi](https://github.com/neurobionics/opensourcelegpi) tool, which is a cloud-based CI tool used to build an up-to-date OS for a [Raspberry Pi](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/) that can be used headless/GUI-less to control autonomous/remote robotic systems. This tool bundles the _opensourceleg_ library and its dependencies into a single OS image, which can be flashed onto a microSD card and used to boot a Raspberry Pi. For more information, click [here](https://github.com/neurobionics/opensourcelegpi/blob/main/README.md).
 
 ### Developing
-To modify, develop, or contribute to the [opensourceleg](https://pypi.org/project/opensourceleg/) library, we encourage you to install [Poetry](https://python-poetry.org), which is a python packaging and dependency management tool. Once you have Poetry installed on your local machine, you can clone the repository and install the *opensourceleg* library by running the following commands:
+
+To modify, develop, or contribute to the [opensourceleg](https://pypi.org/project/opensourceleg/) library, we encourage you to install [Poetry](https://python-poetry.org), which is a python packaging and dependency management tool. Once you have Poetry installed on your local machine, you can clone the repository and install the _opensourceleg_ library by running the following commands:
 
 ```bash
 git clone https://github.com/neurobionics/opensourceleg.git
 cd opensourceleg
 
 poetry install
 poetry shell
@@ -44,19 +45,19 @@
 
 ## Documentation
 
 You can find tutorials and API documentation at [opensourceleg.readthedocs.io](https://opensourceleg.readthedocs.io/en/latest/).
 
 ## License
 
-The *opensourceleg* library is licensed under the terms of the [GPL-3.0 license](https://github.com/neurobionics/opensourceleg/raw/main/LICENSE). This license grants users a number of freedoms:
+The _opensourceleg_ library is licensed under the terms of the [LGPL-v2.1 license](https://github.com/neurobionics/opensourceleg/raw/main/LICENSE). This license grants users a number of freedoms:
 
-* You are free to use the *opensourceleg* library for any purpose.
-* You are free to modify the *opensourceleg* library to suit your needs.
-* You can study how the *opensourceleg* library works and change it.
-* You can distribute modified versions of the *opensourceleg* library.
+- You are free to use the _opensourceleg_ library for any purpose.
+- You are free to modify the _opensourceleg_ library to suit your needs.
+- You can study how the _opensourceleg_ library works and change it.
+- You can distribute modified versions of the _opensourceleg_ library.
 
 The GPL license ensures that all these freedoms are protected, now and in the future, requiring everyone to share their modifications when they also share the library in public.
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! For more details, read our [contribution guidelines](https://github.com/neurobionics/opensourceleg/blob/11765f7f7dd94e5d8699675149d5ff3596ea01b8/CONTRIBUTING.md).
```

### Comparing `opensourceleg-2.1.0/opensourceleg/control/compiled_controller.py` & `opensourceleg-2.2.0/opensourceleg/control/compiled_controller.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.1.0/opensourceleg/control/state_machine.py` & `opensourceleg-2.2.0/opensourceleg/control/state_machine.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.1.0/opensourceleg/hardware/actuators.py` & `opensourceleg-2.2.0/opensourceleg/hardware/actuators.py`

 * *Files 12% similar despite different names*

```diff
@@ -272,17 +272,15 @@
 
     def _entry(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Entering Position mode.")
 
         if not self.has_gains:
             self._set_gains()
 
-        self._set_motor_position(
-            counts=int(self._device.motor_position / RAD_PER_COUNT)
-        )
+        self._device.set_motor_position(self._device.motor_position)
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Position mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
         time.sleep(0.1)
 
     def _set_gains(
@@ -319,17 +317,15 @@
         self._exit_callback = self._exit
 
     def _entry(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Entering Impedance mode.")
         if not self.has_gains:
             self._set_gains()
 
-        self._set_motor_position(
-            counts=int(self._device.motor_position / RAD_PER_COUNT)
-        )
+        self._device.set_motor_position(self._device.motor_position)
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Impedance mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
         time.sleep(1 / self._device.frequency)
 
     def _set_motor_position(self, counts: int) -> None:
@@ -434,17 +430,24 @@
         self._frequency: int = frequency
         self._data: Any = None
         self._name: str = name
 
         self._log: Logger = logger
         self._state = None
 
+        self._encoder_map = None
+
         self._motor_zero_position = 0.0
         self._joint_zero_position = 0.0
 
+        self._joint_offset = 0.0
+        self._motor_offset = 0.0
+
+        self._joint_direction = 1.0
+
         self._thermal_model: ThermalModel = ThermalModel(
             temp_limit_windings=80,
             soft_border_C_windings=10,
             temp_limit_case=70,
             soft_border_C_case=10,
         )
         self._thermal_scale: float = 1.0
@@ -489,14 +492,20 @@
         if self.is_streaming:
             self._data = self.read()
             self._thermal_model.T_c = self.case_temperature
             self._thermal_scale = self._thermal_model.update_and_get_scale(
                 dt=(1 / self._frequency),
                 motor_current=self.motor_current,
             )
+
+            if hasattr(self, "_safety_attributes"):
+                for safety_attribute_name in self._safety_attributes:
+                    self._log.debug(
+                        msg=f"[{self.__repr__()}] Safety mechanism in-place for {safety_attribute_name}: {getattr(self, safety_attribute_name)}"
+                    )
         else:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Please open() the device before streaming data."
             )
 
     def set_mode(self, mode: ActpackMode) -> None:
         if type(mode) in [VoltageMode, CurrentMode, PositionMode, ImpedanceMode]:
@@ -504,21 +513,37 @@
             self._mode = mode
 
         else:
             self._log.warning(msg=f"[{self.__repr__()}] Mode {mode} not found")
             return
 
     def set_motor_zero_position(self, position: float) -> None:
-        """Sets motor zero position in counts"""
+        """Sets motor zero position in radians"""
         self._motor_zero_position = position
 
     def set_joint_zero_position(self, position: float) -> None:
-        """Sets joint zero position in counts"""
+        """Sets joint zero position in radians"""
         self._joint_zero_position = position
 
+    def set_motor_offset(self, position: float) -> None:
+        """Sets joint offset position in radians"""
+        self._motor_offset = position
+
+    def set_joint_offset(self, position: float) -> None:
+        """Sets joint offset position in radians"""
+        self._joint_offset = position
+
+    def set_joint_direction(self, direction: float) -> None:
+        """Sets joint direction to 1 or -1"""
+        self._joint_direction = direction
+
+    def set_encoder_map(self, encoder_map) -> None:
+        """Sets the joint encoder map"""
+        self._encoder_map = encoder_map
+
     def set_position_gains(
         self,
         kp: int = DEFAULT_POSITION_GAINS.kp,
         ki: int = DEFAULT_POSITION_GAINS.ki,
         kd: int = DEFAULT_POSITION_GAINS.kd,
         ff: int = DEFAULT_POSITION_GAINS.ff,
     ) -> None:
@@ -653,36 +678,59 @@
         ]:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set motor position in mode {self._mode}"
             )
             return
 
         self._mode._set_motor_position(
-            int((position / RAD_PER_COUNT) + self.motor_zero_position),
+            int(
+                (position + self.motor_zero_position + self.motor_offset)
+                / RAD_PER_COUNT
+            ),
         )
 
     @property
     def frequency(self) -> int:
         return self._frequency
 
     @property
     def mode(self) -> ActpackMode:
         return self._mode
 
     @property
+    def encoder_map(self):
+        """Polynomial coefficients defining the joint encoder map from counts to radians."""
+        return self._encoder_map
+
+    @property
     def motor_zero_position(self) -> float:
-        """Motor encoder offset in radians."""
+        """Motor encoder zero position in radians."""
         return self._motor_zero_position
 
     @property
     def joint_zero_position(self) -> float:
-        """Joint encoder offset in radians."""
+        """Joint encoder zero position in radians."""
         return self._joint_zero_position
 
     @property
+    def joint_offset(self) -> float:
+        """Joint encoder offset in radians."""
+        return self._joint_offset
+
+    @property
+    def motor_offset(self) -> float:
+        """Motor encoder offset in radians."""
+        return self._motor_offset
+
+    @property
+    def joint_direction(self) -> float:
+        """Joint direction: 1 or -1"""
+        return self._joint_direction
+
+    @property
     def battery_voltage(self) -> float:
         """Battery voltage in mV."""
         if self._data is not None:
             return float(self._data.batt_volt)
         else:
             return 0.0
 
@@ -721,16 +769,18 @@
         else:
             return 0.0
 
     @property
     def motor_position(self) -> float:
         """Angle of the motor in radians."""
         if self._data is not None:
-            return float(
-                int(self._data.mot_ang - self.motor_zero_position) * RAD_PER_COUNT
+            return (
+                float(self._data.mot_ang * RAD_PER_COUNT)
+                - self._motor_zero_position
+                - self.motor_offset
             )
         else:
             return 0.0
 
     @property
     def motor_encoder_counts(self) -> int:
         """Raw reading from motor encoder in counts."""
@@ -757,17 +807,22 @@
         else:
             return 0.0
 
     @property
     def joint_position(self) -> float:
         """Measured angle from the joint encoder in radians."""
         if self._data is not None:
-            return float(
-                int(self._data.ank_ang - self._joint_zero_position) * RAD_PER_COUNT
-            )
+            if self.encoder_map is not None:
+                return float(self.encoder_map(self._data.ank_ang))
+            else:
+                return (
+                    float(self._data.ank_ang * RAD_PER_COUNT)
+                    - self.joint_zero_position
+                    - self.joint_offset
+                ) * self.joint_direction
         else:
             return 0.0
 
     @property
     def joint_velocity(self) -> float:
         """Measured velocity from the joint encoder in rad/s."""
         if self._data is not None:
@@ -1001,17 +1056,24 @@
             "b": 0,
             "ff": 0,
         }
 
         # This is used in the read() method to indicate a data stream
         self.is_streaming: bool = False
 
+        self._encoder_map = None
+
         self._motor_zero_position = 0.0
         self._joint_zero_position = 0.0
 
+        self._joint_offset = 0.0
+        self._motor_offset = 0.0
+
+        self._joint_direction = 1.0
+
         self._thermal_model: ThermalModel = ThermalModel(
             temp_limit_windings=80,
             soft_border_C_windings=10,
             temp_limit_case=70,
             soft_border_C_case=10,
         )
```

### Comparing `opensourceleg-2.1.0/opensourceleg/hardware/joints.py` & `opensourceleg-2.2.0/opensourceleg/hardware/joints.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,33 +55,32 @@
             debug_level=debug_level,
             dephy_log=dephy_log,
         )
 
         self._gear_ratio: float = gear_ratio
         self._is_homed: bool = False
         self._has_loadcell: bool = has_loadcell
-        self._encoder_map = None
 
         self._motor_zero_pos = 0.0
         self._joint_zero_pos = 0.0
 
         self._max_temperature: float = MAX_CASE_TEMPERATURE
 
         if "knee" in name.lower() or "ankle" in name.lower():
             self._name: str = name
         else:
             self._log.warning(msg=f"[{self.__repr__()}] Invalid joint name: {name}")
             return
 
         if os.path.isfile(path=f"./{self._name}_encoder_map.npy"):
             coefficients = np.load(file=f"./{self._name}_encoder_map.npy")
-            self._encoder_map = np.polynomial.polynomial.Polynomial(coef=coefficients)
+            self.set_encoder_map(np.polynomial.polynomial.Polynomial(coef=coefficients))
         else:
             self._log.debug(
-                msg=f"[{self._name}] No encoder map found. Please run the calibration routine."
+                msg=f"[{self._name}] No encoder map found. Please run the make_encoder_map routine if you need more accurate joint position."
             )
 
     def home(
         self,
         homing_voltage: int = 2000,
         homing_frequency: int = 100,
     ) -> None:
@@ -129,33 +128,35 @@
                     is_homing = False
 
         except KeyboardInterrupt:
             self.set_voltage(value=0)
             self._log.warning(msg="Homing interrupted.")
             return
 
-        _motor_zero_pos = self.motor_encoder_counts
-        _joint_zero_pos = self.joint_encoder_counts
+        self.set_motor_zero_position(position=self.motor_position)
+        self.set_joint_zero_position(position=self.joint_position)
 
         time.sleep(0.1)
 
         _zero_pos: int = 0
         _zero_pos_joint: int = 0
 
         if "ankle" in self._name.lower():
-            _zero_pos = int((np.deg2rad(30) * self.gear_ratio) / RAD_PER_COUNT)
-            _zero_pos_joint = int(np.deg2rad(30) / RAD_PER_COUNT)
-
-        self.set_motor_zero_position(position=(_motor_zero_pos + _zero_pos))
-        self.set_joint_zero_position(position=(_joint_zero_pos + _zero_pos_joint))
+            self.set_joint_direction(-1.0)
+            self.set_joint_offset(-np.deg2rad(30))
+            self.set_motor_offset(np.deg2rad(30) * self.gear_ratio)
+        else:
+            self.set_joint_direction(-1.0)
+            self.set_joint_offset(0.0)
+            self.set_motor_offset(0.0)
 
         self._is_homed = True
         self._log.info(f"[{self._name}] Homing complete.")
 
-    def make_encoder_map(self) -> None:
+    def make_encoder_map(self, overwrite=False) -> None:
         """
         This method makes a lookup table to calculate the position measured by the joint encoder.
         This is necessary because the magnetic output encoders are nonlinear.
         By making the map while the joint is unloaded, joint position calculated by motor position * gear ratio
         should be the same as the true joint position.
 
         Output from this function is a file containing a_i values parameterizing the map
@@ -169,52 +170,60 @@
 
         if not self.is_homed:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Please home the joint before making the encoder map."
             )
             return
 
+        if os.path.exists(f"./{self._name}_encoder_map.npy") and not overwrite:
+            self._log.info(
+                msg=f"[{self.__repr__()}] Encoder map exists. Skipping encoder map creation."
+            )
+            return
+
         self.set_mode(mode=self.control_modes.current)
         self.set_current_gains()
         time.sleep(0.1)
         self.set_current_gains()
 
         self.set_output_torque(torque=0.0)
         time.sleep(0.1)
         self.set_output_torque(torque=0.0)
 
-        _joint_position_array = []
+        _joint_encoder_array = []
         _output_position_array = []
 
         self._log.info(
-            msg=f"[{self.__repr__()}] Please manually move the joint numerous times through its full range of motion for 10 seconds. \nPress any key to continue."
+            msg=f"[{self.__repr__()}] Please manually move the joint numerous times through its full range of motion for 10 seconds. \n{input('Press any key when you are ready to start.')}"
         )
 
         _start_time: float = time.time()
 
         try:
             while time.time() - _start_time < 10:
+                self._log.info(
+                    msg=f"[{self.__repr__()}] Mapping joint encoder: {10 - time.time() + _start_time} seconds left."
+                )
                 self.update()
-                _joint_position_array.append(self.joint_position)
+                _joint_encoder_array.append(self._data.ank_ang)
                 _output_position_array.append(self.output_position)
-
                 time.sleep(1 / self.frequency)
 
         except KeyboardInterrupt:
             self._log.warning(msg="Encoder map interrupted.")
             return
 
         self._log.info(msg=f"[{self.__repr__()}] You may now stop moving the joint.")
 
         _power = np.arange(4.0)
-        _a_mat = np.array(_joint_position_array).reshape(-1, 1) ** _power
-        _beta = np.linalg.lstsq(_a_mat, _output_position_array, rcond=None)[0]
+        _a_mat = np.array(_joint_encoder_array).reshape(-1, 1) ** _power
+        _beta = np.linalg.lstsq(_a_mat, _output_position_array, rcond=None)
         _coeffs = _beta[0]
 
-        self._encoder_map = np.polynomial.polynomial.Polynomial(coef=_coeffs)
+        self.set_encoder_map(np.polynomial.polynomial.Polynomial(coef=_coeffs))
 
         np.save(file=f"./{self._name}_encoder_map.npy", arr=_coeffs)
         self._log.info(msg=f"[{self.__repr__()}] Encoder map saved.")
 
     def set_max_temperature(self, temperature: float) -> None:
         """
         Set the maximum temperature of the motor.
@@ -298,44 +307,14 @@
             kp=kp,
             ki=ki,
             K=K / (self.gear_ratio**2),
             B=B / (self.gear_ratio**2),
             ff=ff,
         )
 
-    def convert_to_joint_impedance(
-        self,
-        K: float = 100,
-        B: float = 40,
-    ):
-        joint_stiffness = (K / NM_PER_RAD_TO_K) * self.gear_ratio**2
-        joint_damping = (B / NM_S_PER_RAD_TO_B) * self.gear_ratio**2
-
-        return joint_stiffness, joint_damping
-
-    def convert_to_motor_impedance(
-        self,
-        K: float = 100,
-        B: float = 40,
-    ):
-        motor_stiffness = K / NM_PER_RAD_TO_K
-        motor_damping = B / NM_S_PER_RAD_TO_B
-
-        return motor_stiffness, motor_damping
-
-    def convert_to_pid_impedance(
-        self,
-        K: float = 0.08922,
-        B: float = 0.0038070,
-    ):
-        pid_stiffness = (K / self.gear_ratio**2) * NM_PER_RAD_TO_K
-        pid_damping = (B / self.gear_ratio**2) * NM_S_PER_RAD_TO_B
-
-        return pid_stiffness, pid_damping
-
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def gear_ratio(self) -> float:
         return self._gear_ratio
@@ -347,19 +326,14 @@
 
     @property
     def is_homed(self) -> bool:
         """Indicates if the homing routine has been called yet."""
         return self._is_homed
 
     @property
-    def encoder_map(self):
-        """Polynomial coefficients defining the joint encoder map from counts to radians."""
-        return self._encoder_map
-
-    @property
     def output_position(self) -> float:
         """
         Position of the output in radians.
         This is calculated by scaling the motor angle with the gear ratio.
         Note that this method does not consider compliance from an SEA.
         """
         return self.motor_position / self.gear_ratio
@@ -402,15 +376,14 @@
         dephy_log: bool = False,
     ) -> None:
 
         MockDephyActpack.__init__(self, name, port)
         self._gear_ratio: float = gear_ratio
         self._is_homed: bool = False
         self._has_loadcell: bool = has_loadcell
-        self._encoder_map = None
 
         self._motor_zero_pos = 0.0
         self._joint_zero_pos = 0.0
 
         self._max_temperature: float = MAX_CASE_TEMPERATURE
 
         if "knee" in name.lower() or "ankle" in name.lower():
```

### Comparing `opensourceleg-2.1.0/opensourceleg/hardware/sensors.py` & `opensourceleg-2.2.0/opensourceleg/hardware/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,20 @@
             self._loadcell_data = (
                 np.transpose(
                     a=self._loadcell_matrix.dot(b=np.transpose(a=loadcell_coupled))
                 )
                 - loadcell_zero
             )
 
+        if hasattr(self, "_safety_attributes"):
+            for safety_attribute_name in self._safety_attributes:
+                self._log.debug(
+                    msg=f"[{self.__repr__()}] Safety mechanism in-place for {safety_attribute_name}: {getattr(self, safety_attribute_name)}"
+                )
+
     def initialize(self, number_of_iterations: int = 2000) -> None:
         """
         Obtains the initial loadcell reading (aka) loadcell_zero.
         This is automatically subtraced off for subsequent calls of the update method.
         """
         ideal_loadcell_zero = np.zeros(shape=(1, 6), dtype=np.double)
```

### Comparing `opensourceleg-2.1.0/opensourceleg/hardware/thermal.py` & `opensourceleg-2.2.0/opensourceleg/hardware/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.1.0/opensourceleg/osl.py` & `opensourceleg-2.2.0/opensourceleg/osl.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,14 +350,20 @@
 
         if self.has_loadcell:
             self._loadcell.update()
 
         if log_data:
             self.log.data()
 
+        if hasattr(self, "_safety_attributes"):
+            for safety_attribute_name in self._safety_attributes:
+                self.log.debug(
+                    msg=f"[{self.__repr__()}] Safety mechanism in-place for {safety_attribute_name}: {getattr(self, safety_attribute_name)}"
+                )
+
         self._timestamp = time.time()
 
     def home(self) -> None:
         if self.has_knee:
             self.log.info(msg="[OSL] Homing knee joint.")
             self.knee.home()
 
@@ -368,22 +374,22 @@
         self._is_homed = True
 
     def calibrate_loadcell(self) -> None:
         self.log.debug(msg="[OSL] Calibrating loadcell.")
         if self.has_loadcell:
             self.loadcell.reset()
 
-    def calibrate_encoders(self) -> None:
+    def make_encoder_maps(self, overwrite=False) -> None:
         self.log.debug(msg="[OSL] Calibrating encoders.")
 
         if self.has_knee:
-            self.knee.make_encoder_map()
+            self.knee.make_encoder_map(overwrite=overwrite)
 
         if self.has_ankle:
-            self.ankle.make_encoder_map()
+            self.ankle.make_encoder_map(overwrite=overwrite)
 
     def reset(self) -> None:
         self.log.debug(msg="[OSL] Resetting OSL.")
 
         if self.has_knee:
             self.knee.set_mode(mode=self.knee.control_modes.voltage)
             self.knee.set_voltage(value=0)
```

### Comparing `opensourceleg-2.1.0/opensourceleg/tools/logger.py` & `opensourceleg-2.2.0/opensourceleg/tools/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ) -> None:
 
         self._file_path: str = file_path + ".log"
 
         self._containers: list[Union[object, dict[Any, Any]]] = []
         self._attributes: list[list[str]] = []
 
-        self._file = open(file_path + ".csv", "w")
+        self._file = open(file_path + ".csv", "w", newline="")
         self._writer = csv.writer(self._file)
 
         self._log_levels = {
             "DEBUG": logging.DEBUG,
             "INFO": logging.INFO,
             "WARNING": logging.WARNING,
             "ERROR": logging.ERROR,
```

### Comparing `opensourceleg-2.1.0/opensourceleg/tools/units.py` & `opensourceleg-2.2.0/opensourceleg/tools/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.1.0/opensourceleg/tools/utilities.py` & `opensourceleg-2.2.0/opensourceleg/tools/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.1.0/pyproject.toml` & `opensourceleg-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "2.1.0"
+version = "2.2.0"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prostheses."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
-license = "GNU GPL v3.0"
+license = "GNU LGPL v2.1"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [  #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
-  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+  "License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
 ]
 
 [virtualenvs]
 in-project = true
```

### Comparing `opensourceleg-2.1.0/PKG-INFO` & `opensourceleg-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 2.1.0
+Version: 2.2.0
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prostheses.
 Home-page: https://github.com/neurobionics/opensourceleg
-License: GNU GPL v3.0
+License: GNU LGPL v2.1
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -45,24 +45,25 @@
 
 </div>
 
 <br>
 
 ## Installation
 
-The easiest and quickest way to install the *opensourceleg* library is via [pip](https://pip.pypa.io/en/stable/):
+The easiest and quickest way to install the _opensourceleg_ library is via [pip](https://pip.pypa.io/en/stable/):
 
 ```bash
 pip install opensourceleg
 ```
 
-> If you plan on installing the *opensourceleg* library on a Raspberry Pi, we recommend using [opensourcelegpi](https://github.com/neurobionics/opensourcelegpi) tool, which is a cloud-based CI tool used to build an up-to-date OS for a [Raspberry Pi](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/) that can be used headless/GUI-less to control autonomous/remote robotic systems. This tool bundles the *opensourceleg* library and its dependencies into a single OS image, which can be flashed onto a microSD card and used to boot a Raspberry Pi. For more information, click [here](https://github.com/neurobionics/opensourcelegpi/blob/main/README.md).
+> If you plan on installing the _opensourceleg_ library on a Raspberry Pi, we recommend using [opensourcelegpi](https://github.com/neurobionics/opensourcelegpi) tool, which is a cloud-based CI tool used to build an up-to-date OS for a [Raspberry Pi](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/) that can be used headless/GUI-less to control autonomous/remote robotic systems. This tool bundles the _opensourceleg_ library and its dependencies into a single OS image, which can be flashed onto a microSD card and used to boot a Raspberry Pi. For more information, click [here](https://github.com/neurobionics/opensourcelegpi/blob/main/README.md).
 
 ### Developing
-To modify, develop, or contribute to the [opensourceleg](https://pypi.org/project/opensourceleg/) library, we encourage you to install [Poetry](https://python-poetry.org), which is a python packaging and dependency management tool. Once you have Poetry installed on your local machine, you can clone the repository and install the *opensourceleg* library by running the following commands:
+
+To modify, develop, or contribute to the [opensourceleg](https://pypi.org/project/opensourceleg/) library, we encourage you to install [Poetry](https://python-poetry.org), which is a python packaging and dependency management tool. Once you have Poetry installed on your local machine, you can clone the repository and install the _opensourceleg_ library by running the following commands:
 
 ```bash
 git clone https://github.com/neurobionics/opensourceleg.git
 cd opensourceleg
 
 poetry install
 poetry shell
@@ -70,20 +71,20 @@
 
 ## Documentation
 
 You can find tutorials and API documentation at [opensourceleg.readthedocs.io](https://opensourceleg.readthedocs.io/en/latest/).
 
 ## License
 
-The *opensourceleg* library is licensed under the terms of the [GPL-3.0 license](https://github.com/neurobionics/opensourceleg/raw/main/LICENSE). This license grants users a number of freedoms:
+The _opensourceleg_ library is licensed under the terms of the [LGPL-v2.1 license](https://github.com/neurobionics/opensourceleg/raw/main/LICENSE). This license grants users a number of freedoms:
 
-* You are free to use the *opensourceleg* library for any purpose.
-* You are free to modify the *opensourceleg* library to suit your needs.
-* You can study how the *opensourceleg* library works and change it.
-* You can distribute modified versions of the *opensourceleg* library.
+- You are free to use the _opensourceleg_ library for any purpose.
+- You are free to modify the _opensourceleg_ library to suit your needs.
+- You can study how the _opensourceleg_ library works and change it.
+- You can distribute modified versions of the _opensourceleg_ library.
 
 The GPL license ensures that all these freedoms are protected, now and in the future, requiring everyone to share their modifications when they also share the library in public.
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! For more details, read our [contribution guidelines](https://github.com/neurobionics/opensourceleg/blob/11765f7f7dd94e5d8699675149d5ff3596ea01b8/CONTRIBUTING.md).
```

