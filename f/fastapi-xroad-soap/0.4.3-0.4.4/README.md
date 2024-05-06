# Comparing `tmp/fastapi_xroad_soap-0.4.3.tar.gz` & `tmp/fastapi_xroad_soap-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.4.3.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.4.4.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.4.3.tar` & `fastapi_xroad_soap-0.4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    13831 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/LICENSE
--rw-r--r--   0        0        0     6684 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/README.md
--rw-r--r--   0        0        0      524 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/__init__.py
--rw-r--r--   0        0        0      574 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/elements.py
--rw-r--r--   0        0        0      431 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/faults.py
--rw-r--r--   0        0        0      340 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/__init__.py
--rw-r--r--   0        0        0      666 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/__init__.py
--rw-r--r--   0        0        0     2953 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/base_element_spec.py
--rw-r--r--   0        0        0     1194 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/composite_meta.py
--rw-r--r--   0        0        0      988 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/dynamic_spec.py
--rw-r--r--   0        0        0     4392 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/message_body.py
--rw-r--r--   0        0        0     2705 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/validators.py
--rw-r--r--   0        0        0     1067 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/constants.py
--rw-r--r--   0        0        0      486 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/__init__.py
--rw-r--r--   0        0        0     1061 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/__init__.py
--rw-r--r--   0        0        0     1479 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/boolean.py
--rw-r--r--   0        0        0     1195 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/date.py
--rw-r--r--   0        0        0     1243 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/datetime.py
--rw-r--r--   0        0        0     1180 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/float.py
--rw-r--r--   0        0        0     1223 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/integer.py
--rw-r--r--   0        0        0     1247 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/netres.py
--rw-r--r--   0        0        0     1284 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/string.py
--rw-r--r--   0        0        0     6437 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/swaref.py
--rw-r--r--   0        0        0     1195 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/time.py
--rw-r--r--   0        0        0     2125 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
--rw-r--r--   0        0        0     2276 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/string_type_spec.py
--rw-r--r--   0        0        0     3767 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/validators.py
--rw-r--r--   0        0        0      679 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/factory.py
--rw-r--r--   0        0        0     1425 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/generics.py
--rw-r--r--   0        0        0     1912 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/header.py
--rw-r--r--   0        0        0     2020 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/file_size.py
--rw-r--r--   0        0        0      742 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/bodypart.py
--rw-r--r--   0        0        0     1898 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/decoder.py
--rw-r--r--   0        0        0     2493 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/encoder.py
--rw-r--r--   0        0        0     1020 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/errors.py
--rw-r--r--   0        0        0      955 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/__init__.py
--rw-r--r--   0        0        0     5257 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/action.py
--rw-r--r--   0        0        0     5223 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/faults.py
--rw-r--r--   0        0        0     1654 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/response.py
--rw-r--r--   0        0        0     5291 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.py
--rw-r--r--   0        0        0     2071 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.pyi
--rw-r--r--   0        0        0     2004 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/validators.py
--rw-r--r--   0        0        0     5172 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/storage.py
--rw-r--r--   0        0        0     3249 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/uid_gen.py
--rw-r--r--   0        0        0     1068 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/__init__.py
--rw-r--r--   0        0        0     3057 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/content_utils.py
--rw-r--r--   0        0        0     2673 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/path_utils.py
--rw-r--r--   0        0        0      851 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/route_utils.py
--rw-r--r--   0        0        0      397 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/__init__.py
--rw-r--r--   0        0        0     5381 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/generator.py
--rw-r--r--   0        0        0     4274 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/helpers.py
--rw-r--r--   0        0        0     2050 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/__init__.py
--rw-r--r--   0        0        0     2864 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/binding.py
--rw-r--r--   0        0        0     1270 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/conditions.py
--rw-r--r--   0        0        0     1360 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/definitions.py
--rw-r--r--   0        0        0     1698 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/port_type.py
--rw-r--r--   0        0        0     1315 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
--rw-r--r--   0        0        0     2139 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/schema.py
--rw-r--r--   0        0        0     1361 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/service.py
--rw-r--r--   0        0        0      561 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/utils.py
--rw-r--r--   0        0        0     2587 2024-05-02 11:13:55.607643 fastapi_xroad_soap-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    13831 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6684 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/README.md
+-rw-r--r--   0        0        0      524 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      431 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      666 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     2953 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/base_element_spec.py
+-rw-r--r--   0        0        0     1194 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/composite_meta.py
+-rw-r--r--   0        0        0      988 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/dynamic_spec.py
+-rw-r--r--   0        0        0     4392 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/message_body.py
+-rw-r--r--   0        0        0     2705 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/validators.py
+-rw-r--r--   0        0        0     1067 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0      486 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/boolean.py
+-rw-r--r--   0        0        0     1195 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/date.py
+-rw-r--r--   0        0        0     1243 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/datetime.py
+-rw-r--r--   0        0        0     1180 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/float.py
+-rw-r--r--   0        0        0     1223 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/integer.py
+-rw-r--r--   0        0        0     1247 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/netres.py
+-rw-r--r--   0        0        0     1284 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/string.py
+-rw-r--r--   0        0        0     6437 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/swaref.py
+-rw-r--r--   0        0        0     1195 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/time.py
+-rw-r--r--   0        0        0     2125 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
+-rw-r--r--   0        0        0     2276 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/string_type_spec.py
+-rw-r--r--   0        0        0     3767 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1425 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1912 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     2020 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      742 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     1898 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2493 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1020 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      955 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     5257 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     5223 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     1654 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     5632 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     2312 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     2004 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/validators.py
+-rw-r--r--   0        0        0     5172 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0     3249 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/uid_gen.py
+-rw-r--r--   0        0        0     1068 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     3057 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0      851 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0      397 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     5471 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     4274 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/helpers.py
+-rw-r--r--   0        0        0     2050 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/__init__.py
+-rw-r--r--   0        0        0     2864 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/binding.py
+-rw-r--r--   0        0        0     1270 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/conditions.py
+-rw-r--r--   0        0        0     1360 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/definitions.py
+-rw-r--r--   0        0        0     1698 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/port_type.py
+-rw-r--r--   0        0        0     1315 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
+-rw-r--r--   0        0        0     2139 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/schema.py
+-rw-r--r--   0        0        0     1361 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/service.py
+-rw-r--r--   0        0        0      561 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2587 2024-05-06 12:38:17.049684 fastapi_xroad_soap-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.4/PKG-INFO
```

### Comparing `fastapi_xroad_soap-0.4.3/LICENSE` & `fastapi_xroad_soap-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/README.md` & `fastapi_xroad_soap-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/elements.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/elements.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/base_element_spec.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/base_element_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/composite_meta.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/composite_meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/dynamic_spec.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/dynamic_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/message_body.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/message_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/validators.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/constants.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/boolean.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/boolean.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/date.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/date.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/datetime.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/datetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/float.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/float.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/integer.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/integer.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/netres.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/netres.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/string.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/string.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/swaref.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/swaref.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/time.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/time.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/numeric_type_spec.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/numeric_type_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/string_type_spec.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/string_type_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/validators.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/factory.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/factory.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/generics.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/header.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/header.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/file_size.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/file_size.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/bodypart.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/bodypart.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/decoder.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/encoder.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/errors.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/action.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/action.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/faults.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/faults.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/response.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/response.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import inspect
 import typing as t
 from pathlib import Path
 from lxml.etree import LxmlError
