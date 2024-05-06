# Comparing `tmp/ksc-sdk-python-1.3.64.tar.gz` & `tmp/ksc-sdk-python-1.3.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ksc-sdk-python-1.3.64.tar", last modified: Wed Oct 18 10:38:51 2023, max compression
+gzip compressed data, was "dist/ksc-sdk-python-1.3.65.tar", last modified: Mon May  6 01:17:31 2024, max compression
```

## Comparing `ksc-sdk-python-1.3.64.tar` & `ksc-sdk-python-1.3.65.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/
--rw-r--r--   0 root         (0) root         (0)    10582 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6956 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/cmd-runner
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/acceptance/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/steps/
--rw-r--r--   0 root         (0) root         (0)     3649 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/steps/base.py
--rw-r--r--   0 root         (0) root         (0)     1311 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/smoke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/smoke/iam/
--rw-r--r--   0 root         (0) root         (0)        1 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/acceptance/features/smoke/iam/iam.feature
--rw-r--r--   0 root         (0) root         (0)       58 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.64/tests/acceptance/.kscore.cfg
--rw-r--r--   0 root         (0) root         (0)       57 2019-12-26 03:11:33.000000 ksc-sdk-python-1.3.64/tests/.kscore.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/tests/integration/
--rw-r--r--   0 root         (0) root         (0)      637 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2531 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/integration/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2400 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/integration/test_loaders.py
--rw-r--r--   0 root         (0) root         (0)     1508 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/integration/test_session.py
--rw-r--r--   0 root         (0) root         (0)     1228 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/tests/integration/test_kog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/
--rw-r--r--   0 root         (0) root         (0)        0 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27344 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/six.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/
--rw-r--r--   0 root         (0) root         (0)      820 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/hooks.py
--rw-r--r--   0 root         (0) root         (0)     1861 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      613 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/certs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/
--rw-r--r--   0 root         (0) root         (0)       62 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/
--rw-r--r--   0 root         (0) root         (0)    13359 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/hebrewprober.py
--rw-r--r--   0 root         (0) root         (0)    36011 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/gb2312freq.py
--rw-r--r--   0 root         (0) root         (0)     1295 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/big5prober.py
--rw-r--r--   0 root         (0) root         (0)     3268 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/mbcharsetprober.py
--rw-r--r--   0 root         (0) root         (0)    34872 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euctwfreq.py
--rw-r--r--   0 root         (0) root         (0)    11318 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langhebrewmodel.py
--rw-r--r--   0 root         (0) root         (0)     1782 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/cp949prober.py
--rw-r--r--   0 root         (0) root         (0)    19348 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/jpcntx.py
--rw-r--r--   0 root         (0) root         (0)     3791 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/charsetgroupprober.py
--rw-r--r--   0 root         (0) root         (0)    17725 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langcyrillicmodel.py
--rw-r--r--   0 root         (0) root         (0)     6840 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/universaldetector.py
--rw-r--r--   0 root         (0) root         (0)     1967 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/mbcsgroupprober.py
--rw-r--r--   0 root         (0) root         (0)    12628 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langgreekmodel.py
--rw-r--r--   0 root         (0) root         (0)     3187 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/escprober.py
--rw-r--r--   0 root         (0) root         (0)     2504 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/chardetect.py
--rw-r--r--   0 root         (0) root         (0)     2652 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/utf8prober.py
--rw-r--r--   0 root         (0) root         (0)     1681 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/gb2312prober.py
--rw-r--r--   0 root         (0) root         (0)     2318 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/codingstatemachine.py
--rw-r--r--   0 root         (0) root         (0)     1157 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/compat.py
--rw-r--r--   0 root         (0) root         (0)     3678 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/eucjpprober.py
--rw-r--r--   0 root         (0) root         (0)    82594 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/big5freq.py
--rw-r--r--   0 root         (0) root         (0)     1335 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/constants.py
--rw-r--r--   0 root         (0) root         (0)    12784 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langbulgarianmodel.py
--rw-r--r--   0 root         (0) root         (0)    12536 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langhungarianmodel.py
--rw-r--r--   0 root         (0) root         (0)     3764 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/sjisprober.py
--rw-r--r--   0 root         (0) root         (0)    47315 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/jisfreq.py
--rw-r--r--   0 root         (0) root         (0)     3291 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/sbcsgroupprober.py
--rw-r--r--   0 root         (0) root         (0)     1676 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euctwprober.py
--rw-r--r--   0 root         (0) root         (0)    11275 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langthaimodel.py
--rw-r--r--   0 root         (0) root         (0)     1902 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/charsetprober.py
--rw-r--r--   0 root         (0) root         (0)     4793 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/sbcharsetprober.py
--rw-r--r--   0 root         (0) root         (0)    19590 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/mbcssm.py
--rw-r--r--   0 root         (0) root         (0)     7839 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/escsm.py
--rw-r--r--   0 root         (0) root         (0)     1675 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euckrprober.py
--rw-r--r--   0 root         (0) root         (0)     9226 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/chardistribution.py
--rw-r--r--   0 root         (0) root         (0)     5232 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/latin1prober.py
--rw-r--r--   0 root         (0) root         (0)    45978 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euckrfreq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/
--rw-r--r--   0 root         (0) root         (0)     2055 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5751 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/request.py
--rw-r--r--   0 root         (0) root         (0)    30319 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/connectionpool.py
--rw-r--r--   0 root         (0) root         (0)     5833 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/
--rw-r--r--   0 root         (0) root         (0)       74 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/six.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 root         (0) root         (0)      460 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3778 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 root         (0) root         (0)     8935 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     9011 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/connection.py
--rw-r--r--   0 root         (0) root         (0)    10454 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/_collections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/contrib/
--rw-r--r--   0 root         (0) root         (0)        0 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9326 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 root         (0) root         (0)     4507 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 root         (0) root         (0)     4374 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9406 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/poolmanager.py
--rw-r--r--   0 root         (0) root         (0)    16459 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/
--rw-r--r--   0 root         (0) root         (0)      486 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2089 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/request.py
--rw-r--r--   0 root         (0) root         (0)     5836 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/url.py
--rw-r--r--   0 root         (0) root         (0)     3293 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/connection.py
--rw-r--r--   0 root         (0) root         (0)     9544 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/timeout.py
--rw-r--r--   0 root         (0) root         (0)      566 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/response.py
--rw-r--r--   0 root         (0) root         (0)     9924 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/retry.py
--rw-r--r--   0 root         (0) root         (0)    10037 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/ssl_.py
--rw-r--r--   0 root         (0) root         (0)     2281 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/filepost.py
--rw-r--r--   0 root         (0) root         (0)    17191 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/cookies.py
--rw-r--r--   0 root         (0) root         (0)     2517 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/exceptions.py
--rw-r--r--   0 root         (0) root         (0)   344712 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/cacert.pem
--rw-r--r--   0 root         (0) root         (0)     3200 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/status_codes.py
--rw-r--r--   0 root         (0) root         (0)    24250 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/sessions.py
--rw-r--r--   0 root         (0) root         (0)     5415 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/api.py
--rw-r--r--   0 root         (0) root         (0)     1469 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/compat.py
--rw-r--r--   0 root         (0) root         (0)    29176 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/models.py
--rw-r--r--   0 root         (0) root         (0)     6794 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/auth.py
--rw-r--r--   0 root         (0) root         (0)    21334 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/utils.py
--rw-r--r--   0 root         (0) root         (0)    16810 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/adapters.py
--rw-r--r--   0 root         (0) root         (0)     2977 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/vendored/requests/structures.py
--rw-r--r--   0 root         (0) root         (0)    13619 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/retryhandler.py
--rw-r--r--   0 root         (0) root         (0)    20817 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/hooks.py
--rw-r--r--   0 root         (0) root         (0)    39552 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/credentials.py
--rw-r--r--   0 root         (0) root         (0)     8527 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/regions.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.64/kscore/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2418 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/offline.py
--rw-r--r--   0 root         (0) root         (0)    11004 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/endpoint.py
--rw-r--r--   0 root         (0) root         (0)     3915 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/kls.py
--rw-r--r--   0 root         (0) root         (0)    35082 2021-01-05 13:55:33.000000 ksc-sdk-python-1.3.64/kscore/client.py
--rw-r--r--   0 root         (0) root         (0)    20517 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/paginate.py
--rw-r--r--   0 root         (0) root         (0)     6261 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/config.py
--rw-r--r--   0 root         (0) root         (0)    12177 2019-08-30 16:02:40.000000 ksc-sdk-python-1.3.64/kscore/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3879 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.64/kscore/kvs.py
--rw-r--r--   0 root         (0) root         (0)     4765 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/response.py
--rw-r--r--   0 root         (0) root         (0)    11896 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/waiter.py
--rw-r--r--   0 root         (0) root         (0)    18661 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/ksrequest.py
--rw-r--r--   0 root         (0) root         (0)     9267 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/compat.py
--rw-r--r--   0 root         (0) root         (0)     2758 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/ket.py
--rw-r--r--   0 root         (0) root         (0)    29906 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/docs/
--rw-r--r--   0 root         (0) root         (0)     1550 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4579 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/client.py
--rw-r--r--   0 root         (0) root         (0)     8952 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/params.py
--rw-r--r--   0 root         (0) root         (0)     3685 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/docstring.py
--rw-r--r--   0 root         (0) root         (0)     3448 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/service.py
--rw-r--r--   0 root         (0) root         (0)     8337 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/
--rw-r--r--   0 root         (0) root         (0)      597 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4742 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/docevents.py
--rw-r--r--   0 root         (0) root         (0)    20560 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/textwriter.py
--rw-r--r--   0 root         (0) root         (0)     5896 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/docstringparser.py
--rw-r--r--   0 root         (0) root         (0)    10938 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/style.py
--rw-r--r--   0 root         (0) root         (0)     7229 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/bcdoc/restdoc.py
--rw-r--r--   0 root         (0) root         (0)     3828 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/waiter.py
--rw-r--r--   0 root         (0) root         (0)     6712 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/utils.py
--rw-r--r--   0 root         (0) root         (0)     4495 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/shape.py
--rw-r--r--   0 root         (0) root         (0)     6975 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/paginator.py
--rw-r--r--   0 root         (0) root         (0)     9222 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/sharedexample.py
--rw-r--r--   0 root         (0) root         (0)     9798 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/docs/method.py
--rw-r--r--   0 root         (0) root         (0)    23427 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/signers.py
--rw-r--r--   0 root         (0) root         (0)    28629 2019-12-11 02:51:26.000000 ksc-sdk-python-1.3.64/kscore/utils.py
--rw-r--r--   0 root         (0) root         (0)    35248 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/handlers.py
--rw-r--r--   0 root         (0) root         (0)    32639 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/parsers.py
--rw-r--r--   0 root         (0) root         (0)    38773 2021-01-05 13:55:33.000000 ksc-sdk-python-1.3.64/kscore/session.py
--rw-r--r--   0 root         (0) root         (0)    31248 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/offline/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/offline/2016-09-19/
--rw-r--r--   0 root         (0) root         (0)     2585 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/offline/2016-09-19/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kec/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)     4324 2021-07-26 10:16:34.000000 ksc-sdk-python-1.3.64/kscore/data/kec/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/cdnv2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/cdnv2/2018-01-01/
--rw-r--r--   0 root         (0) root         (0)     2210 2019-12-26 03:11:33.000000 ksc-sdk-python-1.3.64/kscore/data/cdnv2/2018-01-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/vpc/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)     8012 2020-08-11 09:00:01.000000 ksc-sdk-python-1.3.64/kscore/data/vpc/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/ket/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/ket/2017-01-01/
--rw-r--r--   0 root         (0) root         (0)     2509 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/ket/2017-01-01/service-2.yaml
--rw-r--r--   0 root         (0) root         (0)     1392 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/_retry.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/krtpay/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/krtpay/2019-07-19/
--rw-r--r--   0 root         (0) root         (0)      415 2020-07-15 06:39:00.000000 ksc-sdk-python-1.3.64/kscore/data/krtpay/2019-07-19/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kvs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kvs/2017-01-01/
--rw-r--r--   0 root         (0) root         (0)     4728 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.64/kscore/data/kvs/2017-01-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/bill-union/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/bill-union/2020-01-01/
--rw-r--r--   0 root         (0) root         (0)      524 2020-12-07 15:38:22.000000 ksc-sdk-python-1.3.64/kscore/data/bill-union/2020-01-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/monitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/monitor/2010-05-25/
--rw-r--r--   0 root         (0) root         (0)      893 2019-11-28 06:32:47.000000 ksc-sdk-python-1.3.64/kscore/data/monitor/2010-05-25/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/ebs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/ebs/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)     1095 2021-03-24 08:40:22.000000 ksc-sdk-python-1.3.64/kscore/data/ebs/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/tag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/tag/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)      436 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/tag/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kis/2018-09-01/
--rw-r--r--   0 root         (0) root         (0)     4099 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/kis/2018-09-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/bill/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/bill/2018-06-01/
--rw-r--r--   0 root         (0) root         (0)      354 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/bill/2018-06-01/service-2.yaml
--rw-r--r--   0 root         (0) root         (0)     5055 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.64/kscore/data/endpoints.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/slb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/slb/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)     4190 2020-08-11 09:00:01.000000 ksc-sdk-python-1.3.64/kscore/data/slb/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/monitorv2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/monitorv2/2021-01-01/
--rw-r--r--   0 root         (0) root         (0)     1176 2021-09-16 07:32:07.000000 ksc-sdk-python-1.3.64/kscore/data/monitorv2/2021-01-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/krds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/krds/2016-07-01/
--rw-r--r--   0 root         (0) root         (0)     3575 2020-07-07 10:59:42.000000 ksc-sdk-python-1.3.64/kscore/data/krds/2016-07-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/postgresql/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/postgresql/2018-12-25/
--rw-r--r--   0 root         (0) root         (0)     2926 2020-07-07 10:59:42.000000 ksc-sdk-python-1.3.64/kscore/data/postgresql/2018-12-25/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/cdn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/cdn/2016-09-01/
--rw-r--r--   0 root         (0) root         (0)    86372 2020-12-07 15:38:22.000000 ksc-sdk-python-1.3.64/kscore/data/cdn/2016-09-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kkms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kkms/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)      560 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/kkms/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kingpay/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kingpay/V1/
--rw-r--r--   0 root         (0) root         (0)      266 2020-08-06 09:18:48.000000 ksc-sdk-python-1.3.64/kscore/data/kingpay/V1/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/iam/2015-11-01/
--rw-r--r--   0 root         (0) root         (0)     5391 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/iam/2015-11-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kmr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kmr/2021-09-02/
--rw-r--r--   0 root         (0) root         (0)      932 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.64/kscore/data/kmr/2021-09-02/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/eip/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/eip/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)     1215 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/eip/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcm/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)      769 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/kcm/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kls/2017-01-01/
--rw-r--r--   0 root         (0) root         (0)     5410 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/kls/2017-01-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/bws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/bws/2016-03-04/
--rw-r--r--   0 root         (0) root         (0)     1127 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/bws/2016-03-04/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/contact/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/contact/2021-07-08/
--rw-r--r--   0 root         (0) root         (0)      269 2021-07-20 04:30:43.000000 ksc-sdk-python-1.3.64/kscore/data/contact/2021-07-08/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/sks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/sks/2015-11-01/
--rw-r--r--   0 root         (0) root         (0)      516 2019-08-30 08:08:30.000000 ksc-sdk-python-1.3.64/kscore/data/sks/2015-11-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kes/2020-12-15/
--rw-r--r--   0 root         (0) root         (0)     1081 2022-08-02 03:32:28.000000 ksc-sdk-python-1.3.64/kscore/data/kes/2020-12-15/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kce/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kce/2019-08-06/
--rw-r--r--   0 root         (0) root         (0)     2317 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.64/kscore/data/kce/2019-08-06/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/trade/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/trade/2020-01-14/
--rw-r--r--   0 root         (0) root         (0)      264 2020-08-06 09:18:48.000000 ksc-sdk-python-1.3.64/kscore/data/trade/2020-01-14/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/dns/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/dns/2016-06-07/
--rw-r--r--   0 root         (0) root         (0)     1444 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/dns/2016-06-07/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/epc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/epc/2015-11-01/
--rw-r--r--   0 root         (0) root         (0)     4038 2020-04-21 11:23:01.000000 ksc-sdk-python-1.3.64/kscore/data/epc/2015-11-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcev2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcev2/2020-12-31/
--rw-r--r--   0 root         (0) root         (0)      282 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.64/kscore/data/kcev2/2020-12-31/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcsv2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcsv2/2017-04-01/
--rw-r--r--   0 root         (0) root         (0)      542 2020-10-28 06:25:50.000000 ksc-sdk-python-1.3.64/kscore/data/kcsv2/2017-04-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/mongodb/2017-01-01/
--rw-r--r--   0 root         (0) root         (0)     1914 2019-09-27 10:15:27.000000 ksc-sdk-python-1.3.64/kscore/data/mongodb/2017-01-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/cdnv3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/cdnv3/2020-06-30/
--rw-r--r--   0 root         (0) root         (0)      593 2023-03-22 08:00:08.000000 ksc-sdk-python-1.3.64/kscore/data/cdnv3/2020-06-30/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcs/2016-07-01/
--rw-r--r--   0 root         (0) root         (0)     3527 2020-10-28 06:25:50.000000 ksc-sdk-python-1.3.64/kscore/data/kcs/2016-07-01/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kcrs/2021-11-09/
--rw-r--r--   0 root         (0) root         (0)     2467 2022-08-02 03:32:28.000000 ksc-sdk-python-1.3.64/kscore/data/kcrs/2021-11-09/service-2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/kscore/data/kog/2016-08-08/
--rw-r--r--   0 root         (0) root         (0)    37343 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/data/kog/2016-08-08/service-2.yaml
--rw-r--r--   0 root         (0) root         (0)    23525 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/model.py
--rw-r--r--   0 root         (0) root         (0)    16857 2021-01-07 10:21:13.000000 ksc-sdk-python-1.3.64/kscore/loaders.py
--rw-r--r--   0 root         (0) root         (0)    10249 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/validate.py
--rw-r--r--   0 root         (0) root         (0)    21991 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/translate.py
--rw-r--r--   0 root         (0) root         (0)     3467 2020-04-30 05:45:38.000000 ksc-sdk-python-1.3.64/kscore/domain.py
--rw-r--r--   0 root         (0) root         (0)     8324 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/configloader.py
--rw-r--r--   0 root         (0) root         (0)     9500 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.64/kscore/stub.py
--rw-r--r--   0 root         (0) root         (0)    10583 2021-12-24 02:16:50.000000 ksc-sdk-python-1.3.64/README.rst
--rw-r--r--   0 root         (0) root         (0)     1154 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1154 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     7844 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-10-18 10:38:51.000000 ksc-sdk-python-1.3.64/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      192 2019-07-03 08:51:17.000000 ksc-sdk-python-1.3.64/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      150 2021-11-18 07:49:03.000000 ksc-sdk-python-1.3.64/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2656 2021-11-18 07:49:03.000000 ksc-sdk-python-1.3.64/setup.py
--rw-r--r--   0 root         (0) root         (0)      637 2019-07-03 08:51:17.000000 ksc-sdk-python-1.3.64/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/
+-rw-r--r--   0 root         (0) root         (0)    10582 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6956 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/cmd-runner
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/acceptance/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/steps/
+-rw-r--r--   0 root         (0) root         (0)     3649 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/steps/base.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/smoke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/smoke/iam/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/acceptance/features/smoke/iam/iam.feature
+-rw-r--r--   0 root         (0) root         (0)       58 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.65/tests/acceptance/.kscore.cfg
+-rw-r--r--   0 root         (0) root         (0)       57 2019-12-26 03:11:33.000000 ksc-sdk-python-1.3.65/tests/.kscore.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)      637 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/integration/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/integration/test_loaders.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/integration/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/tests/integration/test_kog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27344 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/six.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/
+-rw-r--r--   0 root         (0) root         (0)      820 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      613 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/certs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/
+-rw-r--r--   0 root         (0) root         (0)       62 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/
+-rw-r--r--   0 root         (0) root         (0)    13359 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/hebrewprober.py
+-rw-r--r--   0 root         (0) root         (0)    36011 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/gb2312freq.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/big5prober.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/mbcharsetprober.py
+-rw-r--r--   0 root         (0) root         (0)    34872 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euctwfreq.py
+-rw-r--r--   0 root         (0) root         (0)    11318 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langhebrewmodel.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/cp949prober.py
+-rw-r--r--   0 root         (0) root         (0)    19348 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/jpcntx.py
+-rw-r--r--   0 root         (0) root         (0)     3791 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/charsetgroupprober.py
+-rw-r--r--   0 root         (0) root         (0)    17725 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langcyrillicmodel.py
+-rw-r--r--   0 root         (0) root         (0)     6840 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/universaldetector.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/mbcsgroupprober.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langgreekmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/escprober.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/chardetect.py
+-rw-r--r--   0 root         (0) root         (0)     2652 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/utf8prober.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/gb2312prober.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/codingstatemachine.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/compat.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/eucjpprober.py
+-rw-r--r--   0 root         (0) root         (0)    82594 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/big5freq.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/constants.py
+-rw-r--r--   0 root         (0) root         (0)    12784 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langbulgarianmodel.py
+-rw-r--r--   0 root         (0) root         (0)    12536 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langhungarianmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/sjisprober.py
+-rw-r--r--   0 root         (0) root         (0)    47315 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/jisfreq.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/sbcsgroupprober.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euctwprober.py
+-rw-r--r--   0 root         (0) root         (0)    11275 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langthaimodel.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/charsetprober.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/sbcharsetprober.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/mbcssm.py
+-rw-r--r--   0 root         (0) root         (0)     7839 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/escsm.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euckrprober.py
+-rw-r--r--   0 root         (0) root         (0)     9226 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/chardistribution.py
+-rw-r--r--   0 root         (0) root         (0)     5232 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/latin1prober.py
+-rw-r--r--   0 root         (0) root         (0)    45978 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euckrfreq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/
+-rw-r--r--   0 root         (0) root         (0)     2055 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5751 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/request.py
+-rw-r--r--   0 root         (0) root         (0)    30319 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/connectionpool.py
+-rw-r--r--   0 root         (0) root         (0)     5833 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/
+-rw-r--r--   0 root         (0) root         (0)       74 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/six.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 root         (0) root         (0)      460 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3778 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     8935 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     9011 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/connection.py
+-rw-r--r--   0 root         (0) root         (0)    10540 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/_collections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/contrib/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9326 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 root         (0) root         (0)     4374 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9406 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/poolmanager.py
+-rw-r--r--   0 root         (0) root         (0)    16459 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/
+-rw-r--r--   0 root         (0) root         (0)      486 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/request.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/url.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/connection.py
+-rw-r--r--   0 root         (0) root         (0)     9544 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/timeout.py
+-rw-r--r--   0 root         (0) root         (0)      566 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/response.py
+-rw-r--r--   0 root         (0) root         (0)     9924 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/retry.py
+-rw-r--r--   0 root         (0) root         (0)    10037 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/filepost.py
+-rw-r--r--   0 root         (0) root         (0)    17315 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/cookies.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)   344712 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/cacert.pem
+-rw-r--r--   0 root         (0) root         (0)     3200 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)    24388 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/sessions.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/api.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/compat.py
+-rw-r--r--   0 root         (0) root         (0)    29176 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/models.py
+-rw-r--r--   0 root         (0) root         (0)     6794 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/auth.py
+-rw-r--r--   0 root         (0) root         (0)    21458 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16810 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/adapters.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/vendored/requests/structures.py
+-rw-r--r--   0 root         (0) root         (0)    13619 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/retryhandler.py
+-rw-r--r--   0 root         (0) root         (0)    20817 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/hooks.py
+-rw-r--r--   0 root         (0) root         (0)    39552 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/credentials.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/regions.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/offline.py
+-rw-r--r--   0 root         (0) root         (0)    11004 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/kls.py
+-rw-r--r--   0 root         (0) root         (0)    35082 2021-01-05 13:55:33.000000 ksc-sdk-python-1.3.65/kscore/client.py
+-rw-r--r--   0 root         (0) root         (0)    20517 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/paginate.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/config.py
+-rw-r--r--   0 root         (0) root         (0)    12177 2019-08-30 16:02:40.000000 ksc-sdk-python-1.3.65/kscore/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3879 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.65/kscore/kvs.py
+-rw-r--r--   0 root         (0) root         (0)     4765 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/response.py
+-rw-r--r--   0 root         (0) root         (0)    11896 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/waiter.py
+-rw-r--r--   0 root         (0) root         (0)    18661 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/ksrequest.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/compat.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/ket.py
+-rw-r--r--   0 root         (0) root         (0)    29906 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/docs/
+-rw-r--r--   0 root         (0) root         (0)     1550 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/client.py
+-rw-r--r--   0 root         (0) root         (0)     8952 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/params.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/docstring.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/service.py
+-rw-r--r--   0 root         (0) root         (0)     8337 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/
+-rw-r--r--   0 root         (0) root         (0)      597 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4742 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/docevents.py
+-rw-r--r--   0 root         (0) root         (0)    20560 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/textwriter.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/docstringparser.py
+-rw-r--r--   0 root         (0) root         (0)    10938 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/style.py
+-rw-r--r--   0 root         (0) root         (0)     7229 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/bcdoc/restdoc.py
+-rw-r--r--   0 root         (0) root         (0)     3828 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/shape.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/paginator.py
+-rw-r--r--   0 root         (0) root         (0)     9222 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/sharedexample.py
+-rw-r--r--   0 root         (0) root         (0)     9798 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/docs/method.py
+-rw-r--r--   0 root         (0) root         (0)    23427 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/signers.py
+-rw-r--r--   0 root         (0) root         (0)    28629 2019-12-11 02:51:26.000000 ksc-sdk-python-1.3.65/kscore/utils.py
+-rw-r--r--   0 root         (0) root         (0)    35248 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/handlers.py
+-rw-r--r--   0 root         (0) root         (0)    32639 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/parsers.py
+-rw-r--r--   0 root         (0) root         (0)    38773 2021-01-05 13:55:33.000000 ksc-sdk-python-1.3.65/kscore/session.py
+-rw-r--r--   0 root         (0) root         (0)    31248 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/offline/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/offline/2016-09-19/
+-rw-r--r--   0 root         (0) root         (0)     2585 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/offline/2016-09-19/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kec/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)     4324 2021-07-26 10:16:34.000000 ksc-sdk-python-1.3.65/kscore/data/kec/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/cdnv2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/cdnv2/2018-01-01/
+-rw-r--r--   0 root         (0) root         (0)     2210 2019-12-26 03:11:33.000000 ksc-sdk-python-1.3.65/kscore/data/cdnv2/2018-01-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/vpc/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)     8012 2020-08-11 09:00:01.000000 ksc-sdk-python-1.3.65/kscore/data/vpc/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/ket/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/ket/2017-01-01/
+-rw-r--r--   0 root         (0) root         (0)     2509 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/ket/2017-01-01/service-2.yaml
+-rw-r--r--   0 root         (0) root         (0)     1392 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/_retry.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/krtpay/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/krtpay/2019-07-19/
+-rw-r--r--   0 root         (0) root         (0)      415 2020-07-15 06:39:00.000000 ksc-sdk-python-1.3.65/kscore/data/krtpay/2019-07-19/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kvs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kvs/2017-01-01/
+-rw-r--r--   0 root         (0) root         (0)     4728 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.65/kscore/data/kvs/2017-01-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/bill-union/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/bill-union/2020-01-01/
+-rw-r--r--   0 root         (0) root         (0)      524 2020-12-07 15:38:22.000000 ksc-sdk-python-1.3.65/kscore/data/bill-union/2020-01-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/monitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/monitor/2010-05-25/
+-rw-r--r--   0 root         (0) root         (0)      893 2019-11-28 06:32:47.000000 ksc-sdk-python-1.3.65/kscore/data/monitor/2010-05-25/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/ebs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/ebs/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)     1095 2021-03-24 08:40:22.000000 ksc-sdk-python-1.3.65/kscore/data/ebs/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/tag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/tag/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)      436 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/tag/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kis/2018-09-01/
+-rw-r--r--   0 root         (0) root         (0)     4099 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/kis/2018-09-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/bill/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/bill/2018-06-01/
+-rw-r--r--   0 root         (0) root         (0)      354 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/bill/2018-06-01/service-2.yaml
+-rw-r--r--   0 root         (0) root         (0)     5055 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.65/kscore/data/endpoints.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/slb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/slb/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)     4190 2020-08-11 09:00:01.000000 ksc-sdk-python-1.3.65/kscore/data/slb/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/monitorv2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/monitorv2/2021-01-01/
+-rw-r--r--   0 root         (0) root         (0)     1176 2021-09-16 07:32:07.000000 ksc-sdk-python-1.3.65/kscore/data/monitorv2/2021-01-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/krds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/krds/2016-07-01/
+-rw-r--r--   0 root         (0) root         (0)     3575 2020-07-07 10:59:42.000000 ksc-sdk-python-1.3.65/kscore/data/krds/2016-07-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/postgresql/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/postgresql/2018-12-25/
+-rw-r--r--   0 root         (0) root         (0)     2926 2020-07-07 10:59:42.000000 ksc-sdk-python-1.3.65/kscore/data/postgresql/2018-12-25/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/cdn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/cdn/2016-09-01/
+-rw-r--r--   0 root         (0) root         (0)    86372 2020-12-07 15:38:22.000000 ksc-sdk-python-1.3.65/kscore/data/cdn/2016-09-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kkms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kkms/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)      560 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/kkms/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kingpay/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kingpay/V1/
+-rw-r--r--   0 root         (0) root         (0)      266 2020-08-06 09:18:48.000000 ksc-sdk-python-1.3.65/kscore/data/kingpay/V1/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/iam/2015-11-01/
+-rw-r--r--   0 root         (0) root         (0)     5391 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/iam/2015-11-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kmr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kmr/2021-09-02/
+-rw-r--r--   0 root         (0) root         (0)      932 2023-10-18 10:30:04.000000 ksc-sdk-python-1.3.65/kscore/data/kmr/2021-09-02/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/eip/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/eip/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)     1215 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/eip/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcm/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)      769 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/kcm/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kls/2017-01-01/
+-rw-r--r--   0 root         (0) root         (0)     5410 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/kls/2017-01-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/bws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/bws/2016-03-04/
+-rw-r--r--   0 root         (0) root         (0)     1127 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/bws/2016-03-04/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/contact/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/contact/2021-07-08/
+-rw-r--r--   0 root         (0) root         (0)      269 2021-07-20 04:30:43.000000 ksc-sdk-python-1.3.65/kscore/data/contact/2021-07-08/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/sks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/sks/2015-11-01/
+-rw-r--r--   0 root         (0) root         (0)      516 2019-08-30 08:08:30.000000 ksc-sdk-python-1.3.65/kscore/data/sks/2015-11-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kes/2020-12-15/
+-rw-r--r--   0 root         (0) root         (0)     1081 2022-08-02 03:32:28.000000 ksc-sdk-python-1.3.65/kscore/data/kes/2020-12-15/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kce/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kce/2019-08-06/
+-rw-r--r--   0 root         (0) root         (0)     2317 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.65/kscore/data/kce/2019-08-06/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/trade/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/trade/2020-01-14/
+-rw-r--r--   0 root         (0) root         (0)      264 2020-08-06 09:18:48.000000 ksc-sdk-python-1.3.65/kscore/data/trade/2020-01-14/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/dns/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/dns/2016-06-07/
+-rw-r--r--   0 root         (0) root         (0)     1444 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/dns/2016-06-07/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/epc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/epc/2015-11-01/
+-rw-r--r--   0 root         (0) root         (0)     4038 2020-04-21 11:23:01.000000 ksc-sdk-python-1.3.65/kscore/data/epc/2015-11-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcev2/2020-12-31/
+-rw-r--r--   0 root         (0) root         (0)      282 2021-10-13 07:03:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcev2/2020-12-31/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcsv2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcsv2/2017-04-01/
+-rw-r--r--   0 root         (0) root         (0)      542 2020-10-28 06:25:50.000000 ksc-sdk-python-1.3.65/kscore/data/kcsv2/2017-04-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/mongodb/2017-01-01/
+-rw-r--r--   0 root         (0) root         (0)     1914 2019-09-27 10:15:27.000000 ksc-sdk-python-1.3.65/kscore/data/mongodb/2017-01-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/cdnv3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/cdnv3/2020-06-30/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-03-22 08:00:08.000000 ksc-sdk-python-1.3.65/kscore/data/cdnv3/2020-06-30/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcs/2016-07-01/
+-rw-r--r--   0 root         (0) root         (0)     3527 2020-10-28 06:25:50.000000 ksc-sdk-python-1.3.65/kscore/data/kcs/2016-07-01/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kcrs/2021-11-09/
+-rw-r--r--   0 root         (0) root         (0)     2467 2022-08-02 03:32:28.000000 ksc-sdk-python-1.3.65/kscore/data/kcrs/2021-11-09/service-2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/kscore/data/kog/2016-08-08/
+-rw-r--r--   0 root         (0) root         (0)    37343 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/data/kog/2016-08-08/service-2.yaml
+-rw-r--r--   0 root         (0) root         (0)    23525 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/model.py
+-rw-r--r--   0 root         (0) root         (0)    16857 2021-01-07 10:21:13.000000 ksc-sdk-python-1.3.65/kscore/loaders.py
+-rw-r--r--   0 root         (0) root         (0)    10249 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/validate.py
+-rw-r--r--   0 root         (0) root         (0)    21991 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/translate.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2020-04-30 05:45:38.000000 ksc-sdk-python-1.3.65/kscore/domain.py
+-rw-r--r--   0 root         (0) root         (0)     8324 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/configloader.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2019-07-03 08:51:18.000000 ksc-sdk-python-1.3.65/kscore/stub.py
+-rw-r--r--   0 root         (0) root         (0)    10583 2021-12-24 02:16:50.000000 ksc-sdk-python-1.3.65/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     7844 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-06 01:17:31.000000 ksc-sdk-python-1.3.65/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      192 2019-07-03 08:51:17.000000 ksc-sdk-python-1.3.65/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      150 2021-11-18 07:49:03.000000 ksc-sdk-python-1.3.65/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2656 2021-11-18 07:49:03.000000 ksc-sdk-python-1.3.65/setup.py
+-rw-r--r--   0 root         (0) root         (0)      637 2019-07-03 08:51:17.000000 ksc-sdk-python-1.3.65/LICENSE.txt
```

### Comparing `ksc-sdk-python-1.3.64/tests/__init__.py` & `ksc-sdk-python-1.3.65/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/cmd-runner` & `ksc-sdk-python-1.3.65/tests/cmd-runner`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/acceptance/features/steps/base.py` & `ksc-sdk-python-1.3.65/tests/acceptance/features/steps/base.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/acceptance/features/environment.py` & `ksc-sdk-python-1.3.65/tests/acceptance/features/environment.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/integration/__init__.py` & `ksc-sdk-python-1.3.65/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/integration/test_utils.py` & `ksc-sdk-python-1.3.65/tests/integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/integration/test_loaders.py` & `ksc-sdk-python-1.3.65/tests/integration/test_loaders.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/integration/test_session.py` & `ksc-sdk-python-1.3.65/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/tests/integration/test_kog.py` & `ksc-sdk-python-1.3.65/tests/integration/test_kog.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/six.py` & `ksc-sdk-python-1.3.65/kscore/vendored/six.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/hooks.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/__init__.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/certs.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/certs.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/hebrewprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/gb2312freq.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/__init__.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/big5prober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/mbcharsetprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euctwfreq.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langhebrewmodel.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/cp949prober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/jpcntx.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/charsetgroupprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langcyrillicmodel.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/universaldetector.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/mbcsgroupprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langgreekmodel.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/escprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/chardetect.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/chardetect.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/utf8prober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/gb2312prober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/codingstatemachine.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/compat.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/eucjpprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/big5freq.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/constants.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/constants.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langbulgarianmodel.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langhungarianmodel.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/sjisprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/jisfreq.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/sbcsgroupprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euctwprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/langthaimodel.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/charsetprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/sbcharsetprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/mbcssm.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/escsm.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euckrprober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/chardistribution.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/latin1prober.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/chardet/euckrfreq.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/__init__.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/request.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/connectionpool.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/fields.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/six.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/packages/ordered_dict.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/connection.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/_collections.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from collections import Mapping, MutableMapping
+try:
+    from collections import Mapping, MutableMapping
+except ImportError:
+    from collections.abc import Mapping, MutableMapping
+
 try:
     from threading import RLock
 except ImportError:  # Platform-specific: No threads available
     class RLock:
         def __enter__(self):
             pass
```

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/contrib/pyopenssl.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/contrib/ntlmpool.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/exceptions.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/poolmanager.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/response.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/request.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/url.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/connection.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/timeout.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/response.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/retry.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/util/ssl_.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/packages/urllib3/filepost.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/cookies.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/cookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 requests.utils imports from here, so be careful with imports.
 """
 
 import copy
 import time
 import collections
 from .compat import cookielib, urlparse, urlunparse, Morsel
+try:
+    from collections import Mapping, MutableMapping
+except ImportError:
+    from collections.abc import Mapping, MutableMapping
+
+
+
 
 try:
     import threading
     # grr, pyflakes: this fixes "redefinition of unused 'threading'"
     threading
 except ImportError:
     import dummy_threading as threading
@@ -153,15 +160,15 @@
 
 
 class CookieConflictError(RuntimeError):
     """There are two cookies that meet the criteria specified in the cookie jar.
     Use .get and .set and include domain and path args in order to be more specific."""
 
 
-class RequestsCookieJar(cookielib.CookieJar, collections.MutableMapping):
+class RequestsCookieJar(cookielib.CookieJar, MutableMapping):
     """Compatibility class; is a cookielib.CookieJar, but exposes a dict
     interface.
 
     This is the CookieJar we create by default for requests and sessions that
     don't specify one, since some clients may expect response.cookies and
     session.cookies to support dict operations.
