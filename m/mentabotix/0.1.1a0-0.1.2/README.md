# Comparing `tmp/mentabotix-0.1.1a0.tar.gz` & `tmp/mentabotix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.1a0.tar", last modified: Wed May  1 16:22:14 2024, max compression
+gzip compressed data, was "mentabotix-0.1.2.tar", last modified: Mon May  6 10:37:26 2024, max compression
```

## Comparing `mentabotix-0.1.1a0.tar` & `mentabotix-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    14350 2024-05-01 16:21:51.481188 mentabotix-0.1.1a0/README.md
--rw-r--r--   0        0        0      701 2024-05-01 16:22:14.453434 mentabotix-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0      847 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    56590 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    19645 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     3363 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/tools/algrithm_tools.py
--rw-r--r--   0        0        0      229 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     5457 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/vision/camra.py
--rw-r--r--   0        0        0     8336 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/__init__.py
--rw-r--r--   0        0        0    12243 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_botix.py
--rw-r--r--   0        0        0     8042 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_moving_transition.py
--rw-r--r--   0        0        0    14877 1970-01-01 00:00:00.000000 mentabotix-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    19747 2024-05-06 10:37:03.911770 mentabotix-0.1.2/README.md
+-rw-r--r--   0        0        0      630 2024-05-06 10:37:26.247763 mentabotix-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      847 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    63015 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    19645 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     3363 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/tools/algrithm_tools.py
+-rw-r--r--   0        0        0      229 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     5457 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/vision/camra.py
+-rw-r--r--   0        0        0     8336 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    13373 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_botix.py
+-rw-r--r--   0        0        0     8042 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5578 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    20179 1970-01-01 00:00:00.000000 mentabotix-0.1.2/PKG-INFO
```

### Comparing `mentabotix-0.1.1a0/README.md` & `mentabotix-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,69 @@
+Metadata-Version: 2.1
+Name: mentabotix
+Version: 0.1.2
+Summary: A Bot control lib
+Author-Email: Whth <88489697+Whth@users.noreply.github.com>
+License: MIT
+Requires-Python: >=3.11
+Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pyapriltags>=3.3.0.3
+Requires-Dist: terminaltables>=3.1.10
+Requires-Dist: bdmc>=0.1.4
+Requires-Dist: opencv-python-headless>=4.9.0.80
+Description-Content-Type: text/markdown
+
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
 
 ## Installation
 
 Use `pdm` to install mentabotix
 
 ```shell
+# install pdm
+python -m pip install pdm
+
+# config pdm
+pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
+
+# for stable release
 pdm add mentabotix
+
+# for unstable release
+pdm add mentabotix --pre
+
 ```
 
 ## Usage
 
 ### Menta
 
 You can use `Menta` to create the judge function closure of the robot, using the sensor data as the input.
 
 #### Step 1: Define Sampler Functions
 
 Firstly, you need to define sampler functions that adhere to the specifications outlined by the `Menta` class. These
 could include sequence samplers that return a series of data points, index samplers that provide data at a specific
 index, and direct response samplers that give an immediate value.
 
+|               Sampler                |                 Description                  |                    Type                    |
+|:------------------------------------:|:--------------------------------------------:|:------------------------------------------:|
+| `mentabotix.SamplerType.SEQ_SAMPLER` | The sensor data is returned in a `Sequence`. | `Callable[[], Sequence[Union[float,int]]]` |
+| `mentabotix.SamplerType.IDX_SAMPLER` |         Use a index to get the data.         |    `Callable[[int], Union[float,int]]`     |
+| `mentabotix.SamplerType.DRC_SAMPLER` |  Direct read sensor data without any args.   |      `Callable[[], Union[float,int]]`      |
+
+> Do remember to add return type annotations to your sampler functions, which will be used to classify the samplers into
+> their respective types in the `Menta` class.
+
 ```python
+
 def temperature_sequence_sampler() -> list[float]:
     """Simulates a sequence of temperature readings."""
     return [25.5, 26.0, 25.8]
 
 
 def humidity_index_sampler(index: int) -> float:
     """Returns simulated humidity data at a given index."""
@@ -43,80 +79,160 @@
 #### Step 2: Initialize Menta Instance and Add Samplers
 
 After defining the sampler functions, initialize the `Menta` instance and add these samplers to it.
 
 ```python
 from mentabotix import Menta  # Ensure to import the correct Menta class
 
