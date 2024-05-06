# Comparing `tmp/pyrf24-0.2.5.tar.gz` & `tmp/pyrf24-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrf24-0.2.5.tar", last modified: Tue Dec  5 05:21:33 2023, max compression
+gzip compressed data, was "pyrf24-0.3.0.tar", last modified: Mon May  6 09:38:49 2024, max compression
```

## Comparing `pyrf24-0.2.5.tar` & `pyrf24-0.3.0.tar`

### file list

```diff
@@ -1,203 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.446050 pyrf24-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2023-12-05 04:27:04.000000 pyrf24-0.2.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2023-12-05 04:27:04.000000 pyrf24-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-05 04:27:04.000000 pyrf24-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13682 2023-12-05 05:21:33.442050 pyrf24-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2023-12-05 04:27:04.000000 pyrf24-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.418050 pyrf24-0.2.5/RF24/
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    68031 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/RF24.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    96322 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/RF24.h
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/RF24_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.418050 pyrf24-0.2.5/RF24/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/AutoConfig_RF24_DRIVER.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/CPackInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/Cache.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/CompilerWarnings.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/GetLibInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/Sanitizers.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/StandardProjectSettings.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/StaticAnalyzers.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/detectCPU.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/cmake/pico_sdk_import.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/nRF24L01.h
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/printf.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.418050 pyrf24-0.2.5/RF24/utility/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.418050 pyrf24-0.2.5/RF24/utility/LittleWire/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/LittleWire/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/LittleWire/includes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.422050 pyrf24-0.2.5/RF24/utility/MRAA/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/gpio.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/gpio.h
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/includes.h
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/MRAA/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.422050 pyrf24-0.2.5/RF24/utility/RPi/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (127)    61079 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/bcm2835.c
--rw-r--r--   0 runner    (1001) docker     (127)    96902 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/bcm2835.h
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/includes.h
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/interrupt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/interrupt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/RPi/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.426050 pyrf24-0.2.5/RF24/utility/SPIDEV/
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/gpio.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/gpio.h
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/includes.h
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/interrupt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/interrupt.h
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/SPIDEV/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.426050 pyrf24-0.2.5/RF24/utility/pigpio/
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/gpio.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/gpio.h
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/includes.h
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/interrupt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/interrupt.h
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/pigpio/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.426050 pyrf24-0.2.5/RF24/utility/wiringPi/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/wiringPi/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/wiringPi/includes.h
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/wiringPi/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24/utility/wiringPi/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.426050 pyrf24-0.2.5/RF24Mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19586 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/RF24Mesh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16516 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/RF24Mesh.h
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/RF24Mesh_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.430050 pyrf24-0.2.5/RF24Mesh/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/CPackInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/Cache.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/CompilerWarnings.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/GetLibInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/StandardProjectSettings.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/detectCPU.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/enableNcursesExample.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Mesh/cmake/usePicoSDK.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.430050 pyrf24-0.2.5/RF24Network/
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47308 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/RF24Network.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    42775 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/RF24Network.h
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/RF24Network_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.430050 pyrf24-0.2.5/RF24Network/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/CPackInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/Cache.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/CompilerWarnings.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/GetLibInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/StandardProjectSettings.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/detectCPU.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-05 04:27:09.000000 pyrf24-0.2.5/RF24Network/cmake/usePicoSDK.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.430050 pyrf24-0.2.5/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-12-05 04:27:04.000000 pyrf24-0.2.5/cmake/using_flags.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.430050 pyrf24-0.2.5/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/.codespell-ignore-lines
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.414050 pyrf24-0.2.5/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.434050 pyrf24-0.2.5/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    23959 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    65660 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.438050 pyrf24-0.2.5/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28518 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    52930 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    26305 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    42613 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.438050 pyrf24-0.2.5/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)    31450 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13471 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    79416 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   126420 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    94641 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.438050 pyrf24-0.2.5/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    29747 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.438050 pyrf24-0.2.5/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17650 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.442050 pyrf24-0.2.5/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-05 04:27:09.000000 pyrf24-0.2.5/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2023-12-05 04:27:04.000000 pyrf24-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.442050 pyrf24-0.2.5/pyrf24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13682 2023-12-05 05:21:33.000000 pyrf24-0.2.5/pyrf24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2023-12-05 05:21:33.000000 pyrf24-0.2.5/pyrf24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 05:21:33.000000 pyrf24-0.2.5/pyrf24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 05:21:33.000000 pyrf24-0.2.5/pyrf24.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-05 05:21:33.000000 pyrf24-0.2.5/pyrf24.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-05 04:27:04.000000 pyrf24-0.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-05 04:27:04.000000 pyrf24-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 05:21:33.446050 pyrf24-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-12-05 04:27:04.000000 pyrf24-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.442050 pyrf24-0.2.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)    59874 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyRF24.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyRF24Mesh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23537 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyRF24Network.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 05:21:33.442050 pyrf24-0.2.5/src/pyrf24/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyrf24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35160 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyrf24/fake_ble.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyrf24/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyrf24/rf24.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyrf24/rf24_mesh.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2023-12-05 04:27:04.000000 pyrf24-0.2.5/src/pyrf24/rf24_network.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.258658 pyrf24-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-06 09:06:49.000000 pyrf24-0.3.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-06 09:06:49.000000 pyrf24-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-06 09:06:49.000000 pyrf24-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-05-06 09:38:49.258658 pyrf24-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-06 09:06:49.000000 pyrf24-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.226658 pyrf24-0.3.0/RF24/
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    67952 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/RF24.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    96227 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/RF24.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/RF24_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.230658 pyrf24-0.3.0/RF24/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/AutoConfig_RF24_DRIVER.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/CPackInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/Cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/CompilerWarnings.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/GetLibInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/Sanitizers.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/StaticAnalyzers.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/detectCPU.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/cmake/pico_sdk_import.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/nRF24L01.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/printf.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.230658 pyrf24-0.3.0/RF24/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.230658 pyrf24-0.3.0/RF24/utility/LittleWire/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/LittleWire/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/LittleWire/includes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.230658 pyrf24-0.3.0/RF24/utility/MRAA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/gpio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/includes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/MRAA/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.234658 pyrf24-0.3.0/RF24/utility/RPi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61079 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/bcm2835.c
+-rw-r--r--   0 runner    (1001) docker     (127)    96902 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/bcm2835.h
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/includes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/RPi/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.234658 pyrf24-0.3.0/RF24/utility/SPIDEV/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/gpio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/includes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/SPIDEV/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.238659 pyrf24-0.3.0/RF24/utility/pigpio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/gpio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/includes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/pigpio/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.238659 pyrf24-0.3.0/RF24/utility/wiringPi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/wiringPi/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/wiringPi/includes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/wiringPi/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/wiringPi/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24/utility/wiringPi/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.238659 pyrf24-0.3.0/RF24Mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19586 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/RF24Mesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/RF24Mesh.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/RF24Mesh_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.238659 pyrf24-0.3.0/RF24Mesh/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/CPackInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/Cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/CompilerWarnings.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/GetLibInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/detectCPU.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/enableNcursesExample.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Mesh/cmake/usePicoSDK.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.242658 pyrf24-0.3.0/RF24Network/
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47766 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/RF24Network.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42695 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/RF24Network.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/RF24Network_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.242658 pyrf24-0.3.0/RF24Network/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/CPackInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/Cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/CompilerWarnings.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/GetLibInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/detectCPU.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-06 09:06:52.000000 pyrf24-0.3.0/RF24Network/cmake/usePicoSDK.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.242658 pyrf24-0.3.0/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-06 09:06:49.000000 pyrf24-0.3.0/cmake/using_flags.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.242658 pyrf24-0.3.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.222658 pyrf24-0.3.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.246658 pyrf24-0.3.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    65660 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.250658 pyrf24-0.3.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28518 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    42613 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.250658 pyrf24-0.3.0/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)    31450 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13471 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79416 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   126420 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    94641 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.250658 pyrf24-0.3.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29747 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.250658 pyrf24-0.3.0/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17650 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.254658 pyrf24-0.3.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-06 09:06:52.000000 pyrf24-0.3.0/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 09:06:49.000000 pyrf24-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.258658 pyrf24-0.3.0/pyrf24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-05-06 09:38:49.000000 pyrf24-0.3.0/pyrf24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-06 09:38:49.000000 pyrf24-0.3.0/pyrf24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:38:49.000000 pyrf24-0.3.0/pyrf24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:38:49.000000 pyrf24-0.3.0/pyrf24.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 09:38:49.000000 pyrf24-0.3.0/pyrf24.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 09:06:49.000000 pyrf24-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 09:06:49.000000 pyrf24-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:38:49.258658 pyrf24-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-06 09:06:49.000000 pyrf24-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.254658 pyrf24-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.254658 pyrf24-0.3.0/src/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/linux/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53813 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyRF24.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyRF24.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyRF24Mesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyRF24Mesh.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyRF24Network.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyRF24Network.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:38:49.258658 pyrf24-0.3.0/src/pyrf24/
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyrf24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34950 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyrf24/fake_ble.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyrf24/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyrf24/rf24.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyrf24/rf24_mesh.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-06 09:06:49.000000 pyrf24-0.3.0/src/pyrf24/rf24_network.pyi
```

### Comparing `pyrf24-0.2.5/LICENSE` & `pyrf24-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/MANIFEST.in` & `pyrf24-0.3.0/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 recursive-exclude */cmake/toolchains *.cmake
 recursive-exclude RF24/utility/AT* *.h *.cpp *.c
 recursive-exclude RF24/utility/Teensy *.h
 recursive-exclude RF24/utility/Template* *.h
 recursive-exclude RF24/utility/rp2 *.h *.cpp *.txt
 recursive-exclude RF24*/pyRF24* *
 recursive-exclude RF24Network/RPi/pyRF24Network *
-global-exclude .clang-format .clang-tidy .git* library.json library.properties Doxyfile keywords.txt Makefile* doxygen-custom.css **.yml **.yaml *.pdf .pylintrc
+global-exclude .clang-format .clang-tidy .git* library.json library.properties Doxyfile keywords.txt Makefile* doxygen-custom.css **.yml **.yaml *.pdf
 exclude */*.md */README* RF24/utility/includes.h RF24/configure
 include pyproject.toml setup.py CMakeLists.txt
```

### Comparing `pyrf24-0.2.5/PKG-INFO` & `pyrf24-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrf24
-Version: 0.2.5
+Version: 0.3.0
 Summary: A python package for the wrapping nRF24 related C++ libraries.
 Author-email: Brendan Doherty <2bndy5@gmail.com>
 License: GPLv2
 Project-URL: Documentation, http://nRF24.github.io/pyRF24
 Project-URL: Source, https://github.com/nRF24/pyRF24
 Project-URL: Tracker, https://github.com/nRF24/pyRF24/issues
 Keywords: nrf24l01,nRF24L01+,raspberry,pi,driver,radio,transceiver
@@ -23,27 +23,29 @@
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. image:: https://img.shields.io/piwheels/v/pyrf24?color=informational
+.. |piwheels-badge| image:: https://img.shields.io/piwheels/v/pyrf24?color=informational
     :target: https://www.piwheels.org/project/pyrf24/
     :alt: piwheels
-.. image:: https://img.shields.io/readthedocs/pyrf24?label=ReadTheDocs&logo=readthedocs&logoColor=white
+.. |rtd-badge| image:: https://img.shields.io/readthedocs/pyrf24?label=ReadTheDocs&logo=readthedocs&logoColor=white
     :target: https://pyrf24.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
-.. image:: https://static.pepy.tech/personalized-badge/pyrf24?period=total&units=none&left_color=grey&right_color=blue&left_text=PyPI%20Downloads
+.. |pypi-downloads| image:: https://img.shields.io/pepy/dt/pyrf24?label=PyPI%20Downloads&color=blue
     :target: https://pepy.tech/project/pyrf24
     :alt: PyPI Downloads
-.. image:: https://github.com/nRF24/pyRF24/actions/workflows/build.yml/badge.svg
+.. |ci-badge| image:: https://github.com/nRF24/pyRF24/actions/workflows/build.yml/badge.svg
     :target: https://github.com/nRF24/pyRF24/actions/workflows/build.yml
     :alt: Build CI
 
+|piwheels-badge| |rtd-badge| |pypi-downloads| |ci-badge|
+
 Introduction
 ============
 
 This is the official home of the python wrappers for the RF24 stack. It is meant for Linux-based
 SoC boards like the Raspberry Pi. Documentation is hosted at http://pyrf24.rtfd.io/.
 
 Pinout
@@ -77,24 +79,25 @@
     nRF24L01+PA+LNA modules.
 
 .. important:: It is highly recommended that the nRF24L01's VCC and GND pins have a parallel
     capacitor to stabilize the power supply. Usually 100 microfarad is enough, but the capacitance
     ultimately depends on the nature of your power supply's stability.
 
 .. note::
-    Notice that RPi.GPIO (for python) is used to manage the GPIO pins on the Raspberry Pi
+    Notice that `gpiod <https://pypi.org/project/gpiod>`_ is used to watch the radio's IRQ pin
     (exclusively during the
     `interrupt_configure.py <https://pyrf24.readthedocs.io/en/latest/examples.html#interrupt-configure>`_
     example).
 