```

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/exceptions.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/cacert.pem` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/cacert.pem`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/status_codes.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/sessions.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 ~~~~~~~~~~~~~~~~
 
 This module provides a Session object to manage and persist settings across
 requests (cookies, auth, proxies).
 
 """
 import os
-from collections import Mapping
+# from collections import Mapping
+try:
+    from collections import Mapping, MutableMapping
+except ImportError:
+    from collections.abc import Mapping, MutableMapping
+
+
+
 from datetime import datetime
 
 from .auth import _basic_auth_str
 from .compat import cookielib, OrderedDict, urljoin, urlparse
 from .cookies import (
     cookiejar_from_dict, extract_cookies_to_jar, RequestsCookieJar, merge_cookies)
 from .models import Request, PreparedRequest, DEFAULT_REDIRECT_LIMIT
```

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/api.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/compat.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/models.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/auth.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/utils.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,21 @@
 from .compat import (quote, urlparse, bytes, str, OrderedDict, unquote, is_py2,
                      builtin_str, getproxies, proxy_bypass, urlunparse,
                      basestring)
 from .cookies import RequestsCookieJar, cookiejar_from_dict
 from .structures import CaseInsensitiveDict
 from .exceptions import InvalidURL
 
+try:
+    from collections import Mapping, MutableMapping
+except ImportError:
+    from collections.abc import Mapping, MutableMapping
+
+
+
 _hush_pyflakes = (RequestsCookieJar,)
 
 NETRC_FILES = ('.netrc', '_netrc')
 
 DEFAULT_CA_BUNDLE_PATH = certs.where()
 
 