-menta_instance = Menta(samplers=[temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
 ```
 
 #### Step 3: Update Sampler Types
 
 Invoke the `update_sampler_types` method to automatically classify the samplers into their respective types.
 
 ```python
+from mentabotix import Menta  # Ensure to import the correct Menta class
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
 menta_instance.update_sampler_types()
 ```
 
-#### Step 4: Construct Updater Function
+#### Step 4: Construct Judge Function
 
 To use the samplers in a meaningful way, you can construct an updater function that encapsulates a condition based on
 which system updates might occur. For example:
 
 ```python
-from mentabotix import SamplerUsage
+from mentabotix import SamplerUsage, Menta
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
 
-# Assuming we want to trigger an update when the temperature is above 25 and humidity is below 50%
-judging_source = "temp > 25 and humidity < 50"
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+menta_instance.update_sampler_types()
 
 # Define how samplers will be used
 usages = [
-    SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+
     # Use sequence sampler for first and third temp data
-    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),  # Use index sampler for the first humidity value
-    # For direct response samplers, typically, no required_data_indexes are needed since they return a single value
+    SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+    # Use index sampler for the first humidity value
+    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),
 ]
 
-updater_function = menta_instance.construct_updater(usages)
+# Note: the judge source has some built-in syntaxes.Currently, sensor data indexes flattening and extra data context insertion
+# s0 stands for the data at index 0 of the first sampler
+# s1 stands for the data at index 2 of the first sampler
+# s3 stands for the data at index 1 of the second sampler
+
+judging_source = "(s0 > 25 and s1 < 50) or s3>baseline"
+
+# Extra context for the judge function, here only contains the "baseline"
+extra_context = {"baseline": 47}
+
+from typing import Callable
+
+# Construct the judge function object
+updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
+                                                                               extra_context=extra_context)
+
+# Use the judge function to update the system
+updater_function()
 
-# Execute the updater function
-result = updater_function()
-print(result)
-```
 
-In this scenario, `construct_updater` dynamically creates and executes a function based on the specified sampler usages
-and a logical condition (`judging_source`). This function then returns a result or triggers actions according to the
-given criteria (e.g., temperature and humidity conditions).
+# Below is the equivalent implementation of the judge function, but is defined manually. 
+# It acts exactly the same as the `updater_function` above.
+def manual_judge_function() -> bool:
+    """Manually construct the judge function."""
+    seq_temp = temperature_sequence_sampler()
+    return (seq_temp[0] > 25 and seq_temp[2] < 50) or humidity_index_sampler(0) > 47
+```
 
-Make sure to tailor the sampler functions, the logic expression string, and the usage of samplers to fit your specific
-application needs.
+In this case, a judge function closure is created using `exec()` method.Normally the built should have a better
+performance since the all the calls and variables are inlined and stored in the closure.
+---
 
 ## Botix
 
 Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
 walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
-schemas into executable closures using the Botix framework. Keep in mind that while this explanation avoids deep Python
-specifics, a basic understanding of programming concepts will be helpful.
+schemas into executable closures using the Botix framework.
 
 ### Understanding State-Transition Control Schema
 
 Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
 robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
 these states are triggered by events or conditions, forming a **control schema**.
 
 #### States
 
 - In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
   motor speeds or changing direction.
+- A state describe the robot's **moving behavior**, 4 motor speeds in this case
 
 #### Transitions
 
 - Transitions between states are handled by the `MovingTransition` class. They define how and when the robot moves from
   one state to another, possibly based on sensor inputs or internal conditions.
+- Transitions describe how the robot **moves** from one state to another
 
 ### Building Your Control Schema
 
 #### Step 1: Define States
 
 For each distinct behavior, create a `MovingState` instance. Include the actions or configurations that should occur in
 that state. For instance, creating a state for moving forward might look like this:
@@ -157,17 +273,18 @@
 #### Step 2: Define Transitions
 
 Transitions are created with `MovingTransition`. Specify the duration, any conditions under which the transition should
 occur (using a breaker function), and the source and destination states.
 
 ```python
 from mentabotix import MovingTransition, MovingState
+from random import random
 
-sensor_reading = lambda: 25.5  # Example sensor reading function
-threshold = 25.0
+sensor_reading = lambda: random()  # Example sensor reading function
+threshold = 0.6
 
 
 def stop_condition() -> bool:  # the return type must be annotated, since an exception will be raised otherwise
     return sensor_reading() < threshold
 
 
 moving_forward = MovingState(10)
@@ -215,14 +332,67 @@
 ```
 
 #### Step 3: Connect States with Transitions
 
 Create a collection of your states and transitions, ensuring each transition correctly references its source and target
 states.
 
