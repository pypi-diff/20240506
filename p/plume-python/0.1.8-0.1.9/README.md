# Comparing `tmp/plume_python-0.1.8.tar.gz` & `tmp/plume_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plume_python-0.1.8.tar", max compression
+gzip compressed data, was "plume_python-0.1.9.tar", max compression
```

## Comparing `plume_python-0.1.8.tar` & `plume_python-0.1.9.tar`

### file list

```diff
@@ -1,284 +1,127 @@
--rw-r--r--   0        0        0    35821 2024-03-12 18:05:21.630654 plume_python-0.1.8/LICENSE
--rw-r--r--   0        0        0      137 2024-03-14 14:02:25.156112 plume_python-0.1.8/plume_python/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.646282 plume_python-0.1.8/plume_python/export/__init__.py
--rw-r--r--   0        0        0      167 2024-03-12 18:34:13.250307 plume_python-0.1.8/plume_python/export/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2666 2024-03-14 14:51:04.364402 plume_python-0.1.8/plume_python/export/__pycache__/dataframe_exporter.cpython-312.pyc
--rw-r--r--   0        0        0     4301 2024-03-14 15:47:05.350516 plume_python-0.1.8/plume_python/export/__pycache__/xdf_exporter.cpython-312.pyc
--rw-r--r--   0        0        0    11623 2024-03-14 15:47:05.355167 plume_python-0.1.8/plume_python/export/__pycache__/xdf_writer.cpython-312.pyc
--rw-r--r--   0        0        0     1953 2024-03-14 14:47:06.848804 plume_python-0.1.8/plume_python/export/dataframe_exporter.py
--rw-r--r--   0        0        0     4518 2024-03-14 15:44:58.479296 plume_python-0.1.8/plume_python/export/xdf_exporter.py
--rw-r--r--   0        0        0     6922 2024-03-12 18:05:21.646282 plume_python-0.1.8/plume_python/export/xdf_writer.py
--rw-r--r--   0        0        0      661 2024-03-14 14:13:08.756020 plume_python-0.1.8/plume_python/file_reader.py
--rw-r--r--   0        0        0    11767 2024-03-14 15:57:05.347117 plume_python-0.1.8/plume_python/parser.py
--rw-r--r--   0        0        0     2066 2024-03-14 14:22:39.647355 plume_python-0.1.8/plume_python/record.py
--rw-r--r--   0        0        0      894 2024-03-14 14:49:03.091761 plume_python-0.1.8/plume_python/samples/__init__.py
--rw-r--r--   0        0        0      664 2023-10-02 19:27:51.987226 plume_python-0.1.8/plume_python/samples/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1074 2023-10-02 19:27:51.987226 plume_python-0.1.8/plume_python/samples/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1433 2024-03-14 14:50:50.965325 plume_python-0.1.8/plume_python/samples/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1223 2023-10-02 19:27:51.988227 plume_python-0.1.8/plume_python/samples/__pycache__/camera_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1190 2023-10-02 19:27:51.988227 plume_python-0.1.8/plume_python/samples/__pycache__/packed_sample_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1673 2023-10-02 19:27:51.989227 plume_python-0.1.8/plume_python/samples/__pycache__/packed_sample_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1472 2024-03-14 14:47:57.213037 plume_python-0.1.8/plume_python/samples/__pycache__/packed_sample_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1370 2023-10-02 19:27:51.989227 plume_python-0.1.8/plume_python/samples/__pycache__/record_header_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1745 2023-10-02 19:27:51.990227 plume_python-0.1.8/plume_python/samples/__pycache__/record_header_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2023-10-02 19:27:51.990227 plume_python-0.1.8/plume_python/samples/__pycache__/record_metadata_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1886 2024-03-14 14:47:57.228366 plume_python-0.1.8/plume_python/samples/__pycache__/record_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1454 2023-10-02 19:27:51.990227 plume_python-0.1.8/plume_python/samples/__pycache__/record_version_pb2.cpython-311.pyc
--rw-r--r--   0        0        0      972 2023-10-02 19:27:51.991226 plume_python-0.1.8/plume_python/samples/__pycache__/sample_header_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1411 2023-10-02 19:27:51.991226 plume_python-0.1.8/plume_python/samples/__pycache__/sample_header_pb2.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.653292 plume_python-0.1.8/plume_python/samples/common/__init__.py
--rw-r--r--   0        0        0      467 2023-10-02 19:27:51.992226 plume_python-0.1.8/plume_python/samples/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      695 2023-10-02 19:27:51.992226 plume_python-0.1.8/plume_python/samples/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      175 2024-03-12 18:34:12.995184 plume_python-0.1.8/plume_python/samples/common/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1916 2024-03-14 14:47:57.233460 plume_python-0.1.8/plume_python/samples/common/__pycache__/animation_curve_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1136 2023-10-02 19:27:51.992226 plume_python-0.1.8/plume_python/samples/common/__pycache__/bounds_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1593 2023-10-02 19:27:51.993227 plume_python-0.1.8/plume_python/samples/common/__pycache__/bounds_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1494 2024-03-14 14:49:00.821394 plume_python-0.1.8/plume_python/samples/common/__pycache__/bounds_pb2.cpython-312.pyc
--rw-r--r--   0        0        0      993 2023-10-02 19:27:51.993796 plume_python-0.1.8/plume_python/samples/common/__pycache__/color_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1432 2023-10-02 19:27:51.993796 plume_python-0.1.8/plume_python/samples/common/__pycache__/color_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2408 2024-03-14 14:49:00.834403 plume_python-0.1.8/plume_python/samples/common/__pycache__/color_pb2.cpython-312.pyc
--rw-r--r--   0        0        0      969 2023-10-02 19:27:51.994823 plume_python-0.1.8/plume_python/samples/common/__pycache__/marker_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1408 2023-10-02 19:27:51.994823 plume_python-0.1.8/plume_python/samples/common/__pycache__/marker_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1324 2024-03-14 14:49:00.838392 plume_python-0.1.8/plume_python/samples/common/__pycache__/marker_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1178 2023-10-02 19:27:51.994823 plume_python-0.1.8/plume_python/samples/common/__pycache__/matrix4x4_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1617 2023-10-02 19:27:51.995823 plume_python-0.1.8/plume_python/samples/common/__pycache__/matrix4x4_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1533 2024-03-14 14:49:00.843393 plume_python-0.1.8/plume_python/samples/common/__pycache__/matrix4x4_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1018 2023-10-02 19:27:51.995823 plume_python-0.1.8/plume_python/samples/common/__pycache__/quaternion_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1457 2023-10-02 19:27:51.995823 plume_python-0.1.8/plume_python/samples/common/__pycache__/quaternion_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1373 2024-03-14 14:49:00.848561 plume_python-0.1.8/plume_python/samples/common/__pycache__/quaternion_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1352 2024-03-14 14:49:00.853780 plume_python-0.1.8/plume_python/samples/common/__pycache__/rect_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1252 2023-10-02 19:27:51.996823 plume_python-0.1.8/plume_python/samples/common/__pycache__/spherical_harmonics_l1_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1712 2023-10-02 19:27:51.996823 plume_python-0.1.8/plume_python/samples/common/__pycache__/spherical_harmonics_l1_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1613 2024-03-14 14:49:00.857775 plume_python-0.1.8/plume_python/samples/common/__pycache__/spherical_harmonics_l1_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1409 2023-10-02 19:27:51.997826 plume_python-0.1.8/plume_python/samples/common/__pycache__/spherical_harmonics_l2_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1851 2023-10-02 19:27:51.997826 plume_python-0.1.8/plume_python/samples/common/__pycache__/spherical_harmonics_l2_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1767 2024-03-14 14:49:00.866049 plume_python-0.1.8/plume_python/samples/common/__pycache__/spherical_harmonics_l2_pb2.cpython-312.pyc
--rw-r--r--   0        0        0      981 2023-10-02 19:27:51.998823 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector2_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1420 2023-10-02 19:27:51.998823 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector2_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1336 2024-03-14 14:49:00.870128 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector2_pb2.cpython-312.pyc
--rw-r--r--   0        0        0      992 2023-10-02 19:27:51.998823 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector3_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1431 2023-10-02 19:27:51.999822 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector3_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1347 2024-03-14 14:49:00.829401 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector3_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1003 2023-10-02 19:27:51.999822 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector4_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1442 2023-10-02 19:27:52.000823 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector4_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1358 2024-03-14 14:49:00.861793 plume_python-0.1.8/plume_python/samples/common/__pycache__/vector4_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1973 2024-03-14 14:10:51.724560 plume_python-0.1.8/plume_python/samples/common/animation_curve_pb2.py
--rw-r--r--   0        0        0     2039 2024-03-14 14:10:51.725636 plume_python-0.1.8/plume_python/samples/common/animation_curve_pb2.pyi
--rw-r--r--   0        0        0     1328 2024-03-14 14:48:43.589531 plume_python-0.1.8/plume_python/samples/common/bounds_pb2.py
--rw-r--r--   0        0        0      677 2024-03-14 14:10:51.725636 plume_python-0.1.8/plume_python/samples/common/bounds_pb2.pyi
--rw-r--r--   0        0        0     2668 2024-03-14 14:10:51.726701 plume_python-0.1.8/plume_python/samples/common/color_pb2.py
--rw-r--r--   0        0        0     3076 2024-03-14 14:10:51.727701 plume_python-0.1.8/plume_python/samples/common/color_pb2.pyi
--rw-r--r--   0        0        0     1119 2024-03-14 14:10:51.727701 plume_python-0.1.8/plume_python/samples/common/marker_pb2.py
--rw-r--r--   0        0        0      384 2024-03-14 14:10:51.728704 plume_python-0.1.8/plume_python/samples/common/marker_pb2.pyi
--rw-r--r--   0        0        0     1664 2024-03-14 14:10:51.728704 plume_python-0.1.8/plume_python/samples/common/matrix4x4_pb2.py
--rw-r--r--   0        0        0     1703 2024-03-14 14:10:51.729807 plume_python-0.1.8/plume_python/samples/common/matrix4x4_pb2.pyi
--rw-r--r--   0        0        0     1233 2024-03-14 14:10:51.730810 plume_python-0.1.8/plume_python/samples/common/quaternion_pb2.py
--rw-r--r--   0        0        0      616 2024-03-14 14:10:51.730878 plume_python-0.1.8/plume_python/samples/common/quaternion_pb2.pyi
--rw-r--r--   0        0        0     1210 2024-03-14 14:10:51.730878 plume_python-0.1.8/plume_python/samples/common/rect_pb2.py
--rw-r--r--   0        0        0      646 2024-03-14 14:10:51.731948 plume_python-0.1.8/plume_python/samples/common/rect_pb2.pyi
--rw-r--r--   0        0        0     1471 2024-03-14 14:10:51.733009 plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l1_pb2.py
--rw-r--r--   0        0        0      811 2024-03-14 14:10:51.733009 plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l1_pb2.pyi
--rw-r--r--   0        0        0     2144 2024-03-14 14:10:51.734117 plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l2_pb2.py
--rw-r--r--   0        0        0     2790 2024-03-14 14:10:51.734117 plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l2_pb2.pyi
--rw-r--r--   0        0        0     1157 2024-03-14 14:10:51.735206 plume_python-0.1.8/plume_python/samples/common/vector2_pb2.py
--rw-r--r--   0        0        0      453 2024-03-14 14:10:51.735206 plume_python-0.1.8/plume_python/samples/common/vector2_pb2.pyi
--rw-r--r--   0        0        0     1185 2024-03-14 14:10:51.736302 plume_python-0.1.8/plume_python/samples/common/vector3_pb2.py
--rw-r--r--   0        0        0      533 2024-03-14 14:10:51.736302 plume_python-0.1.8/plume_python/samples/common/vector3_pb2.pyi
--rw-r--r--   0        0        0     1216 2024-03-14 14:10:51.737304 plume_python-0.1.8/plume_python/samples/common/vector4_pb2.py
--rw-r--r--   0        0        0      613 2024-03-14 14:10:51.737304 plume_python-0.1.8/plume_python/samples/common/vector4_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.662301 plume_python-0.1.8/plume_python/samples/lsl/__init__.py
--rw-r--r--   0        0        0      464 2023-10-02 19:27:52.006247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      692 2023-10-02 19:27:52.006247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-03-12 18:34:13.001182 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3078 2024-03-14 14:49:00.877174 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/lsl_stream_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1108 2023-10-02 19:27:52.007247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_close_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1565 2023-10-02 19:27:52.007247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_close_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1060 2023-10-02 19:27:52.008247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_info_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1526 2023-10-02 19:27:52.008247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_info_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1123 2023-10-02 19:27:52.008247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_open_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1580 2023-10-02 19:27:52.009247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_open_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1933 2023-10-02 19:27:52.009247 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_sample_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2670 2023-10-02 19:27:52.010249 plume_python-0.1.8/plume_python/samples/lsl/__pycache__/stream_sample_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3490 2024-03-14 14:10:51.738431 plume_python-0.1.8/plume_python/samples/lsl/lsl_stream_pb2.py
--rw-r--r--   0        0        0     4141 2024-03-14 14:10:51.739432 plume_python-0.1.8/plume_python/samples/lsl/lsl_stream_pb2.pyi
--rw-r--r--   0        0        0     1322 2024-03-14 14:10:51.739497 plume_python-0.1.8/plume_python/samples/packed_sample_pb2.py
--rw-r--r--   0        0        0      628 2024-03-14 14:10:51.740567 plume_python-0.1.8/plume_python/samples/packed_sample_pb2.pyi
--rw-r--r--   0        0        0     1939 2024-03-14 14:10:51.740567 plume_python-0.1.8/plume_python/samples/record_pb2.py
--rw-r--r--   0        0        0     1843 2024-03-14 14:10:51.741647 plume_python-0.1.8/plume_python/samples/record_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.662301 plume_python-0.1.8/plume_python/samples/unity/__init__.py
--rw-r--r--   0        0        0      507 2023-10-02 19:27:52.014858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      755 2023-10-02 19:27:52.014858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      174 2024-03-12 18:34:13.007183 plume_python-0.1.8/plume_python/samples/unity/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2934 2024-03-14 14:49:00.882177 plume_python-0.1.8/plume_python/samples/unity/__pycache__/audio_source_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1229 2023-10-02 19:27:52.015858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/camera_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1741 2023-10-02 19:27:52.015858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/camera_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     5844 2024-03-14 14:49:00.894175 plume_python-0.1.8/plume_python/samples/unity/__pycache__/camera_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1135 2023-10-02 19:27:52.016858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/component_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1595 2023-10-02 19:27:52.016858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/component_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1451 2024-03-14 14:49:00.910173 plume_python-0.1.8/plume_python/samples/unity/__pycache__/frame_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2092 2023-10-02 19:27:52.017864 plume_python-0.1.8/plume_python/samples/unity/__pycache__/game_object_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2888 2023-10-02 19:27:52.017864 plume_python-0.1.8/plume_python/samples/unity/__pycache__/game_object_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1993 2024-03-14 14:49:00.915176 plume_python-0.1.8/plume_python/samples/unity/__pycache__/game_object_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1418 2023-10-02 19:27:52.018864 plume_python-0.1.8/plume_python/samples/unity/__pycache__/identifiers_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2041 2023-10-02 19:27:52.018864 plume_python-0.1.8/plume_python/samples/unity/__pycache__/identifiers_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2159 2024-03-14 14:49:00.889175 plume_python-0.1.8/plume_python/samples/unity/__pycache__/identifiers_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     5279 2023-10-02 19:27:52.019865 plume_python-0.1.8/plume_python/samples/unity/__pycache__/light_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     6791 2023-10-02 19:27:52.019865 plume_python-0.1.8/plume_python/samples/unity/__pycache__/light_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     5303 2024-03-14 14:49:00.924175 plume_python-0.1.8/plume_python/samples/unity/__pycache__/light_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2297 2023-10-02 19:27:52.020863 plume_python-0.1.8/plume_python/samples/unity/__pycache__/lightmap_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2174 2024-03-14 14:49:00.920177 plume_python-0.1.8/plume_python/samples/unity/__pycache__/lightmap_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3887 2024-03-14 14:49:00.928416 plume_python-0.1.8/plume_python/samples/unity/__pycache__/line_renderer_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1340 2023-10-02 19:27:52.020863 plume_python-0.1.8/plume_python/samples/unity/__pycache__/mesh_filter_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1856 2023-10-02 19:27:52.021858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/mesh_filter_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1909 2024-03-14 14:49:00.932419 plume_python-0.1.8/plume_python/samples/unity/__pycache__/mesh_filter_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1514 2023-10-02 19:27:52.021858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/mesh_renderer_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2582 2023-10-02 19:27:52.021858 plume_python-0.1.8/plume_python/samples/unity/__pycache__/mesh_renderer_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1681 2024-03-14 14:49:00.936402 plume_python-0.1.8/plume_python/samples/unity/__pycache__/mesh_renderer_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3447 2023-10-02 19:27:52.023364 plume_python-0.1.8/plume_python/samples/unity/__pycache__/rect_transform_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4461 2023-10-02 19:27:52.023537 plume_python-0.1.8/plume_python/samples/unity/__pycache__/rect_transform_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4131 2023-10-02 19:27:52.024041 plume_python-0.1.8/plume_python/samples/unity/__pycache__/reflection_probe_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4309 2024-03-14 14:49:00.940584 plume_python-0.1.8/plume_python/samples/unity/__pycache__/reflection_probe_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1649 2023-10-02 19:27:52.024041 plume_python-0.1.8/plume_python/samples/unity/__pycache__/render_pipeline_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2873 2023-10-02 19:27:52.025046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/render_settings_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3529 2023-10-02 19:27:52.025046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/render_settings_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2327 2024-03-14 14:49:00.945583 plume_python-0.1.8/plume_python/samples/unity/__pycache__/renderer_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1849 2023-10-02 19:27:52.026046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/rendering_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2540 2024-03-14 14:49:00.898175 plume_python-0.1.8/plume_python/samples/unity/__pycache__/rendering_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1779 2024-03-14 14:49:00.950588 plume_python-0.1.8/plume_python/samples/unity/__pycache__/scene_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2469 2023-10-02 19:27:52.026046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/skinned_mesh_renderer_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3728 2023-10-02 19:27:52.027049 plume_python-0.1.8/plume_python/samples/unity/__pycache__/skinned_mesh_renderer_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2892 2024-03-14 14:49:00.954633 plume_python-0.1.8/plume_python/samples/unity/__pycache__/skinned_mesh_renderer_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2202 2023-10-02 19:27:52.027049 plume_python-0.1.8/plume_python/samples/unity/__pycache__/terrain_collider_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2084 2024-03-14 14:49:00.958600 plume_python-0.1.8/plume_python/samples/unity/__pycache__/terrain_collider_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3449 2023-10-02 19:27:52.028046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/terrain_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4020 2024-03-14 14:49:00.961857 plume_python-0.1.8/plume_python/samples/unity/__pycache__/terrain_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2639 2023-10-02 19:27:52.028046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/transform_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3466 2023-10-02 19:27:52.028046 plume_python-0.1.8/plume_python/samples/unity/__pycache__/transform_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2378 2024-03-14 14:49:00.966085 plume_python-0.1.8/plume_python/samples/unity/__pycache__/transform_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3514 2024-03-14 14:10:51.741647 plume_python-0.1.8/plume_python/samples/unity/audio_source_pb2.py
--rw-r--r--   0        0        0     3640 2024-03-14 14:10:51.742725 plume_python-0.1.8/plume_python/samples/unity/audio_source_pb2.pyi
--rw-r--r--   0        0        0     7709 2024-03-14 14:10:51.743795 plume_python-0.1.8/plume_python/samples/unity/camera_pb2.py
--rw-r--r--   0        0        0     9802 2024-03-14 14:10:51.743795 plume_python-0.1.8/plume_python/samples/unity/camera_pb2.pyi
--rw-r--r--   0        0        0     1292 2024-03-14 14:10:51.744867 plume_python-0.1.8/plume_python/samples/unity/frame_pb2.py
--rw-r--r--   0        0        0      763 2024-03-14 14:10:51.745959 plume_python-0.1.8/plume_python/samples/unity/frame_pb2.pyi
--rw-r--r--   0        0        0     2082 2024-03-14 14:10:51.745959 plume_python-0.1.8/plume_python/samples/unity/game_object_pb2.py
--rw-r--r--   0        0        0     1540 2024-03-14 14:10:51.747022 plume_python-0.1.8/plume_python/samples/unity/game_object_pb2.pyi
--rw-r--r--   0        0        0     2285 2024-03-14 14:10:51.747022 plume_python-0.1.8/plume_python/samples/unity/identifiers_pb2.py
--rw-r--r--   0        0        0     2301 2024-03-14 14:10:51.748082 plume_python-0.1.8/plume_python/samples/unity/identifiers_pb2.pyi
--rw-r--r--   0        0        0     6854 2024-03-14 14:10:51.749084 plume_python-0.1.8/plume_python/samples/unity/light_pb2.py
--rw-r--r--   0        0        0     8669 2024-03-14 14:10:51.749084 plume_python-0.1.8/plume_python/samples/unity/light_pb2.pyi
--rw-r--r--   0        0        0     2178 2024-03-14 14:10:51.750185 plume_python-0.1.8/plume_python/samples/unity/lightmap_pb2.py
--rw-r--r--   0        0        0     2105 2024-03-14 14:10:51.750185 plume_python-0.1.8/plume_python/samples/unity/lightmap_pb2.pyi
--rw-r--r--   0        0        0     4625 2024-03-14 14:10:51.751290 plume_python-0.1.8/plume_python/samples/unity/line_renderer_pb2.py
--rw-r--r--   0        0        0     5010 2024-03-14 14:10:51.752294 plume_python-0.1.8/plume_python/samples/unity/line_renderer_pb2.pyi
--rw-r--r--   0        0        0     1840 2024-03-14 14:10:51.752347 plume_python-0.1.8/plume_python/samples/unity/mesh_filter_pb2.py
--rw-r--r--   0        0        0     1255 2024-03-14 14:10:51.753400 plume_python-0.1.8/plume_python/samples/unity/mesh_filter_pb2.pyi
--rw-r--r--   0        0        0     1525 2024-03-14 14:10:51.753400 plume_python-0.1.8/plume_python/samples/unity/mesh_renderer_pb2.py
--rw-r--r--   0        0        0      823 2024-03-14 14:10:51.754483 plume_python-0.1.8/plume_python/samples/unity/mesh_renderer_pb2.pyi
--rw-r--r--   0        0        0     5308 2024-03-14 14:10:51.754483 plume_python-0.1.8/plume_python/samples/unity/reflection_probe_pb2.py
--rw-r--r--   0        0        0     6222 2024-03-14 14:10:51.755539 plume_python-0.1.8/plume_python/samples/unity/reflection_probe_pb2.pyi
--rw-r--r--   0        0        0     2475 2024-03-14 14:10:51.755539 plume_python-0.1.8/plume_python/samples/unity/renderer_pb2.py
--rw-r--r--   0        0        0     2229 2024-03-14 14:10:51.756612 plume_python-0.1.8/plume_python/samples/unity/renderer_pb2.pyi
--rw-r--r--   0        0        0     2661 2024-03-14 14:10:51.757676 plume_python-0.1.8/plume_python/samples/unity/rendering_pb2.py
--rw-r--r--   0        0        0     2993 2024-03-14 14:10:51.757676 plume_python-0.1.8/plume_python/samples/unity/rendering_pb2.pyi
--rw-r--r--   0        0        0     1640 2024-03-14 14:10:51.758750 plume_python-0.1.8/plume_python/samples/unity/scene_pb2.py
--rw-r--r--   0        0        0     1043 2024-03-14 14:10:51.758750 plume_python-0.1.8/plume_python/samples/unity/scene_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.662301 plume_python-0.1.8/plume_python/samples/unity/settings/__init__.py
--rw-r--r--   0        0        0     1862 2024-03-14 14:49:00.973756 plume_python-0.1.8/plume_python/samples/unity/settings/__pycache__/audio_settings_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1733 2024-03-14 14:49:00.976985 plume_python-0.1.8/plume_python/samples/unity/settings/__pycache__/graphics_settings_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1642 2024-03-14 14:49:00.980984 plume_python-0.1.8/plume_python/samples/unity/settings/__pycache__/quality_settings_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1641 2024-03-14 14:49:00.985981 plume_python-0.1.8/plume_python/samples/unity/settings/__pycache__/urp_global_settings_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1858 2024-03-14 14:10:51.759750 plume_python-0.1.8/plume_python/samples/unity/settings/audio_settings_pb2.py
--rw-r--r--   0        0        0     1405 2024-03-14 14:10:51.760860 plume_python-0.1.8/plume_python/samples/unity/settings/audio_settings_pb2.pyi
--rw-r--r--   0        0        0     1558 2024-03-14 14:10:51.761863 plume_python-0.1.8/plume_python/samples/unity/settings/graphics_settings_pb2.py
--rw-r--r--   0        0        0      878 2024-03-14 14:10:51.761863 plume_python-0.1.8/plume_python/samples/unity/settings/graphics_settings_pb2.pyi
--rw-r--r--   0        0        0     1486 2024-03-14 14:10:51.762983 plume_python-0.1.8/plume_python/samples/unity/settings/quality_settings_pb2.py
--rw-r--r--   0        0        0      731 2024-03-14 14:10:51.764043 plume_python-0.1.8/plume_python/samples/unity/settings/quality_settings_pb2.pyi
--rw-r--r--   0        0        0     1490 2024-03-14 14:10:51.765154 plume_python-0.1.8/plume_python/samples/unity/settings/urp_global_settings_pb2.py
--rw-r--r--   0        0        0      705 2024-03-14 14:10:51.765154 plume_python-0.1.8/plume_python/samples/unity/settings/urp_global_settings_pb2.pyi
--rw-r--r--   0        0        0     3233 2024-03-14 14:10:51.766222 plume_python-0.1.8/plume_python/samples/unity/skinned_mesh_renderer_pb2.py
--rw-r--r--   0        0        0     3059 2024-03-14 14:10:51.767282 plume_python-0.1.8/plume_python/samples/unity/skinned_mesh_renderer_pb2.pyi
--rw-r--r--   0        0        0     2114 2024-03-14 14:10:51.767282 plume_python-0.1.8/plume_python/samples/unity/terrain_collider_pb2.py
--rw-r--r--   0        0        0     1585 2024-03-14 14:10:51.768375 plume_python-0.1.8/plume_python/samples/unity/terrain_collider_pb2.pyi
--rw-r--r--   0        0        0     5055 2024-03-14 14:10:51.769447 plume_python-0.1.8/plume_python/samples/unity/terrain_pb2.py
--rw-r--r--   0        0        0     5955 2024-03-14 14:10:51.770527 plume_python-0.1.8/plume_python/samples/unity/terrain_pb2.pyi
--rw-r--r--   0        0        0     2493 2024-03-14 14:10:51.770527 plume_python-0.1.8/plume_python/samples/unity/transform_pb2.py
--rw-r--r--   0        0        0     2064 2024-03-14 14:10:51.771603 plume_python-0.1.8/plume_python/samples/unity/transform_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.677937 plume_python-0.1.8/plume_python/samples/unity/ui/__init__.py
--rw-r--r--   0        0        0      469 2023-10-02 19:27:52.037272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      697 2023-10-02 19:27:52.037272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1285 2023-10-02 19:27:52.038272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1799 2023-10-02 19:27:52.038272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3274 2024-03-14 14:49:00.989993 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1952 2024-03-14 14:49:00.993948 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_renderer_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1384 2023-10-02 19:27:52.038272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_scaler_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1901 2023-10-02 19:27:52.039271 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_scaler_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2024-03-14 14:49:00.996996 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/canvas_scaler_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2242 2024-03-14 14:49:01.002181 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/content_size_fitter_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1924 2024-03-14 14:49:01.006093 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/graphic_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1585 2023-10-02 19:27:52.039271 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/image_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2171 2023-10-02 19:27:52.039271 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/image_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2125 2024-03-14 14:49:01.010098 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/image_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2324 2024-03-14 14:49:01.014099 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/rect_transform_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2109 2023-10-02 19:27:52.040272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/text_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2807 2023-10-02 19:27:52.040272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/text_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3678 2024-03-14 14:49:01.019100 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/text_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2313 2023-10-02 19:27:52.040272 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/tmp_text_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3029 2023-10-02 19:27:52.041271 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/tmp_text_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2849 2024-03-14 14:49:01.023151 plume_python-0.1.8/plume_python/samples/unity/ui/__pycache__/tmp_text_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3882 2024-03-14 14:10:51.772611 plume_python-0.1.8/plume_python/samples/unity/ui/canvas_pb2.py
--rw-r--r--   0        0        0     4411 2024-03-14 14:10:51.772611 plume_python-0.1.8/plume_python/samples/unity/ui/canvas_pb2.pyi
--rw-r--r--   0        0        0     1912 2024-03-14 14:10:51.773734 plume_python-0.1.8/plume_python/samples/unity/ui/canvas_renderer_pb2.py
--rw-r--r--   0        0        0     1238 2024-03-14 14:10:51.774813 plume_python-0.1.8/plume_python/samples/unity/ui/canvas_renderer_pb2.pyi
--rw-r--r--   0        0        0     3791 2024-03-14 14:10:51.774813 plume_python-0.1.8/plume_python/samples/unity/ui/canvas_scaler_pb2.py
--rw-r--r--   0        0        0     3980 2024-03-14 14:10:51.775887 plume_python-0.1.8/plume_python/samples/unity/ui/canvas_scaler_pb2.pyi
--rw-r--r--   0        0        0     2319 2024-03-14 14:10:51.776956 plume_python-0.1.8/plume_python/samples/unity/ui/content_size_fitter_pb2.py
--rw-r--r--   0        0        0     1772 2024-03-14 14:10:51.778027 plume_python-0.1.8/plume_python/samples/unity/ui/content_size_fitter_pb2.pyi
--rw-r--r--   0        0        0     1907 2024-03-14 14:10:51.778027 plume_python-0.1.8/plume_python/samples/unity/ui/graphic_pb2.py
--rw-r--r--   0        0        0     1276 2024-03-14 14:10:51.779096 plume_python-0.1.8/plume_python/samples/unity/ui/graphic_pb2.pyi
--rw-r--r--   0        0        0     2162 2024-03-14 14:10:51.780197 plume_python-0.1.8/plume_python/samples/unity/ui/image_pb2.py
--rw-r--r--   0        0        0     1816 2024-03-14 14:10:51.780197 plume_python-0.1.8/plume_python/samples/unity/ui/image_pb2.pyi
--rw-r--r--   0        0        0     2445 2024-03-14 14:10:51.781294 plume_python-0.1.8/plume_python/samples/unity/ui/rect_transform_pb2.py
--rw-r--r--   0        0        0     1963 2024-03-14 14:10:51.782366 plume_python-0.1.8/plume_python/samples/unity/ui/rect_transform_pb2.pyi
--rw-r--r--   0        0        0     4455 2024-03-14 14:10:51.782366 plume_python-0.1.8/plume_python/samples/unity/ui/text_pb2.py
--rw-r--r--   0        0        0     5080 2024-03-14 14:10:51.783437 plume_python-0.1.8/plume_python/samples/unity/ui/text_pb2.pyi
--rw-r--r--   0        0        0     3448 2024-03-14 14:10:51.784438 plume_python-0.1.8/plume_python/samples/unity/ui/tmp_text_pb2.py
--rw-r--r--   0        0        0     3442 2024-03-14 14:10:51.784492 plume_python-0.1.8/plume_python/samples/unity/ui/tmp_text_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.677937 plume_python-0.1.8/plume_python/samples/unity/urp/__init__.py
--rw-r--r--   0        0        0      178 2024-03-12 18:34:13.229165 plume_python-0.1.8/plume_python/samples/unity/urp/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3526 2024-03-14 14:49:01.027423 plume_python-0.1.8/plume_python/samples/unity/urp/__pycache__/additional_camera_data_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1717 2024-03-14 14:49:01.034378 plume_python-0.1.8/plume_python/samples/unity/urp/__pycache__/rendering_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2513 2024-03-14 14:49:01.038653 plume_python-0.1.8/plume_python/samples/unity/urp/__pycache__/volume_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     4222 2024-03-14 14:10:51.785562 plume_python-0.1.8/plume_python/samples/unity/urp/additional_camera_data_pb2.py
--rw-r--r--   0        0        0     4357 2024-03-14 14:10:51.785562 plume_python-0.1.8/plume_python/samples/unity/urp/additional_camera_data_pb2.pyi
--rw-r--r--   0        0        0     1626 2024-03-14 14:10:51.786635 plume_python-0.1.8/plume_python/samples/unity/urp/rendering_pb2.py
--rw-r--r--   0        0        0     1139 2024-03-14 14:10:51.787726 plume_python-0.1.8/plume_python/samples/unity/urp/rendering_pb2.pyi
--rw-r--r--   0        0        0     2752 2024-03-14 14:10:51.787726 plume_python-0.1.8/plume_python/samples/unity/urp/volume_pb2.py
--rw-r--r--   0        0        0     2658 2024-03-14 14:10:51.788793 plume_python-0.1.8/plume_python/samples/unity/urp/volume_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-12 18:05:21.677937 plume_python-0.1.8/plume_python/samples/unity/xritk/__init__.py
--rw-r--r--   0        0        0      472 2023-10-02 19:27:52.043876 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      700 2023-10-02 19:27:52.043876 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2514 2023-10-02 19:27:52.044881 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/input_action_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2179 2023-10-02 19:27:52.044881 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/input_action_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     2483 2024-03-14 14:49:01.042653 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/input_action_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2914 2023-10-02 19:27:52.044881 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/xr_base_interactable_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3823 2023-10-02 19:27:52.045880 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/xr_base_interactable_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3577 2024-03-14 14:49:01.046611 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/xr_base_interactable_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2418 2023-10-02 19:27:52.045880 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/xr_base_interactor_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3215 2023-10-02 19:27:52.045880 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/xr_base_interactor_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     3013 2024-03-14 14:49:01.049889 plume_python-0.1.8/plume_python/samples/unity/xritk/__pycache__/xr_base_interactor_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2737 2024-03-14 14:10:51.789849 plume_python-0.1.8/plume_python/samples/unity/xritk/input_action_pb2.py
--rw-r--r--   0        0        0     2931 2024-03-14 14:10:51.789849 plume_python-0.1.8/plume_python/samples/unity/xritk/input_action_pb2.pyi
--rw-r--r--   0        0        0     4034 2024-03-14 14:10:51.790936 plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactable_pb2.py
--rw-r--r--   0        0        0     4199 2024-03-14 14:10:51.792007 plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactable_pb2.pyi
--rw-r--r--   0        0        0     3280 2024-03-14 14:10:51.792007 plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactor_pb2.py
--rw-r--r--   0        0        0     3212 2024-03-14 14:10:51.793086 plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactor_pb2.pyi
--rw-r--r--   0        0        0        0 2024-03-13 16:16:49.697454 plume_python-0.1.8/plume_python/utils/__init__.py
--rw-r--r--   0        0        0      166 2024-03-13 16:17:27.007699 plume_python-0.1.8/plume_python/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3234 2024-03-14 15:44:15.620082 plume_python-0.1.8/plume_python/utils/__pycache__/game_object.cpython-312.pyc
--rw-r--r--   0        0        0    13404 2024-03-14 16:13:26.468513 plume_python-0.1.8/plume_python/utils/__pycache__/transform.cpython-312.pyc
--rw-r--r--   0        0        0     2252 2024-03-14 15:28:44.447580 plume_python-0.1.8/plume_python/utils/game_object.py
--rw-r--r--   0        0        0     9124 2024-03-14 16:12:11.923751 plume_python-0.1.8/plume_python/utils/transform.py
--rw-r--r--   0        0        0      582 2024-03-14 15:39:15.071131 plume_python-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5162 2024-03-14 13:56:46.423408 plume_python-0.1.8/README.md
--rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 plume_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-03-14 22:22:17.139004 plume_python-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5037 2024-03-14 22:22:17.139004 plume_python-0.1.9/README.md
+-rw-r--r--   0        0        0      131 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/export/__init__.py
+-rw-r--r--   0        0        0     5363 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/export/xdf_exporter.py
+-rw-r--r--   0        0        0     6837 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/export/xdf_writer.py
+-rw-r--r--   0        0        0      638 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/file_reader.py
+-rw-r--r--   0        0        0     4221 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/parser.py
+-rw-r--r--   0        0        0     2795 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/record.py
+-rw-r--r--   0        0        0      871 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/__init__.py
+-rw-r--r--   0        0        0     1973 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/animation_curve_pb2.py
+-rw-r--r--   0        0        0     2039 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/animation_curve_pb2.pyi
+-rw-r--r--   0        0        0     1328 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/bounds_pb2.py
+-rw-r--r--   0        0        0      677 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/bounds_pb2.pyi
+-rw-r--r--   0        0        0     2668 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/color_pb2.py
+-rw-r--r--   0        0        0     3076 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/color_pb2.pyi
+-rw-r--r--   0        0        0     1119 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/marker_pb2.py
+-rw-r--r--   0        0        0      384 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/marker_pb2.pyi
+-rw-r--r--   0        0        0     1664 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/matrix4x4_pb2.py
+-rw-r--r--   0        0        0     1703 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/matrix4x4_pb2.pyi
+-rw-r--r--   0        0        0     1233 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/quaternion_pb2.py
+-rw-r--r--   0        0        0      616 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/quaternion_pb2.pyi
+-rw-r--r--   0        0        0     1210 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/rect_pb2.py
+-rw-r--r--   0        0        0      646 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/rect_pb2.pyi
+-rw-r--r--   0        0        0     1471 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l1_pb2.py
+-rw-r--r--   0        0        0      811 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l1_pb2.pyi
+-rw-r--r--   0        0        0     2144 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l2_pb2.py
+-rw-r--r--   0        0        0     2790 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l2_pb2.pyi
+-rw-r--r--   0        0        0     1157 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/vector2_pb2.py
+-rw-r--r--   0        0        0      453 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/vector2_pb2.pyi
+-rw-r--r--   0        0        0     1185 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/vector3_pb2.py
+-rw-r--r--   0        0        0      533 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/vector3_pb2.pyi
+-rw-r--r--   0        0        0     1216 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/vector4_pb2.py
+-rw-r--r--   0        0        0      613 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/common/vector4_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/lsl/__init__.py
+-rw-r--r--   0        0        0     3490 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/lsl/lsl_stream_pb2.py
+-rw-r--r--   0        0        0     4141 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/lsl/lsl_stream_pb2.pyi
+-rw-r--r--   0        0        0     1322 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/packed_sample_pb2.py
+-rw-r--r--   0        0        0      628 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/packed_sample_pb2.pyi
+-rw-r--r--   0        0        0     1939 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/record_pb2.py
+-rw-r--r--   0        0        0     1843 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/record_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/__init__.py
+-rw-r--r--   0        0        0     3514 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/audio_source_pb2.py
+-rw-r--r--   0        0        0     3640 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/audio_source_pb2.pyi
+-rw-r--r--   0        0        0     7709 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/camera_pb2.py
+-rw-r--r--   0        0        0     9802 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/camera_pb2.pyi
+-rw-r--r--   0        0        0     1292 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/frame_pb2.py
+-rw-r--r--   0        0        0      763 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/frame_pb2.pyi
+-rw-r--r--   0        0        0     2082 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/game_object_pb2.py
+-rw-r--r--   0        0        0     1540 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/game_object_pb2.pyi
+-rw-r--r--   0        0        0     2285 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/identifiers_pb2.py
+-rw-r--r--   0        0        0     2301 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/identifiers_pb2.pyi
+-rw-r--r--   0        0        0     6854 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/light_pb2.py
+-rw-r--r--   0        0        0     8669 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/light_pb2.pyi
+-rw-r--r--   0        0        0     2178 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/lightmap_pb2.py
+-rw-r--r--   0        0        0     2105 2024-03-14 22:22:17.139004 plume_python-0.1.9/plume_python/samples/unity/lightmap_pb2.pyi
+-rw-r--r--   0        0        0     4625 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/line_renderer_pb2.py
+-rw-r--r--   0        0        0     5010 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/line_renderer_pb2.pyi
+-rw-r--r--   0        0        0     1840 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/mesh_filter_pb2.py
+-rw-r--r--   0        0        0     1255 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/mesh_filter_pb2.pyi
+-rw-r--r--   0        0        0     1525 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/mesh_renderer_pb2.py
+-rw-r--r--   0        0        0      823 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/mesh_renderer_pb2.pyi
+-rw-r--r--   0        0        0     5308 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/reflection_probe_pb2.py
+-rw-r--r--   0        0        0     6222 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/reflection_probe_pb2.pyi
+-rw-r--r--   0        0        0     2475 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/renderer_pb2.py
+-rw-r--r--   0        0        0     2229 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/renderer_pb2.pyi
+-rw-r--r--   0        0        0     2661 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/rendering_pb2.py
+-rw-r--r--   0        0        0     2993 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/rendering_pb2.pyi
+-rw-r--r--   0        0        0     1640 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/scene_pb2.py
+-rw-r--r--   0        0        0     1043 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/scene_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/__init__.py
+-rw-r--r--   0        0        0     1858 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/audio_settings_pb2.py
+-rw-r--r--   0        0        0     1405 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/audio_settings_pb2.pyi
+-rw-r--r--   0        0        0     1558 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/graphics_settings_pb2.py
+-rw-r--r--   0        0        0      878 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/graphics_settings_pb2.pyi
+-rw-r--r--   0        0        0     1486 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/quality_settings_pb2.py
+-rw-r--r--   0        0        0      731 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/quality_settings_pb2.pyi
+-rw-r--r--   0        0        0     1490 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/urp_global_settings_pb2.py
+-rw-r--r--   0        0        0      705 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/settings/urp_global_settings_pb2.pyi
+-rw-r--r--   0        0        0     3233 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/skinned_mesh_renderer_pb2.py
+-rw-r--r--   0        0        0     3059 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/skinned_mesh_renderer_pb2.pyi
+-rw-r--r--   0        0        0     2114 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/terrain_collider_pb2.py
+-rw-r--r--   0        0        0     1585 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/terrain_collider_pb2.pyi
+-rw-r--r--   0        0        0     5055 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/terrain_pb2.py
+-rw-r--r--   0        0        0     5955 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/terrain_pb2.pyi
+-rw-r--r--   0        0        0     2493 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/transform_pb2.py
+-rw-r--r--   0        0        0     2064 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/transform_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/__init__.py
+-rw-r--r--   0        0        0     3882 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/canvas_pb2.py
+-rw-r--r--   0        0        0     4411 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/canvas_pb2.pyi
+-rw-r--r--   0        0        0     1912 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/canvas_renderer_pb2.py
+-rw-r--r--   0        0        0     1238 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/canvas_renderer_pb2.pyi
+-rw-r--r--   0        0        0     3791 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/canvas_scaler_pb2.py
+-rw-r--r--   0        0        0     3980 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/canvas_scaler_pb2.pyi
+-rw-r--r--   0        0        0     2319 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/content_size_fitter_pb2.py
+-rw-r--r--   0        0        0     1772 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/content_size_fitter_pb2.pyi
+-rw-r--r--   0        0        0     1907 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/graphic_pb2.py
+-rw-r--r--   0        0        0     1276 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/graphic_pb2.pyi
+-rw-r--r--   0        0        0     2162 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/image_pb2.py
+-rw-r--r--   0        0        0     1816 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/image_pb2.pyi
+-rw-r--r--   0        0        0     2445 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/rect_transform_pb2.py
+-rw-r--r--   0        0        0     1963 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/rect_transform_pb2.pyi
+-rw-r--r--   0        0        0     4455 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/text_pb2.py
+-rw-r--r--   0        0        0     5080 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/text_pb2.pyi
+-rw-r--r--   0        0        0     3448 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/tmp_text_pb2.py
+-rw-r--r--   0        0        0     3442 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/ui/tmp_text_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/__init__.py
+-rw-r--r--   0        0        0     4222 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/additional_camera_data_pb2.py
+-rw-r--r--   0        0        0     4357 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/additional_camera_data_pb2.pyi
+-rw-r--r--   0        0        0     1626 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/rendering_pb2.py
+-rw-r--r--   0        0        0     1139 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/rendering_pb2.pyi
+-rw-r--r--   0        0        0     2752 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/volume_pb2.py
+-rw-r--r--   0        0        0     2658 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/urp/volume_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/__init__.py
+-rw-r--r--   0        0        0     2737 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/input_action_pb2.py
+-rw-r--r--   0        0        0     2931 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/input_action_pb2.pyi
+-rw-r--r--   0        0        0     4034 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactable_pb2.py
+-rw-r--r--   0        0        0     4199 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactable_pb2.pyi
+-rw-r--r--   0        0        0     3280 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactor_pb2.py
+-rw-r--r--   0        0        0     3212 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactor_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/utils/__init__.py
+-rw-r--r--   0        0        0     1538 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/utils/dataframe.py
+-rw-r--r--   0        0        0     1707 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/utils/game_object.py
+-rw-r--r--   0        0        0     8558 2024-03-14 22:22:17.143004 plume_python-0.1.9/plume_python/utils/transform.py
+-rw-r--r--   0        0        0      603 2024-03-14 22:22:17.143004 plume_python-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 plume_python-0.1.9/PKG-INFO
```

### Comparing `plume_python-0.1.8/LICENSE` & `plume_python-0.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `plume_python-0.1.8/plume_python/export/dataframe_exporter.py` & `plume_python-0.1.9/plume_python/utils/dataframe.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-import pandas as pd
-from google.protobuf.descriptor_pool import DescriptorPool
-from google.protobuf.json_format import MessageToDict
-
-from plume_python.record import RawSample, FrameSample, MarkerSample
-from plume_python.samples import default_descriptor_pool
-
-
-def markers_to_dataframe(markers: list[MarkerSample]) -> pd.DataFrame:
-    sample_data = []
-    for marker in markers:
-        sample_data.append({"timestamp": marker.timestamp, "marker_label": marker.label})
-    return pd.json_normalize(sample_data)
-
-
-def frames_to_dataframe(frames: list[FrameSample], descriptor_pool: DescriptorPool = default_descriptor_pool) \
-        -> dict[type, pd.DataFrame]:
-    """Converts a list of frames into a dictionary of dataframes. The keys are the types of the payloads and the values are the dataframes."""
-    # Aggregate data from all frames in a single list
-    samples = [data for frame in frames for data in frame.data]
-    return samples_to_dataframes(samples, descriptor_pool)
-
-
-def samples_to_dataframes(samples: list[RawSample], descriptor_pool: DescriptorPool = default_descriptor_pool) \
-        -> dict[type, pd.DataFrame]:
-    dataframes: dict[type, pd.DataFrame] = {}
-
-    # Group samples by payload type
-    groups: dict[type, list[RawSample]] = {}
-    for s in samples:
-        if type(s.payload) not in groups:
-            groups[type(s.payload)] = []
-        groups[type(s.payload)].append(s)
-
-    for (group_key, group_samples) in groups.items():
-        sample_data = []
-
-        for sample in group_samples:
-            sample_payload_fields_value = MessageToDict(sample.payload, including_default_value_fields=True,
-                                                        descriptor_pool=descriptor_pool)
-            sample_data.append({"timestamp": sample.timestamp} | sample_payload_fields_value)
-
-        dataframes[group_key] = pd.json_normalize(sample_data)
-
-    return dataframes
+from typing import TypeVar, cast, Type
+
+import pandas as pd
+from google.protobuf.json_format import MessageToDict
+from google.protobuf.message import Message
+
+from plume_python.record import Sample, FrameDataSample, Record
+
+T = TypeVar('T', bound=Message)
+
+
+def samples_to_dataframe(samples: list[Sample[T]]) -> pd.DataFrame:
+    if len(samples) == 0:
+        return pd.DataFrame()
+
+    sample_data = []
+
+    if isinstance(samples[0], FrameDataSample):
+        frame_samples = cast(list[FrameDataSample[T]], samples)
+        for frame_sample in frame_samples:
+            sample_payload_fields_value = MessageToDict(frame_sample.payload, including_default_value_fields=True)
+            sample_data.append({"timestamp": frame_sample.timestamp,
+                                "frame_number": frame_sample.frame_number} | sample_payload_fields_value)
+    else:
+        for sample in samples:
+            sample_payload_fields_value = MessageToDict(sample.payload, including_default_value_fields=True)
+            if sample.is_timestamped():
+                sample_data.append({"timestamp": sample.timestamp} | sample_payload_fields_value)
+            else:
+                sample_data.append(sample_payload_fields_value)
+
+    return pd.json_normalize(sample_data)
+
+
+def record_to_dataframes(record: Record) -> dict[type, pd.DataFrame]:
+    dataframes: dict[Type[T], pd.DataFrame] = {}
+
+    for payload_type, samples in record.samples_by_type.items():
+        dataframes[payload_type] = samples_to_dataframe(samples)
+
+    return dataframes
```

