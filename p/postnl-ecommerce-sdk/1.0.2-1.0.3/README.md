# Comparing `tmp/postnl_ecommerce_sdk-1.0.2.tar.gz` & `tmp/postnl_ecommerce_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnl_ecommerce_sdk-1.0.2.tar", last modified: Wed May  1 14:28:03 2024, max compression
+gzip compressed data, was "postnl_ecommerce_sdk-1.0.3.tar", last modified: Mon May  6 10:07:05 2024, max compression
```

## Comparing `postnl_ecommerce_sdk-1.0.2.tar` & `postnl_ecommerce_sdk-1.0.3.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.923831 postnl_ecommerce_sdk-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1213 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6994 2024-05-01 14:28:03.922831 postnl_ecommerce_sdk-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6477 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.921831 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6994 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7025 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-01 14:28:03.000000 postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.817830 postnl_ecommerce_sdk-1.0.2/postnlecommerce/
--rw-r--r--   0 root         (0) root         (0)      153 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/__init__.py
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     6068 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.827830 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/
--rw-r--r--   0 root         (0) root         (0)      342 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5194 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/barcode_controller.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     3352 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/checkout_controller.py
--rw-r--r--   0 root         (0) root         (0)     3381 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/confirming_controller.py
--rw-r--r--   0 root         (0) root         (0)    16940 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/deliverydate_controller.py
--rw-r--r--   0 root         (0) root         (0)     3886 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/labelling_controller.py
--rw-r--r--   0 root         (0) root         (0)    18238 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/locations_controller.py
--rw-r--r--   0 root         (0) root         (0)     4107 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/postalcode_check_controller.py
--rw-r--r--   0 root         (0) root         (0)     3915 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipment_controller.py
--rw-r--r--   0 root         (0) root         (0)    14089 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipping_status_controller.py
--rw-r--r--   0 root         (0) root         (0)     6428 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/timeframes_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.835831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_error_exception.py
--rw-r--r--   0 root         (0) root         (0)     1555 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_too_many_request_exception.py
--rw-r--r--   0 root         (0) root         (0)     1683 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/checkout_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/confirming_response_error_1_exception.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1565 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/labelling_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/locations_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/timeframe_response_invalid_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.839830 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/
--rw-r--r--   0 root         (0) root         (0)      118 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.840831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/custom_header_authentication.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1877 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1498 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.919831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/
--rw-r--r--   0 root         (0) root         (0)     2632 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3612 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address.py
--rw-r--r--   0 root         (0) root         (0)     3503 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_1.py
--rw-r--r--   0 root         (0) root         (0)     8750 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_11.py
--rw-r--r--   0 root         (0) root         (0)     8667 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_2.py
--rw-r--r--   0 root         (0) root         (0)     3871 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_3.py
--rw-r--r--   0 root         (0) root         (0)     6698 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_4.py
--rw-r--r--   0 root         (0) root         (0)      498 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount.py
--rw-r--r--   0 root         (0) root         (0)     2153 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount_1.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4678 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_request.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_response.py
--rw-r--r--   0 root         (0) root         (0)      567 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/code_enum.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/complete_status.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_request.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_response.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/contact.py
--rw-r--r--   0 root         (0) root         (0)     3572 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content.py
--rw-r--r--   0 root         (0) root         (0)     3507 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content_1.py
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/countrycode_enum.py
--rw-r--r--   0 root         (0) root         (0)     3312 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cpc_response.py
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/currency_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      576 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/currency_enum.py
--rw-r--r--   0 root         (0) root         (0)     1835 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/current_status.py
--rw-r--r--   0 root         (0) root         (0)     9549 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/custom.py
--rw-r--r--   0 root         (0) root         (0)     3986 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     3940 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_1.py
--rw-r--r--   0 root         (0) root         (0)     2421 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_2.py
--rw-r--r--   0 root         (0) root         (0)     2772 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cut_off_time.py
--rw-r--r--   0 root         (0) root         (0)      974 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/day_enum.py
--rw-r--r--   0 root         (0) root         (0)     2237 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_option.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_options.py
--rw-r--r--   0 root         (0) root         (0)      509 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_options_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/detail.py
--rw-r--r--   0 root         (0) root         (0)     3549 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension_1.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_1.py
--rw-r--r--   0 root         (0) root         (0)     1927 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_2.py
--rw-r--r--   0 root         (0) root         (0)     2247 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_3.py
--rw-r--r--   0 root         (0) root         (0)     2237 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_4.py
--rw-r--r--   0 root         (0) root         (0)     4040 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/event.py
--rw-r--r--   0 root         (0) root         (0)     1936 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/expectation.py
--rw-r--r--   0 root         (0) root         (0)     1876 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/extra_field.py
--rw-r--r--   0 root         (0) root         (0)     2051 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/fault.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday_1.py
--rw-r--r--   0 root         (0) root         (0)     1952 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result_1.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/group.py
--rw-r--r--   0 root         (0) root         (0)     6355 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/hazardous_material.py
--rw-r--r--   0 root         (0) root         (0)     2432 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label.py
--rw-r--r--   0 root         (0) root         (0)     2501 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label_1.py
--rw-r--r--   0 root         (0) root         (0)     3412 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_request.py
--rw-r--r--   0 root         (0) root         (0)     2793 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response_1.py
--rw-r--r--   0 root         (0) root         (0)      602 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/language_enum.py
--rw-r--r--   0 root         (0) root         (0)     4602 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location.py
--rw-r--r--   0 root         (0) root         (0)     6617 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_1.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_response.py
--rw-r--r--   0 root         (0) root         (0)     1915 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/locations_response.py
--rw-r--r--   0 root         (0) root         (0)     2130 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/merged_label.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message.py
--rw-r--r--   0 root         (0) root         (0)     2335 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message_1.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday_1.py
--rw-r--r--   0 root         (0) root         (0)     3301 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/old_status.py
--rw-r--r--   0 root         (0) root         (0)     4332 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/opening_hours.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      811 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_3_enum.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_enum.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options_2_enum.py
--rw-r--r--   0 root         (0) root         (0)     3155 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/pickup_option.py
--rw-r--r--   0 root         (0) root         (0)     2011 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option.py
--rw-r--r--   0 root         (0) root         (0)     2177 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option_1.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_options.py
--rw-r--r--   0 root         (0) root         (0)     3388 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframe.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframes.py
--rw-r--r--   0 root         (0) root         (0)     2795 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment.py
--rw-r--r--   0 root         (0) root         (0)     3281 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_1.py
--rw-r--r--   0 root         (0) root         (0)     3276 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_2.py
--rw-r--r--   0 root         (0) root         (0)     1855 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday.py
--rw-r--r--   0 root         (0) root         (0)     1584 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday_1.py
--rw-r--r--   0 root         (0) root         (0)    18276 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment.py
--rw-r--r--   0 root         (0) root         (0)    18866 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_1.py
--rw-r--r--   0 root         (0) root         (0)     7281 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_11.py
--rw-r--r--   0 root         (0) root         (0)     9494 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_2.py
--rw-r--r--   0 root         (0) root         (0)      946 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     3025 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py
--rw-r--r--   0 root         (0) root         (0)     3067 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response.py
--rw-r--r--   0 root         (0) root         (0)     2231 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_signature.py
--rw-r--r--   0 root         (0) root         (0)     3451 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_updated_shipment.py
--rw-r--r--   0 root         (0) root         (0)     2547 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/signature.py
--rw-r--r--   0 root         (0) root         (0)     3380 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status.py
--rw-r--r--   0 root         (0) root         (0)     3360 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status_2.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      809 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_enum.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday_1.py
--rw-r--r--   0 root         (0) root         (0)     2066 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sustainability.py
--rw-r--r--   0 root         (0) root         (0)     1855 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday.py
--rw-r--r--   0 root         (0) root         (0)     1584 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday_1.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe.py
--rw-r--r--   0 root         (0) root         (0)     2052 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_1.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_response.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_timeframe.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes_1.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday_1.py
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      850 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2889 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning.py
--rw-r--r--   0 root         (0) root         (0)     2020 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_1.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_11.py
--rw-r--r--   0 root         (0) root         (0)     1885 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_2.py
--rw-r--r--   0 root         (0) root         (0)     1688 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warnings.py
--rw-r--r--   0 root         (0) root         (0)     1858 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday.py
--rw-r--r--   0 root         (0) root         (0)     1587 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday_1.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/postnlecommerce_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 14:28:03.921831 postnl_ecommerce_sdk-1.0.2/postnlecommerce/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/postnlecommerce/utilities/file_wrapper.py
--rw-r--r--   0 root         (0) root         (0)      732 2024-05-01 14:27:37.000000 postnl_ecommerce_sdk-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2024-05-01 14:28:03.924831 postnl_ecommerce_sdk-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.410503 postnl_ecommerce_sdk-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6994 2024-05-06 10:07:05.410503 postnl_ecommerce_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6477 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.409504 postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6994 2024-05-06 10:07:05.000000 postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7025 2024-05-06 10:07:05.000000 postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 10:07:05.000000 postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-05-06 10:07:05.000000 postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-06 10:07:05.000000 postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.342503 postnl_ecommerce_sdk-1.0.3/postnlecommerce/
+-rw-r--r--   0 root         (0) root         (0)      153 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.347503 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/
+-rw-r--r--   0 root         (0) root         (0)      342 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5203 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/barcode_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/checkout_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/confirming_controller.py
+-rw-r--r--   0 root         (0) root         (0)    16940 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/deliverydate_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/labelling_controller.py
+-rw-r--r--   0 root         (0) root         (0)    18238 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/locations_controller.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/postalcode_check_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/shipment_controller.py
+-rw-r--r--   0 root         (0) root         (0)    14089 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/shipping_status_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/timeframes_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.351503 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_response_error_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_too_many_request_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/checkout_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/confirming_response_error_1_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/labelling_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/locations_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/timeframe_response_invalid_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.354503 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.355503 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/auth/custom_header_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.408503 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     3503 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_1.py
+-rw-r--r--   0 root         (0) root         (0)     8824 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_11.py
+-rw-r--r--   0 root         (0) root         (0)     8677 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_2.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_3.py
+-rw-r--r--   0 root         (0) root         (0)     6698 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_4.py
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/amount.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/amount_1.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     4678 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/checkout_request.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/checkout_response.py
+-rw-r--r--   0 root         (0) root         (0)      567 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/code_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/complete_status.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/confirming_request.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/confirming_response.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/contact.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/content.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/content_1.py
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/countrycode_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/cpc_response.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/currency_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      576 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/currency_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/current_status.py
+-rw-r--r--   0 root         (0) root         (0)     9651 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/custom.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/customer_1.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/customer_2.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/cut_off_time.py
+-rw-r--r--   0 root         (0) root         (0)      974 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/day_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/delivery_option.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/delivery_options.py
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/delivery_options_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/dimension.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/dimension_1.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_1.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_2.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_3.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_4.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/event.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/expectation.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/extra_field.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/fault.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/friday.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/friday_1.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/get_locations_result.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/get_locations_result_1.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     6355 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/hazardous_material.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/label.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/label_1.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/labelling_request.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/labelling_response.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/labelling_response_1.py
+-rw-r--r--   0 root         (0) root         (0)      602 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/language_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/location_1.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/locations_response.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/merged_label.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/message_1.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/monday.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/monday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/old_status.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/opening_hours.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      811 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_3_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/options.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/options_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/pickup_option.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/product_option.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/product_option_1.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/product_options.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/reason_no_timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/reason_no_timeframes.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/response_shipment.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/response_shipment_1.py
+-rw-r--r--   0 root         (0) root         (0)     3340 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/response_shipment_2.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/saturday.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/saturday_1.py
+-rw-r--r--   0 root         (0) root         (0)    18604 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment.py
+-rw-r--r--   0 root         (0) root         (0)    19193 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_1.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_11.py
+-rw-r--r--   0 root         (0) root         (0)     9678 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_2.py
+-rw-r--r--   0 root         (0) root         (0)      946 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shippingstatus_response.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shippingstatus_response_signature.py
+-rw-r--r--   0 root         (0) root         (0)     3495 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shippingstatus_response_updated_shipment.py
+-rw-r--r--   0 root         (0) root         (0)     2547 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/signature.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/status.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/status_2.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/string_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      809 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/string_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/sunday.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/sunday_1.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/sustainability.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/thursday.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/thursday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe_1.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe_response.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe_timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframes.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframes_1.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/tuesday.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/tuesday_1.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/type_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      850 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning_1.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning_11.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning_2.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/wednesday.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/wednesday_1.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/postnlecommerce_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 10:07:05.409504 postnl_ecommerce_sdk-1.0.3/postnlecommerce/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/postnlecommerce/utilities/file_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-06 10:06:48.000000 postnl_ecommerce_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-06 10:07:05.411503 postnl_ecommerce_sdk-1.0.3/setup.cfg
```

### Comparing `postnl_ecommerce_sdk-1.0.2/LICENSE` & `postnl_ecommerce_sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/PKG-INFO` & `postnl_ecommerce_sdk-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnl-ecommerce-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collection of PostNL API's for ecommerce processes.
 Author-email: PostNL <apimatic@postnl.nl>
 Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,49 +25,49 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-ecommerce-sdk==1.0.2