+A legal control schema should have a start state and at least one end state.
+And each state can **ONLY** connect to **ONE** transition as its input state
+
+```python
+from mentabotix import MovingState, MovingTransition
+import random
+
+moving_left = MovingState.turn("l", 10)
+moving_right = MovingState.turn("r", 10)
+moving_dash = MovingState.straight(100)
+stopped_state = MovingState(0)
+
+start_state = MovingState(100)
+
+
+def _breaker_1() -> int:
+    return random.choice([0, 1, 2])
+
+
+def _breaker_2() -> int:
+    return random.choice([0, 1])
+
+
+transition_1 = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=_breaker_1,  # When to break the transition
+    from_states=stopped_state,
+    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
+)
+
+transition_2 = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=_breaker_2,  # When to break the transition
+    from_states=stopped_state,
+    to_states={0: moving_dash, 1: stopped_state},
+)
+
+
+```
+
+As the above example, `transition_1` and `transition_2` both have the `stopped_state` as the input state,which means
+the `stopped_state` connects more than **ONE** transition. Definition as such is illegal and will not pass the compile
+stage.
+
+Normally, you can ensure that the structure is valid by using `ensure_structure_validity`. to eliminate this problem.
+
+```python
+from mentabotix import Botix
+
+# A StructuralError will be raised if the structure is not valid
+Botix.ensure_structure_validity([transition_1, transition_2])
+```
+
 ### Compiling to Closures with Botix
 
 Once your control schema is defined, Botix can help you compile this structure into executable code, often referred to
 as closures, which can directly control the robot's behavior.
 
 #### Step 4: Compile the Schema
 
@@ -265,15 +435,15 @@
 [
     "def _func():",
     "    con.set_motors_speed((-1, -1, -1, -1)).delay(0.1).set_motors_speed((0, 0, 0, 0)).delay(1).set_motors_speed((1, 1, 1, 1)).delay(2).set_motors_speed((2, 2, 2, 2))",
 ]
 
 ```
 
-But usaully, you want to compile the code into a closure that can be used to control the robot with higher performance
+But usually, you want to compile the code into a closure that can be used to control the robot with higher performance
 and less human error.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 from typing import Callable
 
@@ -282,15 +452,15 @@
                                                             MotorInfo(code_sign=2, direction=-1),
                                                             MotorInfo(code_sign=4, direction=-1)], port="COM3")
 
 start_state = MovingState(-1)
 state_a = MovingState(0)
 state_b = MovingState(1)
 state_c = MovingState(2)
-# 创建一些假的MovingTransition对象用于测试
+# create some transitions
 transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
 transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
 transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
 
 botix = Botix(controller=con)
 botix.token_pool.append(transition_start_a)
 botix.token_pool.append(transition_ab)
@@ -300,29 +470,26 @@
 function_closure: Callable[[], None] = botix.compile(return_median=False)
 
 print(function_closure)
 ```
 
 By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
 
-```python
-< function
-_func
-at
-0x0000020D40EAECA0 >
+```
+< function _func at 0x0000020D40EAECA0 >
 ```
 
 Usage is as follows
 
 ```python
 # call the closure, which will execute the compiled code
 function_closure()
 ```
 
-Of course, you can also build a closure with branch logic in it.
+Of course, you can also build a closure with branching logic in it.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 import random
 from typing import List, Tuple, Dict, Any, Callable
 
@@ -388,13 +555,28 @@
 
 # call the closure, which will execute the compiled code
 compiled_closure()
 
 
 ```
 
-### Conclusion
+## Logging
+
+use `set_log_level` to silent the console to improve the performance in high pressure conditions
+
+```python
+from mentabotix import set_log_level
+
+"""
+Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
+Logging INFO - Information message, used to inform the general program running status, with a value of 20.
+Logging WARN - A warning message indicating that there may be a problem but the program is still running, with a value of 30.
+Logging Error - Error message indicating an issue preventing the program from executing properly, with a value of 40.
+Logging CRITICAL - Fatal error message indicating a serious system failure with a value of 50.
+"""
+
+set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
+
+from logging import CRITICAL
 
-By following these steps, you can design a control schema for your robot using state transitions and compile it into
-executable code using Botix. Remember, practice and experimentation are key – start with simple schemas and gradually
-increase complexity as you become more comfortable with the process. Always test your schemas in a safe environment
-before deploying on actual hardware.
+set_log_level(CRITICAL)  # this has the same effect as above
+```
```

### Comparing `mentabotix-0.1.1a0/src/mentabotix/__init__.py` & `mentabotix-0.1.2/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/src/mentabotix/modules/botix.py` & `mentabotix-0.1.2/src/mentabotix/modules/botix.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 from collections import Counter
 from dataclasses import dataclass
 from inspect import signature, Signature
 from itertools import zip_longest
 from queue import Queue
 from typing import (
     Tuple,
@@ -16,14 +17,15 @@
     TypeVar,
     Dict,
     Optional,
     List,
     ClassVar,
     Set,
     Sequence,
+    get_type_hints,
 )
 
 import numpy as np
 from bdmc import CloseLoopController
 from terminaltables import SingleTable
 
 from .exceptions import StructuralError, TokenizeError
@@ -42,14 +44,76 @@
 KT = TypeVar("KT", bound=Hashable)
 Context: TypeAlias = Dict[str, Any]
 
 __PLACE_HOLDER__ = "Hello World"
 __CONTROLLER_NAME__ = "con"
 
 