### Comparing `plume_python-0.1.8/plume_python/file_reader.py` & `plume_python-0.1.9/plume_python/file_reader.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from io import BytesIO
-from typing import BinaryIO
-
-import lz4.frame
-
-
-def _is_lz4_compressed(raw_bytes: bytes) -> bool:
-    magic_number = raw_bytes[:4][::-1]
-    return magic_number == bytes.fromhex("184d2204")
-
-
-def read_file(filepath: str) -> BinaryIO:
-    if not filepath.endswith('.plm'):
-        raise ValueError("File must be a .plm file")
-
-    with open(filepath, "rb") as file:
-        raw_bytes = file.read()
-
-        if _is_lz4_compressed(raw_bytes):
-            decompressor = lz4.frame.LZ4FrameDecompressor()
-            return BytesIO(decompressor.decompress(raw_bytes))
-        else:
-            return BytesIO(raw_bytes)
+from io import BytesIO
+from typing import BinaryIO
+
+import lz4.frame
+
+
+def _is_lz4_compressed(raw_bytes: bytes) -> bool:
+    magic_number = raw_bytes[:4][::-1]
+    return magic_number == bytes.fromhex("184d2204")
+
+
+def read_file(filepath: str) -> BinaryIO:
+    if not filepath.endswith('.plm'):
+        raise ValueError("File must be a .plm file")
+
+    with open(filepath, "rb") as file:
+        raw_bytes = file.read()
+
+        if _is_lz4_compressed(raw_bytes):
+            decompressor = lz4.frame.LZ4FrameDecompressor()
+            return BytesIO(decompressor.decompress(raw_bytes))
+        else:
+            return BytesIO(raw_bytes)
```

### Comparing `plume_python-0.1.8/plume_python/samples/__init__.py` & `plume_python-0.1.9/plume_python/samples/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import sys
-from os import walk, path
-from importlib.util import spec_from_file_location, module_from_spec
-from google.protobuf import descriptor_pool as _descriptor_pool
-
-
-def build_descriptor_pool(root_folder):
-    """
-    Import all generated *_pb2.py modules dynamically.
-    """
-    for root, dirs, files in walk(root_folder):
-        for file in files:
-            if file.endswith("_pb2.py"):
-                # Dynamically import the module
-                module_name = file[:-6]  # Remove "_pb2.py" from the file name
-                spec = spec_from_file_location(module_name, path.join(root, file))
-                module = module_from_spec(spec)
-                spec.loader.exec_module(module)
-    return _descriptor_pool.Default()
-
-
-sys.path.append(path.abspath(path.dirname(__file__)))
-default_descriptor_pool = build_descriptor_pool(path.dirname(__file__))
+import sys
+from os import walk, path
+from importlib.util import spec_from_file_location, module_from_spec
+from google.protobuf import descriptor_pool as _descriptor_pool
+
+
+def build_descriptor_pool(root_folder):
+    """
+    Import all generated *_pb2.py modules dynamically.
+    """
+    for root, dirs, files in walk(root_folder):
+        for file in files:
+            if file.endswith("_pb2.py"):
+                # Dynamically import the module
+                module_name = file[:-6]  # Remove "_pb2.py" from the file name
+                spec = spec_from_file_location(module_name, path.join(root, file))
+                module = module_from_spec(spec)
+                spec.loader.exec_module(module)
+    return _descriptor_pool.Default()
+
+
+sys.path.append(path.abspath(path.dirname(__file__)))
+default_descriptor_pool = build_descriptor_pool(path.dirname(__file__))
```

### Comparing `plume_python-0.1.8/plume_python/samples/common/animation_curve_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/animation_curve_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/animation_curve_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/animation_curve_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/bounds_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/bounds_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/color_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/color_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/color_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/color_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/marker_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/marker_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/matrix4x4_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/matrix4x4_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/matrix4x4_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/matrix4x4_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/quaternion_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/quaternion_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/quaternion_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/quaternion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/rect_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/rect_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/rect_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/rect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l1_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l1_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l1_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l2_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l2_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/spherical_harmonics_l2_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/spherical_harmonics_l2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/vector2_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/vector2_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/vector3_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/vector3_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/vector3_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/vector3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/vector4_pb2.py` & `plume_python-0.1.9/plume_python/samples/common/vector4_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/common/vector4_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/common/vector4_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/lsl/lsl_stream_pb2.py` & `plume_python-0.1.9/plume_python/samples/lsl/lsl_stream_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/lsl/lsl_stream_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/lsl/lsl_stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/packed_sample_pb2.py` & `plume_python-0.1.9/plume_python/samples/packed_sample_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/packed_sample_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/packed_sample_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/record_pb2.py` & `plume_python-0.1.9/plume_python/samples/record_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/record_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/record_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/audio_source_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/audio_source_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/audio_source_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/audio_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/camera_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/camera_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/camera_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/camera_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/frame_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/frame_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/frame_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/frame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/game_object_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/game_object_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/game_object_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/game_object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/identifiers_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/identifiers_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/identifiers_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/identifiers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/light_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/light_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/light_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/light_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/lightmap_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/lightmap_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/lightmap_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/lightmap_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/line_renderer_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/line_renderer_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/line_renderer_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/line_renderer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/mesh_filter_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/mesh_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/mesh_filter_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/mesh_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/mesh_renderer_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/mesh_renderer_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/mesh_renderer_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/mesh_renderer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/reflection_probe_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/reflection_probe_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/reflection_probe_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/reflection_probe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/renderer_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/renderer_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/renderer_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/renderer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/rendering_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/rendering_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/rendering_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/rendering_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/scene_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/scene_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/scene_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/scene_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/audio_settings_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/settings/audio_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/audio_settings_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/settings/audio_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/graphics_settings_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/settings/graphics_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/graphics_settings_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/settings/graphics_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/quality_settings_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/settings/quality_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/quality_settings_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/settings/quality_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/urp_global_settings_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/settings/urp_global_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/settings/urp_global_settings_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/settings/urp_global_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/skinned_mesh_renderer_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/skinned_mesh_renderer_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/skinned_mesh_renderer_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/skinned_mesh_renderer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/terrain_collider_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/terrain_collider_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/terrain_collider_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/terrain_collider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/terrain_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/terrain_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/terrain_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/terrain_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/transform_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/transform_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/canvas_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/canvas_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/canvas_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/canvas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/canvas_renderer_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/canvas_renderer_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/canvas_renderer_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/canvas_renderer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/canvas_scaler_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/canvas_scaler_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/canvas_scaler_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/canvas_scaler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/content_size_fitter_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/content_size_fitter_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/content_size_fitter_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/content_size_fitter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/graphic_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/graphic_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/graphic_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/graphic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/image_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/image_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/image_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/rect_transform_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/rect_transform_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/rect_transform_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/rect_transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/text_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/text_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/text_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/tmp_text_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/ui/tmp_text_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/ui/tmp_text_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/ui/tmp_text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/urp/additional_camera_data_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/urp/additional_camera_data_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/urp/additional_camera_data_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/urp/additional_camera_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/urp/rendering_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/urp/rendering_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/urp/rendering_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/urp/rendering_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/urp/volume_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/urp/volume_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/urp/volume_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/urp/volume_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/xritk/input_action_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/xritk/input_action_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/xritk/input_action_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/xritk/input_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactable_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactable_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactable_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactor_pb2.py` & `plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactor_pb2.py`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/samples/unity/xritk/xr_base_interactor_pb2.pyi` & `plume_python-0.1.9/plume_python/samples/unity/xritk/xr_base_interactor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plume_python-0.1.8/plume_python/utils/transform.py` & `plume_python-0.1.9/plume_python/utils/transform.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,193 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-
-import numpy as np
-import quaternion
-from tqdm import tqdm
-from typing import Optional
-
-from ..record import Record, FrameSample, RawSample
-from ..samples.unity.transform_pb2 import TransformCreate, TransformUpdate, TransformDestroy
-
-
-def _extract_transform_samples_from_frame(frame: FrameSample):
-    transform_create_samples: list[RawSample[TransformCreate]] = []
-    transform_update_samples: list[RawSample[TransformUpdate]] = []
-    transform_destroy_samples: list[RawSample[TransformDestroy]] = []
-
-    for frame_data in frame.data:
-        if isinstance(frame_data.payload, TransformCreate):
-            transform_create_samples.append(frame_data)
-        elif isinstance(frame_data.payload, TransformUpdate):
-            transform_update_samples.append(frame_data)
-        elif isinstance(frame_data.payload, TransformDestroy):
-            transform_destroy_samples.append(frame_data)
-
-    return transform_create_samples, transform_destroy_samples, transform_update_samples
-
-
-@dataclass(slots=True)
-class Transform:
-    _local_position: np.ndarray = field(default_factory=lambda: np.array(3, dtype=np.float32))
-    _local_rotation: quaternion.quaternion = field(default_factory=lambda: quaternion.quaternion(1, 0, 0, 0))
-    _local_scale: np.ndarray = field(default_factory=lambda: np.array(4, dtype=np.float32))
-    _local_T_mtx: np.ndarray = field(default_factory=lambda: np.eye(4, dtype=np.float32))
-    _local_R_mtx: np.ndarray = field(default_factory=lambda: np.eye(4, dtype=np.float32))
-    _local_S_mtx: np.ndarray = field(default_factory=lambda: np.eye(4, dtype=np.float32))
-    _local_to_world_mtx: np.ndarray = None
-    _parent: Optional[Transform] = None
-    _dirty: bool = True
-
-    def copy(self) -> Transform:
-        parent_copy = None if self._parent is None else self._parent.copy()
-        copy = Transform(_local_position=self._local_position, _local_rotation=self._local_rotation,
-                         _local_scale=self._local_scale, _local_T_mtx=self._local_T_mtx, _local_R_mtx=self._local_R_mtx,
-                         _local_S_mtx=self._local_S_mtx, _parent=parent_copy, _dirty=self._dirty,
-                         _local_to_world_mtx=self._local_to_world_mtx)
-        return copy
-
-    def _is_dirty(self) -> bool:
-        return self._dirty or self._parent is not None and self._parent._is_dirty()
-
-    def set_local_position(self, local_position: np.ndarray):
-        self._local_T_mtx[0:3, 3] = local_position
-        self._local_position = local_position
-        self._dirty = True
-
-    def set_local_rotation(self, local_rotation: quaternion):
-        self._local_R_mtx[0:3, 0:3] = quaternion.as_rotation_matrix(local_rotation)
-        self._local_rotation = local_rotation
-        self._dirty = True
-
-    def set_local_scale(self, local_scale: np.ndarray):
-        self._local_S_mtx[0, 0] = local_scale[0]
-        self._local_S_mtx[1, 1] = local_scale[1]
-        self._local_S_mtx[2, 2] = local_scale[2]
-        self._local_scale = local_scale
-        self._dirty = True
-
-    def get_local_position(self) -> np.ndarray:
-        return self._local_position
-
-    def get_local_rotation(self) -> quaternion:
-        return self._local_rotation
-
-    def get_local_scale(self) -> np.ndarray:
-        return self._local_scale
-
-    def set_parent(self, parent: Optional[Transform]):
-        self._parent = parent
-        self._dirty = True
-
-    def get_parent(self) -> Optional[Transform]:
-        return self._parent
-
-    def get_local_to_world_matrix(self) -> np.ndarray:
-        if self._is_dirty() or self._local_to_world_mtx is None:
-
-            trs_mtx = self._local_T_mtx @ self._local_R_mtx @ self._local_S_mtx
-
-            if self._parent is None:
-                self._local_to_world_mtx = trs_mtx
-            else:
-                self._local_to_world_mtx = self._parent.get_local_to_world_matrix() @ trs_mtx
-
-            self._dirty = False
-
-        return self._local_to_world_mtx
-
-    def get_world_position(self) -> np.ndarray:
-        return self.get_local_to_world_matrix()[0:3, 3].transpose()
-
-    def get_world_rotation(self) -> quaternion:
-        return quaternion.from_rotation_matrix(self.get_local_to_world_matrix()[0:3, 0:3])
-
-    def get_world_scale(self) -> np.ndarray:
-        local_to_world_mtx = self.get_local_to_world_matrix()
-        sx = np.linalg.norm(local_to_world_mtx[0:3, 0])
-        sy = np.linalg.norm(local_to_world_mtx[0:3, 1])
-        sz = np.linalg.norm(local_to_world_mtx[0:3, 2])
-        scale = np.array([sx, sy, sz])
-        return scale
-
-
-@dataclass(frozen=True, slots=True)
-class TimestampedTransform:
-    timestamp: int
-    frame_number: int
-    transform: Transform
-
-    def get_local_position(self) -> np.ndarray:
-        return self.transform.get_local_position()
-
-    def get_local_rotation(self) -> quaternion:
-        return self.transform.get_local_rotation()
-
-    def get_local_scale(self) -> np.ndarray:
-        return self.transform.get_local_scale()
-
-    def get_world_position(self) -> np.ndarray:
-        return self.transform.get_world_position()
-
-    def get_world_rotation(self) -> quaternion:
-        return self.transform.get_world_rotation()
-
-    def get_world_scale(self) -> np.ndarray:
-        return self.transform.get_world_scale()
-
-
-def compute_transform_time_series(record: Record, guid: str) -> list[TimestampedTransform]:
-    transform_time_series = compute_transforms_time_series(record, {guid})
-    return transform_time_series.get(guid, {})
-
-
-def compute_transforms_time_series(record: Record, included_guids: set[str] = None) \
-        -> dict[str, list[TimestampedTransform]]:
-    result: dict[str, list[TimestampedTransform]] = {}
-    current_transforms: dict[str, Transform] = {}
-
-    for frame in tqdm(record.frames, desc="Computing world positions"):
-
-        creation_samples, destruction_samples, update_samples = _extract_transform_samples_from_frame(frame)
-
-        # Add newly created transforms
-        for creation_sample in creation_samples:
-            guid = creation_sample.payload.id.component_id
-            if guid not in current_transforms:
-                current_transforms[guid] = Transform()
-
-        # Remove transforms that were destroyed in this frame
-        for destruction_sample in destruction_samples:
-            guid = destruction_sample.payload.id.component_id
-            if guid in current_transforms:
-                del current_transforms[guid]
-
-        # Apply transform updates
-        for update_sample in update_samples:
-            guid = update_sample.payload.id.component_id
-            local_transform = current_transforms[guid]
-            if update_sample.payload.HasField('local_position'):
-                local_position = update_sample.payload.local_position
-                local_transform.set_local_position(np.array([local_position.x, local_position.y, local_position.z]))
-            if update_sample.payload.HasField('local_rotation'):
-                local_rotation = update_sample.payload.local_rotation
-                q = quaternion.quaternion(local_rotation.w, local_rotation.x, local_rotation.y, local_rotation.z)
-                local_transform.set_local_rotation(q)
-            if update_sample.payload.HasField('local_scale'):
-                local_scale = update_sample.payload.local_scale
-                local_transform.set_local_scale(np.array([local_scale.x, local_scale.y, local_scale.z]))
-            if update_sample.payload.HasField('parent_transform_id'):
-                parent_guid = update_sample.payload.parent_transform_id.component_id
-                if parent_guid == "00000000000000000000000000000000":  # null guid
-                    local_transform.set_parent(None)
-                elif parent_guid in current_transforms:
-                    local_transform.set_parent(current_transforms[parent_guid])
-                else:
-                    parent = Transform()
-                    local_transform.set_parent(parent)
-                    current_transforms[parent_guid] = parent
-
-        if included_guids is not None:
-            for included_guid in included_guids:
-                if included_guid in current_transforms:
-                    if included_guid not in result:
-                        result[included_guid] = []
-                    transform_copy = current_transforms[included_guid].copy()
-                    timestamped_transform = TimestampedTransform(frame.timestamp, frame.frame_number, transform_copy)
-                    result[included_guid].append(timestamped_transform)
-        else:
-            for guid, transform in current_transforms.items():
-                if guid not in result:
-                    result[guid] = []
-                transform_copy = transform.copy()
-                result[guid].append(TimestampedTransform(frame.timestamp, frame.frame_number, transform_copy))
-
-    return result
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from itertools import groupby
+from typing import Optional
+
+import numpy as np
+import quaternion
+from tqdm import tqdm
+
+from ..record import Record
+from ..samples.unity import transform_pb2
+
+
+@dataclass(slots=True)
+class Transform:
+    _guid: str
+    _local_position: np.ndarray = field(default_factory=lambda: np.array(3, dtype=np.float32))
+    _local_rotation: quaternion.quaternion = field(default_factory=lambda: quaternion.quaternion(1, 0, 0, 0))
+    _local_scale: np.ndarray = field(default_factory=lambda: np.array(4, dtype=np.float32))
+    _local_T_mtx: np.ndarray = field(default_factory=lambda: np.eye(4, dtype=np.float32))
+    _local_R_mtx: np.ndarray = field(default_factory=lambda: np.eye(4, dtype=np.float32))
+    _local_S_mtx: np.ndarray = field(default_factory=lambda: np.eye(4, dtype=np.float32))
+    _local_to_world_mtx: np.ndarray = None
+    _parent: Optional[Transform] = None
+    _dirty: bool = True
+
+    def _is_dirty(self) -> bool:
+        return self._dirty or self._parent is not None and self._parent._is_dirty()
+
+    def get_guid(self) -> str:
+        return self._guid
+
+    def set_local_position(self, local_position: np.ndarray):
+        self._local_T_mtx[0:3, 3] = local_position
+        self._local_position = local_position
+        self._dirty = True
+
+    def set_local_rotation(self, local_rotation: quaternion):
+        self._local_R_mtx[0:3, 0:3] = quaternion.as_rotation_matrix(local_rotation)
+        self._local_rotation = local_rotation
+        self._dirty = True
+
+    def set_local_scale(self, local_scale: np.ndarray):
+        self._local_S_mtx[0, 0] = local_scale[0]
+        self._local_S_mtx[1, 1] = local_scale[1]
+        self._local_S_mtx[2, 2] = local_scale[2]
+        self._local_scale = local_scale
+        self._dirty = True
+
+    def get_local_position(self) -> np.ndarray:
+        return self._local_position
+
+    def get_local_rotation(self) -> quaternion:
+        return self._local_rotation
+
+    def get_local_scale(self) -> np.ndarray:
+        return self._local_scale
+
+    def set_parent(self, parent: Optional[Transform]):
+        self._parent = parent
+        self._dirty = True
+
+    def get_parent(self) -> Optional[Transform]:
+        return self._parent
+
+    def get_local_to_world_matrix(self) -> np.ndarray:
+        if self._is_dirty() or self._local_to_world_mtx is None:
+
+            trs_mtx = self._local_T_mtx @ self._local_R_mtx @ self._local_S_mtx
+
+            if self._parent is None:
+                self._local_to_world_mtx = trs_mtx
+            else:
+                self._local_to_world_mtx = self._parent.get_local_to_world_matrix() @ trs_mtx
+
+            self._dirty = False
+
+        return self._local_to_world_mtx
+
+    def get_world_position(self) -> np.ndarray:
+        return self.get_local_to_world_matrix()[0:3, 3].transpose()
+
+    def get_world_rotation(self) -> quaternion:
+        return quaternion.from_rotation_matrix(self.get_local_to_world_matrix()[0:3, 0:3])
+
+    def get_world_scale(self) -> np.ndarray:
+        local_to_world_mtx = self.get_local_to_world_matrix()
+        sx = np.linalg.norm(local_to_world_mtx[0:3, 0])
+        sy = np.linalg.norm(local_to_world_mtx[0:3, 1])
+        sz = np.linalg.norm(local_to_world_mtx[0:3, 2])
+        scale = np.array([sx, sy, sz])
+        return scale
+
+
+@dataclass(frozen=True, slots=True)
+class TimestampedTransform:
+    timestamp: int
+    frame_number: int
+    guid: str
+    parent_guid: Optional[str]
+    local_position: np.ndarray
+    local_rotation: quaternion.quaternion
+    local_scale: np.ndarray
+    local_to_world_mtx: np.ndarray
+
+    def get_world_position(self) -> np.ndarray:
+        return self.local_to_world_mtx[0:3, 3].transpose()
+
+    def get_world_rotation(self) -> quaternion:
+        return quaternion.from_rotation_matrix(self.local_to_world_mtx[0:3, 0:3])
+
+    def get_world_scale(self) -> np.ndarray:
+        sx = np.linalg.norm(self.local_to_world_mtx[0:3, 0])
+        sy = np.linalg.norm(self.local_to_world_mtx[0:3, 1])
+        sz = np.linalg.norm(self.local_to_world_mtx[0:3, 2])
+        scale = np.array([sx, sy, sz])
+        return scale
+
+
+def compute_transform_time_series(record: Record, guid: str) -> list[TimestampedTransform]:
+    transform_time_series = compute_transforms_time_series(record, {guid})
+    return transform_time_series.get(guid, {})
+
+
+def compute_transforms_time_series(record: Record, included_guids: set[str] = None) \
+        -> dict[str, list[TimestampedTransform]]:
+    result: dict[str, list[TimestampedTransform]] = {}
+    current_transforms: dict[str, Transform] = {}
+
+    creation_samples = groupby(record[transform_pb2.TransformCreate], lambda x: x.frame_number)
+    destruction_samples = groupby(record[transform_pb2.TransformDestroy], lambda x: x.frame_number)
+    update_samples = groupby(record[transform_pb2.TransformUpdate], lambda x: x.frame_number)
+
+    for frame in tqdm(record.frames_info, desc="Computing world positions"):
+
+        # Add newly created transforms
+        if frame.frame_number in creation_samples:
+            for creation_sample in creation_samples[frame.frame_number]:
+                guid = creation_sample.payload.id.component_id
+                if guid not in current_transforms:
+                    current_transforms[guid] = Transform(_guid=guid)
+
+        # Remove transforms that were destroyed in this frame
+        if frame.frame_number in destruction_samples:
+            for destruction_sample in destruction_samples[frame.frame_number]:
+                guid = destruction_sample.payload.id.component_id
+                if guid in current_transforms:
+                    del current_transforms[guid]
+
+        # Apply transform updates
+        if frame.frame_number in update_samples:
+            for update_sample in update_samples[frame.frame_number]:
+                guid = update_sample.payload.id.component_id
+                local_transform = current_transforms[guid]
+                if update_sample.payload.HasField('local_position'):
+                    local_position = update_sample.payload.local_position
+                    local_transform.set_local_position(np.array([local_position.x, local_position.y, local_position.z]))
+                if update_sample.payload.HasField('local_rotation'):
+                    local_rotation = update_sample.payload.local_rotation
+                    q = quaternion.quaternion(local_rotation.w, local_rotation.x, local_rotation.y, local_rotation.z)
+                    local_transform.set_local_rotation(q)
+                if update_sample.payload.HasField('local_scale'):
+                    local_scale = update_sample.payload.local_scale
+                    local_transform.set_local_scale(np.array([local_scale.x, local_scale.y, local_scale.z]))
+                if update_sample.payload.HasField('parent_transform_id'):
+                    parent_guid = update_sample.payload.parent_transform_id.component_id
+                    if parent_guid == "00000000000000000000000000000000":  # null guid
+                        local_transform.set_parent(None)
+                    elif parent_guid in current_transforms:
+                        local_transform.set_parent(current_transforms[parent_guid])
+                    else:
+                        parent = Transform(_guid=parent_guid)
+                        local_transform.set_parent(parent)
+                        current_transforms[parent_guid] = parent
+
+        if included_guids is None:
+            included_transforms = current_transforms.values()
+        else:
+            included_transforms = [current_transforms[guid] for guid in included_guids if guid in current_transforms]
+
+        for t in included_transforms:
+            timestamped_transform = TimestampedTransform(timestamp=frame.timestamp,
+                                                         frame_number=frame.frame_number,
+                                                         guid=t.get_guid(),
+                                                         parent_guid=t.get_parent().get_guid(),
+                                                         local_scale=t.get_local_scale(),
+                                                         local_position=t.get_local_position(),
+                                                         local_rotation=t.get_local_rotation(),
+                                                         local_to_world_mtx=t.get_local_to_world_matrix())
+            result[t.get_guid()].append(timestamped_transform)
+
+    return result
```

