# Comparing `tmp/gempyp-1.0.90b1.tar.gz` & `tmp/gempyp-1.0.90b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempyp-1.0.90b1.tar", max compression
+gzip compressed data, was "gempyp-1.0.90b2.tar", max compression
```

## Comparing `gempyp-1.0.90b1.tar` & `gempyp-1.0.90b2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0       25 2024-03-05 12:04:13.028632 gempyp-1.0.90b1/gempyp/__init__.py
--rw-r--r--   0        0        0      108 2024-03-05 12:04:13.028632 gempyp-1.0.90b1/gempyp/cli.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.037550 gempyp-1.0.90b1/gempyp/config/__init__.py
--rw-r--r--   0        0        0     7753 2024-03-05 12:04:13.037550 gempyp-1.0.90b1/gempyp/config/baseConfig.py
--rw-r--r--   0        0        0      198 2024-03-05 12:04:13.037550 gempyp-1.0.90b1/gempyp/config/customParser.py
--rw-r--r--   0        0        0     1827 2024-03-05 12:04:13.028632 gempyp-1.0.90b1/gempyp/config/DefaultSettings.py
--rw-r--r--   0        0        0       62 2024-03-05 12:04:13.037550 gempyp-1.0.90b1/gempyp/config/gempyp.conf
--rw-r--r--   0        0        0     2145 2024-03-05 12:04:13.037550 gempyp-1.0.90b1/gempyp/config/GitLinkXML.py
--rw-r--r--   0        0        0    21143 2024-03-05 12:04:13.037550 gempyp-1.0.90b1/gempyp/config/Result.html
--rw-r--r--   0        0        0       26 2024-03-05 12:04:13.045801 gempyp-1.0.90b1/gempyp/config/suite_conf.json
--rw-r--r--   0        0        0       28 2024-03-05 12:04:13.046015 gempyp-1.0.90b1/gempyp/config/testcase_conf.json
--rw-r--r--   0        0        0     8234 2024-03-05 12:04:13.046015 gempyp-1.0.90b1/gempyp/config/xmlConfig.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.046015 gempyp-1.0.90b1/gempyp/data_compare/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.046015 gempyp-1.0.90b1/gempyp/data_compare/common/__init__.py
--rw-r--r--   0        0        0     3627 2024-03-05 12:04:13.046015 gempyp-1.0.90b1/gempyp/data_compare/common/common_functions.py
--rw-r--r--   0        0        0      956 2024-03-05 12:04:13.046015 gempyp-1.0.90b1/gempyp/data_compare/compare.py
--rw-r--r--   0        0        0      149 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/config/dvm.json
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/configurator/__init__.py
--rw-r--r--   0        0        0     4635 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/configurator/configurator.py
--rw-r--r--   0        0        0      320 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/configurator/validator.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/core/__init__.py
--rw-r--r--   0        0        0      589 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/core/comparator.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.054667 gempyp-1.0.90b1/gempyp/data_compare/core/Compare.py
--rw-r--r--   0        0        0    10157 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/core/python_obj_comparator.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/data/__init__.py
--rw-r--r--   0        0        0     5498 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/data/data.py
--rw-r--r--   0        0        0      869 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/data/database.py
--rw-r--r--   0        0        0     1903 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/data/db_mysql.py
--rw-r--r--   0        0        0     2646 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/data/db_oracle.py
--rw-r--r--   0        0        0     2436 2024-03-05 12:04:13.063154 gempyp-1.0.90b1/gempyp/data_compare/data/db_postgre.py
--rw-r--r--   0        0        0     1999 2024-03-05 12:04:13.071751 gempyp-1.0.90b1/gempyp/data_compare/data/db_sqlite.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.071751 gempyp-1.0.90b1/gempyp/data_compare/data/file_processor.py
--rw-r--r--   0        0        0    11161 2024-03-05 12:04:13.071751 gempyp-1.0.90b1/gempyp/data_compare/data_comp.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.071751 gempyp-1.0.90b1/gempyp/data_compare/report/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.071751 gempyp-1.0.90b1/gempyp/data_compare/tools/__init__.py
--rw-r--r--   0        0        0     6758 2024-03-05 12:04:13.071751 gempyp-1.0.90b1/gempyp/data_uploader.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.080438 gempyp-1.0.90b1/gempyp/dv/__init__.py
--rw-r--r--   0        0        0     2286 2024-03-05 12:04:13.080438 gempyp-1.0.90b1/gempyp/dv/dfOperations.py
--rw-r--r--   0        0        0    10231 2024-03-05 12:04:13.080438 gempyp-1.0.90b1/gempyp/dv/dvCompare.py
--rw-r--r--   0        0        0      682 2024-03-05 12:04:13.080438 gempyp-1.0.90b1/gempyp/dv/dvDatabases.py
--rw-r--r--   0        0        0    10760 2024-03-05 12:04:13.080438 gempyp-1.0.90b1/gempyp/dv/dvDataframe.py
--rw-r--r--   0        0        0     1441 2024-03-05 12:04:13.088800 gempyp-1.0.90b1/gempyp/dv/dvObj.py
--rw-r--r--   0        0        0     3789 2024-03-05 12:04:13.088800 gempyp-1.0.90b1/gempyp/dv/dvReporting.py
--rw-r--r--   0        0        0    23225 2024-03-05 12:04:13.088800 gempyp-1.0.90b1/gempyp/dv/dvRunner.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.088800 gempyp-1.0.90b1/gempyp/engine/__init__.py
--rw-r--r--   0        0        0     5092 2024-03-05 12:04:13.094329 gempyp-1.0.90b1/gempyp/engine/baseTemplate.py
--rw-r--r--   0        0        0     8421 2024-03-05 12:04:13.094329 gempyp-1.0.90b1/gempyp/engine/dataUpload.py
--rw-r--r--   0        0        0    51385 2024-03-05 12:04:50.432412 gempyp-1.0.90b1/gempyp/engine/engine.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.094329 gempyp-1.0.90b1/gempyp/engine/executors/__init__.py
--rw-r--r--   0        0        0      443 2024-03-05 12:04:13.102618 gempyp-1.0.90b1/gempyp/engine/executors/baseExecutor.py
--rw-r--r--   0        0        0      656 2024-03-05 12:04:13.102618 gempyp-1.0.90b1/gempyp/engine/gempypHelper.py
--rw-r--r--   0        0        0     5483 2024-03-05 12:04:13.102618 gempyp-1.0.90b1/gempyp/engine/runner.py
--rw-r--r--   0        0        0     5533 2024-03-05 12:04:13.102618 gempyp-1.0.90b1/gempyp/engine/simpleTestcase.py
--rw-r--r--   0        0        0    12428 2024-03-05 12:04:13.102618 gempyp-1.0.90b1/gempyp/engine/testData.py
--rw-r--r--   0        0        0    64741 2024-03-05 12:04:13.102618 gempyp-1.0.90b1/gempyp/final_report.html
--rw-r--r--   0        0        0     5666 2024-03-05 12:04:13.110730 gempyp-1.0.90b1/gempyp/gemPyp.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.110730 gempyp-1.0.90b1/gempyp/jira/__init__.py
--rw-r--r--   0        0        0     2312 2024-03-05 12:04:13.110730 gempyp-1.0.90b1/gempyp/jira/jiraIntegration.py
--rw-r--r--   0        0        0     4474 2024-03-05 12:04:13.110730 gempyp-1.0.90b1/gempyp/jira/jiraIntegrationCopy.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.110730 gempyp-1.0.90b1/gempyp/libs/__init__.py
--rw-r--r--   0        0        0     9235 2024-03-05 12:04:13.110730 gempyp-1.0.90b1/gempyp/libs/common.py
--rw-r--r--   0        0        0      131 2024-03-05 12:04:13.119040 gempyp-1.0.90b1/gempyp/libs/enums/run_types.py
--rw-r--r--   0        0        0      318 2024-03-05 12:04:13.119040 gempyp-1.0.90b1/gempyp/libs/enums/status.py
--rw-r--r--   0        0        0       47 2024-03-05 12:04:13.119040 gempyp-1.0.90b1/gempyp/libs/exceptions/__init__.py
--rw-r--r--   0        0        0     4352 2024-03-05 12:04:13.119040 gempyp-1.0.90b1/gempyp/libs/gem_s3_common.py
--rw-r--r--   0        0        0     2642 2024-03-05 12:04:13.119040 gempyp-1.0.90b1/gempyp/libs/logConfig.py
--rw-r--r--   0        0        0     1465 2024-03-05 12:04:13.119040 gempyp-1.0.90b1/gempyp/libs/parsers.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.127772 gempyp-1.0.90b1/gempyp/pyprest/__init__.py
--rw-r--r--   0        0        0     7073 2024-03-05 12:04:13.127772 gempyp-1.0.90b1/gempyp/pyprest/apiCommon.py
--rw-r--r--   0        0        0      491 2024-03-05 12:04:13.127772 gempyp-1.0.90b1/gempyp/pyprest/beforeAfterSample.py
--rw-r--r--   0        0        0    14102 2024-03-05 12:04:13.127772 gempyp-1.0.90b1/gempyp/pyprest/compareFunctions.py
--rw-r--r--   0        0        0    13569 2024-03-05 12:04:13.127772 gempyp-1.0.90b1/gempyp/pyprest/keyCheck.py
--rw-r--r--   0        0        0    15661 2024-03-05 12:04:13.136447 gempyp-1.0.90b1/gempyp/pyprest/legacyComparison.py
--rw-r--r--   0        0        0     1933 2024-03-05 12:04:13.136447 gempyp-1.0.90b1/gempyp/pyprest/miscVariables.py
--rw-r--r--   0        0        0    10827 2024-03-05 12:04:50.432412 gempyp-1.0.90b1/gempyp/pyprest/postAssertion.py
--rw-r--r--   0        0        0     5987 2024-03-05 12:04:13.136447 gempyp-1.0.90b1/gempyp/pyprest/postVariables.py
--rw-r--r--   0        0        0     8271 2024-03-05 12:04:13.144855 gempyp-1.0.90b1/gempyp/pyprest/predefinedFunctions.py
--rw-r--r--   0        0        0     4388 2024-03-05 12:04:13.136447 gempyp-1.0.90b1/gempyp/pyprest/preVariables.py
--rw-r--r--   0        0        0    38424 2024-03-05 12:04:50.432412 gempyp-1.0.90b1/gempyp/pyprest/pypRest.py
--rw-r--r--   0        0        0     4432 2024-03-05 12:04:13.144855 gempyp-1.0.90b1/gempyp/pyprest/reporting.py
--rw-r--r--   0        0        0     2725 2024-03-05 12:04:13.144855 gempyp-1.0.90b1/gempyp/pyprest/restEngine.py
--rw-r--r--   0        0        0     1031 2024-03-05 12:04:13.144855 gempyp-1.0.90b1/gempyp/pyprest/restObj.py
--rw-r--r--   0        0        0     6308 2024-03-05 12:04:13.154148 gempyp-1.0.90b1/gempyp/pyprest/utils.py
--rw-r--r--   0        0        0     6157 2024-03-05 12:04:13.154148 gempyp-1.0.90b1/gempyp/pyprest/variableReplacement.py
--rw-r--r--   0        0        0        0 2024-03-05 12:04:13.154148 gempyp-1.0.90b1/gempyp/reporter/__init__.py
--rw-r--r--   0        0        0     8517 2024-03-05 12:04:13.154148 gempyp-1.0.90b1/gempyp/reporter/reportGenerator.py
--rw-r--r--   0        0        0    13032 2024-03-05 12:04:13.154148 gempyp-1.0.90b1/gempyp/sdk/executor.py
--rw-r--r--   0        0        0     2490 2024-03-05 12:04:13.162922 gempyp-1.0.90b1/gempyp/sdk/worker.py
--rw-r--r--   0        0        0    11547 2024-03-05 12:04:13.162922 gempyp-1.0.90b1/gempyp/testcase.html
--rw-r--r--   0        0        0        2 2024-03-05 12:04:13.011117 gempyp-1.0.90b1/LICENSE
--rw-r--r--   0        0        0     1431 2024-03-06 06:26:11.781049 gempyp-1.0.90b1/pyproject.toml
--rw-r--r--   0        0        0     3161 2024-03-05 12:04:13.011117 gempyp-1.0.90b1/README.md
--rw-r--r--   0        0        0     4992 1970-01-01 00:00:00.000000 gempyp-1.0.90b1/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/cli.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/__init__.py
+-rw-r--r--   0        0        0     7753 2024-04-23 05:32:45.965360 gempyp-1.0.90b2/gempyp/config/baseConfig.py
+-rw-r--r--   0        0        0      198 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/customParser.py
+-rw-r--r--   0        0        0     2226 2024-05-06 10:31:27.228674 gempyp-1.0.90b2/gempyp/config/DefaultSettings.py
+-rw-r--r--   0        0        0       62 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/gempyp.conf
+-rw-r--r--   0        0        0     2145 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/GitLinkXML.py
+-rw-r--r--   0        0        0    21143 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/Result.html
+-rw-r--r--   0        0        0       26 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/suite_conf.json
+-rw-r--r--   0        0        0       28 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/config/testcase_conf.json
+-rw-r--r--   0        0        0     8234 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/config/xmlConfig.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/data_compare/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/data_compare/common/__init__.py
+-rw-r--r--   0        0        0     3627 2024-04-23 05:31:05.678699 gempyp-1.0.90b2/gempyp/data_compare/common/common_functions.py
+-rw-r--r--   0        0        0      956 2024-04-23 05:31:05.693479 gempyp-1.0.90b2/gempyp/data_compare/compare.py
+-rw-r--r--   0        0        0      149 2024-04-23 05:31:05.694480 gempyp-1.0.90b2/gempyp/data_compare/config/dvm.json
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/configurator/__init__.py
+-rw-r--r--   0        0        0     4635 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/configurator/configurator.py
+-rw-r--r--   0        0        0      320 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/configurator/validator.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/core/__init__.py
+-rw-r--r--   0        0        0      589 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/core/comparator.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/core/Compare.py
+-rw-r--r--   0        0        0    10157 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/core/python_obj_comparator.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/__init__.py
+-rw-r--r--   0        0        0     5498 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/data.py
+-rw-r--r--   0        0        0      869 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/database.py
+-rw-r--r--   0        0        0     1903 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/db_mysql.py
+-rw-r--r--   0        0        0     2646 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/db_oracle.py
+-rw-r--r--   0        0        0     2436 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/db_postgre.py
+-rw-r--r--   0        0        0     1999 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/db_sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data/file_processor.py
+-rw-r--r--   0        0        0    11161 2024-04-23 05:31:05.695706 gempyp-1.0.90b2/gempyp/data_compare/data_comp.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711228 gempyp-1.0.90b2/gempyp/data_compare/report/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/data_compare/tools/__init__.py
+-rw-r--r--   0        0        0     6758 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/data_uploader.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/dv/__init__.py
+-rw-r--r--   0        0        0     2286 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/dv/dfOperations.py
+-rw-r--r--   0        0        0    10231 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/dv/dvCompare.py
+-rw-r--r--   0        0        0      682 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/dv/dvDatabases.py
+-rw-r--r--   0        0        0    10760 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/dv/dvDataframe.py
+-rw-r--r--   0        0        0     1441 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/dv/dvObj.py
+-rw-r--r--   0        0        0     3789 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/dv/dvReporting.py
+-rw-r--r--   0        0        0    23225 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/dv/dvRunner.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/engine/__init__.py
+-rw-r--r--   0        0        0     5092 2024-04-23 05:31:05.711975 gempyp-1.0.90b2/gempyp/engine/baseTemplate.py
+-rw-r--r--   0        0        0     8421 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/engine/dataUpload.py
+-rw-r--r--   0        0        0    51385 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/engine/engine.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.728857 gempyp-1.0.90b2/gempyp/engine/executors/__init__.py
+-rw-r--r--   0        0        0      443 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/engine/executors/baseExecutor.py
+-rw-r--r--   0        0        0      656 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/engine/gempypHelper.py
+-rw-r--r--   0        0        0     5483 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/engine/runner.py
+-rw-r--r--   0        0        0     5533 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/engine/simpleTestcase.py
+-rw-r--r--   0        0        0    12428 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/engine/testData.py
+-rw-r--r--   0        0        0    64741 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/final_report.html
+-rw-r--r--   0        0        0     5666 2024-04-23 05:32:45.980999 gempyp-1.0.90b2/gempyp/gemPyp.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/jira/__init__.py
+-rw-r--r--   0        0        0     2312 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/jira/jiraIntegration.py
+-rw-r--r--   0        0        0     4474 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/jira/jiraIntegrationCopy.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.729072 gempyp-1.0.90b2/gempyp/libs/__init__.py
+-rw-r--r--   0        0        0     9328 2024-04-23 05:37:15.962177 gempyp-1.0.90b2/gempyp/libs/common.py
+-rw-r--r--   0        0        0      131 2024-04-23 05:31:05.743503 gempyp-1.0.90b2/gempyp/libs/enums/run_types.py
+-rw-r--r--   0        0        0      318 2024-04-23 05:31:05.744504 gempyp-1.0.90b2/gempyp/libs/enums/status.py
+-rw-r--r--   0        0        0       47 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/libs/exceptions/__init__.py
+-rw-r--r--   0        0        0     4352 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/libs/gem_s3_common.py
+-rw-r--r--   0        0        0     2642 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/libs/logConfig.py
+-rw-r--r--   0        0        0     1465 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/libs/parsers.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/pyprest/__init__.py
+-rw-r--r--   0        0        0     7073 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/apiCommon.py
+-rw-r--r--   0        0        0      491 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/pyprest/beforeAfterSample.py
+-rw-r--r--   0        0        0    14091 2024-04-23 06:32:44.195355 gempyp-1.0.90b2/gempyp/pyprest/compareFunctions.py
+-rw-r--r--   0        0        0    13569 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/keyCheck.py
+-rw-r--r--   0        0        0    15661 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/pyprest/legacyComparison.py
+-rw-r--r--   0        0        0     1933 2024-04-23 05:31:05.745590 gempyp-1.0.90b2/gempyp/pyprest/miscVariables.py
+-rw-r--r--   0        0        0    10827 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/postAssertion.py
+-rw-r--r--   0        0        0     5987 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/postVariables.py
+-rw-r--r--   0        0        0     8271 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/pyprest/predefinedFunctions.py
+-rw-r--r--   0        0        0     4388 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/preVariables.py
+-rw-r--r--   0        0        0    38424 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/pypRest.py
+-rw-r--r--   0        0        0     4432 2024-04-23 05:32:45.996783 gempyp-1.0.90b2/gempyp/pyprest/reporting.py
+-rw-r--r--   0        0        0     2725 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/pyprest/restEngine.py
+-rw-r--r--   0        0        0     1031 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/pyprest/restObj.py
+-rw-r--r--   0        0        0     6308 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/pyprest/utils.py
+-rw-r--r--   0        0        0     6157 2024-04-23 05:32:46.012474 gempyp-1.0.90b2/gempyp/pyprest/variableReplacement.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/reporter/__init__.py
+-rw-r--r--   0        0        0     8517 2024-04-23 05:32:46.012474 gempyp-1.0.90b2/gempyp/reporter/reportGenerator.py
+-rw-r--r--   0        0        0    13032 2024-04-23 05:32:46.012474 gempyp-1.0.90b2/gempyp/sdk/executor.py
+-rw-r--r--   0        0        0     2490 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/sdk/worker.py
+-rw-r--r--   0        0        0    11547 2024-04-23 05:31:05.762677 gempyp-1.0.90b2/gempyp/testcase.html
+-rw-r--r--   0        0        0        2 2024-04-23 05:31:05.660636 gempyp-1.0.90b2/LICENSE
+-rw-r--r--   0        0        0     1431 2024-05-06 10:29:53.374013 gempyp-1.0.90b2/pyproject.toml
+-rw-r--r--   0        0        0     3161 2024-04-23 05:31:05.660636 gempyp-1.0.90b2/README.md
+-rw-r--r--   0        0        0     4992 1970-01-01 00:00:00.000000 gempyp-1.0.90b2/PKG-INFO
```

### Comparing `gempyp-1.0.90b1/gempyp/config/baseConfig.py` & `gempyp-1.0.90b2/gempyp/config/baseConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/config/DefaultSettings.py` & `gempyp-1.0.90b2/gempyp/config/DefaultSettings.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,20 +24,26 @@
         if response.status_code == 200:
             url_enter_point = response.json()
             urls["data"]=url_enter_point["data"]
             global apiSuccess
             apiSuccess = True
         elif re.search('50[0-9]',str(response.status_code)):
             logging.warning("Error Occurs While Getting the BASE_URLs")