+def get_function_annotations(func: Callable) -> str:
+    """
+    Get the function annotations of a given function.
+
+    Args:
+        func (callable): The function to get the annotations for.
+
+    Returns:
+        str: A string representation of the function annotations.
+    """
+    try:
+        # Get the function's signature
+        sig = inspect.signature(func)
+    except ValueError as e:
+        # Handle cases where func is not a valid function
+        raise ValueError(f"Invalid function: {func}") from e
+
+    # Get the type annotations
+    type_hints = get_type_hints(func)
+
+    # Initialize strings for parameter types and return type
+    param_types = []
+
+    for param_name, param in sig.parameters.items():
+        # Check if the parameter has an annotation
+        if param.annotation != inspect.Parameter.empty:
+            hint = type_hints.get(param_name)
+            # Convert the type hint to a string representation,
+            # handling complex hints like List[int] properly
+            param_type_str = convert_type_str(hint)
+            param_types.append(param_type_str)
+        else:
+            # Use 'Any' for parameters without annotations
+            param_types.append("Any")
+
+    # Handle the return type
+    return_type = convert_type_str(type_hints.get("return", Any))
+
+    # Concatenate the parameter type strings and return type to form the annotation string
+    params_str = ", ".join(param_types)
+    return f"{func.__name__}({params_str}) -> {return_type}"
+
+
+def convert_type_str(hint) -> str:
+    """
+    Convert a type hint to a string representation, handling complex types and generics.
+
+    Args:
+        hint: The type hint to convert.
+
+    Returns:
+        str: The string representation of the type hint.
+    """
+    if hint is None:
+        return "None"
+    elif hint in {int, float, bool, str, list, tuple, set, dict}:
+        return hint.__name__
+    else:
+        # For other types, convert directly to string
+        return str(hint).replace("typing.", "")
+
+
 class MovingState:
     """
     Describes the movement state of the bot.
     Include:
     - halt: make a stop state,all wheels stop moving
     - straight: make a straight moving state,all wheels move in the same direction,same speed
     - turn: make a turning state,left and right wheels turn in different direction,same speed
@@ -618,52 +682,76 @@
 
 class Botix:
 
     def __init__(self, controller: CloseLoopController, token_pool: Optional[List[MovingTransition]] = None):
         self.controller: CloseLoopController = controller
         self.token_pool: TokenPool = token_pool or []
 
-    @staticmethod
-    def acquire_unique_start(token_pool: TokenPool, none_check: bool = True) -> MovingState | None:
+    def acquire_unique_start(self, token_pool: TokenPool, none_check: bool = True) -> MovingState | None:
         """
         Retrieves a unique starting state from the given token pool.
 
         Parameters:
         - token_pool: An instance of TokenPool, representing a collection of tokens.
         - none_check: A boolean, defaulting to True. If True, raises a ValueError when no unique starting state is found; otherwise, returns None.
 
         Returns:
         - Either a MovingState or None. Returns the starting state (with indegree 0) if uniquely identified; based on none_check's value, either returns None or raises an exception.
         """
+        # Identifies states with an indegree of zero
+        zero_indegree_states = list(states_indegree := self.acquire_start_states(token_pool))
+
+        # Validates that there is exactly one state with an indegree of zero
+        if len(zero_indegree_states) == 1:
+            return zero_indegree_states[0]
+        else:
+            if none_check:
+                # Raises an error if none_check is enabled and no unique starting state is present
+                raise ValueError(f"There must be exactly one state with a zero indegree, got {states_indegree}")
+            return None
+
+    @staticmethod
+    def acquire_start_states(token_pool: TokenPool) -> Set[MovingState]:
+        """
+        Calculates the starting states in the given token pool.
 
+        Parameters:
+            token_pool (TokenPool): A list of MovingTransition objects representing the token pool.
+
+        Returns:
+            Set[MovingState]: A set of MovingState objects representing the starting states in the token pool.
+                The starting states are the states with an indegree of zero.
+
+        Algorithm:
+            1. Initialize a dictionary to hold the indegree of each state.
+            2. Calculate the indegree for each state by examining token transitions.
+            3. Identify states with an indegree of zero.
+            4. Return a set of MovingState objects representing the starting states.
+
+        Note:
+            - The indegree of a state is the number of tokens that can reach that state.
+            - A state is considered a starting state if it has an indegree of zero.
+        """
         # Initialize a dictionary to hold the indegree of each state
         states_indegree: Dict[MovingState, int] = {}
 
         # Calculates the indegree for each state by examining token transitions
         for token in token_pool:
             for state in token.from_states:
                 states_indegree[state] = states_indegree.get(state, 0)
             for state in token.to_states.values():
                 # Increments the indegree for each state that a token can reach
                 states_indegree[state] = states_indegree.get(state, 0) + 1
 
         # Identifies states with an indegree of zero
-        zero_indegree_states = [state for state, indegree in states_indegree.items() if indegree == 0]
-
-        # Validates that there is exactly one state with an indegree of zero
-        if len(zero_indegree_states) == 1:
-            return zero_indegree_states[0]
-        else:
-            if none_check:
-                # Raises an error if none_check is enabled and no unique starting state is present
-                raise ValueError(f"There must be exactly one state with a zero indegree, got {states_indegree}")
-            return None
+        zero_indegree_states = {state for state, indegree in states_indegree.items() if indegree == 0}
+        return zero_indegree_states
 
     @staticmethod
-    def acquire_end_state(token_pool: TokenPool) -> Set[MovingState]:
+    def acquire_end_states(token_pool: TokenPool) -> Set[MovingState]:
         """
         Calculates the end states of the given token pool.
 
         This function iterates through each token in the provided token pool,
         counting the number of outgoing transitions from each state.
         States with no outgoing transitions are considered end states.
 