-from pydantic import ValidationError
+from pydantic import Field, ValidationError, validate_call
 from fastapi import FastAPI, Request, Response
 from fastapi.types import DecoratedCallable
 from starlette.types import Lifespan
 from starlette.middleware.base import BaseHTTPMiddleware
 from ..multipart import MultipartError
 from ..storage import GlobalWeakStorage
 from .. import utils, wsdl
@@ -30,27 +30,31 @@
 
 SoapMiddleware: t.TypeAlias = BaseHTTPMiddleware
 FuncOrCoro = t.Union[t.Callable[..., t.Any], t.Awaitable[t.Any]]
 ActionType = t.Callable[[DecoratedCallable], DecoratedCallable]
 
 
 class SoapService(FastAPI):
+	@validate_call
 	def __init__(
 			self,
 			*,
-			name: str = "SoapService",
-			path: str = "/service",
-			this_namespace: str = "https://example.org",
+			name: t.Annotated[str, Field(min_length=5)] = "SoapService",
+			path: t.Annotated[str, Field(min_length=1)] = "/service",
+			version: t.Annotated[int, Field(ge=1, le=99)] = 1,
+			this_namespace: t.Annotated[str, Field(min_length=5)] = "https://example.org",
 			wsdl_override: t.Optional[t.Union[str, Path]] = None,
 			lifespan: t.Optional[Lifespan[FastAPI]] = None,
 			fault_callback: t.Optional[t.Callable[[Request, Exception], None]] = None,
 			hide_ise_cause: bool = False,
 			debug: bool = False
 	) -> None:
 		self._name = name