-    RPi.GPIO is not required for normal usage (when not using the radio's IRQ pin).
+    `gpiod <https://pypi.org/project/gpiod>`_ is not required for normal usage (when not using the radio's IRQ pin).
 
     .. code-block:: bash
 
-        sudo apt install python3-rpi.gpio
+        sudo apt install python3-dev
+        pip install gpiod
 
 Installing from PyPI
 ~~~~~~~~~~~~~~~~~~~~
 
 Simply use:
 
 .. code-block:: python
@@ -195,20 +198,22 @@
        the third commit (``dev3``) since the first "post release" (``post1``) after the
        tagged version ``0.1.1``. This adhere's to `PEP440 <https://peps.python.org/pep-0440>`_.
    - ``cp3X`` is the version of python used to build the wheel (ie ``cp39`` for CPython 3.9)
      The second occurrence of ``cp3X`` describes the CPython ABI compatibility.
    - ``ARCH`` is the architecture type of the CPU. This corresponds to the compiler used.
      On Raspberry Pi OS (32 bit), this will be ``armv7l``.
 
+.. _using-specific-driver:
+
 Using a specific RF24 driver
 ----------------------------
 
-By default, this package is built using the RF24 driver SPIDEV. If you want to build the
-package using a different RF24 driver (like ``RPi``, ``MRAA``, ``wiringPi``, etc), then
-it is necessary to use an environment variable containing additional arguments for CMake:
+By default, this package is built using the RF24 driver ``SPIDEV``. If you want to build the
+package using a different RF24 driver (like ``RPi``, ``MRAA``, ``wiringPi``, or ``pigpio``),
+then it is necessary to use an environment variable containing additional arguments for CMake:
 
 .. code-block:: bash
 
     export CMAKE_ARGS="-DRF24_DRIVER=RPi"
 
 .. hint::
     You can also use this environment variable to enable debug output from different
```

### Comparing `pyrf24-0.2.5/README.rst` & `pyrf24-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-.. image:: https://img.shields.io/piwheels/v/pyrf24?color=informational
+.. |piwheels-badge| image:: https://img.shields.io/piwheels/v/pyrf24?color=informational
     :target: https://www.piwheels.org/project/pyrf24/
     :alt: piwheels
-.. image:: https://img.shields.io/readthedocs/pyrf24?label=ReadTheDocs&logo=readthedocs&logoColor=white
+.. |rtd-badge| image:: https://img.shields.io/readthedocs/pyrf24?label=ReadTheDocs&logo=readthedocs&logoColor=white
     :target: https://pyrf24.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
-.. image:: https://static.pepy.tech/personalized-badge/pyrf24?period=total&units=none&left_color=grey&right_color=blue&left_text=PyPI%20Downloads
+.. |pypi-downloads| image:: https://img.shields.io/pepy/dt/pyrf24?label=PyPI%20Downloads&color=blue
     :target: https://pepy.tech/project/pyrf24
     :alt: PyPI Downloads
-.. image:: https://github.com/nRF24/pyRF24/actions/workflows/build.yml/badge.svg
+.. |ci-badge| image:: https://github.com/nRF24/pyRF24/actions/workflows/build.yml/badge.svg
     :target: https://github.com/nRF24/pyRF24/actions/workflows/build.yml
     :alt: Build CI
 
+|piwheels-badge| |rtd-badge| |pypi-downloads| |ci-badge|
+
 Introduction
 ============
 
 This is the official home of the python wrappers for the RF24 stack. It is meant for Linux-based
 SoC boards like the Raspberry Pi. Documentation is hosted at http://pyrf24.rtfd.io/.
 
 Pinout
@@ -48,24 +50,25 @@
     nRF24L01+PA+LNA modules.
 
 .. important:: It is highly recommended that the nRF24L01's VCC and GND pins have a parallel
     capacitor to stabilize the power supply. Usually 100 microfarad is enough, but the capacitance
     ultimately depends on the nature of your power supply's stability.
 
 .. note::
-    Notice that RPi.GPIO (for python) is used to manage the GPIO pins on the Raspberry Pi
+    Notice that `gpiod <https://pypi.org/project/gpiod>`_ is used to watch the radio's IRQ pin
     (exclusively during the
     `interrupt_configure.py <https://pyrf24.readthedocs.io/en/latest/examples.html#interrupt-configure>`_
     example).
 
-    RPi.GPIO is not required for normal usage (when not using the radio's IRQ pin).
+    `gpiod <https://pypi.org/project/gpiod>`_ is not required for normal usage (when not using the radio's IRQ pin).
 
     .. code-block:: bash
 
-        sudo apt install python3-rpi.gpio
+        sudo apt install python3-dev
+        pip install gpiod
 
 Installing from PyPI
 ~~~~~~~~~~~~~~~~~~~~
 
 Simply use:
 
 .. code-block:: python
@@ -166,20 +169,22 @@
        the third commit (``dev3``) since the first "post release" (``post1``) after the
        tagged version ``0.1.1``. This adhere's to `PEP440 <https://peps.python.org/pep-0440>`_.
    - ``cp3X`` is the version of python used to build the wheel (ie ``cp39`` for CPython 3.9)
      The second occurrence of ``cp3X`` describes the CPython ABI compatibility.
    - ``ARCH`` is the architecture type of the CPU. This corresponds to the compiler used.
      On Raspberry Pi OS (32 bit), this will be ``armv7l``.
 
+.. _using-specific-driver:
+
 Using a specific RF24 driver
 ----------------------------
 
-By default, this package is built using the RF24 driver SPIDEV. If you want to build the
-package using a different RF24 driver (like ``RPi``, ``MRAA``, ``wiringPi``, etc), then
-it is necessary to use an environment variable containing additional arguments for CMake:
+By default, this package is built using the RF24 driver ``SPIDEV``. If you want to build the
+package using a different RF24 driver (like ``RPi``, ``MRAA``, ``wiringPi``, or ``pigpio``),
+then it is necessary to use an environment variable containing additional arguments for CMake:
 
 .. code-block:: bash
 
     export CMAKE_ARGS="-DRF24_DRIVER=RPi"
 
 .. hint::
     You can also use this environment variable to enable debug output from different
```

### Comparing `pyrf24-0.2.5/RF24/CMakeLists.txt` & `pyrf24-0.3.0/RF24/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -132,18 +132,20 @@
 endif()
 if(DEFINED RF24_SPI_SPEED)
     message(STATUS "RF24_SPI_SPEED set to ${RF24_SPI_SPEED}")
     target_compile_definitions(${LibTargetName} PUBLIC
         RF24_SPI_SPEED=${RF24_SPI_SPEED}
     )
 endif()
-# conditionally disable interruot support (a pigpio specific feature)
-if("${LibPIGPIO}" STREQUAL "LibPIGPIO-NOTFOUND" OR DEFINED RF24_NO_INTERRUPT)
-    message(STATUS "Disabling IRQ pin support")
-    target_compile_definitions(${LibTargetName} PUBLIC RF24_NO_INTERRUPT)
+# allow user customization of default GPIO chip used with the SPIDEV driver
+if(DEFINED RF24_LINUX_GPIO_CHIP)
+    message(STATUS "RF24_LINUX_GPIO_CHIP set to ${RF24_LINUX_GPIO_CHIP}")
+    target_compile_definitions(${LibTargetName} PUBLIC
+        RF24_LINUX_GPIO_CHIP="${RF24_LINUX_GPIO_CHIP}"
+    )
 endif()
 
 
 #####################################
 ### Install rules for root source dir
 ### There are separate install rules defined for each utility driver
 ### Installing the library requires sudo privileges
```

### Comparing `pyrf24-0.2.5/RF24/LICENSE` & `pyrf24-0.3.0/RF24/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/RF24.cpp` & `pyrf24-0.3.0/RF24/RF24.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1026,19 +1026,14 @@
     if (!isValid()) {
         // didn't specify the CSN & CE pins to c'tor nor begin()
         return false;
     }
 
 #if defined(RF24_LINUX)
 
-    #if defined(MRAA)
-    GPIO();
-    gpio.begin(ce_pin, csn_pin);
-    #endif
-
     pinMode(ce_pin, OUTPUT);
     ce(LOW);
     delay(100);
 
 #elif defined(LITTLEWIRE)
     pinMode(csn_pin, OUTPUT);
     csn(HIGH);
```

### Comparing `pyrf24-0.2.5/RF24/RF24.h` & `pyrf24-0.3.0/RF24/RF24.h`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,14 @@
 
 #if defined(RF24_LINUX) || defined(XMEGA_D3) /* XMEGA can use SPI class */
     SPI spi;
 #endif // defined (RF24_LINUX) || defined (XMEGA_D3)
 #if defined(RF24_SPI_PTR)
     _SPI* _spi;
 #endif // defined (RF24_SPI_PTR)
-#if defined(MRAA)
-    GPIO gpio;
-#endif
 
     rf24_gpio_pin_t ce_pin;  /* "Chip Enable" pin, activates the RX or TX role */
     rf24_gpio_pin_t csn_pin; /* SPI Chip select */
     uint32_t spi_speed;      /* SPI Bus Speed */
 #if defined(RF24_LINUX) || defined(XMEGA_D3) || defined(RF24_RP2)
     uint8_t spi_rxbuff[32 + 1]; //SPI receive buffer (payload max 32 bytes)
     uint8_t spi_txbuff[32 + 1]; //SPI transmit buffer (payload max 32 bytes + 1 byte for the command)
@@ -251,15 +248,15 @@
      * calling this function.
      *
      * @warning This function is for the Arduino platforms only
      *
      * @param spiBus A pointer or reference to an instantiated SPI bus object.
      * The `_SPI` datatype is a "wrapped" definition that will represent
      * various SPI implementations based on the specified platform.
-     * @see Review the [Arduino support page](md_docs_arduino.html).
+     * @see Review the [Arduino support page](arduino.md).
      *
      * @return same result as begin()
      */
     bool begin(_SPI* spiBus);
 
     /**
      * Same as begin(), but allows dynamically specifying a SPI bus, CE pin,
@@ -274,15 +271,15 @@
      * The `_SPI` datatype is a "wrapped" definition that will represent
      * various SPI implementations based on the specified platform.
      * @param _cepin The pin attached to Chip Enable on the RF module
      * @param _cspin The pin attached to Chip Select (often labeled CSN) on the radio module.
      * - For the Arduino Due board, the [Arduino Due extended SPI feature](https://www.arduino.cc/en/Reference/DueExtendedSPI)
      * is not supported. This means that the Due's pins 4, 10, or 52 are not mandated options (can use any digital output pin) for the radio's CSN pin.
      *
-     * @see Review the [Arduino support page](md_docs_arduino.html).
+     * @see Review the [Arduino support page](arduino.md).
      *
      * @return same result as begin()
      */
     bool begin(_SPI* spiBus, rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin);
 #endif // defined (RF24_SPI_PTR) || defined (DOXYGEN_FORCED)
 
     /**
@@ -874,15 +871,15 @@
      * @warning
      * @parblock
      * It is important to never keep the nRF24L01 in TX mode and FIFO full for more than 4ms at a time. If the auto
      * retransmit is enabled, the nRF24L01 is never in TX mode long enough to disobey this rule. Allow the FIFO
      * to clear by issuing txStandBy() or ensure appropriate time between transmissions.
      *
      * Use txStandBy() when this function returns `false`.
-     * 
+     *
      * Example (Partial blocking):
      * @code
      * radio.writeFast(&buf,32);  // Writes 1 payload to the buffers
      * txStandBy();     		   // Returns 0 if failed. 1 if success. Blocks only until MAX_RT timeout or success. Data flushed on fail.
      *
      * radio.writeFast(&buf,32);  // Writes 1 payload to the buffers
      * txStandBy(1000);		   // Using extended timeouts, returns 1 if success. Retries failed payloads for 1 seconds before returning 0.
@@ -1273,19 +1270,19 @@
      *
      * Useful to check for interference on the current channel and
      * channel hopping strategies.
      *
      * @code
      * bool goodSignal = radio.testRPD();
      * if(radio.available()){
-     *    Serial.println(goodSignal ? "Strong signal > 64dBm" : "Weak signal < 64dBm" );
-     *    radio.read(0,0);
+     *    Serial.println(goodSignal ? "Strong signal > -64dBm" : "Weak signal < -64dBm" );
+     *    radio.read(&payload,sizeof(payload));
      * }
      * @endcode
-     * @return true if a signal less than or equal to -64dBm was detected,
+     * @return true if a signal greater than or equal to -64dBm was detected,
      * false if not.
      */
     bool testRPD(void);
 
     /**
      * Test whether this is a real radio, or a mock shim for
      * debugging.  Setting either pin to 0xff is the way to
@@ -2232,15 +2229,15 @@
 
 /**
  * @example{lineno} examples_linux/getting_started.py
  * Written by [2bndy5](http://github.com/2bndy5) in 2020
  *
  * This is a simple example of using the RF24 class on a Raspberry Pi.
  *
- * Remember to install the [Python wrapper](md_docs_python_wrapper.html), then
+ * Remember to install the [Python wrapper](python_wrapper.md), then
  * navigate to the "RF24/examples_linux" folder.
  * <br>To run this example, enter
  * @code{.sh}python3 getting_started.py @endcode and follow the prompts.
  *
  * @note this example requires python v3.7 or newer because it measures
  * transmission time with `time.monotonic_ns()`.
  */
@@ -2248,15 +2245,15 @@
 /**
  * @example{lineno} examples_linux/acknowledgement_payloads.py
  * Written by [2bndy5](http://github.com/2bndy5) in 2020
  *
  * This is a simple example of using the RF24 class on a Raspberry Pi to
  * transmit and retrieve custom automatic acknowledgment payloads.
  *
- * Remember to install the [Python wrapper](md_docs_python_wrapper.html), then
+ * Remember to install the [Python wrapper](python_wrapper.md), then
  * navigate to the "RF24/examples_linux" folder.
  * <br>To run this example, enter
  * @code{.sh}python3 acknowledgement_payloads.py @endcode and follow the prompts.
  *
  * @note this example requires python v3.7 or newer because it measures
  * transmission time with `time.monotonic_ns()`.
  */
@@ -2267,15 +2264,15 @@
  *
  * This is a simple example of using the RF24 class on a Raspberry Pi to
  * transmit and respond with acknowledgment (ACK) transmissions. Notice that
  * the auto-ack feature is enabled, but this example doesn't use automatic ACK
  * payloads because automatic ACK payloads' data will always be outdated by 1
  * transmission. Instead, this example uses a call and response paradigm.
  *
- * Remember to install the [Python wrapper](md_docs_python_wrapper.html), then
+ * Remember to install the [Python wrapper](python_wrapper.md), then
  * navigate to the "RF24/examples_linux" folder.
  * <br>To run this example, enter
  * @code{.sh}python3 manual_acknowledgements.py @endcode and follow the prompts.
  *
  * @note this example requires python v3.7 or newer because it measures
  * transmission time with `time.monotonic_ns()`.
  */
@@ -2283,15 +2280,15 @@
 /**
  * @example{lineno} examples_linux/streaming_data.py
  * Written by [2bndy5](http://github.com/2bndy5) in 2020
  *
  * This is a simple example of using the RF24 class on a Raspberry Pi for
  * streaming multiple payloads.
  *
- * Remember to install the [Python wrapper](md_docs_python_wrapper.html), then
+ * Remember to install the [Python wrapper](python_wrapper.md), then
  * navigate to the "RF24/examples_linux" folder.
  * <br>To run this example, enter
  * @code{.sh}python3 streaming_data.py @endcode and follow the prompts.
  *
  * @note this example requires python v3.7 or newer because it measures
  * transmission time with `time.monotonic_ns()`.
  */
@@ -2299,15 +2296,15 @@
 /**
  * @example{lineno} examples_linux/interrupt_configure.py
  * Written by [2bndy5](http://github.com/2bndy5) in 2020
  *
  * This is a simple example of using the RF24 class on a Raspberry Pi to
  * detecting (and verifying) the IRQ (interrupt) pin on the nRF24L01.
  *
- * Remember to install the [Python wrapper](md_docs_python_wrapper.html), then
+ * Remember to install the [Python wrapper](python_wrapper.md), then
  * navigate to the "RF24/examples_linux" folder.
  * <br>To run this example, enter
  * @code{.sh}python3 interrupt_configure.py @endcode and follow the prompts.
  *
  * @note this example requires python v3.7 or newer because it measures
  * transmission time with `time.monotonic_ns()`.
  */
@@ -2316,15 +2313,15 @@
  * @example{lineno} examples_linux/multiceiver_demo.py
  * Written by [2bndy5](http://github.com/2bndy5) in 2020
  *
  * This is a simple example of using the RF24 class on a Raspberry Pi for
  * using 1 nRF24L01 to receive data from up to 6 other transceivers. This
  * technique is called "multiceiver" in the datasheet.
  *
- * Remember to install the [Python wrapper](md_docs_python_wrapper.html), then
+ * Remember to install the [Python wrapper](python_wrapper.md), then
  * navigate to the "RF24/examples_linux" folder.
  * <br>To run this example, enter
  * @code{.sh}python3 multiceiver_demo.py @endcode and follow the prompts.
  *
  * @note this example requires python v3.7 or newer because it measures
  * transmission time with `time.monotonic_ns()`.
  */
```

### Comparing `pyrf24-0.2.5/RF24/RF24_config.h` & `pyrf24-0.3.0/RF24/RF24_config.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/AutoConfig_RF24_DRIVER.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/CPackInfo.cmake` & `pyrf24-0.3.0/RF24/cmake/CPackInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/Cache.cmake` & `pyrf24-0.3.0/RF24/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/CompilerWarnings.cmake` & `pyrf24-0.3.0/RF24/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/GetLibInfo.cmake` & `pyrf24-0.3.0/RF24/cmake/GetLibInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/PreventInSourceBuilds.cmake` & `pyrf24-0.3.0/RF24/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/Sanitizers.cmake` & `pyrf24-0.3.0/RF24/cmake/Sanitizers.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/StandardProjectSettings.cmake` & `pyrf24-0.3.0/RF24/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/StaticAnalyzers.cmake` & `pyrf24-0.3.0/RF24/cmake/StaticAnalyzers.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/detectCPU.cmake` & `pyrf24-0.3.0/RF24/cmake/detectCPU.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/cmake/pico_sdk_import.cmake` & `pyrf24-0.3.0/RF24/cmake/pico_sdk_import.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/nRF24L01.h` & `pyrf24-0.3.0/RF24/nRF24L01.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
     Copyright (c) 2007 Stefan Engelke <mbox@stefanengelke.de>
-	Portions Copyright (C) 2011 Greg Copeland
+    Portions Copyright (C) 2011 Greg Copeland
 
     Permission is hereby granted, free of charge, to any person
     obtaining a copy of this software and associated documentation
     files (the "Software"), to deal in the Software without
     restriction, including without limitation the rights to use, copy,
     modify, merge, publish, distribute, sublicense, and/or sell copies
     of the Software, and to permit persons to whom the Software is
```

### Comparing `pyrf24-0.2.5/RF24/printf.h` & `pyrf24-0.3.0/RF24/printf.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/utility/CMakeLists.txt` & `pyrf24-0.3.0/RF24/utility/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,112 +4,84 @@
 if ("${RF24_DRIVER}" STREQUAL  "wiringPi") # Use wiringPi
     set(RF24_LINKED_DRIVER ${LibWiringPi} PARENT_SCOPE)
     add_compile_options(-pthread)
     set(RF24_DRIVER_SOURCES
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.h
         PARENT_SCOPE
     )
     install(FILES
             ${RF24_DRIVER}/includes.h
             ${RF24_DRIVER}/spi.h
             ${RF24_DRIVER}/RF24_arch_config.h
+            ${RF24_DRIVER}/interrupt.h
         DESTINATION include/RF24/utility/${RF24_DRIVER}
     )
 elseif("${RF24_DRIVER}" STREQUAL "RPi") # use RPi
     install(FILES
             ${RF24_DRIVER}/includes.h
             ${RF24_DRIVER}/bcm2835.h
             ${RF24_DRIVER}/spi.h
             ${RF24_DRIVER}/compatibility.h
             ${RF24_DRIVER}/RF24_arch_config.h
+            ${RF24_DRIVER}/interrupt.h
         DESTINATION include/RF24/utility/${RF24_DRIVER}
     )
-    if(NOT "${LibPIGPIO}" STREQUAL "LibPIGPIO-NOTFOUND" AND NOT DEFINED RF24_NO_INTERRUPT)
-        set(RF24_LINKED_DRIVER ${LibPIGPIO} PARENT_SCOPE)
-        message(STATUS "linking to pigpio lib for interrupt functionality")
-        install(FILES
-                ${RF24_DRIVER}/interrupt.h
-            DESTINATION include/RF24/utility/${RF24_DRIVER}
-        )
-        set(RF24_DRIVER_SOURCES
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/bcm2835.c
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.cpp
-            PARENT_SCOPE
-        )
-    else()
-        set(RF24_DRIVER_SOURCES
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/bcm2835.c
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
-            PARENT_SCOPE
-        )
-    endif()
+    set(RF24_DRIVER_SOURCES
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/bcm2835.c
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.cpp
+        PARENT_SCOPE
+    )
 elseif("${RF24_DRIVER}" STREQUAL "SPIDEV") # use SPIDEV
     if(NOT SPIDEV_EXISTS)
         message(WARNING "Detecting /dev/spidev0.0 failed - continuing anyway. Please make sure SPI is enabled.")
     endif()
     install(FILES
             ${RF24_DRIVER}/includes.h
             ${RF24_DRIVER}/gpio.h
             ${RF24_DRIVER}/spi.h
             ${RF24_DRIVER}/compatibility.h
             ${RF24_DRIVER}/RF24_arch_config.h
+            ${RF24_DRIVER}/interrupt.h
         DESTINATION include/RF24/utility/${RF24_DRIVER}
     )
-    if(NOT "${LibPIGPIO}" STREQUAL "LibPIGPIO-NOTFOUND" AND NOT DEFINED RF24_NO_INTERRUPT)
-        set(RF24_LINKED_DRIVER ${LibPIGPIO} PARENT_SCOPE)
-        message(STATUS "linking to pigpio lib for interrupt functionality")
-        install(FILES
-                ${RF24_DRIVER}/interrupt.h
-            DESTINATION include/RF24/utility/${RF24_DRIVER}
-        )
-        set(RF24_DRIVER_SOURCES
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/gpio.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.cpp
-            PARENT_SCOPE
-        )
-    else()
-        set(RF24_DRIVER_SOURCES
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/gpio.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
-            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
-            PARENT_SCOPE
-        )
-    endif()
+    set(RF24_DRIVER_SOURCES
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/gpio.cpp
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.cpp
+        PARENT_SCOPE
+    )
 elseif("${RF24_DRIVER}" STREQUAL "MRAA") # use MRAA
     set(RF24_LINKED_DRIVER ${LibMRAA} PARENT_SCOPE)
     set(RF24_DRIVER_SOURCES
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/gpio.cpp
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/compatibility.cpp
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/RF24_arch_config.h
+        ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.cpp
         PARENT_SCOPE
     )
     install(FILES
             ${RF24_DRIVER}/includes.h
             ${RF24_DRIVER}/gpio.h
             ${RF24_DRIVER}/spi.h
             ${RF24_DRIVER}/compatibility.h
             ${RF24_DRIVER}/RF24_arch_config.h
-        DESTINATION include/RF24/utility/${RF24_DRIVER}
+            ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/interrupt.h
+            DESTINATION include/RF24/utility/${RF24_DRIVER}
     )
 elseif("${RF24_DRIVER}" STREQUAL "pigpio") # use pigpio
     set(RF24_LINKED_DRIVER ${LibPIGPIO} PARENT_SCOPE)
     set(RF24_DRIVER_SOURCES
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/includes.h
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/gpio.cpp
         ${CMAKE_CURRENT_LIST_DIR}/${RF24_DRIVER}/spi.cpp
```

### Comparing `pyrf24-0.2.5/RF24/utility/LittleWire/RF24_arch_config.h` & `pyrf24-0.3.0/RF24/utility/LittleWire/RF24_arch_config.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/utility/MRAA/RF24_arch_config.h` & `pyrf24-0.3.0/RF24/utility/MRAA/RF24_arch_config.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 #ifndef RF24_UTILITY_MRAA_RF24_ARCH_CONFIG_H_
 #define RF24_UTILITY_MRAA_RF24_ARCH_CONFIG_H_
 
+#include <stdint.h> // uint16_t
+#include <stdio.h>  // printf
+#include <string.h> // strlen
 #include "mraa.h"
 #include "spi.h"
 #include "gpio.h"
 #include "compatibility.h"
 
-#include <stdint.h>
-#include <stdio.h>
-#include <time.h>
-#include <string.h>
-#include <sys/time.h>
-#include <stddef.h>
-#include <iostream>
-#include <unistd.h>
-#include <stdlib.h>
-
 //#include <UtilTime.h> // Precompiled arduino x86 based utiltime for timing functions
 
 // GCC a Arduino Missing
 #define HIGH             1
 #define LOW              0
 #define _BV(x)           (1 << (x))
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
 #define pgm_read_ptr(p)  (*(void* const*)(p))
 #define _SPI             spi
 
 #define RF24_LINUX
 //typedef uint16_t prog_uint16_t;
-typedef uint16_t rf24_gpio_pin_t;
-#define RF24_PIN_INVALID 0xFFFF
 
 #define PSTR(x)   (x)
 #define printf_P  printf
 #define sprintf_P sprintf
 #define strlen_P  strlen
 #define PROGMEM
 #define PRIPSTR "%s"
 
 #ifdef SERIAL_DEBUG
     #define IF_SERIAL_DEBUG(x) ({ x; })
 #else
     #define IF_SERIAL_DEBUG(x)
 #endif
 
-#define digitalWrite(pin, value) gpio.write(pin, value)
+#define digitalWrite(pin, value) GPIO::write(pin, value)
 #define digitalRead(pin)         GPIO::read(pin)
-#define pinMode(pin, direction)  gpio.open(pin, direction)
+#define pinMode(pin, direction)  GPIO::open(pin, direction)
 
 #ifndef __TIME_H__
     // Prophet: Redefine time functions only if precompiled arduino time is not included
     #define delay(milisec)          __msleep(milisec)
     #define delayMicroseconds(usec) __usleep(usec)
     #define millis()                __millis()
 #endif
```

### Comparing `pyrf24-0.2.5/RF24/utility/MRAA/spi.cpp` & `pyrf24-0.3.0/RF24/utility/MRAA/spi.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 
+#include <mraa.h> // mraa_strresult(), mraa_result_t
 #include "spi.h"
-#include "mraa.h"
 
 SPI::SPI()
 {
     mspi = NULL;
 }
 
 void SPI::begin(int busNo, uint32_t spi_speed)
 {
     // init mraa spi bus, it will handle chip select internally. For CS pin wiring user must check SPI details in hardware manual
     mspi = new mraa::Spi(busNo);
 
-    mspi->mode(mraa::SPI_MODE0);
-    mspi->bitPerWord(8);
+    mraa::Result result;
+
+    result = mspi->mode(mraa::SPI_MODE0);
+    if (result != mraa::Result::SUCCESS) {
+        std::string msg = "[SPI::begin] Could not set bus mode;";
+        msg += mraa_strresult((mraa_result_t)result);
+        throw SPIException(msg);
+        return;
+    }
+
+    result = mspi->bitPerWord(8);
+    if (result != mraa::Result::SUCCESS) {
+        std::string msg = "[SPI::begin] Could not set bus bits per word;";
+        msg += mraa_strresult((mraa_result_t)result);
+        throw SPIException(msg);
+        return;
+    }
 
     // Prophet: this will try to set 8MHz, however MRAA will reset to max platform speed and syslog a message of it
-    mspi->frequency(spi_speed);
+    result = mspi->frequency(spi_speed);
+    if (result != mraa::Result::SUCCESS) {
+        std::string msg = "[SPI::begin] Could not set bus frequency;";
+        msg += mraa_strresult((mraa_result_t)result);
+        throw SPIException(msg);
+        return;
+    }
 }
 
 void SPI::end()
 {
     // Prophet: we should check for existence of mspi before deleting it
     if (mspi != NULL) {
         delete mspi;
```

### Comparing `pyrf24-0.2.5/RF24/utility/MRAA/spi.h` & `pyrf24-0.3.0/RF24/utility/RPi/spi.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,95 @@
 /*
  * TMRh20 2015
- * SPI layer for RF24
+ * SPI layer for RF24 <-> BCM2835
  */
-
-#ifndef RF24_UTILITY_MRAA_SPI_H_
-#define RF24_UTILITY_MRAA_SPI_H_
 /**
  * @file spi.h
  * Class declaration for SPI helper files
  */
+#ifndef RF24_UTILITY_RPI_SPI_H_
+#define RF24_UTILITY_RPI_SPI_H_
 
 #include <stdio.h>
-#include "mraa.h"
-#include "mraa.hpp"
+#include "bcm2835.h"
+#include "../../RF24_config.h"
+
+#define SPI_HAS_TRANSACTION
+#define MSBFIRST  BCM2835_SPI_BIT_ORDER_MSBFIRST
+#define SPI_MODE0 BCM2835_SPI_MODE0
+//#define RF24_SPI_SPEED 10000000 //BCM2835_SPI_SPEED_4MHZ
 
-#include "../../RF24_config.h" // This is cyclical and should be fixed
+class SPISettings
+{
+public:
+    SPISettings(uint32_t clock, uint8_t bitOrder, uint8_t dataMode)
+    {
+        init(clock, bitOrder, dataMode);
+    }
+
+    SPISettings()
+    {
+        init(RF24_SPI_SPEED, MSBFIRST, SPI_MODE0);
+    }
+
+    uint32_t clck;
+    uint8_t border;
+    uint8_t dmode;
+
+private:
+    void init(uint32_t clock, uint8_t bitOrder, uint8_t dataMode)
+    {
+        clck = clock;
+        border = bitOrder;
+        dmode = dataMode;
+    }
+
+    friend class SPIClass;
+};
 
 class SPI
 {
 public:
     SPI();
 
     virtual ~SPI();
 
-    mraa::Spi* mspi;
+    inline static uint8_t transfer(uint8_t _data);
+
+    inline static void transfernb(char* tbuf, char* rbuf, uint32_t len);
 
-    inline uint8_t transfer(uint8_t _data);
+    inline static void transfern(char* buf, uint32_t len);
 
-    inline void transfernb(char* tbuf, char* rbuf, uint32_t len);
+    static void begin(int busNo, uint32_t spi_speed = RF24_SPI_SPEED);
 
-    inline void transfern(char* buf, uint32_t len);
+    static void end();
 
-    void begin(int busNo, uint32_t spi_speed = RF24_SPI_SPEED);
+    static void setBitOrder(uint8_t bit_order);
 
-    void end();
+    static void setDataMode(uint8_t data_mode);
 
-    void setBitOrder(uint8_t bit_order);
+    static void setClockDivider(uint32_t spi_speed);
 
-    void setDataMode(uint8_t data_mode);
+    static void chipSelect(int csn_pin);
 
-    void setClockDivider(uint32_t spi_speed);
+    static void beginTransaction(SPISettings settings);
 
-    void chipSelect(int csn_pin);
+    static void endTransaction();
 };
 
 uint8_t SPI::transfer(uint8_t _data)
 {
-    return mspi->writeByte(_data);
+    uint8_t data = bcm2835_spi_transfer(_data);
+    return data;
 }
 
 void SPI::transfernb(char* tbuf, char* rbuf, uint32_t len)
 {
-    mspi->transfer((uint8_t*)tbuf, (uint8_t*)rbuf, len);
+    bcm2835_spi_transfernb(tbuf, rbuf, len);
 }
 
 void SPI::transfern(char* buf, uint32_t len)
 {
     transfernb(buf, buf, len);
 }
 
-#endif // RF24_UTILITY_MRAA_SPI_H_
+#endif // RF24_UTILITY_RPI_SPI_H_
```

### Comparing `pyrf24-0.2.5/RF24/utility/RPi/bcm2835.c` & `pyrf24-0.3.0/RF24/utility/RPi/bcm2835.c`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/utility/RPi/bcm2835.h` & `pyrf24-0.3.0/RF24/utility/RPi/bcm2835.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/utility/RPi/spi.cpp` & `pyrf24-0.3.0/RF24/utility/RPi/spi.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24/utility/SPIDEV/RF24_arch_config.h` & `pyrf24-0.3.0/RF24/utility/SPIDEV/RF24_arch_config.h`

 * *Files 9% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 
  */
 #ifndef RF24_UTILITY_SPIDEV_RF24_ARCH_CONFIG_H_
 #define RF24_UTILITY_SPIDEV_RF24_ARCH_CONFIG_H_
 
 #define RF24_LINUX
 
-#include <stddef.h>
+#include <stdint.h> // uint16_t
+#include <stdio.h>  // printf
+#include <string.h> // strlen
 #include "spi.h"
 #include "gpio.h"
 #include "compatibility.h"
-#include <stdint.h>
-#include <stdio.h>
-#include <time.h>
-#include <string.h>
-#include <sys/time.h>
+#include "interrupt.h"
 
 //#define RF24_SPI_SPEED RF24_SPIDEV_SPEED
 
 #define _BV(x) (1 << (x))
 #define _SPI   spi
 
 //#undef SERIAL_DEBUG
@@ -40,16 +38,14 @@
         #define PROGMEM __attribute__((section(".progmem.data")))
         #undef PSTR
         #define PSTR(s) (__extension__({static const char __c[] PROGMEM = (s); &__c[0]; }))
     #endif
 #endif
 
 typedef uint16_t prog_uint16_t;
-typedef uint16_t rf24_gpio_pin_t;
-#define RF24_PIN_INVALID 0xFFFF
 
 #define PSTR(x)  (x)
 #define printf_P printf
 #define strlen_P strlen
 #define PROGMEM
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define PRIPSTR          "%s"
```

### Comparing `pyrf24-0.2.5/RF24/utility/SPIDEV/compatibility.h` & `pyrf24-0.3.0/RF24/utility/SPIDEV/compatibility.h`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 #define RF24_UTILITY_SPIDEV_COMPATIBLITY_H_
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include <stdint.h> // for uintXX_t types
-#include <stddef.h>
-#include <time.h>
-#include <sys/time.h>
 
 void __msleep(int milisec);
 
 void __usleep(int milisec);
 
 void __start_timer();
```

### Comparing `pyrf24-0.2.5/RF24/utility/SPIDEV/spi.cpp` & `pyrf24-0.3.0/RF24/utility/SPIDEV/spi.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -6,23 +6,23 @@
  *
  * Patched for exception handling and selectable SPI SPEED by ldiaz 2018.
  *
  * Inspired from spidev test in linux kernel documentation
  * www.kernel.org/doc/Documentation/spi/spidev_test.c
  */
 
-#include "spi.h"
-
 #include <fcntl.h>
 #include <linux/spi/spidev.h>
-#include <memory.h>
 #include <stdio.h>
-#include <stdlib.h>
 #include <sys/ioctl.h>
 #include <unistd.h>
+#include <errno.h>
+#include <string.h>
+
+#include "spi.h"
 
 #define RF24_SPIDEV_BITS 8
 
 SPI::SPI()
     : fd(-1), _spi_speed(RF24_SPI_SPEED)
 {
 }
@@ -47,22 +47,21 @@
     {
         close(this->fd);
         this->fd = -1;
     }
 
     this->fd = open(device, O_RDWR);
     if (this->fd < 0) {
-        throw SPIException("can't open device");
+        std::string msg = "[SPI::begin] Can't open device ";
+        msg += device;
+        msg += "; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*
-  {
-        perror("can't open device");
-        abort();
 
-  }*/
     this->spiIsInitialized = true;
     init(spi_speed);
 }
 
 void SPI::init(uint32_t speed)
 {
     uint8_t bits = RF24_SPIDEV_BITS;
@@ -70,70 +69,60 @@
 
     int ret;
     /*
      * spi mode
      */
     ret = ioctl(this->fd, SPI_IOC_WR_MODE, &mode);
     if (ret == -1) {
-        throw SPIException("cant set WR spi mode");
+        std::string msg = "[SPI::init] Can't set WR spi mode; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't set spi mode");
-        abort();
-    }*/
 
     ret = ioctl(this->fd, SPI_IOC_RD_MODE, &mode);
     if (ret == -1) {
-        throw SPIException("can't set RD spi mode");
+        std::string msg = "[SPI::init] Can't set RD spi mode; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't set spi mode");
-        abort();
-    }*/
 
     /*
      * bits per word
      */
     ret = ioctl(this->fd, SPI_IOC_WR_BITS_PER_WORD, &bits);
     if (ret == -1) {
-        throw SPIException("can't set WR bits per word");
+        std::string msg = "[SPI::init] Can't set WR bits per word; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't set bits per word");
-        abort();
-    }*/
 
     ret = ioctl(this->fd, SPI_IOC_RD_BITS_PER_WORD, &bits);
     if (ret == -1) {
-        throw SPIException("can't set RD bits per word");
+        std::string msg = "[SPI::init] Can't set RD bits per word; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't set bits per word");
-        abort();
-    }*/
+
     /*
      * max speed hz
      */
     ret = ioctl(this->fd, SPI_IOC_WR_MAX_SPEED_HZ, &speed);
     if (ret == -1) {
-        throw SPIException("can't WR set max speed hz");
+        std::string msg = "[SPI::init] Can't set max WR speed hz; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't set max speed hz");
-        abort();
-    }*/
 
     ret = ioctl(this->fd, SPI_IOC_RD_MAX_SPEED_HZ, &speed);
     if (ret == -1) {
-        throw SPIException("can't RD set max speed hz");
+        std::string msg = "[SPI::init] Can't set max RD speed hz; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't set max speed hz");
-        abort();
-    }*/
+
     _spi_speed = speed;
 }
 
 uint8_t SPI::transfer(uint8_t tx)
 {
     struct spi_ioc_transfer tr;
     memset(&tr, 0, sizeof(tr));
@@ -145,20 +134,18 @@
     tr.delay_usecs = 0;
     tr.bits_per_word = RF24_SPIDEV_BITS;
     tr.cs_change = 0;
 
     int ret;
     ret = ioctl(this->fd, SPI_IOC_MESSAGE(1), &tr);
     if (ret < 1) {
-        throw SPIException("can't send spi message");
+        std::string msg = "[SPI::transfer] Can't send spi message; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't send spi message");
-        abort();
-    }*/
 
     return rx;
 }
 
 void SPI::transfernb(char* tbuf, char* rbuf, uint32_t len)
 {
     struct spi_ioc_transfer tr;
@@ -170,20 +157,18 @@
     tr.delay_usecs = 0;
     tr.bits_per_word = RF24_SPIDEV_BITS;
     tr.cs_change = 0;
 
     int ret;
     ret = ioctl(this->fd, SPI_IOC_MESSAGE(1), &tr);
     if (ret < 1) {
-        throw SPIException("can't send spi message");
+        std::string msg = "[SPI::transfernb] Can't send spi message; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
-    /*{
-        perror("can't send spi message");
-        abort();
-    }*/
 }
 
 void SPI::transfern(char* buf, uint32_t len)
 {
     transfernb(buf, buf, len);
 }
```

### Comparing `pyrf24-0.2.5/RF24/utility/SPIDEV/spi.h` & `pyrf24-0.3.0/RF24/utility/SPIDEV/spi.h`

 * *Files 24% similar despite different names*

```diff
@@ -6,20 +6,22 @@
  *
  * Class declaration for SPI helper files
  */
 
 #ifndef RF24_UTILITY_SPIDEV_SPI_H_
 #define RF24_UTILITY_SPIDEV_SPI_H_
 
-#include <inttypes.h>
+#include <stdint.h>
 #include <stdexcept>
 
-#include "../../RF24_config.h" // This is cyclical and should be fixed
+#ifndef RF24_SPI_SPEED
+    #define RF24_SPI_SPEED 10000000
+#endif
 
-/** Specific excpetion for SPI errors */
+/** Specific exception for SPI errors */
 class SPIException : public std::runtime_error
 {
 public:
     explicit SPIException(const std::string& msg)
         : std::runtime_error(msg)
     {
     }
```

### Comparing `pyrf24-0.2.5/RF24/utility/pigpio/RF24_arch_config.h` & `pyrf24-0.3.0/RF24/utility/pigpio/RF24_arch_config.h`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,25 @@
  Copyright (C) 2011 J. Coliz <maniacbug@ymail.com>
 
  This program is free software; you can redistribute it and/or
  modify it under the terms of the GNU General Public License
  version 2 as published by the Free Software Foundation.
 
  */
-#ifndef __ARCH_CONFIG_H__
-#define __ARCH_CONFIG_H__
+#ifndef RF24_UTILITY_PIGPIO_RF24_ARCH_CONFIG_H_
+#define RF24_UTILITY_PIGPIO_RF24_ARCH_CONFIG_H_
 
 #define RF24_LINUX
 
-#include <stddef.h>
+#include <stdint.h> // uint16_t
+#include <stdio.h>  // printf
+#include <string.h> // strlen
 #include "spi.h"
 #include "gpio.h"
 #include "compatibility.h"
-#include <stdint.h>
-#include <stdio.h>
-#include <time.h>
-#include <string.h>
-#include <sys/time.h>
 
 //#define RF24_SPI_SPEED RF24_SPIDEV_SPEED
 
 #define _BV(x) (1 << (x))
 #define _SPI   spi
 
 //#undef SERIAL_DEBUG
@@ -68,8 +65,8 @@
 #define OUTPUT                   GPIO::DIRECTION_OUT
 #define digitalWrite(pin, value) GPIO::write(pin, value)
 #define pinMode(pin, direction)  GPIO::open(pin, direction)
 #define delay(milisec)           __msleep(milisec)
 #define delayMicroseconds(usec)  __usleep(usec)
 #define millis()                 __millis()
 
-#endif // __ARCH_CONFIG_H__
+#endif // RF24_UTILITY_PIGPIO_RF24_ARCH_CONFIG_H_
```

### Comparing `pyrf24-0.2.5/RF24/utility/pigpio/compatibility.cpp` & `pyrf24-0.3.0/RF24/utility/pigpio/compatibility.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,29 @@
+#include <time.h>
+#include <chrono>
 #include "compatibility.h"
 
 long long mtime, seconds, useconds;
 //static struct timeval start, end;
 //struct timespec start, end;
-#include <time.h>
-#include <chrono>
-/**********************************************************************/
-/**
- * This function is added in order to simulate arduino delay() function
- * @param milisec
- */
+
 void __msleep(int milisec)
 {
     struct timespec req; // = {0};
     req.tv_sec = (time_t)milisec / 1000;
     req.tv_nsec = (milisec % 1000) * 1000000L;
     //nanosleep(&req, (struct timespec *)NULL);
     clock_nanosleep(CLOCK_REALTIME, 0, &req, NULL);
 }
 
 void __usleep(int microsec)
 {
     struct timespec req; // = {0};
     req.tv_sec = (time_t)microsec / 1000000;
-    req.tv_nsec = (microsec / 1000000) * 1000;
+    req.tv_nsec = (microsec % 1000000) * 1000;
     //nanosleep(&req, (struct timespec *)NULL);
     clock_nanosleep(CLOCK_REALTIME, 0, &req, NULL);
 }
 
 /**
  * This function is added in order to simulate arduino millis() function
  */
```

### Comparing `pyrf24-0.2.5/RF24/utility/pigpio/spi.cpp` & `pyrf24-0.3.0/RF24/utility/pigpio/spi.cpp`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 /*
  *
  */
 
-#include "spi.h"
 #include <pigpio.h>
+#include "spi.h"
 
 SPI::SPI()
 {
 }
 
 void SPI::begin(int busNo, uint32_t spi_speed)
 {
```

### Comparing `pyrf24-0.2.5/RF24/utility/wiringPi/RF24_arch_config.h` & `pyrf24-0.3.0/RF24/utility/wiringPi/RF24_arch_config.h`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,19 @@
 
  */
 #ifndef RF24_UTILITY_WIRINGPI_RF24_ARCH_CONFIG_H_
 #define RF24_UTILITY_WIRINGPI_RF24_ARCH_CONFIG_H_
 
 #define RF24_LINUX
 
-#include <stddef.h>
+#include <stdint.h> // uint16_t
+#include <stdio.h>  // printf
+#include <string.h> // strlen
 #include "spi.h"
 #include "wiringPi.h"
-#include <stdint.h>
-#include <stdio.h>
-#include <time.h>
-#include <string.h>
-#include <sys/time.h>
 
 #define _BV(x) (1 << (x))
 #define _SPI   spi
 
 #undef SERIAL_DEBUG
 #ifdef SERIAL_DEBUG
     #define IF_SERIAL_DEBUG(x) ({ x; })
```

### Comparing `pyrf24-0.2.5/RF24/utility/wiringPi/spi.cpp` & `pyrf24-0.3.0/RF24/utility/wiringPi/spi.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -4,84 +4,77 @@
  *
  * Created on
  *
  * Inspired from spi speed test from wiringPi
  * wiringPi/examples/spiSpeed.c
  */
 
-#include "spi.h"
-
-#include <wiringPi.h>
-#include <wiringPiSPI.h>
-
-#include <stdlib.h>
 #include <unistd.h>
 #include <stdint.h>
 #include <string.h>
 #include <errno.h>
 
-#define RF24_SPI_CHANNEL 0
+#include <wiringPi.h>
+#include <wiringPiSPI.h>
+#include "spi.h"
 
-SPI::SPI() : fd(-1)
+SPI::SPI() : fd(-1), channel(0)
 {
-    printf("wiringPi RF24 DRIVER\n");
 }
 
 void SPI::begin(int csn_pin, uint32_t spi_speed)
 {
+    channel = csn_pin % 10;
+
     // initialize the wiringPiSPI
     wiringPiSetup();
-    if ((this->fd = wiringPiSPISetup(RF24_SPI_CHANNEL, spi_speed)) < 0) {
-        printf("Cannot configure the SPI device!\n");
-        fflush(stdout);
-        abort();
-    }
-    else {
-        printf("Configured SPI fd: %d - pin: %d\n", fd, csn_pin);
+    if ((this->fd = wiringPiSPISetup(channel, spi_speed)) < 0) {
+        std::string msg = "[SPI::begin] Cannot configure the SPI device!; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
 }
 
 uint8_t SPI::transfer(uint8_t tx)
 {
-    memset(&msgByte, 0, sizeof(msgByte));
-    memcpy(&msgByte, &tx, sizeof(tx));
+    memset(&xferByte, 0, sizeof(xferByte));
+    memcpy(&xferByte, &tx, sizeof(tx));
 
-    if (wiringPiSPIDataRW(RF24_SPI_CHANNEL, &msgByte, sizeof(tx)) < 0) {
-        printf("transfer(): Cannot send data: %s\n", strerror(errno));
-        fflush(stdout);
-        abort();
+    if (wiringPiSPIDataRW(channel, &xferByte, sizeof(tx)) < 0) {
+        std::string msg = "[SPI::transfer] Cannot send spi message; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
+        return 0;
     }
 
-    return msgByte;
+    return xferByte;
 }
 
 void SPI::transfern(char* buf, uint32_t len)
 {
-    printf("transfern(tx: %s)\n", buf);
-
-    if (wiringPiSPIDataRW(RF24_SPI_CHANNEL, (uint8_t*)buf, len) < 0) {
-        printf("transfern(): Cannot send data %s\n", strerror(errno));
-        fflush(stdout);
-        abort();
+    if (wiringPiSPIDataRW(channel, (uint8_t*)buf, len) < 0) {
+        std::string msg = "[SPI::transfern] Cannot send spi message; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
 }
 
 void SPI::transfernb(char* tbuf, char* rbuf, uint32_t len)
 {
     // using an auxiliary buffer to keep tx and rx different
-    memset(msg, 0, sizeof(msg));
-    memcpy(msg, tbuf, len);
+    memset(xferBuf, 0, sizeof(xferBuf));
+    memcpy(xferBuf, tbuf, len);
 
-    if (wiringPiSPIDataRW(RF24_SPI_CHANNEL, msg, len) < 0) {
-        printf("transfernb() Cannot send data %s\n", strerror(errno));
-        fflush(stdout);
-        abort();
+    if (wiringPiSPIDataRW(channel, xferBuf, len) < 0) {
+        std::string msg = "[SPI::transfernb] Cannot send spi message; ";
+        msg += strerror(errno);
+        throw SPIException(msg);
     }
 
-    memcpy(rbuf, msg, len);
+    memcpy(rbuf, xferBuf, len);
 }
 
 SPI::~SPI()
 {
     if (this->fd >= 0) {
         close(this->fd);
         this->fd = -1;
```

### Comparing `pyrf24-0.2.5/RF24/utility/wiringPi/spi.h` & `pyrf24-0.3.0/RF24/utility/wiringPi/spi.h`

 * *Files 23% similar despite different names*

```diff
@@ -2,20 +2,31 @@
  * @file spi.h
  * Class declaration for SPI helper files
  */
 
 #ifndef RF24_UTILITY_WIRINGPI_SPI_H_
 #define RF24_UTILITY_WIRINGPI_SPI_H_
 
-#include <stdio.h>
-#include <inttypes.h>
+#include <stdint.h>
+#include <stdexcept>
+#include <string>
+
+#ifndef RF24_SPI_SPEED
+    #define RF24_SPI_SPEED 10000000
+#endif
 
-#include "../../RF24_config.h" // This is cyclical and should be fixed
-
-using namespace std;
+/** Specific exception for SPI errors */
+class SPIException : public std::runtime_error
+{
+public:
+    explicit SPIException(const std::string& msg)
+        : std::runtime_error(msg)
+    {
+    }
+};
 
 class SPI
 {
 
 public:
     SPI();
 
@@ -27,12 +38,13 @@
 
     void transfern(char*, const uint32_t);
 
     virtual ~SPI();
 
 private:
     int fd;
-    uint8_t msg[32 + 1];
-    uint8_t msgByte;
+    int channel;
+    uint8_t xferBuf[32 + 1];
+    uint8_t xferByte;
 };
 
 #endif // RF24_UTILITY_WIRINGPI_SPI_H_
```

### Comparing `pyrf24-0.2.5/RF24Mesh/CMakeLists.txt` & `pyrf24-0.3.0/RF24Mesh/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/LICENSE` & `pyrf24-0.3.0/RF24Mesh/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/RF24Mesh.cpp` & `pyrf24-0.3.0/RF24Mesh/RF24Mesh.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/RF24Mesh.h` & `pyrf24-0.3.0/RF24Mesh/RF24Mesh.h`

 * *Files 0% similar despite different names*

```diff
@@ -76,26 +76,26 @@
      * The mesh library and class documentation is currently in active development and usage may change.
      */
     /**@{*/
 
 public:
     /**
      * Construct the mesh.
-     * 
+     *
      * v2.0 supports a backward compatible constructor:
      * @code
      * RF24 radio(7, 8);
      * RF24Network network(radio);
      * RF24Mesh mesh(radio, network); // for nRF24L01
      *
      * nrf_to_nrf radio1;
      * RF52Network network1(radio1);
      * RF52Mesh mesh1(network1, radio1); // for nRF52xxx family
      * @endcode
-     * 
+     *
      * @see v2.0 supports [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf)
      * for nrf52 chips' internal radio.
      * @param _radio The underlying radio driver instance
      * @param _network The underlying network instance
      */
     ESBMesh(radio_t& _radio, network_t& _network);
 
@@ -367,19 +367,19 @@
     bool meshStarted;
     /** Returns the number of octal digits in the specified address. */
     uint8_t getLevel(uint16_t address);
 };
 
 /**
  * A type definition of the template class `ESBMesh` to maintain backward compatibility.
- * 
+ *
  * ```.cpp
  * RF24 radio(7, 8);
  * RF24Network network(radio);
- * 
+ *
  * RF24Mesh mesh(radio, network);
  * // is equivalent to
  * ESBMesh<ESBNetwork<RF24>, RF24> mesh(radio, network);
  * ```
  */
 typedef ESBMesh<ESBNetwork<RF24>, RF24> RF24Mesh;
 #if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840) || defined(ARDUINO_ARCH_NRF52833)
```

### Comparing `pyrf24-0.2.5/RF24Mesh/RF24Mesh_config.h` & `pyrf24-0.3.0/RF24Mesh/RF24Mesh_config.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake` & `pyrf24-0.3.0/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/CPackInfo.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/CPackInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/Cache.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/CompilerWarnings.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/GetLibInfo.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/GetLibInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/PreventInSourceBuilds.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/StandardProjectSettings.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/detectCPU.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/detectCPU.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Mesh/cmake/enableNcursesExample.cmake` & `pyrf24-0.3.0/RF24Mesh/cmake/enableNcursesExample.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/CMakeLists.txt` & `pyrf24-0.3.0/RF24Network/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/LICENSE` & `pyrf24-0.3.0/RF24Network/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/RF24Network.cpp` & `pyrf24-0.3.0/RF24Network/RF24Network.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -844,15 +844,15 @@
 {
     bool ok = false;
     bool isAckType = false;
     if (frame_buffer[6] > 64 && frame_buffer[6] < 192)
         isAckType = true;
 
     /*if( ( (frame_buffer[7] % 2) && frame_buffer[6] == NETWORK_MORE_FRAGMENTS) ){
-	isAckType = 0;
+    isAckType = 0;
     }*/
 
     // Throw it away if it's not a valid address
     if (!is_valid_address(to_node))
         return false;
 
     //Load info into our conversion structure, and get the converted address info
@@ -1177,22 +1177,30 @@
 #endif // !defined(RF24NetworkMulticast)
 /******************************************************************/
 
 template<class radio_t>
 uint64_t ESBNetwork<radio_t>::pipe_address(uint16_t node, uint8_t pipe)
 {
 
-    static uint8_t address_translation[] = {0xc3, 0x3c, 0x33, 0xce, 0x3e, 0xe3, 0xec
+    static uint8_t address_translation[] = { 0xc3,
+                                             0x3c,
+                                             0x33,
+                                             0xce,
+                                             0x3e,
+                                             0xe3,
+                                             0xec
 #if NUM_PIPES > 6
-, 0xee
+                                             ,
+                                             0xee
     #if NUM_PIPES > 7
-, 0xed
+                                             ,
+                                             0xed
     #endif
 #endif
-};
+    };
     uint64_t result = 0xCCCCCCCCCCLL;
     uint8_t* out = reinterpret_cast<uint8_t*>(&result);
 
     // Translate the address to use our optimally chosen radio address bytes
     uint8_t count = 1;
     uint16_t dec = node;
```

### Comparing `pyrf24-0.2.5/RF24Network/RF24Network.h` & `pyrf24-0.3.0/RF24Network/RF24Network.h`

 * *Files 1% similar despite different names*

```diff
@@ -313,40 +313,40 @@
     /** Header which is sent with each message */
     RF24NetworkHeader header;
 
     /** The size in bytes of the payload length */
     uint16_t message_size;
 
 /**
-     * On Arduino, the message buffer is just a pointer, and can be pointed to any memory location.
-     * On Linux the message buffer is a standard byte array, equal in size to the defined MAX_PAYLOAD_SIZE
-     */
+ * On Arduino, the message buffer is just a pointer, and can be pointed to any memory location.
+ * On Linux the message buffer is a standard byte array, equal in size to the defined MAX_PAYLOAD_SIZE
+ */
 #if defined(RF24_LINUX)
     uint8_t message_buffer[MAX_PAYLOAD_SIZE]; // Array to store the message
 #else
     uint8_t* message_buffer; // Pointer to the buffer storing the actual message
 #endif
 
     /**
      * Default constructor
      *
      * Simply constructs a blank frame. Frames are generally used internally. See RF24NetworkHeader.
      */
     RF24NetworkFrame() {}
 
 /**
-     * **Constructor for Linux platforms** - create a network frame with data
-     * Frames are constructed and handled differently on Arduino/AVR and Linux devices (`#if defined RF24_LINUX`)
-     *
-     * @param _header The RF24Network header to be stored in the frame
-     * @param _message The 'message' or data.
-     * @param _len The size of the 'message' or data.
-     *
-     * Frames are used internally and by external systems. See RF24NetworkHeader.
-     */
+ * **Constructor for Linux platforms** - create a network frame with data
+ * Frames are constructed and handled differently on Arduino/AVR and Linux devices (`#if defined RF24_LINUX`)
+ *
+ * @param _header The RF24Network header to be stored in the frame
+ * @param _message The 'message' or data.
+ * @param _len The size of the 'message' or data.
+ *
+ * Frames are used internally and by external systems. See RF24NetworkHeader.
+ */
 #if defined(RF24_LINUX) || defined(DOXYGEN_FORCED)
     RF24NetworkFrame(RF24NetworkHeader& _header, const void* _message = NULL, uint16_t _len = 0) : header(_header), message_size(_len)
     {
         if (_message && _len) {
             memcpy(message_buffer, _message, _len);
         }
     }
@@ -398,29 +398,29 @@
      * @code
      * RF24 radio(7, 8);
      * RF24Network network(radio); // for nRF24L01
      *
      * nrf_to_nrf radio1;
      * RF52Network network(radio1); // for nRF52xxx family
      * @endcode
-     * 
+     *
      * @see v2.0 supports [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf)
      * for nrf52 chips' internal radio.
-     * 
+     *
      * @param _radio The underlying radio driver instance
      */
     ESBNetwork(radio_t& _radio);
 
     /**
      * Bring up the network using the current radio frequency/channel.
      * Calling begin brings up the network, and configures the address, which designates the
-     * location of the node within [RF24Network topology](md_docs_tuning.html).
+     * location of the node within [RF24Network topology](tuning.md).
      *
      * @note Node addresses are specified in Octal format, see
-     * [RF24Network Addressing](md_docs_addressing.html) for more information. The address `04444`
+     * [RF24Network Addressing](addressing.md) for more information. The address `04444`
      * is reserved for RF24Mesh usage (when a mesh node is connecting to the network).
      * @warning Be sure to first call `RF24::begin()` to initialize the radio properly.
      *
      * **Example 1:** Begin on current radio channel with address 0 (master node)
      * @code network.begin(00); @endcode
      * **Example 2:** Begin with address 01 (child of master)
      * @code network.begin(01); @endcode
@@ -690,15 +690,15 @@
      * Provided a node address and a pipe number, will return the RF24Network address of that child pipe for that node.
      */
     uint16_t addressOfPipe(uint16_t node, uint8_t pipeNo);
 
     /**
      * Validate a network address as a proper logical address
      * @note Addresses are specified in octal form, ie 011, 034.
-     * Review [RF24Network addressing](md_docs_addressing.html) for more information.
+     * Review [RF24Network addressing](addressing.md) for more information.
      * @param node The specified logical address of a network node.
      * @return True if the specified `node` address is a valid network address, otherwise false.
      * @remark This function will validate an improper address of `0100` as it is the reserved
      * @ref NETWORK_MULTICAST_ADDRESS used for multicasted messages.
      */
     bool is_valid_address(uint16_t node);
```

### Comparing `pyrf24-0.2.5/RF24Network/RF24Network_config.h` & `pyrf24-0.3.0/RF24Network/RF24Network_config.h`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     /* Enable tracking of success and failures for all transmissions, routed and user initiated */
     //#define ENABLE_NETWORK_STATS
 
     #ifndef DISABLE_DYNAMIC_PAYLOADS
         /** Enable dynamic payloads - If using different types of nRF24L01 modules, some may be incompatible when using this feature **/
         #define ENABLE_DYNAMIC_PAYLOADS
     #endif // DISABLE_DYNAMIC_PAYLOADS
-    
+
     /** The number of 'pipes' available for addressing in the current device
      * Networks with NRF24L01 devices only have 6 pipes
      * NRF52x networks support up to 8 pipes
      */
     #define NUM_PIPES 6
 
     /* Debug Options */
```

### Comparing `pyrf24-0.2.5/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake` & `pyrf24-0.3.0/RF24/cmake/AutoConfig_RF24_DRIVER.cmake`

 * *Files 21% similar despite different names*

```diff
@@ -22,35 +22,37 @@
 if(EXISTS /dev/spidev0.0)
     set(SPIDEV_EXISTS TRUE)
 else()
     set(SPIDEV_EXISTS FALSE)
 endif()
 
 
-if(${RF24_DRIVER} STREQUAL "UNKNOWN") # invokes automatic configuration
-    if("${SOC}" STREQUAL "BCM2708" OR "${SOC}" STREQUAL "BCM2709" OR "${SOC}" STREQUAL "BCM2835")
-        set(RF24_DRIVER RPi CACHE STRING "using folder /utility/RPi" FORCE)
-    elseif(NOT "${LibPIGPIO}" STREQUAL "LibPIGPIO-NOTFOUND")
-        message(STATUS "Found pigpio library: ${LibPIGPIO}")
-        set(RF24_DRIVER pigpio CACHE STRING "using folder /utility/pigpio" FORCE)
-    elseif(NOT "${LibWiringPi}" STREQUAL "LibWiringPi-NOTFOUND")
-        message(STATUS "Found wiringPi library: ${LibWiringPi}")
-        set(RF24_DRIVER wiringPi CACHE STRING "using folder /utility/wiringPi" FORCE)
-    elseif(NOT "${LibLittleWire}" STREQUAL "LibLittleWire-NOTFOUND")
-        message(STATUS "Found LittleWire library: ${LibLittleWire}")
-        set(RF24_DRIVER LittleWire CACHE STRING "using folder /utility/LittleWire" FORCE)
-    elseif(NOT "${LibMRAA}" STREQUAL "LibMRAA-NOTFOUND")
-        message(STATUS "Found MRAA library: ${LibMRAA}")
-        set(RF24_DRIVER MRAA CACHE STRING "using folder /utility/MRAA" FORCE)
-    elseif(SPIDEV_EXISTS) # should be a non-empty string if SPI is enabled
-        message(STATUS "detected that SPIDEV is enabled: ${SPIDEV_EXISTS}")
-        set(RF24_DRIVER SPIDEV CACHE STRING "using folder /utility/SPIDEV" FORCE)
-    endif()
-endif()
+# if(${RF24_DRIVER} STREQUAL "UNKNOWN") # invokes automatic configuration
+#     if("${SOC}" STREQUAL "BCM2708" OR "${SOC}" STREQUAL "BCM2709" OR "${SOC}" STREQUAL "BCM2835")
+#         set(RF24_DRIVER RPi CACHE STRING "using folder /utility/RPi" FORCE)
+#     elseif(NOT "${LibPIGPIO}" STREQUAL "LibPIGPIO-NOTFOUND")
+#         message(STATUS "Found pigpio library: ${LibPIGPIO}")
+#         set(RF24_DRIVER pigpio CACHE STRING "using folder /utility/pigpio" FORCE)
+#     elseif(NOT "${LibWiringPi}" STREQUAL "LibWiringPi-NOTFOUND")
+#         message(STATUS "Found wiringPi library: ${LibWiringPi}")
+#         set(RF24_DRIVER wiringPi CACHE STRING "using folder /utility/wiringPi" FORCE)
+#     elseif(NOT "${LibLittleWire}" STREQUAL "LibLittleWire-NOTFOUND")
+#         message(STATUS "Found LittleWire library: ${LibLittleWire}")
+#         set(RF24_DRIVER LittleWire CACHE STRING "using folder /utility/LittleWire" FORCE)
+#     elseif(NOT "${LibMRAA}" STREQUAL "LibMRAA-NOTFOUND")
+#         message(STATUS "Found MRAA library: ${LibMRAA}")
+#         set(RF24_DRIVER MRAA CACHE STRING "using folder /utility/MRAA" FORCE)
+#     elseif(SPIDEV_EXISTS) # should be a non-empty string if SPI is enabled
+#         message(STATUS "detected that SPIDEV is enabled: ${SPIDEV_EXISTS}")
+#         set(RF24_DRIVER SPIDEV CACHE STRING "using folder /utility/SPIDEV" FORCE)
+#     endif()
+# endif()
 
 # override the auto-detect if RF24_DRIVER is defined in an env var
 if(DEFINED ENV{RF24_DRIVER})
     message(STATUS "RF24_DRIVER (set from env var) = $ENV{RF24_DRIVER}")
     set(RF24_DRIVER $ENV{RF24_DRIVER} CACHE STRING "" FORCE)
+elseif(${RF24_DRIVER} STREQUAL "UNKNOWN")
+    set(RF24_DRIVER SPIDEV CACHE STRING "using folder /utility/SPIDEV" FORCE)
 endif()
 
 message(STATUS "Using driver: ${RF24_DRIVER}")
```

### Comparing `pyrf24-0.2.5/RF24Network/cmake/CPackInfo.cmake` & `pyrf24-0.3.0/RF24Network/cmake/CPackInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/cmake/Cache.cmake` & `pyrf24-0.3.0/RF24Network/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/cmake/CompilerWarnings.cmake` & `pyrf24-0.3.0/RF24Network/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/cmake/GetLibInfo.cmake` & `pyrf24-0.3.0/RF24Network/cmake/GetLibInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/cmake/PreventInSourceBuilds.cmake` & `pyrf24-0.3.0/RF24Network/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/cmake/StandardProjectSettings.cmake` & `pyrf24-0.3.0/RF24Network/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/RF24Network/cmake/detectCPU.cmake` & `pyrf24-0.3.0/RF24Network/cmake/detectCPU.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/cmake/using_flags.cmake` & `pyrf24-0.3.0/cmake/using_flags.cmake`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 
 ####################### DEBUG (& EXTRA) FLAGS ######################
 
 # RF24 core specific options
 option(RF24_DEBUG "enable/disable debugging output for RF24 lib" OFF)
 
-# Disabling IRQ support should be always done because
-# IRQ support can be handled in python with different libs.
-option(RF24_NO_INTERRUPT "disable IRQ support (dependent on pigpio)" ON)
-# does not affect pigpio driver though
-
 # RF24Network specific options
 option(SERIAL_DEBUG "enable/disable debugging output for RF24Network lib" OFF)
 option(SERIAL_DEBUG_MINIMAL "enable/disable minimal debugging output for RF24Network lib" OFF)
 option(SERIAL_DEBUG_ROUTING
     "enable/disable debugging output related to transmission routing for RF24Network lib"
     OFF
 )
@@ -56,25 +51,27 @@
 #     mesh.write() (only when using node_id instead of a node's logical address).
 #     This is cumulative to MESH_LOOKUP_TIMEOUT.
 
 
 ###############################################
 # function to apply flags to applicable targets
 function(apply_flags target)
-    # apply RF24 flags to all targets
-    if(RF24_NO_INTERRUPT)
-        target_compile_definitions(${target} PUBLIC RF24_NO_INTERRUPT)
-    endif()
-    if(RF24_DEBUG)
-        message(STATUS "RF24_DEBUG asserted for ${target}")
-        target_compile_definitions(${target} PUBLIC SERIAL_DEBUG)
+    # apply RF24 flags to cpp_rf24 target
+    if("${target}" STREQUAL "cpp_rf24")
+        if(RF24_DEBUG)
+            message(STATUS "RF24_DEBUG asserted for ${target}")
+            target_compile_definitions(${target} PUBLIC SERIAL_DEBUG)
+        endif()
     endif()
 
-    # apply RF24Network flags to rf24_mesh and rf24_network targets
-    if("${target}" STREQUAL "rf24_network" OR "${target}" STREQUAL "rf24_mesh")
+    #  pass driver used to expose as a constant in rf24 module.
+    target_compile_definitions(${target} PUBLIC RF24_DRIVER="${RF24_DRIVER}")
+
+    # apply RF24Network flags to cpp_rf24_network target
+    if("${target}" STREQUAL "cpp_rf24_network")
         if(SERIAL_DEBUG)
             message(STATUS "SERIAL_DEBUG asserted for ${target}")
             target_compile_definitions(${target} PUBLIC SERIAL_DEBUG)
         endif()
         if(SERIAL_DEBUG_MINIMAL)
             message(STATUS "SERIAL_DEBUG_MINIMAL asserted for ${target}")
             target_compile_definitions(${target} PUBLIC SERIAL_DEBUG_MINIMAL)
@@ -102,16 +99,16 @@
         endif()
         if(DEFINED SLOW_ADDR_POLL_RESPONSE)
             message(STATUS "SLOW_ADDR_POLL_RESPONSE set to ${SLOW_ADDR_POLL_RESPONSE} for ${target}")
             target_compile_definitions(${target} PUBLIC SLOW_ADDR_POLL_RESPONSE=${SLOW_ADDR_POLL_RESPONSE})
         endif()
     endif()
 
-    # apply RF24Mesh flags to only rf24_mesh target
-    if("${target}" STREQUAL "rf24_mesh")
+    # apply RF24Mesh flags to cpp_rf24_mesh target
+    if("${target}" STREQUAL "cpp_rf24_mesh")
         if(MESH_NOMASTER)
             message(STATUS "MESH_NOMASTER asserted for ${target}")
             target_compile_definitions(${target} PUBLIC MESH_NOMASTER)
         endif()
         if(MESH_DEBUG)
             message(STATUS "MESH_DEBUG asserted for ${target}")
             target_compile_definitions(${target} PUBLIC MESH_DEBUG)
```

### Comparing `pyrf24-0.2.5/pybind11/.codespell-ignore-lines` & `pyrf24-0.3.0/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/CMakeLists.txt` & `pyrf24-0.3.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/LICENSE` & `pyrf24-0.3.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/attr.h` & `pyrf24-0.3.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/buffer_info.h` & `pyrf24-0.3.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/cast.h` & `pyrf24-0.3.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/chrono.h` & `pyrf24-0.3.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/complex.h` & `pyrf24-0.3.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/class.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/common.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/descr.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/init.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/internals.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/type_caster_base.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/detail/typeid.h` & `pyrf24-0.3.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/eigen/matrix.h` & `pyrf24-0.3.0/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/eigen/tensor.h` & `pyrf24-0.3.0/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/embed.h` & `pyrf24-0.3.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/eval.h` & `pyrf24-0.3.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/functional.h` & `pyrf24-0.3.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/gil.h` & `pyrf24-0.3.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/iostream.h` & `pyrf24-0.3.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/numpy.h` & `pyrf24-0.3.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/operators.h` & `pyrf24-0.3.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/options.h` & `pyrf24-0.3.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/pybind11.h` & `pyrf24-0.3.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/pytypes.h` & `pyrf24-0.3.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/stl/filesystem.h` & `pyrf24-0.3.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/stl.h` & `pyrf24-0.3.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/include/pybind11/stl_bind.h` & `pyrf24-0.3.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/noxfile.py` & `pyrf24-0.3.0/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/pybind11/__main__.py` & `pyrf24-0.3.0/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/pybind11/commands.py` & `pyrf24-0.3.0/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/pybind11/setup_helpers.py` & `pyrf24-0.3.0/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/pyproject.toml` & `pyrf24-0.3.0/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/setup.cfg` & `pyrf24-0.3.0/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/setup.py` & `pyrf24-0.3.0/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/FindCatch.cmake` & `pyrf24-0.3.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/FindEigen3.cmake` & `pyrf24-0.3.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/FindPythonLibsNew.cmake` & `pyrf24-0.3.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/JoinPaths.cmake` & `pyrf24-0.3.0/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/check-style.sh` & `pyrf24-0.3.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/cmake_uninstall.cmake.in` & `pyrf24-0.3.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pyrf24-0.3.0/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/libsize.py` & `pyrf24-0.3.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/make_changelog.py` & `pyrf24-0.3.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/pybind11Common.cmake` & `pyrf24-0.3.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/pybind11Config.cmake.in` & `pyrf24-0.3.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/pybind11NewTools.cmake` & `pyrf24-0.3.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/pybind11Tools.cmake` & `pyrf24-0.3.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/setup_global.py.in` & `pyrf24-0.3.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pybind11/tools/setup_main.py.in` & `pyrf24-0.3.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pyproject.toml` & `pyrf24-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.5/pyrf24.egg-info/PKG-INFO` & `pyrf24-0.3.0/pyrf24.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrf24
-Version: 0.2.5
+Version: 0.3.0
 Summary: A python package for the wrapping nRF24 related C++ libraries.
 Author-email: Brendan Doherty <2bndy5@gmail.com>
 License: GPLv2
 Project-URL: Documentation, http://nRF24.github.io/pyRF24
 Project-URL: Source, https://github.com/nRF24/pyRF24
 Project-URL: Tracker, https://github.com/nRF24/pyRF24/issues
 Keywords: nrf24l01,nRF24L01+,raspberry,pi,driver,radio,transceiver
@@ -23,27 +23,29 @@
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. image:: https://img.shields.io/piwheels/v/pyrf24?color=informational
+.. |piwheels-badge| image:: https://img.shields.io/piwheels/v/pyrf24?color=informational
     :target: https://www.piwheels.org/project/pyrf24/
     :alt: piwheels
-.. image:: https://img.shields.io/readthedocs/pyrf24?label=ReadTheDocs&logo=readthedocs&logoColor=white
+.. |rtd-badge| image:: https://img.shields.io/readthedocs/pyrf24?label=ReadTheDocs&logo=readthedocs&logoColor=white
     :target: https://pyrf24.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
-.. image:: https://static.pepy.tech/personalized-badge/pyrf24?period=total&units=none&left_color=grey&right_color=blue&left_text=PyPI%20Downloads
+.. |pypi-downloads| image:: https://img.shields.io/pepy/dt/pyrf24?label=PyPI%20Downloads&color=blue
     :target: https://pepy.tech/project/pyrf24
     :alt: PyPI Downloads
-.. image:: https://github.com/nRF24/pyRF24/actions/workflows/build.yml/badge.svg
+.. |ci-badge| image:: https://github.com/nRF24/pyRF24/actions/workflows/build.yml/badge.svg
     :target: https://github.com/nRF24/pyRF24/actions/workflows/build.yml
     :alt: Build CI
 
+|piwheels-badge| |rtd-badge| |pypi-downloads| |ci-badge|
+
 Introduction
 ============
 
 This is the official home of the python wrappers for the RF24 stack. It is meant for Linux-based
 SoC boards like the Raspberry Pi. Documentation is hosted at http://pyrf24.rtfd.io/.
 
 Pinout
@@ -77,24 +79,25 @@
     nRF24L01+PA+LNA modules.
 
 .. important:: It is highly recommended that the nRF24L01's VCC and GND pins have a parallel
     capacitor to stabilize the power supply. Usually 100 microfarad is enough, but the capacitance
     ultimately depends on the nature of your power supply's stability.
 
 .. note::
-    Notice that RPi.GPIO (for python) is used to manage the GPIO pins on the Raspberry Pi
+    Notice that `gpiod <https://pypi.org/project/gpiod>`_ is used to watch the radio's IRQ pin
     (exclusively during the
     `interrupt_configure.py <https://pyrf24.readthedocs.io/en/latest/examples.html#interrupt-configure>`_
     example).
 
-    RPi.GPIO is not required for normal usage (when not using the radio's IRQ pin).
+    `gpiod <https://pypi.org/project/gpiod>`_ is not required for normal usage (when not using the radio's IRQ pin).
 
     .. code-block:: bash
 
-        sudo apt install python3-rpi.gpio
+        sudo apt install python3-dev
+        pip install gpiod
 
 Installing from PyPI
 ~~~~~~~~~~~~~~~~~~~~
 
 Simply use:
 
 .. code-block:: python
@@ -195,20 +198,22 @@
        the third commit (``dev3``) since the first "post release" (``post1``) after the
        tagged version ``0.1.1``. This adhere's to `PEP440 <https://peps.python.org/pep-0440>`_.
    - ``cp3X`` is the version of python used to build the wheel (ie ``cp39`` for CPython 3.9)
      The second occurrence of ``cp3X`` describes the CPython ABI compatibility.
    - ``ARCH`` is the architecture type of the CPU. This corresponds to the compiler used.
      On Raspberry Pi OS (32 bit), this will be ``armv7l``.
 
+.. _using-specific-driver:
+
 Using a specific RF24 driver
 ----------------------------
 
-By default, this package is built using the RF24 driver SPIDEV. If you want to build the
-package using a different RF24 driver (like ``RPi``, ``MRAA``, ``wiringPi``, etc), then
-it is necessary to use an environment variable containing additional arguments for CMake:
+By default, this package is built using the RF24 driver ``SPIDEV``. If you want to build the
+package using a different RF24 driver (like ``RPi``, ``MRAA``, ``wiringPi``, or ``pigpio``),
+then it is necessary to use an environment variable containing additional arguments for CMake:
 
 .. code-block:: bash
 
     export CMAKE_ARGS="-DRF24_DRIVER=RPi"
 
 .. hint::
     You can also use this environment variable to enable debug output from different
```

### Comparing `pyrf24-0.2.5/pyrf24.egg-info/SOURCES.txt` & `pyrf24-0.3.0/pyrf24.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 RF24/utility/LittleWire/includes.h
 RF24/utility/MRAA/RF24_arch_config.h
 RF24/utility/MRAA/compatibility.cpp
 RF24/utility/MRAA/compatibility.h
 RF24/utility/MRAA/gpio.cpp
 RF24/utility/MRAA/gpio.h
 RF24/utility/MRAA/includes.h
+RF24/utility/MRAA/interrupt.cpp
+RF24/utility/MRAA/interrupt.h
 RF24/utility/MRAA/spi.cpp
 RF24/utility/MRAA/spi.h
 RF24/utility/RPi/RF24_arch_config.h
 RF24/utility/RPi/bcm2835.c
 RF24/utility/RPi/bcm2835.h
 RF24/utility/RPi/compatibility.cpp
 RF24/utility/RPi/compatibility.h
@@ -63,14 +65,15 @@
 RF24/utility/pigpio/includes.h
 RF24/utility/pigpio/interrupt.cpp
 RF24/utility/pigpio/interrupt.h
 RF24/utility/pigpio/spi.cpp
 RF24/utility/pigpio/spi.h
 RF24/utility/wiringPi/RF24_arch_config.h
 RF24/utility/wiringPi/includes.h
+RF24/utility/wiringPi/interrupt.h
 RF24/utility/wiringPi/spi.cpp
 RF24/utility/wiringPi/spi.h
 RF24Mesh/CMakeLists.txt
 RF24Mesh/LICENSE
 RF24Mesh/RF24Mesh.cpp
 RF24Mesh/RF24Mesh.h
 RF24Mesh/RF24Mesh_config.h
@@ -161,15 +164,19 @@
 pybind11/tools/setup_main.py.in
 pyrf24.egg-info/PKG-INFO
 pyrf24.egg-info/SOURCES.txt
 pyrf24.egg-info/dependency_links.txt
 pyrf24.egg-info/not-zip-safe
 pyrf24.egg-info/top_level.txt
 src/pyRF24.cpp
+src/pyRF24.h
 src/pyRF24Mesh.cpp
+src/pyRF24Mesh.h
 src/pyRF24Network.cpp
+src/pyRF24Network.h
+src/linux/gpio.h
 src/pyrf24/__init__.py
 src/pyrf24/fake_ble.py
 src/pyrf24/py.typed
 src/pyrf24/rf24.pyi
 src/pyrf24/rf24_mesh.pyi
 src/pyrf24/rf24_network.pyi
```

### Comparing `pyrf24-0.2.5/setup.py` & `pyrf24-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Build & Install script for the pyrf24 package or python wrappers about
 the RF24 C++ libraries."""
+
 import os
 import platform
 import subprocess
 import sys
 from pathlib import Path
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
@@ -13,23 +14,25 @@
 
 class CMakeExtension(Extension):
     """A class that wraps the generic mechanism for compiling a python C-extension.
 
     A CMakeExtension needs a sourcedir instead of a file list.
     The name must be the single output extension from the CMake build.
     """
+
     def __init__(self, name, sourcedir="", **kwargs):
         kwargs.pop("sources", None)
         Extension.__init__(self, name, sources=[], **kwargs)
         self.sourcedir = str(Path(sourcedir).resolve())
 
 
 class CMakeBuild(build_ext):
     """A class that wraps the builtin mechanism for building a
     distributable wheel from a compiled c-extension"""
+
     def build_extension(self, ext: Extension):
         extdir = str(
             (Path(self.get_ext_fullpath(ext.name)).parent / ext.name).resolve()
         )
 
         # required for auto-detection & inclusion of auxiliary "native" libs
         if not extdir.endswith(os.sep):
```

### Comparing `pyrf24-0.2.5/src/pyRF24.cpp` & `pyrf24-0.3.0/src/pyRF24.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,253 +1,14 @@
 #include <pybind11/pybind11.h>
-#include <RF24.h>
-#include <nRF24L01.h>
-
-namespace py = pybind11;
-
-void throw_ba_exception(void)
-{
-    PyErr_SetString(PyExc_TypeError, "buf parameter must be bytes or bytearray");
-    py::error_already_set();
-}
-
-char* get_bytes_or_bytearray_str(py::object buf)
-{
-    PyObject* py_ba;
-    py_ba = buf.ptr();
-    if (PyByteArray_Check(py_ba))
-        return PyByteArray_AsString(py_ba);
-    else if (PyBytes_Check(py_ba))
-        return PyBytes_AsString(py_ba);
-    else
-        throw_ba_exception();
-
-    return NULL;
-}
-
-int get_bytes_or_bytearray_ln(py::object buf)
-{
-    PyObject* py_ba;
-    py_ba = buf.ptr();
-    if (PyByteArray_Check(py_ba))
-        return PyByteArray_Size(py_ba);
-    else if (PyBytes_Check(py_ba))
-        return PyBytes_Size(py_ba);
-    else
-        throw_ba_exception();
-
-    return 0;
-}
-
-class RF24Wrapper : public RF24
-{
-
-public:
-    RF24Wrapper(rf24_gpio_pin_t _ce_pin, rf24_gpio_pin_t _csn_pin, uint32_t _spi_speed = 10000000) : RF24(_ce_pin, _csn_pin, _spi_speed)
-    {
-    }
-
-    RF24Wrapper(uint32_t _spi_speed = 10000000) : RF24(_spi_speed)
-    {
-    }
-
-    // needed for polymorphic recognition
-    virtual ~RF24Wrapper() = default;
-
-    std::tuple<bool, uint8_t> available_pipe()
-    {
-        uint8_t pipe = 7;
-        bool is_available = RF24::available(&pipe);
-        return std::tuple<bool, uint8_t>(is_available, pipe);
-    }
-
-    std::tuple<bool, bool, bool> what_happened()
-    {
-        bool ds = 0, df = 0, dr = 0;
-        RF24::whatHappened(ds, df, dr);
-        return std::tuple<bool, bool, bool>(ds, df, dr);
-    }
-
-    void open_tx_pipe(py::buffer address)
-    {
-        RF24::openWritingPipe(reinterpret_cast<uint8_t*>(get_bytes_or_bytearray_str(address)));
-    }
-
-    void open_rx_pipe(uint8_t number, py::buffer address)
-    {
-        RF24::openReadingPipe(number, reinterpret_cast<uint8_t*>(get_bytes_or_bytearray_str(address)));
-    }
-
-    py::bytearray read(uint8_t length = 0)
-    {
-        if (!length)
-            length = RF24::dynamic_payloads_enabled ? RF24::getDynamicPayloadSize() : RF24::getPayloadSize();
-        else
-            length = rf24_min(length, static_cast<uint8_t>(32));
-        char* payload = new char[length + 1];
-        RF24::read(payload, length);
-        payload[length] = '\0';
-        py::bytearray buf = py::bytearray(payload, length);
-        delete[] payload;
-        return buf;
-    }
-
-    void startFastWrite(py::buffer buf, const bool multicast = false, bool startTx = true)
-    {
-        RF24::startFastWrite(
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            multicast, startTx);
-    }
-
-    bool startWrite(py::buffer buf, const bool multicast)
-    {
-        return RF24::startWrite(
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            multicast);
-    }
-
-    bool writeFast(py::buffer buf, const bool multicast = false)
-    {
-        return RF24::writeFast(
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            multicast);
-    }
-
-    bool write(py::buffer buf, const bool multicast = false)
-    {
-        return RF24::write(
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            multicast);
-    }
-
-    bool writeBlocking(py::buffer buf, uint32_t timeout)
-    {
-        return RF24::writeBlocking(
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            timeout);
-    }
-
-    bool writeAckPayload(uint8_t pipe, py::buffer buf)
-    {
-        return RF24::writeAckPayload(
-            pipe,
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)));
-    }
-
-    char* sprintfDetails()
-    {
-        char* debug_info = new char[870];
-        RF24::sprintfPrettyDetails(debug_info);
-        return debug_info;
-    }
-
-    void set_radiation(rf24_pa_dbm_e level, rf24_datarate_e speed, bool lna_enable = true)
-    {
-        RF24::setRadiation(level, speed, lna_enable);
-    }
-
-    /*********************************************************************************/
-    /* wrappers for python-like properties */
-
-    uint8_t get_address_width()
-    {
-        return RF24::addr_width;
-    }
-
-    bool is_ack_payloads_enabled()
-    {
-        return RF24::ack_payloads_enabled;
-    }
-
-    void toggle_ack_payloads(const bool enable)
-    {
-        if (enable)
-            RF24::enableAckPayload();
-        else
-            RF24::disableAckPayload();
-    }
-
-    bool is_dynamic_payloads_enabled()
-    {
-        return RF24::dynamic_payloads_enabled;
-    }
-
-    void dynamic_payloads(const bool enable)
-    {
-        if (enable)
-            RF24::enableDynamicPayloads();
-        else
-            RF24::disableDynamicPayloads();
-    }
-
-    bool isPowerUp()
-    {
-        return read_register(NRF_CONFIG) & _BV(PWR_UP);
-    }
-
-    void set_pa_level(rf24_pa_dbm_e level)
-    {
-        RF24::setPALevel(level);
-    }
-
-    rf24_pa_dbm_e get_pa_level()
-    {
-        uint8_t ret_val = RF24::getPALevel();
-        if (ret_val == RF24_PA_MAX)
-            return RF24_PA_MAX;
-        if (ret_val == RF24_PA_HIGH)
-            return RF24_PA_HIGH;
-        if (ret_val == RF24_PA_LOW)
-            return RF24_PA_LOW;
-        // if (ret_val == RF24_PA_MIN)
-        return RF24_PA_MIN;
-    }
-
-    rf24_datarate_e get_data_rate()
-    {
-        uint8_t ret_val = RF24::getDataRate();
-        if (ret_val == RF24_2MBPS)
-            return RF24_2MBPS;
-        if (ret_val == RF24_1MBPS)
-            return RF24_1MBPS;
-        // if (ret_val == RF24_250KBPS)
-        return RF24_250KBPS;
-    }
-
-    void power(const bool enable)
-    {
-        if (enable)
-            powerUp();
-        else
-            powerDown();
-    }
-
-    bool isListening()
-    {
-        return read_register(NRF_CONFIG) & _BV(PRIM_RX);
-    }
-
-    void listen(const bool enable)
-    {
-        if (enable)
-            startListening();
-        else
-            stopListening();
-    }
-};
+#include "pyRF24.h"
 
 PYBIND11_MODULE(rf24, m)
 {
     m.doc() = "A Python module that wraps all RF24 C++ library's API";
+    m.attr("RF24_DRIVER") = RF24_DRIVER;
 
     // ********************** Enum structs
     py::enum_<rf24_crclength_e>(m, "rf24_crclength_e")
         .value("RF24_CRC_DISABLED", RF24_CRC_DISABLED, R"docstr(
             to disable using CRC checksums
         )docstr")
         .value("RF24_CRC_8", RF24_CRC_8, R"docstr(
```

### Comparing `pyrf24-0.2.5/src/pyRF24Mesh.cpp` & `pyrf24-0.3.0/src/pyRF24Mesh.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,8 @@
-#include <pybind11/pybind11.h>
-#include "pyRF24Network.cpp"
-#include <RF24Mesh.h>
-
-namespace py = pybind11;
-
-class RF24MeshWrapper : public RF24Mesh
-{
-public:
-    RF24MeshWrapper(RF24Wrapper& _radio, RF24NetworkWrapper& _network)
-        : RF24Mesh(static_cast<RF24&>(_radio), static_cast<RF24Network&>(_network))
-    {
-    }
-
-    // needed for polymorphic recognition
-    virtual ~RF24MeshWrapper() = default;
-
-    bool write(py::buffer buf, uint8_t msg_type, uint8_t nodeID = 0)
-    {
-        return RF24Mesh::write(
-            get_bytes_or_bytearray_str(buf),
-            msg_type,
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            nodeID);
-    }
-
-    bool write(uint16_t to_node, py::buffer buf, uint8_t msg_type)
-    {
-        return RF24Mesh::write(
-            to_node,
-            get_bytes_or_bytearray_str(buf),
-            msg_type,
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)));
-    }
-
-    uint8_t get_node_id()
-    {
-        return RF24Mesh::_nodeID;
-    }
-
-    py::list get_addrList()
-    {
-        py::list list;
-        for (uint8_t i = 0; i < RF24Mesh::addrListTop; ++i) {
-            list.append(RF24Mesh::addrList[i]);
-        }
-        return list;
-    }
-};
+#include "pyRF24Mesh.h"
 
 PYBIND11_MODULE(rf24_mesh, m)
 {
     m.doc() = "A Python module that wraps the RF24Mesh C++ library's API";
     py::options options;
     options.disable_function_signatures();
```

### Comparing `pyrf24-0.2.5/src/pyRF24Network.cpp` & `pyrf24-0.3.0/src/pyRF24Network.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,125 +1,8 @@
-#include <pybind11/pybind11.h>
-#include "pyRF24.cpp"
-#include <RF24Network.h>
-// #include <queue>
-// #include <pybind11/stl.h>
-
-namespace py = pybind11;
-
-/*
-namespace pybind11 {
-namespace detail {
-
-    template<typename Type, typename Alloc>
-    struct type_caster<std::queue<Type, Alloc>> : list_caster<std::queue<Type, Alloc>, Type>
-    {
-    };
-} // namespace detail
-} // namespace pybind11
-
-struct RF24NetworkFrameWrapper : public RF24NetworkFrame
-{
-    RF24NetworkFrameWrapper() : RF24NetworkFrame()
-    {
-    }
-
-    RF24NetworkFrameWrapper(RF24NetworkHeader& header, py::object message)
-    {
-        RF24NetworkFrame::header = header;
-        set_message(message);
-    }
-
-    py::bytearray get_message()
-    {
-        char* buf = new char[RF24NetworkFrame::message_size];
-        memcpy(reinterpret_cast<uint8_t*>(buf), RF24NetworkFrame::message_buffer, RF24NetworkFrame::message_size);
-        py::bytearray py_ba = py::bytearray(buf, RF24NetworkFrame::message_size);
-        delete[] buf;
-        return py_ba;
-    }
-
-    void set_message(py::object message)
-    {
-        RF24NetworkFrame::message_size = static_cast<uint16_t>(get_bytes_or_bytearray_ln(message));
-        memcpy(RF24NetworkFrame::message_buffer, reinterpret_cast<uint8_t*>(get_bytes_or_bytearray_str(message)), RF24NetworkFrame::message_size);
-    }
-};
-*/
-class RF24NetworkWrapper : public RF24Network
-{
-public:
-    RF24NetworkWrapper(RF24Wrapper& _radio) : RF24Network(static_cast<RF24&>(_radio))
-    {
-    }
-
-    // needed for polymorphic recognition
-    virtual ~RF24NetworkWrapper() = default;
-
-    uint16_t peek_header(RF24NetworkHeader& header)
-    {
-        return RF24Network::peek(header);
-    }
-
-    std::tuple<RF24NetworkHeader, py::bytearray> peek_frame(uint16_t maxlen = MAX_PAYLOAD_SIZE)
-    {
-        RF24NetworkHeader header;
-        maxlen = static_cast<uint16_t>(rf24_min(maxlen, RF24Network::peek(header)));
-        char* buf = new char[maxlen + 1];
-        RF24Network::peek(header, buf, maxlen);
-        py::bytearray py_ba = py::bytearray(buf, maxlen);
-        delete[] buf;
-        return std::tuple<RF24NetworkHeader, py::bytearray>(header, py_ba);
-    }
-
-#if defined(RF24NetworkMulticast)
-    bool multicast(RF24NetworkHeader header, py::buffer buf, uint8_t level = 7)
-    {
-        return RF24Network::multicast(
-            header,
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint16_t>(get_bytes_or_bytearray_ln(buf)),
-            level);
-    }
-
-    void set_multicast_level(uint8_t level)
-    {
-        RF24Network::multicastLevel(level);
-    }
-
-    uint8_t get_multicast_level()
-    {
-        return RF24Network::_multicast_level;
-    }
-#endif // defined (RF24NetworkMulticast)
-
-    std::tuple<RF24NetworkHeader, py::bytearray> read(uint16_t maxlen = MAX_PAYLOAD_SIZE)
-    {
-        char* buf = new char[maxlen + 1];
-        RF24NetworkHeader header;
-        uint16_t len = RF24Network::read(header, buf, maxlen);
-        py::bytearray py_ba = py::bytearray(buf, len);
-        delete[] buf;
-        return std::tuple<RF24NetworkHeader, py::bytearray>(header, py_ba);
-    }
-
-    bool write(RF24NetworkHeader& header, py::buffer buf, uint16_t writeDirect = NETWORK_AUTO_ROUTING)
-    {
-        return RF24Network::write(
-            header,
-            get_bytes_or_bytearray_str(buf),
-            static_cast<uint8_t>(get_bytes_or_bytearray_ln(buf)),
-            writeDirect);
-    }
-
-    uint16_t get_node_address()
-    {
-        return RF24Network::node_address;
-    }
-};
+#include "pyRF24Network.h"
 
 PYBIND11_MODULE(rf24_network, m)
 {
     m.doc() = "A Python module that wraps the RF24Network C++ library's API";
     py::options options;
     options.disable_function_signatures();
```

### Comparing `pyrf24-0.2.5/src/pyrf24/fake_ble.py` & `pyrf24-0.3.0/src/pyrf24/fake_ble.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,19 @@
        :py:attr:`~pyrf24.rf24.RF24.data_rate`, so that too has
        been hard coded.
     8. Only the "on data sent" & "on data ready" events will have
        an effect on the interrupt (IRQ) pin. The "on data fail"  is never
        triggered because auto-ack feature is disabled. Keep this in mind when using
        `mask_irq()`.
 """
-# pylint: disable=too-few-public-methods,missing-docstring,too-many-instance-attributes
+
 from os import urandom
 import struct
 from typing import Union, List, Optional
-from .rf24 import (  # pylint: disable=import-error
+from .rf24 import (
     RF24,
     RF24_CRC_DISABLED,
     RF24_PA_HIGH,
     RF24_PA_LOW,
     RF24_PA_MIN,
 )
 
@@ -107,17 +107,15 @@
         Defaults to an empty string.
 
     :Returns:
         A string of hexadecimal characters in big endian form of the
         specified ``buf`` parameter.
     """
     order = range(len(buf) - 1, -1, -1) if reverse else range(len(buf))
-    # pylint: disable=consider-using-f-string
     return delimit.join(["%02X" % buf[byte] for byte in order])
-    # pylint: enable=consider-using-f-string
 
 
 def swap_bits(original: int) -> int:
     """This function reverses the bit order for a single byte.
 
     :returns:
         An `int` containing the byte whose bits are reversed
@@ -405,16 +403,16 @@
         if not success:
             return False
         self._radio.crc_length = RF24_CRC_DISABLED
         self._radio.set_auto_ack(False)
         self._radio.dynamic_payloads = False
         self._radio.set_retries(0, 0)
         self._radio.address_width = 4  # use only 4 byte address length
-        self._radio.open_tx_pipe(b"\x71\x91\x7D\x6B\0")
-        self._radio.open_rx_pipe(0, b"\x71\x91\x7D\x6B\0")
+        self._radio.open_tx_pipe(b"\x71\x91\x7d\x6b\0")
+        self._radio.open_rx_pipe(0, b"\x71\x91\x7d\x6b\0")
         self.hop_channel()
         self._radio.power = True
         self._radio.listen = True
         return success
 
     @property
     def mac(self):
```

### Comparing `pyrf24-0.2.5/src/pyrf24/rf24.pyi` & `pyrf24-0.3.0/src/pyrf24/rf24.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# pylint: skip-file
-from typing import Tuple, Union, overload, Optional
+from typing import Tuple, Union, overload, Optional, Literal
+
+RF24_DRIVER: Literal["SPIDEV", "wiringPi", "pigpio", "MRAA", "RPi"]
 
 class rf24_crclength_e:
     RF24_CRC_DISABLED: "rf24_crclength_e"
     RF24_CRC_8: "rf24_crclength_e"
     RF24_CRC_16: "rf24_crclength_e"
 
 RF24_CRC_DISABLED: rf24_crclength_e = rf24_crclength_e.RF24_CRC_DISABLED
```

### Comparing `pyrf24-0.2.5/src/pyrf24/rf24_mesh.pyi` & `pyrf24-0.3.0/src/pyrf24/rf24_mesh.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: skip-file
 from typing import Union, overload, List
 from .rf24 import RF24, rf24_datarate_e
 from .rf24_network import RF24Network
 
 MESH_DEFAULT_ADDRESS: int = 0o4444
 MESH_ADDR_LOOKUP: int = 196
 MESH_ADDR_RELEASE: int = 197
```

### Comparing `pyrf24-0.2.5/src/pyrf24/rf24_network.pyi` & `pyrf24-0.3.0/src/pyrf24/rf24_network.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# pylint: skip-file
-from typing import Tuple, Union, List, overload, Optional
+from typing import Tuple, Union, overload
 from .rf24 import RF24
 
 MAX_USER_DEFINED_HEADER_TYPE: int = 127
 MAX_PAYLOAD_SIZE: int = 1514
 NETWORK_ADDR_RESPONSE: int = 128
 NETWORK_PING: int = 130
 EXTERNAL_DATA_TYPE: int = 131
```