@@ -677,14 +765,16 @@
         # for each state.
         states_outdegree: Dict[MovingState, int] = {}
 
         # Count the number of outgoing transitions from each state.
         for token in token_pool:
             for from_state in token.from_states:
                 states_outdegree[from_state] = states_outdegree.get(from_state, 0) + 1
+            for to_state in token.to_states.values():
+                states_outdegree[to_state] = states_outdegree.get(to_state, 0)
 
         # Identify end states by finding states with an outdegree of 0.
         end_states = {state for state, outdegree in states_outdegree.items() if outdegree == 0}
 
         return end_states
 
     @staticmethod
@@ -963,15 +1053,15 @@
                 return response[0]
             case _:
                 return response
 
     def _check_met_requirements(self):
         self.ensure_structure_validity(self.token_pool)
         start_state = self.acquire_unique_start(self.token_pool)
-        end_states = self.acquire_end_state(self.token_pool)
+        end_states = self.acquire_end_states(self.token_pool)
         self.ensure_accessibility(self.token_pool, start_state, end_states)
         if self.acquire_loops():
             raise ValueError("Loops detected! All State-Transition should be implemented using breaker")
 
     def _assembly_match_cases(self, match_expression: str | List[str], cases: Dict[str, str | List[str]]) -> List[str]:
         """
         Assembles a list of strings representing match cases based on the given match expression and cases dictionary.
@@ -1144,14 +1234,79 @@
                 lines = self._assembly_match_cases(match_expression=match_expr, cases=match_branch)
                 return lines
             case _:
                 compiled_lines.append(line)
                 # If no forward transition is present, return the compiled lines
                 return compiled_lines
 
+    def export_structure(self, save_path: str, transitions: Optional[List[MovingTransition]] = None) -> Self:
+        """
+        Export the structure to a UML file based on the provided transitions.
+
+        Args:
+            save_path (str): The path to save the UML file.
+            transitions (Optional[List[MovingTransition]]): The list of transitions to represent in the UML.
+
+        Returns:
+            Self: The current instance.
+        """
+        transitions: TokenPool = transitions or self.token_pool
+        start_string = "@startuml\n"
+        end_string = "@enduml\n"
+
+        used_state: Dict[MovingState, str] = {}
+
+        lines: List[str] = []
+        name_gen: NameGenerator = NameGenerator(basename="state_")
+        break_gen: NameGenerator = NameGenerator(basename="break_")
+        for transition in transitions:
+            for from_state in transition.from_states:
+
+                if from_state in used_state:
+                    from_state_alias = used_state.get(from_state)
+                else:
+                    from_state_alias: str = name_gen()
+                    used_state[from_state] = from_state_alias
+                    lines.insert(0, f'state "{from_state}" as {from_state_alias}\n')
+
+                if len(transition.to_states) == 1:
+                    to_state = list(transition.to_states.values())[0]
+                    if to_state not in used_state:
+                        to_state_alias: str = name_gen()
+                        used_state[to_state] = to_state_alias
+                        lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
+                    else:
+                        to_state_alias = used_state.get(to_state)
+                    lines.append(f"{from_state_alias} --> {to_state_alias}\n")
+                else:
+                    break_node_name: str = break_gen()
+                    lines.insert(0, f"state {break_node_name} <<choice>>\n")
+                    lines.append(f"{from_state_alias} --> {break_node_name}\n")
+                    for case_name, to_state in transition.to_states.items():
+
+                        if to_state not in used_state:
+                            to_state_alias: str = name_gen()
+                            used_state[to_state] = to_state_alias
+                            lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
+                        else:
+                            to_state_alias = used_state.get(to_state)
+
+                        lines.append(f"{break_node_name} --> {to_state_alias}: {case_name}\n")
+
+        start_states = self.acquire_start_states(token_pool=transitions)
+        end_states = self.acquire_end_states(token_pool=transitions)
+
+        start_heads: List[str] = [f"[*] --> {used_state.get(sta)}\n" for sta in start_states]
+        end_heads: List[str] = [f"{used_state.get(sta)} --> [*]\n" for sta in end_states]
+
+        with open(save_path, "w") as f:
+
+            f.writelines([start_string, *lines, "\n", *start_heads, "\n", *end_heads, "\n", end_string])
+        return self
+
     def compile(self, return_median: bool = False) -> Callable[[], None] | Tuple[List[str], Context]:
         """
         Compiles the bot's code and returns a callable function or a tuple of compiled lines and context.
 
         Args:
             return_median (bool, optional): Whether to return the compiled lines and context instead of a callable function. Defaults to False.