### Comparing `plume_python-0.1.8/README.md` & `plume_python-0.1.9/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-<a name="readme-top"></a>
-<div align="center">
-    <picture>
-        <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_banner_dark.png">
-        <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_banner_light.png">
-        <img alt="PLUME banner." src="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_banner_light.png">
-    </picture>
-    <br />
-    <br />
-    <p align="center">
-        <strong>PLUME: Record, Replay, Analyze and Share User Behavior in 6DoF XR Experiences</strong>
-        <br />
-        Charles Javerliat, Sophie Villenave, Pierre Raimbaud, Guillaume Lavoué
-        <br />
-        <em>(Journal Track) IEEE Conference on Virtual Reality and 3D User Interfaces</em>
-        <br />
-        <a href="https://www.youtube.com/watch?v=_6krSw7fNqg"><strong>Video »</strong><a>
-        <a href="https://hal.science/hal-04488824"><strong>Paper »</strong></a>
-        <a href="https://github.com/liris-xr/PLUME/wiki/"><strong>Explore the docs »</strong></a>
-        <br />
-        <br />
-        <a href="https://github.com/liris-xr/PLUME/issues">Report Bug</a>
-        ·
-        <a href="https://github.com/liris-xr/PLUME/issues">Request Feature</a>
-    </p>
-</div>
-
-<img alt="PLUME Python" src="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_python.png">
-
-<details>
-    <summary>Table of Contents</summary>
-    <ol>
-        <li><a href="#about-plume-python">About PLUME Python</a></li>
-        <li>
-            <a href="#getting-started">Getting Started</a>
-            <ul>
-                <li><a href="#prerequisites">Prerequisites</a></li>
-                <li><a href="#installation">Installation</a></li>
-                <li><a href="#usage">Usage</a></li>
-            </ul>
-        </li>
-        <li><a href="#customization">Customization</a></li>
-        <li><a href="#customization">Roadmap</a></li>
-        <li><a href="#contributing">Contributing</a></li>
-        <li><a href="#license">License</a></li>
-        <li><a href="#contact">Contact</a></li>
-        <li><a href="#citation">Citation</a></li>
-    </ol>
-</details>
-
-## About PLUME Python
-
-The interoperability of PLUME record files allows for other language to load those files for external analysis. PLUME
-Python is a module that can load record files using the Protobuf package to filter and convert the data into more
-commonly used formats in data analysis like pandas dataframe or CSV files. Embedded data such as LabStreamingLayer's
-samples can be exported to XDF files for external use in tools such as SigViewer, EEGLAB or MoBILAB.
-
-## Getting Started
-
-### Prerequisites
-
-* Python 3.10 or later
-* protobuf
-* pandas
-
-### Installation
-
-Download the latest release or clone the repository.
-
-### Usage
-
-Use the CLI to load and convert your records
-
-```
-python cli.py input_file output_dir --csv --xdf --descriptors [DESCRIPTORS ...]
-```
-
-* **input_file**: Input PLUME record file (.plm) to be converted.
-* **output_dir**: Output directory where all generated files will be saved. Directory will be created if it does not
-  exist.
-* **--csv**: Convert to CSV with optional filters.
-* **--xdf**: Convert markers and physiological signals to XDF .
-* **-descriptors**: Descriptor name used for filtering which samples to output as CSV files. Short name will
-  automatically be preprended (eg. TransformUpdate -> plume.sample.unity.TransformUpdate).
-
-## Customization
-
-If you have customized your PLUME Record as
-instructed <a href="https://github.com/liris-xr/PLUME-Recorder?tab=readme-ov-file#customisation">here</a>, import your
-generated protos for Python in the samples folder: `PLUME-Python/plume/samples`.
-
-## Roadmap
-
-See the [open issues](https://github.com/liris-xr/PLUME/issues) for a full list of proposed features (and known issues).
-
-## Contributing
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
-contributions you make are **greatly appreciated**.
-Don't forget to give the project a star! Thanks again!
-
-## License
-
-Distributed under the <a rel="license" href="https://github.com/liris-xr/PLUME-Python/blob/master/LICENSE">GPLv3
-License</a>.
-
-## Contact
-
-Charles JAVERLIAT - charles.javerliat@gmail.com
-
-Sophie VILLENAVE - sophie.villenave@ec-lyon.fr
-
-## Citation
-
-```
-@article{javerliat_plume_2024,
-	title = {{PLUME}: {Record}, {Replay}, {Analyze} and {Share} {User} {Behavior} in {6DoF} {XR} {Experiences}},
-	url = {https://ieeexplore.ieee.org/document/10458415},
-	doi = {10.1109/TVCG.2024.3372107},
-	journal = {IEEE Transactions on Visualization and Computer Graphics},
-	author = {Javerliat, Charles and Villenave, Sophie and Raimbaud, Pierre and Lavoué, Guillaume},
-	year = {2024},
-	note = {Conference Name: IEEE Transactions on Visualization and Computer Graphics},
-	pages = {1--11}
-}
+<a name="readme-top"></a>
+<div align="center">
+    <picture>
+        <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_banner_dark.png">
+        <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_banner_light.png">
+        <img alt="PLUME banner." src="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_banner_light.png">
+    </picture>
+    <br />
+    <br />
+    <p align="center">
+        <strong>PLUME: Record, Replay, Analyze and Share User Behavior in 6DoF XR Experiences</strong>
+        <br />
+        Charles Javerliat, Sophie Villenave, Pierre Raimbaud, Guillaume Lavoué
+        <br />
+        <em>(Journal Track) IEEE Conference on Virtual Reality and 3D User Interfaces</em>
+        <br />
+        <a href="https://www.youtube.com/watch?v=_6krSw7fNqg"><strong>Video »</strong><a>
+        <a href="https://hal.science/hal-04488824"><strong>Paper »</strong></a>
+        <a href="https://github.com/liris-xr/PLUME/wiki/"><strong>Explore the docs »</strong></a>
+        <br />
+        <br />
+        <a href="https://github.com/liris-xr/PLUME/issues">Report Bug</a>
+        ·
+        <a href="https://github.com/liris-xr/PLUME/issues">Request Feature</a>
+    </p>
+</div>
+
+<img alt="PLUME Python" src="https://raw.githubusercontent.com/liris-xr/PLUME-Python/master/Documentation%7E/Images/plume_python.png">
+
+<details>
+    <summary>Table of Contents</summary>
+    <ol>
+        <li><a href="#about-plume-python">About PLUME Python</a></li>
+        <li>
+            <a href="#getting-started">Getting Started</a>
+            <ul>
+                <li><a href="#prerequisites">Prerequisites</a></li>
+                <li><a href="#installation">Installation</a></li>
+                <li><a href="#usage">Usage</a></li>
+            </ul>
+        </li>
+        <li><a href="#customization">Customization</a></li>
+        <li><a href="#customization">Roadmap</a></li>
+        <li><a href="#contributing">Contributing</a></li>
+        <li><a href="#license">License</a></li>
+        <li><a href="#contact">Contact</a></li>
+        <li><a href="#citation">Citation</a></li>
+    </ol>
+</details>
+
+## About PLUME Python
+
+The interoperability of PLUME record files allows for other language to load those files for external analysis. PLUME
+Python is a module that can load record files using the Protobuf package to filter and convert the data into more
+commonly used formats in data analysis like pandas dataframe or CSV files. Embedded data such as LabStreamingLayer's
+samples can be exported to XDF files for external use in tools such as SigViewer, EEGLAB or MoBILAB.
+
+## Getting Started
+
+### Prerequisites
+
+* Python 3.10 or later
+* protobuf
+* pandas
+
+### Installation
+
+Download the latest release or clone the repository.
+
+### Usage
+
+Use the CLI to load and convert your records
+
+```
+python cli.py input_file output_dir --csv --xdf --descriptors [DESCRIPTORS ...]
+```
+
+* **input_file**: Input PLUME record file (.plm) to be converted.
+* **output_dir**: Output directory where all generated files will be saved. Directory will be created if it does not
+  exist.
+* **--csv**: Convert to CSV with optional filters.
+* **--xdf**: Convert markers and physiological signals to XDF .
+* **-descriptors**: Descriptor name used for filtering which samples to output as CSV files. Short name will
+  automatically be preprended (eg. TransformUpdate -> plume.sample.unity.TransformUpdate).
+
+## Customization
+
+If you have customized your PLUME Record as
+instructed <a href="https://github.com/liris-xr/PLUME-Recorder?tab=readme-ov-file#customisation">here</a>, import your
+generated protos for Python in the samples folder: `PLUME-Python/plume/samples`.
+
+## Roadmap
+
+See the [open issues](https://github.com/liris-xr/PLUME/issues) for a full list of proposed features (and known issues).
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
+contributions you make are **greatly appreciated**.
+Don't forget to give the project a star! Thanks again!
+
+## License
+
+Distributed under the <a rel="license" href="https://github.com/liris-xr/PLUME-Python/blob/master/LICENSE">GPLv3
+License</a>.
+
+## Contact
+
+Charles JAVERLIAT - charles.javerliat@gmail.com
+
+Sophie VILLENAVE - sophie.villenave@ec-lyon.fr
+
+## Citation
+
+```
+@article{javerliat_plume_2024,
+	title = {{PLUME}: {Record}, {Replay}, {Analyze} and {Share} {User} {Behavior} in {6DoF} {XR} {Experiences}},
+	url = {https://ieeexplore.ieee.org/document/10458415},
+	doi = {10.1109/TVCG.2024.3372107},
+	journal = {IEEE Transactions on Visualization and Computer Graphics},
+	author = {Javerliat, Charles and Villenave, Sophie and Raimbaud, Pierre and Lavoué, Guillaume},
+	year = {2024},
+	note = {Conference Name: IEEE Transactions on Visualization and Computer Graphics},
+	pages = {1--11}
+}
 ```
```

### Comparing `plume_python-0.1.8/PKG-INFO` & `plume_python-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plume-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Set of utilities to work with PLM record files.
 License: GPLv3
 Author: Charles JAVERLIAT
 Author-email: charles.javerliat@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plume-python Version: 0.1.8 Summary: Set of
+Metadata-Version: 2.1 Name: plume-python Version: 0.1.9 Summary: Set of
 utilities to work with PLM record files. License: GPLv3 Author: Charles
 JAVERLIAT Author-email: charles.javerliat@gmail.com Requires-Python:
 >=3.12,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.12 Requires-Dist: delimited-protobuf (>=1.0.0,<2.0.0) Requires-Dist: lz4
 (>=4.3.3,<5.0.0) Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: numpy-
 quaternion (>=2023.0.3,<2024.0.0) Requires-Dist: pandas (>=2.2.1,<3.0.0)
```