+		self._path = path
+		self._version = version
 		self._tns = this_namespace
 		self._wsdl_response = None
 		self._wsdl_override = wsdl_override
 		self._fault_callback = fault_callback
 		self._hide_ise_cause = hide_ise_cause
 		self._storage = GlobalWeakStorage()
 		self._actions = dict()
@@ -73,15 +77,17 @@
 		app.add_middleware(
 			middleware_class=SoapMiddleware,
 			dispatch=self._soap_middleware
 		)
 
 	async def _soap_middleware(self, http_request: Request, _: t.Callable) -> t.Optional[Response]:
 		try:
-			if "wsdl" in http_request.query_params:
+			if http_request.url.path != self._path:
+				return Response(status_code=404)
+			elif "wsdl" in http_request.query_params:
 				if self._wsdl_response is None:
 					self.regenerate_wsdl()
 				return self._wsdl_response
 			elif http_request.method != "POST":
 				raise f.InvalidMethodFault(http_request.method)
 			action = self._determine_action(http_request)
 
@@ -161,10 +167,11 @@
 				"SoapService has wsdl_override argument set."
 			)
 		self._wsdl_response = Response(
 			media_type="text/xml",
 			content=wsdl.generate(
 				self._actions,
 				self._name,
-				self._tns
+				self._tns,
+				self._version
 			)
 		)
```

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.pyi` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #   The contents of this file are subject to the terms and conditions defined in the License.
 #   You may not use, modify, or distribute this file except in compliance with the License.
 #
 #   SPDX-License-Identifier: EUPL-1.2
 #
 import typing as t
 from pathlib import Path
+from pydantic import Field, validate_call
 from fastapi.types import DecoratedCallable
 from starlette.types import Scope, Receive, Send, Lifespan
 from fastapi import Request, Response, FastAPI as ASGIApp
 from ..storage import GlobalWeakStorage
 from .action import SoapAction
 
 
@@ -22,28 +23,32 @@
 
 class FastAPI:
 	def __call__(self, scope: Scope, receive: Receive, send: Send) -> t.Awaitable[None]: ...
 
 
 class SoapService(FastAPI):
 	_name: str
+	_path: str
+	_version: int
 	_tns: str
 	_wsdl_response: t.Union[Response, None]
 	_wsdl_override: t.Optional[t.Union[str, Path]]
 	_fault_callback: t.Optional[t.Callable[[Request, Exception], None]] = None
 	_hide_ise_cause: bool = False
 	_storage: GlobalWeakStorage
 	_actions: dict[str, SoapAction]
 