```

### Comparing `mentabotix-0.1.1a0/src/mentabotix/modules/logger.py` & `mentabotix-0.1.2/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/src/mentabotix/modules/menta.py` & `mentabotix-0.1.2/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/src/mentabotix/tools/algrithm_tools.py` & `mentabotix-0.1.2/src/mentabotix/tools/algrithm_tools.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/src/mentabotix/vision/camra.py` & `mentabotix-0.1.2/src/mentabotix/vision/camra.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.2/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/tests/test_botix.py` & `mentabotix-0.1.2/tests/test_botix.py`

 * *Files 5% similar despite different names*

```diff
@@ -292,11 +292,43 @@
                 "                    con.set_motors_speed((600, 600, 600, 600))",
             ],
             compiled[0],
         )
 
         obj = self.botix_instance.compile()
         obj()
+        self.botix_instance.export_structure("test.puml")
+
+    def test_export_structure(self):
+        MovingState.__state_id_counter__ = 0
+        MovingTransition.__state_id_counter__ = 0
+        state_a = MovingState(100)
+        state_b = MovingState(200)
+        state_c = MovingState(300)
+        state_d = MovingState(400)
+        state_e = MovingState(500)
+        state_f = MovingState(600)
+
+        def transition_breaker_fac(lst: List[int]):
+            def _inner() -> int:
+                return random.choice(lst)
+
+            return _inner
+
+        transition_a_bcd = MovingTransition(
+            duration=1,
+            from_states=state_a,
+            to_states={1: state_b, 2: state_c, 3: state_d},
+            breaker=transition_breaker_fac([1, 2, 3]),
+        )
+        transition_d_ef = MovingTransition(
+            duration=1,
+            from_states=state_d,
+            to_states={1: state_e, 2: state_f},
+            breaker=transition_breaker_fac([1, 2]),
+        )
+        self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
+        self.botix_instance.export_structure("test.puml")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.1a0/tests/test_menta.py` & `mentabotix-0.1.2/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/tests/test_moving_state.py` & `mentabotix-0.1.2/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/tests/test_moving_transition.py` & `mentabotix-0.1.2/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1a0/PKG-INFO` & `mentabotix-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-Metadata-Version: 2.1
-Name: mentabotix
-Version: 0.1.1a0
-Summary: A Bot control lib
-Author-Email: Whth <88489697+Whth@users.noreply.github.com>
-License: MIT
-Requires-Python: >=3.11
-Requires-Dist: pydantic>=2.7.0
-Requires-Dist: coloredlogs>=15.0.1
-Requires-Dist: bdmc>=0.1.3
-Requires-Dist: pyyaml>=6.0.1
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyuptech>=0.1.4a0
-Requires-Dist: opencv-python-headless>=4.9.0.80
-Requires-Dist: pyapriltags>=3.3.0.3
-Requires-Dist: terminaltables>=3.1.10
-Description-Content-Type: text/markdown
-
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
 
 ## Installation
 
 Use `pdm` to install mentabotix
 
 ```shell
+# install pdm
+python -m pip install pdm
+
+# config pdm
+pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
+
+# for stable release
 pdm add mentabotix
+
+# for unstable release
+pdm add mentabotix --pre
+
 ```
 
 ## Usage
 
 ### Menta
 
 You can use `Menta` to create the judge function closure of the robot, using the sensor data as the input.
 
 #### Step 1: Define Sampler Functions
 
 Firstly, you need to define sampler functions that adhere to the specifications outlined by the `Menta` class. These
 could include sequence samplers that return a series of data points, index samplers that provide data at a specific
 index, and direct response samplers that give an immediate value.
 
+|               Sampler                |                 Description                  |                    Type                    |
+|:------------------------------------:|:--------------------------------------------:|:------------------------------------------:|
+| `mentabotix.SamplerType.SEQ_SAMPLER` | The sensor data is returned in a `Sequence`. | `Callable[[], Sequence[Union[float,int]]]` |
+| `mentabotix.SamplerType.IDX_SAMPLER` |         Use a index to get the data.         |    `Callable[[int], Union[float,int]]`     |
+| `mentabotix.SamplerType.DRC_SAMPLER` |  Direct read sensor data without any args.   |      `Callable[[], Union[float,int]]`      |
+
+> Do remember to add return type annotations to your sampler functions, which will be used to classify the samplers into
+> their respective types in the `Menta` class.
+
 ```python
+
 def temperature_sequence_sampler() -> list[float]:
     """Simulates a sequence of temperature readings."""
     return [25.5, 26.0, 25.8]
 
 
 def humidity_index_sampler(index: int) -> float:
     """Returns simulated humidity data at a given index."""
@@ -61,80 +64,160 @@
 #### Step 2: Initialize Menta Instance and Add Samplers
 
 After defining the sampler functions, initialize the `Menta` instance and add these samplers to it.
 
 ```python
 from mentabotix import Menta  # Ensure to import the correct Menta class
 