+            logging.warning("Response status code: "+response.status_code)
+            logging.warning("Response: "+response.text)
         else:
             logging.info("Some Error From the Client Side, Maybe username or bridgeToken, Therefore terminating execution")
+            logging.warning("Response status code: "+response.status_code)
+            logging.warning("Response: "+response.text)
             sys.exit()
     except Exception as e:
             traceback.print_exc()
             logging.warning("Error Occurs While Getting the BASE_URLs")
+            logging.warning("Response status code: "+response.status_code)
+            logging.warning("Response: "+response.text)
             sys.exit()
 
 # for sending urls to dataupload file
 def getUrls(apiName):
     return urls["data"].get(apiName, None)
 
 def checkUrl(url):
```

### Comparing `gempyp-1.0.90b1/gempyp/config/GitLinkXML.py` & `gempyp-1.0.90b2/gempyp/config/GitLinkXML.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/config/Result.html` & `gempyp-1.0.90b2/gempyp/config/Result.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/config/xmlConfig.py` & `gempyp-1.0.90b2/gempyp/config/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/common/common_functions.py` & `gempyp-1.0.90b2/gempyp/data_compare/common/common_functions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/compare.py` & `gempyp-1.0.90b2/gempyp/data_compare/compare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/configurator/configurator.py` & `gempyp-1.0.90b2/gempyp/data_compare/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/core/comparator.py` & `gempyp-1.0.90b2/gempyp/data_compare/core/comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/core/python_obj_comparator.py` & `gempyp-1.0.90b2/gempyp/data_compare/core/python_obj_comparator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data/data.py` & `gempyp-1.0.90b2/gempyp/data_compare/data/data.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data/database.py` & `gempyp-1.0.90b2/gempyp/data_compare/data/database.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data/db_mysql.py` & `gempyp-1.0.90b2/gempyp/data_compare/data/db_mysql.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data/db_oracle.py` & `gempyp-1.0.90b2/gempyp/data_compare/data/db_oracle.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data/db_postgre.py` & `gempyp-1.0.90b2/gempyp/data_compare/data/db_postgre.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data/db_sqlite.py` & `gempyp-1.0.90b2/gempyp/data_compare/data/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_compare/data_comp.py` & `gempyp-1.0.90b2/gempyp/data_compare/data_comp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/data_uploader.py` & `gempyp-1.0.90b2/gempyp/data_uploader.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dfOperations.py` & `gempyp-1.0.90b2/gempyp/dv/dfOperations.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dvCompare.py` & `gempyp-1.0.90b2/gempyp/dv/dvCompare.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dvDatabases.py` & `gempyp-1.0.90b2/gempyp/dv/dvDatabases.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dvDataframe.py` & `gempyp-1.0.90b2/gempyp/dv/dvDataframe.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dvObj.py` & `gempyp-1.0.90b2/gempyp/dv/dvObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dvReporting.py` & `gempyp-1.0.90b2/gempyp/dv/dvReporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/dv/dvRunner.py` & `gempyp-1.0.90b2/gempyp/dv/dvRunner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/baseTemplate.py` & `gempyp-1.0.90b2/gempyp/engine/baseTemplate.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/dataUpload.py` & `gempyp-1.0.90b2/gempyp/engine/dataUpload.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/engine.py` & `gempyp-1.0.90b2/gempyp/engine/engine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/gempypHelper.py` & `gempyp-1.0.90b2/gempyp/engine/gempypHelper.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/runner.py` & `gempyp-1.0.90b2/gempyp/engine/runner.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/simpleTestcase.py` & `gempyp-1.0.90b2/gempyp/engine/simpleTestcase.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/engine/testData.py` & `gempyp-1.0.90b2/gempyp/engine/testData.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/final_report.html` & `gempyp-1.0.90b2/gempyp/final_report.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/gemPyp.py` & `gempyp-1.0.90b2/gempyp/gemPyp.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/jira/jiraIntegration.py` & `gempyp-1.0.90b2/gempyp/jira/jiraIntegration.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/jira/jiraIntegrationCopy.py` & `gempyp-1.0.90b2/gempyp/jira/jiraIntegrationCopy.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/libs/common.py` & `gempyp-1.0.90b2/gempyp/libs/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,15 @@
     
             #trying rerun of base url api in case of api failure
             if base_url and DefaultSettings.apiSuccess == False:
                 logging.info("Trying to call Api for getting urls")
                 DefaultSettings.getEnterPoint(base_url ,bridgetoken,username)
             if not base_url:
                 DefaultSettings.getEnterPoint(DefaultSettings.default_baseurl ,bridgetoken, username)