+pip install postnl-ecommerce-sdk==1.0.3
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2
+https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.3
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION_SERVER`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
 | `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
 | `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
 | `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 3** |
 | `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential object for Custom Header Signature |
+| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md) | The credential object for Custom Header Signature |
 
 The API client can be initialized as follows:
 
 ```python
 client = PostnlecommerceClient(
     custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials(
         apikey='apikey'
@@ -98,28 +98,28 @@
 | Production server | **Default** Production server |
 | Non-Production server | Sandbox environment for testing |
 
 ## Authorization
 
 This API uses the following authentication schemes.
 
-* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md)
+* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md)
 
 ## List of APIs
 
-* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/postalcodecheck.md)
-* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/barcode.md)
-* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/checkout.md)
-* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/confirming.md)
-* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/deliverydate.md)
-* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/labelling.md)
-* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/locations.md)
-* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipment.md)
-* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipping-status.md)
-* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md)
+* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/postalcodecheck.md)
+* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/barcode.md)
+* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/checkout.md)
+* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/confirming.md)
+* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/deliverydate.md)
+* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/labelling.md)
+* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/locations.md)
+* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/shipment.md)
+* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/shipping-status.md)
+* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/timeframes.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-response.md)
-* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-request.md)
+* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-response.md)
+* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-request.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.3 Summary:
 Collection of PostNL API's for ecommerce processes. Author-email: PostNL
 postnl.nl> Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: apimatic-core~=0.2.0
 Requires-Dist: apimatic-core-interfaces~=0.1.0 Requires-Dist: apimatic-
 requests-client-adapter~=0.1.0 Requires-Dist: enum34>=1.1.10,~=1.1 Provides-
 Extra: testutils Requires-Dist: pytest>=7.2.2; extra == "testutils" # Getting
@@ -21,22 +21,22 @@
 the solution.
 Contact our integrations team to have your test calls reviewed and gain access
 to our API production environment. Once everything is configured and validated,
 you'll be ready to go live and start using the PostNL service.
 For help contact us via our support form: _N_e_e_d_ _h_e_l_p_?_ _S_u_b_m_i_t_ _a_ _c_a_s_e_ _|_ _P_o_s_t_N_L.
 ## Install the Package The package is compatible with Python versions `3 >=3.7,
 <= 3.11`. Install the package from PyPi using the following pip command:
-```python pip install postnl-ecommerce-sdk==1.0.2 ``` You can also view the
-package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2 ## Test the
+```python pip install postnl-ecommerce-sdk==1.0.3 ``` You can also view the
+package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.3 ## Test the
 SDK You can test the generated SDK and the server with test cases. `unittest`
 is used as the testing framework and `pytest` is used as the test runner. You
 can run the tests as follows: Navigate to the root directory of the SDK and run
 the following commands ``` pip install -r test-requirements.txt pytest ``` ##
 Initialize the API Client **_Note:_** Documentation for the client can be found
-[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/
+[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/
 doc/client.md) The following parameters are configurable for the API Client: |
 Parameter | Type | Description | | --- | --- | --- | | `environment` |
 `Environment` | The API environment.
 **Default: `Environment.PRODUCTION_SERVER`** | | `http_client_instance` |
 `HttpClient` | The Http Client passed from the sdk user for making requests | |
 `override_http_client_configuration` | `bool` | The value which determines to
 override properties of the passed Http Client from the sdk user | |
@@ -50,16 +50,16 @@
 **Default: 2** | | `retry_statuses` | `Array of int` | The http statuses on
 which retry is to be done.
 **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** | |
 `retry_methods` | `Array of string` | The http methods on which retry is to be
 done.
 **Default: ['GET', 'PUT']** | | `custom_header_authentication_credentials` |
 [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential
+ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-
+ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md) | The credential
 object for Custom Header Signature | The API client can be initialized as
 follows: ```python client = PostnlecommerceClient
 (
 custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials
 ( apikey='apikey' ) ) ``` API calls return an `ApiResponse` object that
 includes the following fields: | Field | Description | | --- | --- | |
 `status_code` | Status code of the HTTP response | | `reason_phrase` | Reason
@@ -68,30 +68,30 @@
 | HTTP request info | | `errors` | Errors, if they exist | | `body` | The
 deserialized body of the HTTP response | ## Environments The SDK can be
 configured to use a different environment for making API calls. Available
 environments are: ### Fields | Name | Description | | --- | --- | | Production
 server | **Default** Production server | | Non-Production server | Sandbox
 environment for testing | ## Authorization This API uses the following
 authentication schemes. * [`APIKeyHeader (Custom Header Signature)`](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-
 signature.md) ## List of APIs * [Postalcodecheck](https://www.github.com/
-postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 postalcodecheck.md) * [Barcode](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/controllers/barcode.md) * [Checkout](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+sdk-python/tree/1.0.3/doc/controllers/barcode.md) * [Checkout](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 checkout.md) * [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.2/doc/controllers/confirming.md) * [Deliverydate](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+python/tree/1.0.3/doc/controllers/confirming.md) * [Deliverydate](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 deliverydate.md) * [Labelling](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/controllers/labelling.md) * [Locations](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+sdk-python/tree/1.0.3/doc/controllers/labelling.md) * [Locations](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 locations.md) * [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.2/doc/controllers/shipment.md) * [Shipping Status](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+python/tree/1.0.3/doc/controllers/shipment.md) * [Shipping Status](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 shipping-status.md) * [Timeframes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md) ## Classes
+ecommerce-sdk-python/tree/1.0.3/doc/controllers/timeframes.md) ## Classes
 Documentation * [Utility Classes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md) * [HttpResponse](https:
-//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-
+ecommerce-sdk-python/tree/1.0.3/doc/utility-classes.md) * [HttpResponse](https:
+//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-
 response.md) * [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/http-request.md)
+sdk-python/tree/1.0.3/doc/http-request.md)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/README.md` & `postnl_ecommerce_sdk-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-ecommerce-sdk==1.0.2
+pip install postnl-ecommerce-sdk==1.0.3
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2
+https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.3
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION_SERVER`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
 | `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
 | `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
 | `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 3** |
 | `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential object for Custom Header Signature |
+| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md) | The credential object for Custom Header Signature |
 
 The API client can be initialized as follows:
 
 ```python
 client = PostnlecommerceClient(
     custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials(
         apikey='apikey'
@@ -81,28 +81,28 @@
 | Production server | **Default** Production server |
 | Non-Production server | Sandbox environment for testing |
 
 ## Authorization
 
 This API uses the following authentication schemes.
 
-* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md)
+* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md)
 
 ## List of APIs
 
-* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/postalcodecheck.md)
-* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/barcode.md)
-* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/checkout.md)
-* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/confirming.md)
-* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/deliverydate.md)
-* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/labelling.md)
-* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/locations.md)
-* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipment.md)
-* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipping-status.md)
-* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md)
+* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/postalcodecheck.md)
+* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/barcode.md)
+* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/checkout.md)
+* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/confirming.md)
+* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/deliverydate.md)
+* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/labelling.md)
+* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/locations.md)
+* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/shipment.md)
+* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/shipping-status.md)
+* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/timeframes.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-response.md)
-* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-request.md)
+* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-response.md)
+* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-request.md)
```

#### html2text {}