-menta_instance = Menta(samplers=[temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
 ```
 
 #### Step 3: Update Sampler Types
 
 Invoke the `update_sampler_types` method to automatically classify the samplers into their respective types.
 
 ```python
+from mentabotix import Menta  # Ensure to import the correct Menta class
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
 menta_instance.update_sampler_types()
 ```
 
-#### Step 4: Construct Updater Function
+#### Step 4: Construct Judge Function
 
 To use the samplers in a meaningful way, you can construct an updater function that encapsulates a condition based on
 which system updates might occur. For example:
 
 ```python
-from mentabotix import SamplerUsage
+from mentabotix import SamplerUsage, Menta
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
 
-# Assuming we want to trigger an update when the temperature is above 25 and humidity is below 50%
-judging_source = "temp > 25 and humidity < 50"
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+menta_instance.update_sampler_types()
 
 # Define how samplers will be used
 usages = [
-    SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+
     # Use sequence sampler for first and third temp data
-    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),  # Use index sampler for the first humidity value
-    # For direct response samplers, typically, no required_data_indexes are needed since they return a single value
+    SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+    # Use index sampler for the first humidity value
+    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),
 ]
 
-updater_function = menta_instance.construct_updater(usages)
+# Note: the judge source has some built-in syntaxes.Currently, sensor data indexes flattening and extra data context insertion
+# s0 stands for the data at index 0 of the first sampler
+# s1 stands for the data at index 2 of the first sampler
+# s3 stands for the data at index 1 of the second sampler
+
+judging_source = "(s0 > 25 and s1 < 50) or s3>baseline"
+
+# Extra context for the judge function, here only contains the "baseline"
+extra_context = {"baseline": 47}
+
+from typing import Callable
+
+# Construct the judge function object
+updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
+                                                                               extra_context=extra_context)
+
+# Use the judge function to update the system
+updater_function()
 
-# Execute the updater function
-result = updater_function()
-print(result)
-```
 
-In this scenario, `construct_updater` dynamically creates and executes a function based on the specified sampler usages
-and a logical condition (`judging_source`). This function then returns a result or triggers actions according to the
-given criteria (e.g., temperature and humidity conditions).
+# Below is the equivalent implementation of the judge function, but is defined manually. 
+# It acts exactly the same as the `updater_function` above.
+def manual_judge_function() -> bool:
+    """Manually construct the judge function."""
+    seq_temp = temperature_sequence_sampler()
+    return (seq_temp[0] > 25 and seq_temp[2] < 50) or humidity_index_sampler(0) > 47
+```
 
-Make sure to tailor the sampler functions, the logic expression string, and the usage of samplers to fit your specific
-application needs.
+In this case, a judge function closure is created using `exec()` method.Normally the built should have a better
+performance since the all the calls and variables are inlined and stored in the closure.
+---
 
 ## Botix
 
 Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
 walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
-schemas into executable closures using the Botix framework. Keep in mind that while this explanation avoids deep Python
-specifics, a basic understanding of programming concepts will be helpful.
+schemas into executable closures using the Botix framework.
 
 ### Understanding State-Transition Control Schema
 
 Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
 robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
 these states are triggered by events or conditions, forming a **control schema**.
 
 #### States
 
 - In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
   motor speeds or changing direction.
+- A state describe the robot's **moving behavior**, 4 motor speeds in this case
 
 #### Transitions
 
 - Transitions between states are handled by the `MovingTransition` class. They define how and when the robot moves from
   one state to another, possibly based on sensor inputs or internal conditions.
+- Transitions describe how the robot **moves** from one state to another
 
 ### Building Your Control Schema
 
 #### Step 1: Define States
 
 For each distinct behavior, create a `MovingState` instance. Include the actions or configurations that should occur in
 that state. For instance, creating a state for moving forward might look like this:
@@ -175,17 +258,18 @@
 #### Step 2: Define Transitions
 
 Transitions are created with `MovingTransition`. Specify the duration, any conditions under which the transition should
 occur (using a breaker function), and the source and destination states.
 
 ```python
 from mentabotix import MovingTransition, MovingState
+from random import random
 
-sensor_reading = lambda: 25.5  # Example sensor reading function
-threshold = 25.0
+sensor_reading = lambda: random()  # Example sensor reading function
+threshold = 0.6
 
 
 def stop_condition() -> bool:  # the return type must be annotated, since an exception will be raised otherwise
     return sensor_reading() < threshold
 
 
 moving_forward = MovingState(10)
@@ -233,14 +317,67 @@
 ```
 
 #### Step 3: Connect States with Transitions
 
 Create a collection of your states and transitions, ensuring each transition correctly references its source and target
 states.
 