+                logging.info("Base_url not found in suite data. Fetching default base_url")
 
 
 def sendMail(s_run_id,mails,bridge_token,username):
     try:
         # payload={"to": mails, "s_run_id": s_run_id}
         mails["s_run_id"]=s_run_id
         response = requests.request(
```

### Comparing `gempyp-1.0.90b1/gempyp/libs/gem_s3_common.py` & `gempyp-1.0.90b2/gempyp/libs/gem_s3_common.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/libs/logConfig.py` & `gempyp-1.0.90b2/gempyp/libs/logConfig.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/libs/parsers.py` & `gempyp-1.0.90b2/gempyp/libs/parsers.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/apiCommon.py` & `gempyp-1.0.90b2/gempyp/pyprest/apiCommon.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/compareFunctions.py` & `gempyp-1.0.90b2/gempyp/pyprest/compareFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     actual_value = key_val_dict.get(key, key)
     if isinstance(actual_value, (int, float)):
         actual_value = str(actual_value)
         exp_value = str(value.strip('"').strip("'"))
     else:
         actual_value = str(actual_value).lower()
-        exp_value = value.strip('"').strip("'").lower()
+        exp_value = value.strip('"').lower()
         if actual_value == value:
             exp_value = value 
         
     if actual_value == exp_value:
         if isLegacyPresent:
             if isLegacyResponse:
                 obj.addRow(f"Running validation for {key}",f"Operator = To",status.PASS, CURRENT_API = "-",LEGACY_API = f"Expected:-- {str(exp_value)} <br> Actual:-- {str(actual_value)} <br>condition satisfied" )
```

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/keyCheck.py` & `gempyp-1.0.90b2/gempyp/pyprest/keyCheck.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/legacyComparison.py` & `gempyp-1.0.90b2/gempyp/pyprest/legacyComparison.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/miscVariables.py` & `gempyp-1.0.90b2/gempyp/pyprest/miscVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/postAssertion.py` & `gempyp-1.0.90b2/gempyp/pyprest/postAssertion.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/postVariables.py` & `gempyp-1.0.90b2/gempyp/pyprest/postVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/predefinedFunctions.py` & `gempyp-1.0.90b2/gempyp/pyprest/predefinedFunctions.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/preVariables.py` & `gempyp-1.0.90b2/gempyp/pyprest/preVariables.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/pypRest.py` & `gempyp-1.0.90b2/gempyp/pyprest/pypRest.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/reporting.py` & `gempyp-1.0.90b2/gempyp/pyprest/reporting.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/restEngine.py` & `gempyp-1.0.90b2/gempyp/pyprest/restEngine.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/restObj.py` & `gempyp-1.0.90b2/gempyp/pyprest/restObj.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/utils.py` & `gempyp-1.0.90b2/gempyp/pyprest/utils.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/pyprest/variableReplacement.py` & `gempyp-1.0.90b2/gempyp/pyprest/variableReplacement.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/reporter/reportGenerator.py` & `gempyp-1.0.90b2/gempyp/reporter/reportGenerator.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/sdk/executor.py` & `gempyp-1.0.90b2/gempyp/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/sdk/worker.py` & `gempyp-1.0.90b2/gempyp/sdk/worker.py`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/gempyp/testcase.html` & `gempyp-1.0.90b2/gempyp/testcase.html`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/pyproject.toml` & `gempyp-1.0.90b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gempyp"
-version = "1.0.90b1"
+version = "1.0.90b2"
 description = "An ecosystem of libraries useful for software development"
 authors = ["Gemini Solutions-QA"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gempyp.readthedocs.io/en/latest/"
 homepage = "https://github.com/Gemini-Solutions/gempyp"
 repository = "https://github.com/Gemini-Solutions/gempyp"
@@ -17,19 +17,19 @@
 certifi = "^2022.6.15"
 cffi = "^1.15.0"
 charset-normalizer = "^2.0.12"
 coloredlogs = "^15.0.1"
 cryptography = "^38.0.1"
 humanfriendly = "^10.0"
 idna = "^3.4"
-lxml = "^5.1.0"
+lxml = "^4.9.0"
 mysql-connector-python = "^8.0.30"
 ntlm-auth = "^1.5.0"
-numpy = "^1.24.4"
-pandas = "^1.5.3"
+numpy = "^1.19.5"
+pandas = "^1.1.5"
 pg8000 = "^1.26.0"
 pycparser = "^2.21"
 pyreadline = "^2.1"
 pyreadline3 = "^3.4.1"
 python-dateutil = "^2.8.2"
 pytz = "^2022.2.1"
 requests = "^2.27.1"
```

### Comparing `gempyp-1.0.90b1/README.md` & `gempyp-1.0.90b2/README.md`

 * *Files identical despite different names*

### Comparing `gempyp-1.0.90b1/PKG-INFO` & `gempyp-1.0.90b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gempyp
-Version: 1.0.90b1
+Version: 1.0.90b2
 Summary: An ecosystem of libraries useful for software development
 Home-page: https://github.com/Gemini-Solutions/gempyp
 License: MIT
 Author: Gemini Solutions-QA
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,19 +18,19 @@
 Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
 Requires-Dist: cffi (>=1.15.0,<2.0.0)
 Requires-Dist: charset-normalizer (>=2.0.12,<3.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: cryptography (>=38.0.1,<39.0.0)
 Requires-Dist: humanfriendly (>=10.0,<11.0)
 Requires-Dist: idna (>=3.4,<4.0)
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.30,<9.0.0)
 Requires-Dist: ntlm-auth (>=1.5.0,<2.0.0)
-Requires-Dist: numpy (>=1.24.4,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: numpy (>=1.19.5,<2.0.0)
+Requires-Dist: pandas (>=1.1.5,<2.0.0)
 Requires-Dist: pg8000 (>=1.26.0,<2.0.0)
 Requires-Dist: pycparser (>=2.21,<3.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: pyreadline (>=2.1,<3.0)
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0)
 Requires-Dist: pytest (>=6.2.4,<7.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: gempyp Version: 1.0.90b1 Summary: An ecosystem of
+Metadata-Version: 2.1 Name: gempyp Version: 1.0.90b2 Summary: An ecosystem of
 libraries useful for software development Home-page: https://github.com/Gemini-
 Solutions/gempyp License: MIT Author: Gemini Solutions-QA Requires-Python:
 >=3.6.8,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: XlsxWriter
 (>=3.0.3,<4.0.0) Requires-Dist: certifi (>=2022.6.15,<2023.0.0) Requires-Dist:
 cffi (>=1.15.0,<2.0.0) Requires-Dist: charset-normalizer (>=2.0.12,<3.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0) Requires-Dist: cryptography
 (>=38.0.1,<39.0.0) Requires-Dist: humanfriendly (>=10.0,<11.0) Requires-Dist:
-idna (>=3.4,<4.0) Requires-Dist: lxml (>=5.1.0,<6.0.0) Requires-Dist: mysql-
+idna (>=3.4,<4.0) Requires-Dist: lxml (>=4.9.0,<5.0.0) Requires-Dist: mysql-
 connector-python (>=8.0.30,<9.0.0) Requires-Dist: ntlm-auth (>=1.5.0,<2.0.0)
-Requires-Dist: numpy (>=1.24.4,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: numpy (>=1.19.5,<2.0.0) Requires-Dist: pandas (>=1.1.5,<2.0.0)
 Requires-Dist: pg8000 (>=1.26.0,<2.0.0) Requires-Dist: pycparser (>=2.21,<3.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0) Requires-Dist: pyreadline (>=2.1,<3.0)
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) Requires-Dist: pytest
 (>=6.2.4,<7.0.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist:
 pytz (>=2022.2.1,<2023.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-
 Dist: requests-ntlm (>=1.1.0,<2.0.0) Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: snowflake-connector-python (>=3.0.1,<4.0.0) Requires-Dist:
```