+	@validate_call
 	def __init__(
 			self,
 			*,
-			name: str = "SoapService",
-			path: str = "/service",
-			this_namespace: str = "https://example.org",
+			name: t.Annotated[str, Field(min_length=5)] = "SoapService",
+			path: t.Annotated[str, Field(min_length=1)] = "/service",
+			version: t.Annotated[int, Field(ge=1, le=99)] = 1,
+			this_namespace: t.Annotated[str, Field(min_length=5)] = "https://example.org",
 			wsdl_override: t.Optional[t.Union[str, Path]] = None,
 			lifespan: t.Optional[Lifespan[FastAPI]] = None,
 			fault_callback: t.Optional[t.Callable[[Request, Exception], None]] = None,
 			hide_ise_cause: bool = False
 	) -> None: ...
 
 	async def _soap_middleware(self, http_request: Request, _: t.Callable) -> t.Optional[Response]: ...
```

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/validators.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/storage.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/uid_gen.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/uid_gen.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/content_utils.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/content_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/path_utils.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/route_utils.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/route_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/generator.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ..elements.models import SwaRefSpec
 from . import helpers, models as mod
 
 
 __all__ = ["generate"]
 
 
-def generate(actions: t.Dict[str, SoapAction], name: str, tns: str) -> bytes:
+def generate(actions: t.Dict[str, SoapAction], name: str, tns: str, version: int) -> bytes:
 	wsdl_def = type(
 		"WSDLDefinitions", (mod.WSDLDefinitions,),
 		{}, nsmap={**WSDL_NSMAP, "tns": tns}
 	)
 	wsdl_data: str = wsdl_def(
 		target_ns=tns,
 		name=name,
@@ -35,15 +35,15 @@
 				imports=_generate_imports(actions),
 				elements=_generate_elements(actions),
 				**_generate_types(actions)
 			)
 		),
 		messages=_generate_messages(actions),
 		port_type=_generate_port_type(actions),
-		binding=_generate_binding(actions),
+		binding=_generate_binding(actions, version),
 		service=mod.WSDLService(
 			port=mod.WSDLPortBinding(
 				address=mod.SOAPAddress()
 			)
 		)
 	).to_xml(pretty_print=True).decode()
 	return helpers.format_wsdl_definitions(wsdl_data)
@@ -186,20 +186,21 @@
 			input=port_input,
 			output=port_output,
 			name=name
 		))
 	return mod.WSDLPortType(operations=ops)
 
 
-def _generate_binding(actions: t.Dict[str, SoapAction]) -> mod.WSDLBinding:
+def _generate_binding(actions: t.Dict[str, SoapAction], version: int) -> mod.WSDLBinding:
 	return mod.WSDLBinding(
 		binding=mod.SOAPBinding(),
 		operations=[
 			mod.WSDLOperationBinding(
 				name=key,
 				operation=mod.SOAPOperationBinding(
 					soap_action=key
-				)
+				),
+				version=mod.XROADVersion(version=f"v{version}")
 			)
 			for key in actions.keys()
 		]
 	)
```

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/helpers.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/__init__.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/binding.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/binding.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/conditions.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/conditions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/definitions.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/definitions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/port_type.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/port_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/restrictions.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/restrictions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/schema.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/service.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/utils.py` & `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.3/pyproject.toml` & `fastapi_xroad_soap-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-xroad-soap"
-version = "0.4.3"
+version = "0.4.4"
 description = "FastAPI Extension for X-Road SOAP"
 authors = ["Zero Reports Team <zero.dev@rik.ee>"]
 license = "EUPL-1.2"
 readme = "README.md"
 keywords = ["fastapi", "xroad", "soap"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `fastapi_xroad_soap-0.4.3/PKG-INFO` & `fastapi_xroad_soap-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xroad-soap
-Version: 0.4.3
+Version: 0.4.4
 Summary: FastAPI Extension for X-Road SOAP
 License: EUPL-1.2
 Keywords: fastapi,xroad,soap
 Author: Zero Reports Team
 Author-email: zero.dev@rik.ee
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