+A legal control schema should have a start state and at least one end state.
+And each state can **ONLY** connect to **ONE** transition as its input state
+
+```python
+from mentabotix import MovingState, MovingTransition
+import random
+
+moving_left = MovingState.turn("l", 10)
+moving_right = MovingState.turn("r", 10)
+moving_dash = MovingState.straight(100)
+stopped_state = MovingState(0)
+
+start_state = MovingState(100)
+
+
+def _breaker_1() -> int:
+    return random.choice([0, 1, 2])
+
+
+def _breaker_2() -> int:
+    return random.choice([0, 1])
+
+
+transition_1 = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=_breaker_1,  # When to break the transition
+    from_states=stopped_state,
+    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
+)
+
+transition_2 = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=_breaker_2,  # When to break the transition
+    from_states=stopped_state,
+    to_states={0: moving_dash, 1: stopped_state},
+)
+
+
+```
+
+As the above example, `transition_1` and `transition_2` both have the `stopped_state` as the input state,which means
+the `stopped_state` connects more than **ONE** transition. Definition as such is illegal and will not pass the compile
+stage.
+
+Normally, you can ensure that the structure is valid by using `ensure_structure_validity`. to eliminate this problem.
+
+```python
+from mentabotix import Botix
+
+# A StructuralError will be raised if the structure is not valid
+Botix.ensure_structure_validity([transition_1, transition_2])
+```
+
 ### Compiling to Closures with Botix
 
 Once your control schema is defined, Botix can help you compile this structure into executable code, often referred to
 as closures, which can directly control the robot's behavior.
 
 #### Step 4: Compile the Schema
 
@@ -283,15 +420,15 @@
 [
     "def _func():",
     "    con.set_motors_speed((-1, -1, -1, -1)).delay(0.1).set_motors_speed((0, 0, 0, 0)).delay(1).set_motors_speed((1, 1, 1, 1)).delay(2).set_motors_speed((2, 2, 2, 2))",
 ]
 
 ```
 
-But usaully, you want to compile the code into a closure that can be used to control the robot with higher performance
+But usually, you want to compile the code into a closure that can be used to control the robot with higher performance
 and less human error.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 from typing import Callable
 
@@ -300,15 +437,15 @@
                                                             MotorInfo(code_sign=2, direction=-1),
                                                             MotorInfo(code_sign=4, direction=-1)], port="COM3")
 
 start_state = MovingState(-1)
 state_a = MovingState(0)
 state_b = MovingState(1)
 state_c = MovingState(2)
-# 创建一些假的MovingTransition对象用于测试
+# create some transitions
 transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
 transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
 transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
 
 botix = Botix(controller=con)
 botix.token_pool.append(transition_start_a)
 botix.token_pool.append(transition_ab)
@@ -318,29 +455,26 @@
 function_closure: Callable[[], None] = botix.compile(return_median=False)
 
 print(function_closure)
 ```
 
 By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
 
-```python
-< function
-_func
-at
-0x0000020D40EAECA0 >
+```
+< function _func at 0x0000020D40EAECA0 >
 ```
 
 Usage is as follows
 
 ```python
 # call the closure, which will execute the compiled code
 function_closure()
 ```
 
-Of course, you can also build a closure with branch logic in it.
+Of course, you can also build a closure with branching logic in it.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 import random
 from typing import List, Tuple, Dict, Any, Callable
 
@@ -406,13 +540,28 @@
 
 # call the closure, which will execute the compiled code
 compiled_closure()
 
 
 ```
 
-### Conclusion
+## Logging
+
+use `set_log_level` to silent the console to improve the performance in high pressure conditions
+
+```python
+from mentabotix import set_log_level
+
+"""
+Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
+Logging INFO - Information message, used to inform the general program running status, with a value of 20.
+Logging WARN - A warning message indicating that there may be a problem but the program is still running, with a value of 30.
+Logging Error - Error message indicating an issue preventing the program from executing properly, with a value of 40.
+Logging CRITICAL - Fatal error message indicating a serious system failure with a value of 50.
+"""
+
+set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
+
+from logging import CRITICAL
 
-By following these steps, you can design a control schema for your robot using state transitions and compile it into
-executable code using Botix. Remember, practice and experimentation are key – start with simple schemas and gradually
-increase complexity as you become more comfortable with the process. Always test your schemas in a safe environment
-before deploying on actual hardware.
+set_log_level(CRITICAL)  # this has the same effect as above
+```
```