@@ -159,15 +166,15 @@
     """
     if value is None:
         return None
 
     if isinstance(value, (str, bytes, bool, int)):
         raise ValueError('cannot encode objects that are not 2-tuples')
 
-    if isinstance(value, collections.Mapping):
+    if isinstance(value, Mapping):
         value = value.items()
 
     return list(value)
 
 
 # From mitsuhiko/werkzeug (used with permission).
 def parse_list_header(value):
```

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/adapters.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/vendored/requests/structures.py` & `ksc-sdk-python-1.3.65/kscore/vendored/requests/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 ~~~~~~~~~~~~~~~~~~~
 
 Data structures that power Requests.
 
 """
 
 import collections
+try:
+    from collections import Mapping, MutableMapping
+except ImportError:
+    from collections.abc import Mapping, MutableMapping
 
 
-class CaseInsensitiveDict(collections.MutableMapping):
+
+class CaseInsensitiveDict(MutableMapping):
     """
     A case-insensitive ``dict``-like object.
 
     Implements all methods and operations of
     ``collections.MutableMapping`` as well as dict's ``copy``. Also
     provides ``lower_items``.
```

### Comparing `ksc-sdk-python-1.3.64/kscore/retryhandler.py` & `ksc-sdk-python-1.3.65/kscore/retryhandler.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/hooks.py` & `ksc-sdk-python-1.3.65/kscore/hooks.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/credentials.py` & `ksc-sdk-python-1.3.65/kscore/credentials.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/regions.py` & `ksc-sdk-python-1.3.65/kscore/regions.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/__init__.py` & `ksc-sdk-python-1.3.65/kscore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
 import re
 import logging
 
-__version__ = '1.3.64'
+__version__ = '1.3.65'
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
 
 # Configure default logger to do nothing
```

### Comparing `ksc-sdk-python-1.3.64/kscore/offline.py` & `ksc-sdk-python-1.3.65/kscore/offline.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/endpoint.py` & `ksc-sdk-python-1.3.65/kscore/endpoint.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/kls.py` & `ksc-sdk-python-1.3.65/kscore/kls.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/client.py` & `ksc-sdk-python-1.3.65/kscore/client.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/paginate.py` & `ksc-sdk-python-1.3.65/kscore/paginate.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/config.py` & `ksc-sdk-python-1.3.65/kscore/config.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/exceptions.py` & `ksc-sdk-python-1.3.65/kscore/exceptions.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/kvs.py` & `ksc-sdk-python-1.3.65/kscore/kvs.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/response.py` & `ksc-sdk-python-1.3.65/kscore/response.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/waiter.py` & `ksc-sdk-python-1.3.65/kscore/waiter.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/ksrequest.py` & `ksc-sdk-python-1.3.65/kscore/ksrequest.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/compat.py` & `ksc-sdk-python-1.3.65/kscore/compat.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/ket.py` & `ksc-sdk-python-1.3.65/kscore/ket.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/auth.py` & `ksc-sdk-python-1.3.65/kscore/auth.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/__init__.py` & `ksc-sdk-python-1.3.65/kscore/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/client.py` & `ksc-sdk-python-1.3.65/kscore/docs/client.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/params.py` & `ksc-sdk-python-1.3.65/kscore/docs/params.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/docstring.py` & `ksc-sdk-python-1.3.65/kscore/docs/docstring.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/service.py` & `ksc-sdk-python-1.3.65/kscore/docs/service.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/example.py` & `ksc-sdk-python-1.3.65/kscore/docs/example.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/bcdoc/__init__.py` & `ksc-sdk-python-1.3.65/kscore/docs/bcdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/bcdoc/docevents.py` & `ksc-sdk-python-1.3.65/kscore/docs/bcdoc/docevents.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/bcdoc/textwriter.py` & `ksc-sdk-python-1.3.65/kscore/docs/bcdoc/textwriter.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/bcdoc/docstringparser.py` & `ksc-sdk-python-1.3.65/kscore/docs/bcdoc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/bcdoc/style.py` & `ksc-sdk-python-1.3.65/kscore/docs/bcdoc/style.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/bcdoc/restdoc.py` & `ksc-sdk-python-1.3.65/kscore/docs/bcdoc/restdoc.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/waiter.py` & `ksc-sdk-python-1.3.65/kscore/docs/waiter.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/utils.py` & `ksc-sdk-python-1.3.65/kscore/docs/utils.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/shape.py` & `ksc-sdk-python-1.3.65/kscore/docs/shape.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/paginator.py` & `ksc-sdk-python-1.3.65/kscore/docs/paginator.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/sharedexample.py` & `ksc-sdk-python-1.3.65/kscore/docs/sharedexample.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/docs/method.py` & `ksc-sdk-python-1.3.65/kscore/docs/method.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/signers.py` & `ksc-sdk-python-1.3.65/kscore/signers.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/utils.py` & `ksc-sdk-python-1.3.65/kscore/utils.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/handlers.py` & `ksc-sdk-python-1.3.65/kscore/handlers.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/parsers.py` & `ksc-sdk-python-1.3.65/kscore/parsers.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/session.py` & `ksc-sdk-python-1.3.65/kscore/session.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/serialize.py` & `ksc-sdk-python-1.3.65/kscore/serialize.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/offline/2016-09-19/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/offline/2016-09-19/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kec/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kec/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/cdnv2/2018-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/cdnv2/2018-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/vpc/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/vpc/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/ket/2017-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/ket/2017-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/_retry.yaml` & `ksc-sdk-python-1.3.65/kscore/data/_retry.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kvs/2017-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kvs/2017-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/bill-union/2020-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/bill-union/2020-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/monitor/2010-05-25/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/monitor/2010-05-25/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/ebs/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/ebs/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kis/2018-09-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kis/2018-09-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/endpoints.yaml` & `ksc-sdk-python-1.3.65/kscore/data/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/slb/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/slb/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/monitorv2/2021-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/monitorv2/2021-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/krds/2016-07-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/krds/2016-07-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/postgresql/2018-12-25/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/postgresql/2018-12-25/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/cdn/2016-09-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/cdn/2016-09-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kkms/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kkms/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/iam/2015-11-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/iam/2015-11-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kmr/2021-09-02/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kmr/2021-09-02/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/eip/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/eip/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kcm/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kcm/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kls/2017-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kls/2017-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/bws/2016-03-04/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/bws/2016-03-04/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/sks/2015-11-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/sks/2015-11-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kes/2020-12-15/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kes/2020-12-15/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kce/2019-08-06/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kce/2019-08-06/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/dns/2016-06-07/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/dns/2016-06-07/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/epc/2015-11-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/epc/2015-11-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kcsv2/2017-04-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kcsv2/2017-04-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/mongodb/2017-01-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/mongodb/2017-01-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/cdnv3/2020-06-30/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/cdnv3/2020-06-30/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kcs/2016-07-01/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kcs/2016-07-01/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kcrs/2021-11-09/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kcrs/2021-11-09/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/data/kog/2016-08-08/service-2.yaml` & `ksc-sdk-python-1.3.65/kscore/data/kog/2016-08-08/service-2.yaml`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/model.py` & `ksc-sdk-python-1.3.65/kscore/model.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/loaders.py` & `ksc-sdk-python-1.3.65/kscore/loaders.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/validate.py` & `ksc-sdk-python-1.3.65/kscore/validate.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/translate.py` & `ksc-sdk-python-1.3.65/kscore/translate.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/domain.py` & `ksc-sdk-python-1.3.65/kscore/domain.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/configloader.py` & `ksc-sdk-python-1.3.65/kscore/configloader.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/kscore/stub.py` & `ksc-sdk-python-1.3.65/kscore/stub.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/README.rst` & `ksc-sdk-python-1.3.65/README.rst`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/PKG-INFO` & `ksc-sdk-python-1.3.65/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ksc-sdk-python
-Version: 1.3.64
+Version: 1.3.65
 Summary: Low-level, data-driven core of ksc.
 Home-page: https://github.com/KscSDK/ksc-sdk-python
 Author: liuyichen,xuyaming,ksc_online_sdk
 Author-email: ksc_sdk@kingsoft.com,xuyaming@kingsoft.com,ksc_online_sdk@kingsoft.com
 License: Apache License 2.0
 Description: A low-level interface to a growing number of KSC Web Services.
 Platform: UNKNOWN
```

### Comparing `ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/PKG-INFO` & `ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ksc-sdk-python
-Version: 1.3.64
+Version: 1.3.65
 Summary: Low-level, data-driven core of ksc.
 Home-page: https://github.com/KscSDK/ksc-sdk-python
 Author: liuyichen,xuyaming,ksc_online_sdk
 Author-email: ksc_sdk@kingsoft.com,xuyaming@kingsoft.com,ksc_online_sdk@kingsoft.com
 License: Apache License 2.0
 Description: A low-level interface to a growing number of KSC Web Services.
 Platform: UNKNOWN
```

### Comparing `ksc-sdk-python-1.3.64/ksc_sdk_python.egg-info/SOURCES.txt` & `ksc-sdk-python-1.3.65/ksc_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/setup.py` & `ksc-sdk-python-1.3.65/setup.py`

 * *Files identical despite different names*

### Comparing `ksc-sdk-python-1.3.64/LICENSE.txt` & `ksc-sdk-python-1.3.65/LICENSE.txt`

 * *Files identical despite different names*