```diff
@@ -13,22 +13,22 @@
 the solution.
 Contact our integrations team to have your test calls reviewed and gain access
 to our API production environment. Once everything is configured and validated,
 you'll be ready to go live and start using the PostNL service.
 For help contact us via our support form: _N_e_e_d_ _h_e_l_p_?_ _S_u_b_m_i_t_ _a_ _c_a_s_e_ _|_ _P_o_s_t_N_L.
 ## Install the Package The package is compatible with Python versions `3 >=3.7,
 <= 3.11`. Install the package from PyPi using the following pip command:
-```python pip install postnl-ecommerce-sdk==1.0.2 ``` You can also view the
-package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2 ## Test the
+```python pip install postnl-ecommerce-sdk==1.0.3 ``` You can also view the
+package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.3 ## Test the
 SDK You can test the generated SDK and the server with test cases. `unittest`
 is used as the testing framework and `pytest` is used as the test runner. You
 can run the tests as follows: Navigate to the root directory of the SDK and run
 the following commands ``` pip install -r test-requirements.txt pytest ``` ##
 Initialize the API Client **_Note:_** Documentation for the client can be found
-[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/
+[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/
 doc/client.md) The following parameters are configurable for the API Client: |
 Parameter | Type | Description | | --- | --- | --- | | `environment` |
 `Environment` | The API environment.
 **Default: `Environment.PRODUCTION_SERVER`** | | `http_client_instance` |
 `HttpClient` | The Http Client passed from the sdk user for making requests | |
 `override_http_client_configuration` | `bool` | The value which determines to
 override properties of the passed Http Client from the sdk user | |
@@ -42,16 +42,16 @@
 **Default: 2** | | `retry_statuses` | `Array of int` | The http statuses on
 which retry is to be done.
 **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** | |
 `retry_methods` | `Array of string` | The http methods on which retry is to be
 done.
 **Default: ['GET', 'PUT']** | | `custom_header_authentication_credentials` |
 [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential
+ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-
+ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md) | The credential
 object for Custom Header Signature | The API client can be initialized as
 follows: ```python client = PostnlecommerceClient
 (
 custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials
 ( apikey='apikey' ) ) ``` API calls return an `ApiResponse` object that
 includes the following fields: | Field | Description | | --- | --- | |
 `status_code` | Status code of the HTTP response | | `reason_phrase` | Reason
@@ -60,30 +60,30 @@
 | HTTP request info | | `errors` | Errors, if they exist | | `body` | The
 deserialized body of the HTTP response | ## Environments The SDK can be
 configured to use a different environment for making API calls. Available
 environments are: ### Fields | Name | Description | | --- | --- | | Production
 server | **Default** Production server | | Non-Production server | Sandbox
 environment for testing | ## Authorization This API uses the following
 authentication schemes. * [`APIKeyHeader (Custom Header Signature)`](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-
 signature.md) ## List of APIs * [Postalcodecheck](https://www.github.com/
-postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 postalcodecheck.md) * [Barcode](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/controllers/barcode.md) * [Checkout](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+sdk-python/tree/1.0.3/doc/controllers/barcode.md) * [Checkout](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 checkout.md) * [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.2/doc/controllers/confirming.md) * [Deliverydate](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+python/tree/1.0.3/doc/controllers/confirming.md) * [Deliverydate](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 deliverydate.md) * [Labelling](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/controllers/labelling.md) * [Locations](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+sdk-python/tree/1.0.3/doc/controllers/labelling.md) * [Locations](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 locations.md) * [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.2/doc/controllers/shipment.md) * [Shipping Status](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+python/tree/1.0.3/doc/controllers/shipment.md) * [Shipping Status](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 shipping-status.md) * [Timeframes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md) ## Classes
+ecommerce-sdk-python/tree/1.0.3/doc/controllers/timeframes.md) ## Classes
 Documentation * [Utility Classes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md) * [HttpResponse](https:
-//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-
+ecommerce-sdk-python/tree/1.0.3/doc/utility-classes.md) * [HttpResponse](https:
+//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-
 response.md) * [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/http-request.md)
+sdk-python/tree/1.0.3/doc/http-request.md)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/PKG-INFO` & `postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnl-ecommerce-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collection of PostNL API's for ecommerce processes.
 Author-email: PostNL <apimatic@postnl.nl>
 Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,49 +25,49 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-ecommerce-sdk==1.0.2
+pip install postnl-ecommerce-sdk==1.0.3
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2
+https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.3
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION_SERVER`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
 | `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
 | `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
 | `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
 | `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 3** |
 | `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
 | `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
 | `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential object for Custom Header Signature |
+| `custom_header_authentication_credentials` | [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md) | The credential object for Custom Header Signature |
 
 The API client can be initialized as follows:
 
 ```python
 client = PostnlecommerceClient(
     custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials(
         apikey='apikey'
@@ -98,28 +98,28 @@
 | Production server | **Default** Production server |
 | Non-Production server | Sandbox environment for testing |
 
 ## Authorization
 
 This API uses the following authentication schemes.
 
-* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md)
+* [`APIKeyHeader (Custom Header Signature)`](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md)
 
 ## List of APIs
 
-* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/postalcodecheck.md)
-* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/barcode.md)
-* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/checkout.md)
-* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/confirming.md)
-* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/deliverydate.md)
-* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/labelling.md)
-* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/locations.md)
-* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipment.md)
-* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/shipping-status.md)
-* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md)
+* [Postalcodecheck](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/postalcodecheck.md)
+* [Barcode](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/barcode.md)
+* [Checkout](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/checkout.md)
+* [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/confirming.md)
+* [Deliverydate](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/deliverydate.md)
+* [Labelling](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/labelling.md)
+* [Locations](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/locations.md)
+* [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/shipment.md)
+* [Shipping Status](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/shipping-status.md)
+* [Timeframes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/timeframes.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-response.md)
-* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-request.md)
+* [Utility Classes](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-response.md)
+* [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-request.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: postnl-ecommerce-sdk Version: 1.0.3 Summary:
 Collection of PostNL API's for ecommerce processes. Author-email: PostNL
 postnl.nl> Project-URL: Documentation, https://developer.postnl.nl/docs
 Keywords: PostNL,SDK,API,ecommerce Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: apimatic-core~=0.2.0
 Requires-Dist: apimatic-core-interfaces~=0.1.0 Requires-Dist: apimatic-
 requests-client-adapter~=0.1.0 Requires-Dist: enum34>=1.1.10,~=1.1 Provides-
 Extra: testutils Requires-Dist: pytest>=7.2.2; extra == "testutils" # Getting
@@ -21,22 +21,22 @@
 the solution.
 Contact our integrations team to have your test calls reviewed and gain access
 to our API production environment. Once everything is configured and validated,
 you'll be ready to go live and start using the PostNL service.
 For help contact us via our support form: _N_e_e_d_ _h_e_l_p_?_ _S_u_b_m_i_t_ _a_ _c_a_s_e_ _|_ _P_o_s_t_N_L.
 ## Install the Package The package is compatible with Python versions `3 >=3.7,
 <= 3.11`. Install the package from PyPi using the following pip command:
-```python pip install postnl-ecommerce-sdk==1.0.2 ``` You can also view the
-package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.2 ## Test the
+```python pip install postnl-ecommerce-sdk==1.0.3 ``` You can also view the
+package at: https://pypi.python.org/pypi/postnl-ecommerce-sdk/1.0.3 ## Test the
 SDK You can test the generated SDK and the server with test cases. `unittest`
 is used as the testing framework and `pytest` is used as the test runner. You
 can run the tests as follows: Navigate to the root directory of the SDK and run
 the following commands ``` pip install -r test-requirements.txt pytest ``` ##
 Initialize the API Client **_Note:_** Documentation for the client can be found
-[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/
+[here.](https://www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/
 doc/client.md) The following parameters are configurable for the API Client: |
 Parameter | Type | Description | | --- | --- | --- | | `environment` |
 `Environment` | The API environment.
 **Default: `Environment.PRODUCTION_SERVER`** | | `http_client_instance` |
 `HttpClient` | The Http Client passed from the sdk user for making requests | |
 `override_http_client_configuration` | `bool` | The value which determines to
 override properties of the passed Http Client from the sdk user | |
@@ -50,16 +50,16 @@
 **Default: 2** | | `retry_statuses` | `Array of int` | The http statuses on
 which retry is to be done.
 **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** | |
 `retry_methods` | `Array of string` | The http methods on which retry is to be
 done.
 **Default: ['GET', 'PUT']** | | `custom_header_authentication_credentials` |
 [`CustomHeaderAuthenticationCredentials`](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/custom-header-signature.md) | The credential
+ecommerce-sdk-python/tree/1.0.3/doc/$a/https://www.github.com/postnl/postnl-
+ecommerce-sdk-python/tree/1.0.3/custom-header-signature.md) | The credential
 object for Custom Header Signature | The API client can be initialized as
 follows: ```python client = PostnlecommerceClient
 (
 custom_header_authentication_credentials=CustomHeaderAuthenticationCredentials
 ( apikey='apikey' ) ) ``` API calls return an `ApiResponse` object that
 includes the following fields: | Field | Description | | --- | --- | |
 `status_code` | Status code of the HTTP response | | `reason_phrase` | Reason
@@ -68,30 +68,30 @@
 | HTTP request info | | `errors` | Errors, if they exist | | `body` | The
 deserialized body of the HTTP response | ## Environments The SDK can be
 configured to use a different environment for making API calls. Available
 environments are: ### Fields | Name | Description | | --- | --- | | Production
 server | **Default** Production server | | Non-Production server | Sandbox
 environment for testing | ## Authorization This API uses the following
 authentication schemes. * [`APIKeyHeader (Custom Header Signature)`](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/$a/https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/custom-header-
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/$a/https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/custom-header-
 signature.md) ## List of APIs * [Postalcodecheck](https://www.github.com/
-postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 postalcodecheck.md) * [Barcode](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/controllers/barcode.md) * [Checkout](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+sdk-python/tree/1.0.3/doc/controllers/barcode.md) * [Checkout](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 checkout.md) * [Confirming](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.2/doc/controllers/confirming.md) * [Deliverydate](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+python/tree/1.0.3/doc/controllers/confirming.md) * [Deliverydate](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 deliverydate.md) * [Labelling](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/controllers/labelling.md) * [Locations](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+sdk-python/tree/1.0.3/doc/controllers/labelling.md) * [Locations](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 locations.md) * [Shipment](https://www.github.com/postnl/postnl-ecommerce-sdk-
-python/tree/1.0.2/doc/controllers/shipment.md) * [Shipping Status](https://
-www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/controllers/
+python/tree/1.0.3/doc/controllers/shipment.md) * [Shipping Status](https://
+www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/controllers/
 shipping-status.md) * [Timeframes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/controllers/timeframes.md) ## Classes
+ecommerce-sdk-python/tree/1.0.3/doc/controllers/timeframes.md) ## Classes
 Documentation * [Utility Classes](https://www.github.com/postnl/postnl-
-ecommerce-sdk-python/tree/1.0.2/doc/utility-classes.md) * [HttpResponse](https:
-//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.2/doc/http-
+ecommerce-sdk-python/tree/1.0.3/doc/utility-classes.md) * [HttpResponse](https:
+//www.github.com/postnl/postnl-ecommerce-sdk-python/tree/1.0.3/doc/http-
 response.md) * [HttpRequest](https://www.github.com/postnl/postnl-ecommerce-
-sdk-python/tree/1.0.2/doc/http-request.md)
+sdk-python/tree/1.0.3/doc/http-request.md)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnl_ecommerce_sdk.egg-info/SOURCES.txt` & `postnl_ecommerce_sdk-1.0.3/postnl_ecommerce_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/api_helper.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/api_helper.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/configuration.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/configuration.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/barcode_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/barcode_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             customer_number (str): The customer code for which you want a
                 barcode to be generated
             mtype (TypeEnum): The barcode type that you want to be generated
             serie (str, optional): Barcode serie in the format
                 '###000000-###000000', for example 100000-20000. The range
                 must consist of a minimal difference of 100.000. It is allowed
                 to add extra leading zeros at the beginning of the serie. See
-                [Guidelines](https://developer.postnl.nl/browse-apis/send-and-t
-                rack/barcode-webservice/) for more information.
+                [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoi
+                nts/send-track/barcode/guidelines) for more information.
             range (str, optional): Only used for International Mail and Packet
                 products (PEPS) shipments (with type LA, RI, UE). Identifying
                 the issuing postal administration's country (NL in this
                 case).
 
         Returns:
             ApiResponse: An object with the response value as well as other
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/base_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/checkout_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/checkout_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/confirming_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/confirming_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/deliverydate_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/deliverydate_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/labelling_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/labelling_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/locations_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/locations_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/postalcode_check_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/postalcode_check_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipment_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/shipment_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/shipping_status_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/shipping_status_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/controllers/timeframes_controller.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/controllers/timeframes_controller.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/api_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_method_not_allowed_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_error_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_response_error_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/barcode_too_many_request_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/barcode_too_many_request_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/checkout_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/checkout_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/confirming_response_error_1_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/confirming_response_error_1_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/deliverydate_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/labelling_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/labelling_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/locations_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/locations_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/exceptions/timeframe_response_invalid_exception.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/exceptions/timeframe_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/api_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/api_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/auth/custom_header_authentication.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/auth/custom_header_authentication.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_request.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/http_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/http/http_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/http/http_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/__init__.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/__init__.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_11.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_11.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     """Implementation of the 'Address11' model.
 
     TODO: type model description here.
 
     Attributes:
         address_type (str): Type of the address. This is a code. You can find
             the possible values at [Address
-            types](#tag/Reference-codes/Address-types)
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/address-types)
         area (str): Area of the address
         buildingname (str): Building name of the address
         city (str): City of the address
         company_name (str): This field has a dependency with the field Name.
             One of both fields must be filled mandatory; using both fields is
             also allowed. Mandatory when AddressType is 09.
         countrycode (str): The ISO2 country codes
@@ -45,16 +46,16 @@
         region (str): Region of the address. Mandatory for Non EU destinations
             where a region is applicable.
         street (str): This field has a dependency with the field
             StreetHouseNrExt. One of both fields must be filled mandatory.
             Using both fields simultaneously is discouraged.
         street_house_nr_ext (str): Combination of Street, HouseNr and
             HouseNrExt. Please see
-            [Guidelines](https://developer.postnl.nl/browse-apis/send-and-track
-            /labelling-webservice/) for the explanation.
+            [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoints/
+            send-track/confirming/guidelines) for the explanation.
         zipcode (str): Zipcode of the address. Mandatory for shipments to
             Benelux. Max length (NL) 6 characters,(BE;LU) 4 numeric
             characters
 
     """
 
     # Create a mapping from Model property names to API property names
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_2.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
             experience of your customer.
         region (str): Region of the address
         street (str): This field has a dependency with the field
             StreetHouseNrExt. One of both fields must be filled mandatory;
             using both fields simultaneously is discouraged.
         street_house_nr_ext (str): Combination of Street, HouseNr and
             HouseNrExt. Please see
-            [Guidelines](https://developer.postnl.nl/browse-apis/send-and-track
-            /labelling-webservice/) for the explanation.
+            [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoints/
+            send-track/confirming/guidelines) for the explanation.
         zipcode (str): Zipcode of the address. Mandatory for shipments to
             Benelux. Max length (NL) 6 characters,(BE;LU) 4 numeric
             characters
 
     """
 
     # Create a mapping from Model property names to API property names
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_3.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_3.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/address_4.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/address_4.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/amount.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
     """Implementation of the 'Amount' model.
 
     TODO: type model description here.
 
     Attributes:
         amount_type (str): Amount type. Please see [Amount
-            types](#tag/Reference-codes/Amount-types) for the available
-            types.
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/amount-types) for the available types.
         account_name (str): Name of bank account owner
         bic (str): BIC number,optional for COD shipments (mandatory for bank
             account number other than originating in The Netherlands)
         currency (str): Currency code. only EUR, GBP, USD and CNY are
             allowed.
         iban (str): IBAN bank account number,mandatory for COD shipments.
             Dutch IBAN numbers are 18 characters
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/amount_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/amount_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/barcode_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_request.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/checkout_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/checkout_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/checkout_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/code_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/code_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/complete_status.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/complete_status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_request.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/confirming_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/confirming_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/confirming_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/contact.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/contact.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,25 +14,25 @@
     """Implementation of the 'Contact' model.
 
     TODO: type model description here.
 
     Attributes:
         contact_type (str): Type of the contact. This is a code. Please refer
             to the available [Contact
-            types](#tag/Reference-codes/Contact-types) for the possible
-            values.
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/contact-types) for the possible values.
         email (str): Email address of the contact. Mandatory in some cases.
             Either the Email or Telnr needs to be filled in for Non EU
             destinations. Please see
-            [Guidelines](https://developer.postnl.nl/browse-apis/send-and-track
-            /labelling-webservice/).
+            [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoints/
+            send-track/confirming/guidelines).
         sms_nr (str): Mobile phone number of the contact. Mandatory in some
             cases. Please see
-            [Guidelines](https://developer.postnl.nl/browse-apis/send-and-track
-            /labelling-webservice/).
+            [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoints/
+            send-track/confirming/guidelines).
         tel_nr (str): Phone number of the contact. Either the Email or Telnr
             needs to be filled in for Non EU destinations. Preferably prefixed
             with “+” and the international dialling code.
 
     """
 
     # Create a mapping from Model property names to API property names
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/content.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/content_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/content_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cpc_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/cpc_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/currency_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/currency_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/current_status.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/current_status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/custom.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,19 @@
             *VOEC is a Norwegian VAT number.
         importer_reference_code (str): This is the reference of the recipient.
             Fill in a Tax Code or VAT number or Importer code. Depending on
             the destination with this reference the customs process can be
             faster. For example Brazil uses an TAXID number for natural
             persons, known as CPF.
         transaction_code (str): See the [Reference
-            data](#tag/Reference-codes/Transaction-codes) for possible
-            values.
+            data](https://developer.postnl.nl/docs/#/http/reference-data/refere
+            nce-codes/transaction-codes) for possible values.
         transaction_description (str): Transaction description; see
-            [here](#tag/Reference-codes/Transaction-codes) for common
-            examples.
+            [here](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/transaction-codes) for common examples.
         content (List[Content]): The contents of the shipment. This section is
             mandatory (minimum once, maximum 5). Fill per unique item.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/customer.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/customer_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/customer_2.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/customer_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/cut_off_time.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/cut_off_time.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/day_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/day_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_option.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/delivery_option.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/delivery_options.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/delivery_options.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/detail.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/detail.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/dimension.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class Dimension(object):
 
     """Implementation of the 'Dimension' model.
 
     Note: Length, Width, Height values are about the order of the size and
     need to be filled in from the longest to the shortest value. For example:
-    shipment’s official height is 700mm, width 500mm, length 300mm. The
+    shipment's official height is 700mm, width 500mm, length 300mm. The
     longest side (highest value) of 700mm needs to be entered at Length. Width
     value becomes 500mm, Height value: 300mm (the lowest). Entering the
     dimensions in the wrong order may result in incorrect shipping labels and
     longer delivery times. The maximum dimensions can be found in your PostNL
     contract.
 
     Attributes:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/dimension_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/dimension_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_2.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_2.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_3.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_3.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/error_4.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/error_4.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/event.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/event.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/expectation.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/expectation.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/extra_field.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/extra_field.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/fault.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/fault.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/friday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/friday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/friday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/get_locations_result.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/get_locations_result_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/get_locations_result_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/group.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/group.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     """Implementation of the 'Group' model.
 
     TODO: type model description here.
 
     Attributes:
         group_type (str): Group sort that determines the type of group that is
             indicated. This is a code. For possible values, please see
-            [here](#tag/Reference-codes/Group-types)
+            [here](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/group-types)
         group_sequence (int): Sequence number of the collo within the complete
             shipment (e.g. collo 2 of 4) Mandatory for multicollo shipments
         group_count (int): Total number of colli in the shipment (in case of
             multicolli shipments) Mandatory for multicollo shipments
         main_barcode (str): Main barcode for the shipment (in case of
             multicolli shipments) Mandatory for multicollo shipments
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/hazardous_material.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/hazardous_material.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/label_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 This file was automatically generated for PostNL by APIMATIC v3.0 (
  https://www.apimatic.io ).
 """
 from postnlecommerce.api_helper import APIHelper
 
 
-class Label(object):
+class Label1(object):
 
-    """Implementation of the 'Label' model.
+    """Implementation of the 'Label1' model.
 
     TODO: type model description here.
 
     Attributes:
         content (str): Base64 encoded label content
-        labeltype (str): Type of the label. See possible [Label
-            types](#tag/Reference-codes/Label-types)
-        output_type (str): Content type of the label, e.g. zebra of pdf.
+        labeltype (str): Type of the label. See Guidelines
+        output_type (str): Content type of the label, e.g. zebra of pdf. Note:
+            It is not recommended to send .PDF files/labels directly to a
+            Zebra printer. See Guidelines.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "content": 'Content',
         "labeltype": 'Labeltype',
@@ -36,15 +37,15 @@
         'output_type',
     ]
 
     def __init__(self,
                  content=APIHelper.SKIP,
                  labeltype=APIHelper.SKIP,
                  output_type=APIHelper.SKIP):
-        """Constructor for the Label class"""
+        """Constructor for the Label1 class"""
 
         # Initialize members of the class
         if content is not APIHelper.SKIP:
             self.content = content 
         if labeltype is not APIHelper.SKIP:
             self.labeltype = labeltype 
         if output_type is not APIHelper.SKIP:
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/label_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/label.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 This file was automatically generated for PostNL by APIMATIC v3.0 (
  https://www.apimatic.io ).
 """
 from postnlecommerce.api_helper import APIHelper
 
 
-class Label1(object):
+class Label(object):
 
-    """Implementation of the 'Label1' model.
+    """Implementation of the 'Label' model.
 
     TODO: type model description here.
 
     Attributes:
         content (str): Base64 encoded label content
-        labeltype (str): Type of the label. See Guidelines
-        output_type (str): Content type of the label, e.g. zebra of pdf. Note:
-            It is not recommended to send .PDF files/labels directly to a
-            Zebra printer. See Guidelines.
+        labeltype (str): Type of the label. See possible [Label
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/label-types)
+        output_type (str): Content type of the label, e.g. zebra of pdf.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "content": 'Content',
         "labeltype": 'Labeltype',
@@ -37,15 +37,15 @@
         'output_type',
     ]
 
     def __init__(self,
                  content=APIHelper.SKIP,
                  labeltype=APIHelper.SKIP,
                  output_type=APIHelper.SKIP):
-        """Constructor for the Label1 class"""
+        """Constructor for the Label class"""
 
         # Initialize members of the class
         if content is not APIHelper.SKIP:
             self.content = content 
         if labeltype is not APIHelper.SKIP:
             self.labeltype = labeltype 
         if output_type is not APIHelper.SKIP:
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_request.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/labelling_request.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/labelling_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/labelling_response_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/labelling_response_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/language_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/language_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,17 @@
         opening_hours (OpeningHours): The standard opening hours of the pickup
             location
         distance (int): The calculated distance (in meters) between the
             location specified and the address provided in the request
         location_code (str): The location identifier
         partner_id (str): The partner identifier; not used anymore
         sustainability (Sustainability): Sustainability score; see
-            [Sustainability codes](#tag/Reference-codes/Sustainability-codes)
-            for possible values.
+            [Sustainability
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes) for possible values.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "address": 'Address',
         "pickup_time": 'PickupTime',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/location_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         latitude (float): The latitude of the pickup location
         location_code (int): The pickup location identifier
         longitude (float): The longitude of the pickup location
         name (str): The name of the pickup location
         opening_hours (OpeningHours): The standard opening times of the pickup
             location
         sustainability (Warning1): Sustainability score; see [Sustainability
-            codes](#tag/Reference-codes/Sustainability-codes) for possible
-            values.
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/sustainability-codes) for possible values.
         partner_name (str): The partner name belonging to the pickup location.
             Can be ignored, no longer used.
         retail_network_id (str): The retail network belonging to the pickup
             location. Can be ignored, no longer used
 
     """
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/location_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/location_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/locations_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/locations_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/merged_label.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/merged_label.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/message.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/message_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/message_1.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
     Attributes:
         message_id (str): ID of the message
         message_time_stamp (str): Date/time of sending the message. Format:
             dd-mm-yyyy hh:mm:ss
         printertype (str): Printer type that will be used to process the
             label, e.g. Zebra printer or PDF See [Printer
-            types](#tag/Reference-codes/Printer-types) for the available
-            printer types.
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/printer-types) for the available printer types.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "message_id": 'MessageID',
         "message_time_stamp": 'MessageTimeStamp',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/monday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/monday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/monday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/old_status.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/old_status.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/opening_hours.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/opening_hours.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_1_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_2_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_2_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_3_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_3_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/option_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/option_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 class Options(object):
 
     """Implementation of the 'Options' model.
 
     The delivery options for which a delivery date is returned. Only one
     delivery option is specified. See [Delivery
-    Options](#tag/Reference-codes/Delivery-options) for possible values.
+    Options](https://developer.postnl.nl/docs/#/http/reference-data/reference-c
+    odes/delivery-options) for possible values.
 
     Attributes:
         string (str): TODO: type description here.
 
     """
 
     # Create a mapping from Model property names to API property names
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/options_2_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/options_2_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/pickup_option.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/pickup_option.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shippingstatus_response_signature.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,46 +2,52 @@
 
 """
 postnlecommerce
 
 This file was automatically generated for PostNL by APIMATIC v3.0 (
  https://www.apimatic.io ).
 """
+from postnlecommerce.api_helper import APIHelper
+from postnlecommerce.models.signature import Signature
+from postnlecommerce.models.warnings import Warnings
 
 
-class ProductOption(object):
+class ShippingstatusResponseSignature(object):
 
-    """Implementation of the 'ProductOption' model.
+    """Implementation of the 'shippingstatusResponseSignature' model.
 
     TODO: type model description here.
 
     Attributes:
-        characteristic (str): The characteristic of the ProductOption.
-            Mandatory for some products, please see the [Products
-            page](#tag/Product-codes)
-        option (str): The product option code for this ProductOption.
-            Mandatory for some products, please see the [Products
-            page](#tag/Product-codes)
+        signature (Signature): TODO: type description here.
+        warnings (Warnings): TODO: type description here.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
-        "characteristic": 'Characteristic',
-        "option": 'Option'
+        "signature": 'Signature',
+        "warnings": 'Warnings'
     }
 
+    _optionals = [
+        'signature',
+        'warnings',
+    ]
+
     def __init__(self,
-                 characteristic='118',
-                 option='006'):
-        """Constructor for the ProductOption class"""
+                 signature=APIHelper.SKIP,
+                 warnings=APIHelper.SKIP):
+        """Constructor for the ShippingstatusResponseSignature class"""
 
         # Initialize members of the class
-        self.characteristic = characteristic 
-        self.option = option 
+        if signature is not APIHelper.SKIP:
+            self.signature = signature 
+        if warnings is not APIHelper.SKIP:
+            self.warnings = warnings 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
         Args:
@@ -54,12 +60,12 @@
 
         """
 
         if dictionary is None:
             return None
 
         # Extract variables from the dictionary
-        characteristic = dictionary.get("Characteristic") if dictionary.get("Characteristic") else '118'
-        option = dictionary.get("Option") if dictionary.get("Option") else '006'
+        signature = Signature.from_dictionary(dictionary.get('Signature')) if 'Signature' in dictionary.keys() else APIHelper.SKIP
+        warnings = Warnings.from_dictionary(dictionary.get('Warnings')) if 'Warnings' in dictionary.keys() else APIHelper.SKIP
         # Return an object of this model
-        return cls(characteristic,
-                   option)
+        return cls(signature,
+                   warnings)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_option_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/product_option_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/product_options.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/product_options.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframe.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/reason_no_timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/reason_no_timeframes.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/reason_no_timeframes.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning_1.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,59 +3,51 @@
 """
 postnlecommerce
 
 This file was automatically generated for PostNL by APIMATIC v3.0 (
  https://www.apimatic.io ).
 """
 from postnlecommerce.api_helper import APIHelper
-from postnlecommerce.models.error_2 import Error2
-from postnlecommerce.models.warning_1 import Warning1
 
 
-class ResponseShipment(object):
+class Warning1(object):
 
-    """Implementation of the 'ResponseShipment' model.
+    """Implementation of the 'Warning1' model.
 
-    TODO: type model description here.
+    Sustainability score; see [Sustainability
+    codes](https://developer.postnl.nl/docs/#/http/reference-data/reference-cod
+    es/delivery-options) for possible values.
 
     Attributes:
-        errors (List[Error2]): Possible errors. See the [Error
-            Codes](#tag/Error codes) for possible values
-        warnings (List[Warning1]): Possible warnings. See the [Error
-            Codes](#tag/Error codes) for possible values
-        barcode (str): The barcode used
+        code (str): The Warning code
+        description (str): The warning description
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
-        "errors": 'Errors',
-        "warnings": 'Warnings',
-        "barcode": 'Barcode'
+        "code": 'Code',
+        "description": 'Description'
     }
 
     _optionals = [
-        'errors',
-        'warnings',
-        'barcode',
+        'code',
+        'description',
     ]
 
     def __init__(self,
-                 errors=APIHelper.SKIP,
-                 warnings=APIHelper.SKIP,
-                 barcode=APIHelper.SKIP):
-        """Constructor for the ResponseShipment class"""
+                 code=APIHelper.SKIP,
+                 description=APIHelper.SKIP):
+        """Constructor for the Warning1 class"""
 
         # Initialize members of the class
-        if errors is not APIHelper.SKIP:
-            self.errors = errors 
-        if warnings is not APIHelper.SKIP:
-            self.warnings = warnings 
-        if barcode is not APIHelper.SKIP:
-            self.barcode = barcode 
+        if code is not APIHelper.SKIP:
+            self.code = code 
+        if description is not APIHelper.SKIP:
+            self.description = description 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
         Args:
@@ -68,22 +60,12 @@
 
         """
 
         if dictionary is None:
             return None
 
         # Extract variables from the dictionary
-        errors = None
-        if dictionary.get('Errors') is not None:
-            errors = [Error2.from_dictionary(x) for x in dictionary.get('Errors')]
-        else:
-            errors = APIHelper.SKIP
-        warnings = None
-        if dictionary.get('Warnings') is not None:
-            warnings = [Warning1.from_dictionary(x) for x in dictionary.get('Warnings')]
-        else:
-            warnings = APIHelper.SKIP
-        barcode = dictionary.get("Barcode") if dictionary.get("Barcode") else APIHelper.SKIP
+        code = dictionary.get("Code") if dictionary.get("Code") else APIHelper.SKIP
+        description = dictionary.get("Description") if dictionary.get("Description") else APIHelper.SKIP
         # Return an object of this model
-        return cls(errors,
-                   warnings,
-                   barcode)
+        return cls(code,
+                   description)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/response_shipment_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     TODO: type model description here.
 
     Attributes:
         product_code_delivery (str): The product code of the shipment
         labels (List[Label1]): All labels belonging to the selected product
         barcode (str): The barcode used on the label
         warnings (List[Warning1]): Possible warnings. See the [Error
-            Codes](#tag/Error-codes) for possible values
+            Codes](https://developer.postnl.nl/docs/#/http/reference-data/error
+            -codes) for possible values
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "product_code_delivery": 'ProductCodeDelivery',
         "labels": 'Labels',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/response_shipment_2.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/response_shipment_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     TODO: type model description here.
 
     Attributes:
         product_code_delivery (str): The product code of the shipment
         labels (List[Label]): All labels belonging to the selected product
         barcode (str): The barcode used on the label
         warnings (List[Warning1]): Possible warnings. See the [Error
-            Codes](#tag/Error-codes) for possible values
+            Codes](https://developer.postnl.nl/docs/#/http/reference-data/error
+            -codes) for possible values
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "product_code_delivery": 'ProductCodeDelivery',
         "labels": 'Labels',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/saturday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/saturday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/saturday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,66 +8,69 @@
 """
 from postnlecommerce.api_helper import APIHelper
 from postnlecommerce.models.address_11 import Address11
 from postnlecommerce.models.amount import Amount
 from postnlecommerce.models.contact import Contact
 from postnlecommerce.models.custom import Custom
 from postnlecommerce.models.dimension import Dimension
+from postnlecommerce.models.extra_field import ExtraField
 from postnlecommerce.models.group import Group
 from postnlecommerce.models.hazardous_material import HazardousMaterial
 from postnlecommerce.models.product_option import ProductOption
 
 
-class Shipment(object):
+class Shipment1(object):
 
-    """Implementation of the 'Shipment' model.
+    """Implementation of the 'Shipment1' model.
 
     TODO: type model description here.
 
     Attributes:
         addresses (List[Address11]): List of 1 or more Address type elements.
             At least 1 address type is mandatory. See [Address
-            types](#tag/Reference-codes/Address-types) for the available
-            types.
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/address-types) for the available types.
         amounts (List[Amount]): List of amount types. An amount represents a
             value of the shipment. Amount type 01 mandatory for COD-shipments,
             Amount type 02 mandatory for domestic insured shipments. Please
-            see [Amount types](#tag/Reference-codes/Amount-types) for the
-            available types.
+            see [Amount
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/amount-types) for the available types.
         barcode (str): Barcode of the shipment. This is a unique value. Note:
             If you leave this attribute out of your request an unique barcode
             will be generated automatically.
         coding_text (str): Code used for logistic purposes (usually generated
             by the service itself and returned in the response). Please note
             that this must be provided when  using the Confirm API to confirm
             shipments where coding texts are required (e.g. letterbox
             parcels).
         collection_time_stamp_start (str): Starting date/time of the
             collection of the shipment. Format: dd-MM-yyyy hh:mm:ss
         collection_time_stamp_end (str): Ending date/time of the collection of
             the shipment. Format: dd-MM-yyyy hh:mm:ss
         contacts (List[Contact]): One or more ContactType elements belonging
             to a shipment. Mandatory in some cases. Please refer to the
-            available [Contact types](#tag/Reference-codes/Contact-types) for
-            the possible values.
+            available [Contact
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/contact-types) for the possible values.
         content (str): Content of the shipment. Mandatory for Extra@Home
             shipments
         cost_center (str): Cost center of the shipment. This value will appear
             on your invoice
         customer_order_number (str): Order number of the customer
-        customs (List[Custom]): The Customs type is mandatory for non-EU
-            shipments and not allowed for any other shipment types.
+        customs (Custom): The Customs type is mandatory for non-EU shipments
+            and not allowed for any other shipment types.
         delivery_address (str): Delivery address specification. This field is
             mandatory when AddressType on the Address is 09.
         delivery_date (str): Mandatory when using Mailbox Parcels (for
             generation of the coding rule) and delivery options like
             Evening/Morning/Sameday delivery etc.
         dimension (Dimension): Note: Length, Width, Height values are about
             the order of the size and need to be filled in from the longest to
-            the shortest value. For example: shipment’s official height is
+            the shortest value. For example: shipment's official height is
             700mm, width 500mm, length 300mm. The longest side (highest value)
             of 700mm needs to be entered at Length. Width value becomes 500mm,
             Height value: 300mm (the lowest). Entering the dimensions in the
             wrong order may result in incorrect shipping labels and longer
             delivery times. The maximum dimensions can be found in your PostNL
             contract.
         down_partner_barcode (str): Barcode of the downstream network partner
@@ -76,26 +79,29 @@
         down_partner_id (str): Identification of the downstream network
             partner of PostNL Pakketten.
         down_partner_location (str): Identification of the location of the
             downstream network partner of PostNL Pakketten.
         groups (List[Group]): List of 0 or more Group types with data,
             grouping multiple shipments together. Mandatory for multicollo
             shipments. Please see
-            [Guidelines](https://developer.postnl.nl/browse-apis/send-and-track
-            /labelling-webservice/) (Multiple shipments) for more
+            [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoints/
+            send-track/labelling/guidelines) (Multiple shipments) for more
             information.
         hazardous_material (List[HazardousMaterial]): Array of hazardous
             materials contained in the shipment
         product_code_collect (str): Deprecated. Collection product code of a
             shipment.
         product_code_delivery (str): Product code of the shipment. See the
-            [Products page](#tag/Product-codes) for possible products.
+            [Products
+            page](https://developer.postnl.nl/docs/#/http/reference-data/produc
+            t-codes) for possible products.
         product_options (List[ProductOption]): Product options for the
             shipment, mandatory for certain products, see the [Products
-            page](#tag/Product-codes).
+            page](https://developer.postnl.nl/docs/#/http/reference-data/produc
+            t-codes).
         receiver_date_of_birth (str): Date of birth. Mandatory for Age check
             products
         reference (str): Your own reference of the shipment. Mandatory for
             Extra@Home shipments; for E@H this is used to create your order
             number, so this should be unique for each request.
         reference_collect (str): Additional reference of the collect order of
             the shipment
@@ -103,14 +109,16 @@
         return_barcode (str): Return barcode of the shipment. PostNL will
             provide you with a separate customer code specifically for
             generating the returnBarcode. Mandatory for Label in the Box
             (return label) shipments.
         return_reference (str): Return reference of the shipment
         timeslot_id (str): Deprecated. ID of the chosen timeslot as returned
             by the timeslot webservice
+        extra_fields (List[ExtraField]): Possibility to provide extra
+            key-value pairs to the webservice. Not used at the moment.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "addresses": 'Addresses',
         "barcode": 'Barcode',
@@ -136,15 +144,16 @@
         "product_options": 'ProductOptions',
         "receiver_date_of_birth": 'ReceiverDateOfBirth',
         "reference": 'Reference',
         "reference_collect": 'ReferenceCollect',
         "remark": 'Remark',
         "return_barcode": 'ReturnBarcode',
         "return_reference": 'ReturnReference',
-        "timeslot_id": 'TimeslotID'
+        "timeslot_id": 'TimeslotID',
+        "extra_fields": 'ExtraFields'
     }
 
     _optionals = [
         'amounts',
         'coding_text',
         'collection_time_stamp_start',
         'collection_time_stamp_end',
@@ -165,14 +174,15 @@
         'receiver_date_of_birth',
         'reference',
         'reference_collect',
         'remark',
         'return_barcode',
         'return_reference',
         'timeslot_id',
+        'extra_fields',
     ]
 
     def __init__(self,
                  addresses=None,
                  barcode=None,
                  dimension=None,
                  product_code_delivery='3085',
@@ -196,16 +206,17 @@
                  product_options=APIHelper.SKIP,
                  receiver_date_of_birth=APIHelper.SKIP,
                  reference=APIHelper.SKIP,
                  reference_collect=APIHelper.SKIP,
                  remark=APIHelper.SKIP,
                  return_barcode=APIHelper.SKIP,
                  return_reference=APIHelper.SKIP,
-                 timeslot_id=APIHelper.SKIP):
-        """Constructor for the Shipment class"""
+                 timeslot_id=APIHelper.SKIP,
+                 extra_fields=APIHelper.SKIP):
+        """Constructor for the Shipment1 class"""
 
         # Initialize members of the class
         self.addresses = addresses 
         if amounts is not APIHelper.SKIP:
             self.amounts = amounts 
         self.barcode = barcode 
         if coding_text is not APIHelper.SKIP:
@@ -254,14 +265,16 @@
             self.remark = remark 
         if return_barcode is not APIHelper.SKIP:
             self.return_barcode = return_barcode 
         if return_reference is not APIHelper.SKIP:
             self.return_reference = return_reference 
         if timeslot_id is not APIHelper.SKIP:
             self.timeslot_id = timeslot_id 
+        if extra_fields is not APIHelper.SKIP:
+            self.extra_fields = extra_fields 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
         Args:
@@ -296,19 +309,15 @@
         if dictionary.get('Contacts') is not None:
             contacts = [Contact.from_dictionary(x) for x in dictionary.get('Contacts')]
         else:
             contacts = APIHelper.SKIP
         content = dictionary.get("Content") if dictionary.get("Content") else APIHelper.SKIP
         cost_center = dictionary.get("CostCenter") if dictionary.get("CostCenter") else APIHelper.SKIP
         customer_order_number = dictionary.get("CustomerOrderNumber") if dictionary.get("CustomerOrderNumber") else APIHelper.SKIP
-        customs = None
-        if dictionary.get('Customs') is not None:
-            customs = [Custom.from_dictionary(x) for x in dictionary.get('Customs')]
-        else:
-            customs = APIHelper.SKIP
+        customs = Custom.from_dictionary(dictionary.get('Customs')) if 'Customs' in dictionary.keys() else APIHelper.SKIP
         delivery_address = dictionary.get("DeliveryAddress") if dictionary.get("DeliveryAddress") else APIHelper.SKIP
         delivery_date = dictionary.get("DeliveryDate") if dictionary.get("DeliveryDate") else APIHelper.SKIP
         down_partner_barcode = dictionary.get("DownPartnerBarcode") if dictionary.get("DownPartnerBarcode") else APIHelper.SKIP
         down_partner_id = dictionary.get("DownPartnerID") if dictionary.get("DownPartnerID") else APIHelper.SKIP
         down_partner_location = dictionary.get("DownPartnerLocation") if dictionary.get("DownPartnerLocation") else APIHelper.SKIP
         groups = None
         if dictionary.get('Groups') is not None:
@@ -329,14 +338,19 @@
         receiver_date_of_birth = dictionary.get("ReceiverDateOfBirth") if dictionary.get("ReceiverDateOfBirth") else APIHelper.SKIP
         reference = dictionary.get("Reference") if dictionary.get("Reference") else APIHelper.SKIP
         reference_collect = dictionary.get("ReferenceCollect") if dictionary.get("ReferenceCollect") else APIHelper.SKIP
         remark = dictionary.get("Remark") if dictionary.get("Remark") else APIHelper.SKIP
         return_barcode = dictionary.get("ReturnBarcode") if dictionary.get("ReturnBarcode") else APIHelper.SKIP
         return_reference = dictionary.get("ReturnReference") if dictionary.get("ReturnReference") else APIHelper.SKIP
         timeslot_id = dictionary.get("TimeslotID") if dictionary.get("TimeslotID") else APIHelper.SKIP
+        extra_fields = None
+        if dictionary.get('ExtraFields') is not None:
+            extra_fields = [ExtraField.from_dictionary(x) for x in dictionary.get('ExtraFields')]
+        else:
+            extra_fields = APIHelper.SKIP
         # Return an object of this model
         return cls(addresses,
                    barcode,
                    dimension,
                    product_code_delivery,
                    amounts,
                    coding_text,
@@ -358,8 +372,9 @@
                    product_options,
                    receiver_date_of_birth,
                    reference,
                    reference_collect,
                    remark,
                    return_barcode,
                    return_reference,
-                   timeslot_id)
+                   timeslot_id,
+                   extra_fields)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,67 +8,68 @@
 """
 from postnlecommerce.api_helper import APIHelper
 from postnlecommerce.models.address_11 import Address11
 from postnlecommerce.models.amount import Amount
 from postnlecommerce.models.contact import Contact
 from postnlecommerce.models.custom import Custom
 from postnlecommerce.models.dimension import Dimension
-from postnlecommerce.models.extra_field import ExtraField
 from postnlecommerce.models.group import Group
 from postnlecommerce.models.hazardous_material import HazardousMaterial
 from postnlecommerce.models.product_option import ProductOption
 
 
-class Shipment1(object):
+class Shipment(object):
 
-    """Implementation of the 'Shipment1' model.
+    """Implementation of the 'Shipment' model.
 
     TODO: type model description here.
 
     Attributes:
         addresses (List[Address11]): List of 1 or more Address type elements.
             At least 1 address type is mandatory. See [Address
-            types](#tag/Reference-codes/Address-types) for the available
-            types.
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/address-types) for the available types.
         amounts (List[Amount]): List of amount types. An amount represents a
             value of the shipment. Amount type 01 mandatory for COD-shipments,
             Amount type 02 mandatory for domestic insured shipments. Please
-            see [Amount types](#tag/Reference-codes/Amount-types) for the
-            available types.
+            see [Amount
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/amount-types) for the available types.
         barcode (str): Barcode of the shipment. This is a unique value. Note:
             If you leave this attribute out of your request an unique barcode
             will be generated automatically.
         coding_text (str): Code used for logistic purposes (usually generated
             by the service itself and returned in the response). Please note
             that this must be provided when  using the Confirm API to confirm
             shipments where coding texts are required (e.g. letterbox
             parcels).
         collection_time_stamp_start (str): Starting date/time of the
             collection of the shipment. Format: dd-MM-yyyy hh:mm:ss
         collection_time_stamp_end (str): Ending date/time of the collection of
             the shipment. Format: dd-MM-yyyy hh:mm:ss
         contacts (List[Contact]): One or more ContactType elements belonging
             to a shipment. Mandatory in some cases. Please refer to the
-            available [Contact types](#tag/Reference-codes/Contact-types) for
-            the possible values.
+            available [Contact
+            types](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/contact-types) for the possible values.
         content (str): Content of the shipment. Mandatory for Extra@Home
             shipments
         cost_center (str): Cost center of the shipment. This value will appear
             on your invoice
         customer_order_number (str): Order number of the customer
-        customs (Custom): The Customs type is mandatory for non-EU shipments
-            and not allowed for any other shipment types.
+        customs (List[Custom]): The Customs type is mandatory for non-EU
+            shipments and not allowed for any other shipment types.
         delivery_address (str): Delivery address specification. This field is
             mandatory when AddressType on the Address is 09.
         delivery_date (str): Mandatory when using Mailbox Parcels (for
             generation of the coding rule) and delivery options like
             Evening/Morning/Sameday delivery etc.
         dimension (Dimension): Note: Length, Width, Height values are about
             the order of the size and need to be filled in from the longest to
-            the shortest value. For example: shipment’s official height is
+            the shortest value. For example: shipment's official height is
             700mm, width 500mm, length 300mm. The longest side (highest value)
             of 700mm needs to be entered at Length. Width value becomes 500mm,
             Height value: 300mm (the lowest). Entering the dimensions in the
             wrong order may result in incorrect shipping labels and longer
             delivery times. The maximum dimensions can be found in your PostNL
             contract.
         down_partner_barcode (str): Barcode of the downstream network partner
@@ -77,26 +78,29 @@
         down_partner_id (str): Identification of the downstream network
             partner of PostNL Pakketten.
         down_partner_location (str): Identification of the location of the
             downstream network partner of PostNL Pakketten.
         groups (List[Group]): List of 0 or more Group types with data,
             grouping multiple shipments together. Mandatory for multicollo
             shipments. Please see
-            [Guidelines](https://developer.postnl.nl/browse-apis/send-and-track
-            /labelling-webservice/) (Multiple shipments) for more
+            [Guidelines](https://developer.postnl.nl/docs/#/http/api-endpoints/
+            send-track/confirming/guidelines) (Multiple shipments) for more
             information.
         hazardous_material (List[HazardousMaterial]): Array of hazardous
             materials contained in the shipment
         product_code_collect (str): Deprecated. Collection product code of a
             shipment.
         product_code_delivery (str): Product code of the shipment. See the
-            [Products page](#tag/Product-codes) for possible products.
+            [Products
+            page](https://developer.postnl.nl/docs/#/http/reference-data/produc
+            t-codes) for possible products.
         product_options (List[ProductOption]): Product options for the
             shipment, mandatory for certain products, see the [Products
-            page](#tag/Product-codes).
+            page](https://developer.postnl.nl/docs/#/http/reference-data/produc
+            t-codes).
         receiver_date_of_birth (str): Date of birth. Mandatory for Age check
             products
         reference (str): Your own reference of the shipment. Mandatory for
             Extra@Home shipments; for E@H this is used to create your order
             number, so this should be unique for each request.
         reference_collect (str): Additional reference of the collect order of
             the shipment
@@ -104,16 +108,14 @@
         return_barcode (str): Return barcode of the shipment. PostNL will
             provide you with a separate customer code specifically for
             generating the returnBarcode. Mandatory for Label in the Box
             (return label) shipments.
         return_reference (str): Return reference of the shipment
         timeslot_id (str): Deprecated. ID of the chosen timeslot as returned
             by the timeslot webservice
-        extra_fields (List[ExtraField]): Possibility to provide extra
-            key-value pairs to the webservice. Not used at the moment.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "addresses": 'Addresses',
         "barcode": 'Barcode',
@@ -139,16 +141,15 @@
         "product_options": 'ProductOptions',
         "receiver_date_of_birth": 'ReceiverDateOfBirth',
         "reference": 'Reference',
         "reference_collect": 'ReferenceCollect',
         "remark": 'Remark',
         "return_barcode": 'ReturnBarcode',
         "return_reference": 'ReturnReference',
-        "timeslot_id": 'TimeslotID',
-        "extra_fields": 'ExtraFields'
+        "timeslot_id": 'TimeslotID'
     }
 
     _optionals = [
         'amounts',
         'coding_text',
         'collection_time_stamp_start',
         'collection_time_stamp_end',
@@ -169,15 +170,14 @@
         'receiver_date_of_birth',
         'reference',
         'reference_collect',
         'remark',
         'return_barcode',
         'return_reference',
         'timeslot_id',
-        'extra_fields',
     ]
 
     def __init__(self,
                  addresses=None,
                  barcode=None,
                  dimension=None,
                  product_code_delivery='3085',
@@ -201,17 +201,16 @@
                  product_options=APIHelper.SKIP,
                  receiver_date_of_birth=APIHelper.SKIP,
                  reference=APIHelper.SKIP,
                  reference_collect=APIHelper.SKIP,
                  remark=APIHelper.SKIP,
                  return_barcode=APIHelper.SKIP,
                  return_reference=APIHelper.SKIP,
-                 timeslot_id=APIHelper.SKIP,
-                 extra_fields=APIHelper.SKIP):
-        """Constructor for the Shipment1 class"""
+                 timeslot_id=APIHelper.SKIP):
+        """Constructor for the Shipment class"""
 
         # Initialize members of the class
         self.addresses = addresses 
         if amounts is not APIHelper.SKIP:
             self.amounts = amounts 
         self.barcode = barcode 
         if coding_text is not APIHelper.SKIP:
@@ -260,16 +259,14 @@
             self.remark = remark 
         if return_barcode is not APIHelper.SKIP:
             self.return_barcode = return_barcode 
         if return_reference is not APIHelper.SKIP:
             self.return_reference = return_reference 
         if timeslot_id is not APIHelper.SKIP:
             self.timeslot_id = timeslot_id 
-        if extra_fields is not APIHelper.SKIP:
-            self.extra_fields = extra_fields 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
         Args:
@@ -304,15 +301,19 @@
         if dictionary.get('Contacts') is not None:
             contacts = [Contact.from_dictionary(x) for x in dictionary.get('Contacts')]
         else:
             contacts = APIHelper.SKIP
         content = dictionary.get("Content") if dictionary.get("Content") else APIHelper.SKIP
         cost_center = dictionary.get("CostCenter") if dictionary.get("CostCenter") else APIHelper.SKIP
         customer_order_number = dictionary.get("CustomerOrderNumber") if dictionary.get("CustomerOrderNumber") else APIHelper.SKIP
-        customs = Custom.from_dictionary(dictionary.get('Customs')) if 'Customs' in dictionary.keys() else APIHelper.SKIP
+        customs = None
+        if dictionary.get('Customs') is not None:
+            customs = [Custom.from_dictionary(x) for x in dictionary.get('Customs')]
+        else:
+            customs = APIHelper.SKIP
         delivery_address = dictionary.get("DeliveryAddress") if dictionary.get("DeliveryAddress") else APIHelper.SKIP
         delivery_date = dictionary.get("DeliveryDate") if dictionary.get("DeliveryDate") else APIHelper.SKIP
         down_partner_barcode = dictionary.get("DownPartnerBarcode") if dictionary.get("DownPartnerBarcode") else APIHelper.SKIP
         down_partner_id = dictionary.get("DownPartnerID") if dictionary.get("DownPartnerID") else APIHelper.SKIP
         down_partner_location = dictionary.get("DownPartnerLocation") if dictionary.get("DownPartnerLocation") else APIHelper.SKIP
         groups = None
         if dictionary.get('Groups') is not None:
@@ -333,19 +334,14 @@
         receiver_date_of_birth = dictionary.get("ReceiverDateOfBirth") if dictionary.get("ReceiverDateOfBirth") else APIHelper.SKIP
         reference = dictionary.get("Reference") if dictionary.get("Reference") else APIHelper.SKIP
         reference_collect = dictionary.get("ReferenceCollect") if dictionary.get("ReferenceCollect") else APIHelper.SKIP
         remark = dictionary.get("Remark") if dictionary.get("Remark") else APIHelper.SKIP
         return_barcode = dictionary.get("ReturnBarcode") if dictionary.get("ReturnBarcode") else APIHelper.SKIP
         return_reference = dictionary.get("ReturnReference") if dictionary.get("ReturnReference") else APIHelper.SKIP
         timeslot_id = dictionary.get("TimeslotID") if dictionary.get("TimeslotID") else APIHelper.SKIP
-        extra_fields = None
-        if dictionary.get('ExtraFields') is not None:
-            extra_fields = [ExtraField.from_dictionary(x) for x in dictionary.get('ExtraFields')]
-        else:
-            extra_fields = APIHelper.SKIP
         # Return an object of this model
         return cls(addresses,
                    barcode,
                    dimension,
                    product_code_delivery,
                    amounts,
                    coding_text,
@@ -367,9 +363,8 @@
                    product_options,
                    receiver_date_of_birth,
                    reference,
                    reference_collect,
                    remark,
                    return_barcode,
                    return_reference,
-                   timeslot_id,
-                   extra_fields)
+                   timeslot_id)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_11.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_11.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         reference (str): The customer reference belonging to the shipment
         delivery_date (str): The expected delivery date of the shipment
         dimension (Dimension1): TODO: type description here.
         address (List[Address4]): A list of addresses belonging to the
             shipment
         product_options (ProductOptions): A list of product options.
         status (Status): The current status of the shipment (see the [Status
-            codes](#tag/TandT-status-codes/Status-codes) for possible values.
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/t-t-s
+            tatus-codes/event-codes) for possible values.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "main_barcode": 'MainBarcode',
         "barcode": 'Barcode',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_2.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,25 @@
         reference (str): The customer reference belonging to the shipment
         delivery_date (str): The expected delivery date of the shipment
         dimension (Dimension1): TODO: type description here.
         amount (Amount1): The amounts belonging to the shipment
         address (List[Address4]): A list of addresses belonging to the
             shipment
         event (List[Event]): The events of the shipment. (see the [Event
-            Codes](#tag/TandT-status-codes/Event-codes) for possible values.
+            Codes](https://developer.postnl.nl/docs/#/http/reference-data/t-t-s
+            tatus-codes/event-codes) for possible values.
         expectation (Expectation): The expected delivery timeframe
         product_options (ProductOptions): A list of product options.
         status (Status): The current status of the shipment (see the [Status
-            codes](#tag/TandT-status-codes/Status-codes) for possible values.
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/t-t-s
+            tatus-codes/event-codes) for possible values.
         old_status (List[OldStatus]): A list of previous status codes (see the
-            [Status codes](#tag/TandT-status-codes/Status-codes) for possible
-            values.
+            [Status
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/t-t-s
+            tatus-codes/event-codes) for possible values.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "main_barcode": 'MainBarcode',
         "barcode": 'Barcode',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_type_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_type_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_v_22_calculate_date_delivery_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
     TODO: type model description here.
 
     Attributes:
         delivery_date (str): TODO: type description here.
         options (Options): The delivery options for which a delivery date is
             returned. Only one delivery option is specified. See [Delivery
-            Options](#tag/Reference-codes/Delivery-options) for possible
-            values.
+            Options](https://developer.postnl.nl/docs/#/http/reference-data/ref
+            erence-codes/delivery-options) for possible values.
         sustainability (Warning1): Sustainability score; see [Sustainability
-            codes](#tag/Reference-codes/Sustainability-codes) for possible
-            values.
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes/delivery-options) for possible values.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "delivery_date": 'DeliveryDate',
         "options": 'Options',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shipment_v_22_calculate_date_shipping_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shippingstatus_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
     Attributes:
         complete_status (CompleteStatus): The current status and old statuses
             of the shipment
         current_status (CurrentStatus): The current status and old statuses of
             the shipment
         warnings (List[Warning2]): Possible warnings (see [Error
-            Codes](#tag/Error-codes) for possible values)
+            Codes](https://developer.postnl.nl/docs/#/http/reference-data/error
+            -codes) for possible values)
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "complete_status": 'CompleteStatus',
         "current_status": 'CurrentStatus',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_signature.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warnings.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,51 +3,44 @@
 """
 postnlecommerce
 
 This file was automatically generated for PostNL by APIMATIC v3.0 (
  https://www.apimatic.io ).
 """
 from postnlecommerce.api_helper import APIHelper
-from postnlecommerce.models.signature import Signature
-from postnlecommerce.models.warnings import Warnings
+from postnlecommerce.models.warning_11 import Warning11
 
 
-class ShippingstatusResponseSignature(object):
+class Warnings(object):
 
-    """Implementation of the 'shippingstatusResponseSignature' model.
+    """Implementation of the 'Warnings' model.
 
     TODO: type model description here.
 
     Attributes:
-        signature (Signature): TODO: type description here.
-        warnings (Warnings): TODO: type description here.
+        warning (Warning11): TODO: type description here.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
-        "signature": 'Signature',
-        "warnings": 'Warnings'
+        "warning": 'Warning'
     }
 
     _optionals = [
-        'signature',
-        'warnings',
+        'warning',
     ]
 
     def __init__(self,
-                 signature=APIHelper.SKIP,
-                 warnings=APIHelper.SKIP):
-        """Constructor for the ShippingstatusResponseSignature class"""
+                 warning=APIHelper.SKIP):
+        """Constructor for the Warnings class"""
 
         # Initialize members of the class
-        if signature is not APIHelper.SKIP:
-            self.signature = signature 
-        if warnings is not APIHelper.SKIP:
-            self.warnings = warnings 
+        if warning is not APIHelper.SKIP:
+            self.warning = warning 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
         Args:
@@ -60,12 +53,10 @@
 
         """
 
         if dictionary is None:
             return None
 
         # Extract variables from the dictionary
-        signature = Signature.from_dictionary(dictionary.get('Signature')) if 'Signature' in dictionary.keys() else APIHelper.SKIP
-        warnings = Warnings.from_dictionary(dictionary.get('Warnings')) if 'Warnings' in dictionary.keys() else APIHelper.SKIP
+        warning = Warning11.from_dictionary(dictionary.get('Warning')) if 'Warning' in dictionary.keys() else APIHelper.SKIP
         # Return an object of this model
-        return cls(signature,
-                   warnings)
+        return cls(warning)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/shippingstatus_response_updated_shipment.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/shippingstatus_response_updated_shipment.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
     Attributes:
         barcode (str): The barcode belonging to the status update
         creation_date (str): The date of the update
         customer_number (str): The customer number
         customer_code (str): The customer code
         status (Status2): The status update. See [Status
-            codes](#tag/TandT-status-codes/Status-codes) for possible values.
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/error
+            -codes) for possible values.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "barcode": 'Barcode',
         "creation_date": 'CreationDate',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/signature.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/signature.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/status.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 
 class Status(object):
 
     """Implementation of the 'Status' model.
 
     The current status of the shipment (see the [Status
-    codes](#tag/TandT-status-codes/Status-codes) for possible values.
+    codes](https://developer.postnl.nl/docs/#/http/reference-data/t-t-status-co
+    des/event-codes) for possible values.
 
     Attributes:
         time_stamp (str): The status timestamp
         status_code (str): The status code
         status_description (str): The status description
         phase_code (str): The phase code
         phase_description (str): The phase description
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/status_2.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/status_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 
 class Status2(object):
 
     """Implementation of the 'Status2' model.
 
     The status update. See [Status
-    codes](#tag/TandT-status-codes/Status-codes) for possible values.
+    codes](https://developer.postnl.nl/docs/#/http/reference-data/error-codes)
+    for possible values.
 
     Attributes:
         timestamp (str): The timestamp of the update
         status_code (str): The status code
         status_description (str): The status description
         phase_code (str): The phase code
         phase_description (str): The phase description
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_1_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/string_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/string_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/string_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/sunday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sunday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/sunday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/sustainability.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/sustainability.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 
 class Sustainability(object):
 
     """Implementation of the 'Sustainability' model.
 
     Sustainability score; see [Sustainability
-    codes](#tag/Reference-codes/Sustainability-codes) for possible values.
+    codes](https://developer.postnl.nl/docs/#/http/reference-data/reference-cod
+    es) for possible values.
 
     Attributes:
         code (CodeEnum): Sustainability score code
         description (str): Sustainability score code description
 
     """
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/thursday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/thursday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/thursday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     TODO: type model description here.
 
     Attributes:
         mfrom (str): Format hh:mm:ss
         to (str): Format hh:mm:ss
         options (List[Option1Enum]): The delivery options applicable to the
             timeframe information. See [Delivery
-            Options](#tag/Reference-codes/Delivery-options) for possible
-            values.
+            Options](https://developer.postnl.nl/docs/#/http/reference-data/ref
+            erence-codes) for possible values.
         shipping_date (str): The date when you need to deliver the shipment to
             PostNL to ensure the expected delivery date is achieved. Will be
             returned as 'null' if not calculated
         sustainability (Sustainability): Sustainability score; see
-            [Sustainability codes](#tag/Reference-codes/Sustainability-codes)
-            for possible values.
+            [Sustainability
+            codes](https://developer.postnl.nl/docs/#/http/reference-data/refer
+            ence-codes) for possible values.
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "mfrom": 'From',
         "to": 'To',
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_response.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe_response.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframe_timeframe.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframe_timeframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     TODO: type model description here.
 
     Attributes:
         mfrom (str): The start time of the expected delivery window
         options (Options): The delivery option for which the timeframe is
             calculated. See [Delivery
-            Options](#tag/Reference-codes/Delivery-options) for possible
-            values.
+            Options](https://developer.postnl.nl/docs/#/http/reference-data/ref
+            erence-codes/delivery-options) for possible values.
         to (str): The end time of the expected delivery window
         sustainability (Warning1): Sustainability score
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframes.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/timeframes_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/timeframes_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/tuesday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/tuesday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/tuesday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_1_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/type_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/type_enum.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/type_enum.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning_2.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,47 @@
 
 This file was automatically generated for PostNL by APIMATIC v3.0 (
  https://www.apimatic.io ).
 """
 from postnlecommerce.api_helper import APIHelper
 
 
-class Warning1(object):
+class Warning2(object):
 
-    """Implementation of the 'Warning1' model.
+    """Implementation of the 'Warning2' model.
 
-    Sustainability score; see [Sustainability
-    codes](#tag/Reference-codes/Sustainability-codes) for possible values.
+    TODO: type model description here.
 
     Attributes:
-        code (str): The Warning code
-        description (str): The warning description
+        message (str): The warning message
+        code (str): The warning code
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
-        "code": 'Code',
-        "description": 'Description'
+        "message": 'Message',
+        "code": 'Code'
     }
 
     _optionals = [
+        'message',
         'code',
-        'description',
     ]
 
     def __init__(self,
-                 code=APIHelper.SKIP,
-                 description=APIHelper.SKIP):
-        """Constructor for the Warning1 class"""
+                 message=APIHelper.SKIP,
+                 code=APIHelper.SKIP):
+        """Constructor for the Warning2 class"""
 
         # Initialize members of the class
+        if message is not APIHelper.SKIP:
+            self.message = message 
         if code is not APIHelper.SKIP:
             self.code = code 
-        if description is not APIHelper.SKIP:
-            self.description = description 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
         Args:
@@ -59,12 +58,12 @@
 
         """
 
         if dictionary is None:
             return None
 
         # Extract variables from the dictionary
+        message = dictionary.get("Message") if dictionary.get("Message") else APIHelper.SKIP
         code = dictionary.get("Code") if dictionary.get("Code") else APIHelper.SKIP
-        description = dictionary.get("Description") if dictionary.get("Description") else APIHelper.SKIP
         # Return an object of this model
-        return cls(code,
-                   description)
+        return cls(message,
+                   code)
```

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/warning_11.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/warning_11.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/wednesday.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/models/wednesday_1.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/models/wednesday_1.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/postnlecommerce/postnlecommerce_client.py` & `postnl_ecommerce_sdk-1.0.3/postnlecommerce/postnlecommerce_client.py`

 * *Files identical despite different names*

### Comparing `postnl_ecommerce_sdk-1.0.2/pyproject.toml` & `postnl_ecommerce_sdk-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "postnl-ecommerce-sdk"
 description = "Collection of PostNL API's for ecommerce processes."
-version = "1.0.2"
+version = "1.0.3"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["PostNL", "SDK", "API", "ecommerce"]
 authors = [{name = "PostNL", email = "apimatic@postnl.nl"}]
 urls = {Documentation = "https://developer.postnl.nl/docs"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "enum34~=1.1, >=1.1.10"]
 classifiers = []
```

