# Comparing `tmp/cirrus-geo-0.9.0b0.tar.gz` & `tmp/cirrus-geo-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirrus-geo-0.9.0b0.tar", last modified: Tue Nov 15 17:41:04 2022, max compression
+gzip compressed data, was "cirrus-geo-0.9.0rc0.tar", last modified: Wed Nov 16 17:27:12 2022, max compression
```

## Comparing `cirrus-geo-0.9.0b0.tar` & `cirrus-geo-0.9.0rc0.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.037650 cirrus-geo-0.9.0b0/
--rw-r--r--   0 runner    (1001) docker     (121)    11341 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10809 2022-11-15 17:41:04.037650 cirrus-geo-0.9.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10247 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 17:41:04.037650 cirrus-geo-0.9.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/builtins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/basic-compute-environments.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/batch-jobs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/outputs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/resources.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/api.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8124 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/post-batch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/post-batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/post-batch/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/post-batch/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/pre-batch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/pre-batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/pre-batch/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/pre-batch/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8306 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/lambda_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.025650 cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/publish-only/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/publish-only/definition.yml
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/publish-only/test-config.json
--rw-r--r--   0 runner    (1001) docker     (121)     8698 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/publish-only/test-payload.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/cli/utils/logging_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12526 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/mappings.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.029650 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/templates/s3.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/templates/vpc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/core/components/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/core/components/base/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8436 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/base/_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     8491 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/base/component.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/base/step_function.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/feeders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/core/components/files/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/files/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6096 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/files/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/files/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/files/readmes.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/components/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/core/config/
--rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/group_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     7497 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/core/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/json_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/pseudo_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/core/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/10_intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/20_arch.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8291 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/30_payload.rst
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/40_config-deploy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/50_operation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/60_components.rst
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/65_cloudformation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/70_statedb.rst
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/80_monitoring.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/90_examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/docs/components/
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/feeders.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9980 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/lambdas.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/docs/components/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)    32591 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/tasks/batch.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8851 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/tasks/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/batch.rst
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/callbacks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/chaining.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10722 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/examples/e2e-notebook.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.033650 cirrus-geo-0.9.0b0/src/cirrus/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    61726 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/images/arch-overview.png
--rw-r--r--   0 runner    (1001) docker     (121)    32093 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/docs/images/workflow-example.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.037650 cirrus-geo-0.9.0b0/src/cirrus/lib2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7003 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/eventdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    14036 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/process_payload.py
--rw-r--r--   0 runner    (1001) docker     (121)    21946 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/statedb.py
--rw-r--r--   0 runner    (1001) docker     (121)     8984 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/lib2/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-15 17:40:54.000000 cirrus-geo-0.9.0b0/src/cirrus/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:41:04.037650 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10809 2022-11-15 17:41:03.000000 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-11-15 17:41:04.000000 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-15 17:41:03.000000 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-15 17:41:03.000000 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-15 17:41:03.000000 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-15 17:41:03.000000 cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.260119 cirrus-geo-0.9.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11341 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10810 2022-11-16 17:27:12.260119 cirrus-geo-0.9.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10247 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-16 17:27:12.260119 cirrus-geo-0.9.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2678 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.248118 cirrus-geo-0.9.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.248118 cirrus-geo-0.9.0rc0/src/cirrus/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.248118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.248118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/basic-compute-environments.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/batch-jobs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/outputs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     5194 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/resources.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.248118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8124 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1803 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     7402 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/post-batch/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/post-batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/post-batch/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/post-batch/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/pre-batch/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/pre-batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/pre-batch/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/pre-batch/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8306 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/lambda_function.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.248118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/publish-only/
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/publish-only/definition.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/publish-only/test-config.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8698 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/publish-only/test-payload.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4329 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/logging_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.252118 cirrus-geo-0.9.0rc0/src/cirrus/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/templates/s3.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4622 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/templates/vpc.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8436 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8491 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/step_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/feeders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/readmes.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/components/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     4626 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/group_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7497 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/project.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/json_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/pseudo_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5347 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/core/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/10_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/20_arch.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8291 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/30_payload.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/40_config-deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/50_operation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1381 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/60_components.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/65_cloudformation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/70_statedb.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/80_monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/90_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/feeders.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9980 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/lambdas.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/tasks/
+-rw-r--r--   0 runner    (1001) docker     (122)    32591 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/tasks/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8851 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/tasks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     6663 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/callbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/chaining.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10722 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.256119 cirrus-geo-0.9.0rc0/src/cirrus/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/examples/e2e-notebook.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.260119 cirrus-geo-0.9.0rc0/src/cirrus/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (122)    61726 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/images/arch-overview.png
+-rw-r--r--   0 runner    (1001) docker     (122)    32093 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/docs/images/workflow-example.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.260119 cirrus-geo-0.9.0rc0/src/cirrus/lib2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/eventdb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14036 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/process_payload.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22031 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/statedb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8984 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/lib2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2022-11-16 17:27:05.000000 cirrus-geo-0.9.0rc0/src/cirrus/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 17:27:12.260119 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10810 2022-11-16 17:27:12.000000 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5202 2022-11-16 17:27:12.000000 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2022-11-16 17:27:12.000000 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2022-11-16 17:27:12.000000 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-16 17:27:12.000000 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-16 17:27:12.000000 cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/top_level.txt
```

### Comparing `cirrus-geo-0.9.0b0/LICENSE` & `cirrus-geo-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/PKG-INFO` & `cirrus-geo-0.9.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirrus-geo
-Version: 0.9.0b0
+Version: 0.9.0rc0
 Summary: cli for cirrus, a severless STAC-based processing pipeline
 Home-page: https://github.com/cirrus-geo/cirrus
 Author: Matthew Hanson (matthewhanson), Jarrett Keifer (jkeifer), Element 84
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cirrus-geo-0.9.0b0/README.md` & `cirrus-geo-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/setup.py` & `cirrus-geo-0.9.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/basic-compute-environments.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/basic-compute-environments.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/batch-jobs.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/batch-jobs.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/cloudformation/resources.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/cloudformation/resources.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/README.md` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/README.md`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/feeders/feed-rerun/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/feeders/feed-rerun/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/api.yaml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/api.yaml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/api/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/api/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/process/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/process/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/functions/update-state/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/functions/update-state/lambda_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 
 def workflow_completed(execution: Execution) -> None:
     # I think changing the state should be done before
     # trying the sns publish, but I could see it the other
     # way too. If we have issues here we might want to consider
     # a different order/behavior (fail on error or something?).
-    statedb.set_completed(execution.input["id"])
+    statedb.set_completed(execution.input["id"], execution_arn=execution.arn)
     if execution.output:
         with batch_handler(send_batch, {}, "messages", batch_size=10) as handler:
             for next_payload in execution.output.next_payloads():
                 handler.add(json.dumps(next_payload))
 
 
 def workflow_aborted(execution: Execution) -> None:
```

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/post-batch/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/post-batch/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/post-batch/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/post-batch/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/pre-batch/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/pre-batch/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/pre-batch/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/pre-batch/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/README.md` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/README.md`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/tasks/publish/lambda_function.py` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/tasks/publish/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/publish-only/definition.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/publish-only/definition.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/builtins/workflows/publish-only/test-payload.json` & `cirrus-geo-0.9.0rc0/src/cirrus/builtins/workflows/publish-only/test-payload.json`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/cli/commands.py` & `cirrus-geo-0.9.0rc0/src/cirrus/cli/commands.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/cli/utils/click.py` & `cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/click.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/cli/utils/logging.py` & `cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/cli/utils/logging_classes.py` & `cirrus-geo-0.9.0rc0/src/cirrus/cli/utils/logging_classes.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/base.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/base.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/resources.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/resources.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/cloudformation/templates/vpc.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/core/cloudformation/templates/vpc.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/base/_lambda.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/_lambda.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/base/component.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/base/component.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/files/base.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/base.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/files/definitions.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/definitions.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/files/handlers.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/handlers.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/files/readmes.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/files/readmes.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/components/tasks.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/components/tasks.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/config/__init__.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/config/default.yml` & `cirrus-geo-0.9.0rc0/src/cirrus/core/config/default.yml`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/group_meta.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/group_meta.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/groups.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/groups.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/project.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/project.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/utils/json_compare.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/utils/json_compare.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/utils/misc.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/utils/plugins.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/core/utils/yaml.py` & `cirrus-geo-0.9.0rc0/src/cirrus/core/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/10_intro.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/10_intro.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/20_arch.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/20_arch.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/30_payload.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/30_payload.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/40_config-deploy.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/40_config-deploy.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/50_operation.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/50_operation.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/60_components.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/60_components.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/feeders.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/feeders.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/functions.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/functions.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/lambdas.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/lambdas.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/tasks/batch.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/tasks/batch.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/tasks/index.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/tasks/index.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/batch.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/batch.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/chaining.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/chaining.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/definitions.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/definitions.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/components/workflows/index.rst` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/components/workflows/index.rst`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/images/arch-overview.png` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/images/arch-overview.png`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/docs/images/workflow-example.png` & `cirrus-geo-0.9.0rc0/src/cirrus/docs/images/workflow-example.png`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/lib2/eventdb.py` & `cirrus-geo-0.9.0rc0/src/cirrus/lib2/eventdb.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/lib2/logging.py` & `cirrus-geo-0.9.0rc0/src/cirrus/lib2/logging.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/lib2/process_payload.py` & `cirrus-geo-0.9.0rc0/src/cirrus/lib2/process_payload.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/lib2/statedb.py` & `cirrus-geo-0.9.0rc0/src/cirrus/lib2/statedb.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,14 +365,16 @@
             UpdateExpression=expr,
             ExpressionAttributeValues=expr_attrs,
         )
         logger.debug("set completed", extra=key.update({"outputs": outputs}))
 
         if execution_arn:
             self.write_timeseries_record(key, StateEnum.COMPLETED, now, execution_arn)
+        else:
+            logger.debug("set completed called with no execution ARN")
 
         return response
 
     def set_failed(self, payload_id, msg, execution_arn: Optional[str] = None):
         """Adds new item as failed"""
         """ Adds new item with state function execution """
         now = datetime.now(timezone.utc).isoformat()
```

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/lib2/utils.py` & `cirrus-geo-0.9.0rc0/src/cirrus/lib2/utils.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus/test.py` & `cirrus-geo-0.9.0rc0/src/cirrus/test.py`

 * *Files identical despite different names*

### Comparing `cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/PKG-INFO` & `cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirrus-geo
-Version: 0.9.0b0
+Version: 0.9.0rc0
 Summary: cli for cirrus, a severless STAC-based processing pipeline
 Home-page: https://github.com/cirrus-geo/cirrus
 Author: Matthew Hanson (matthewhanson), Jarrett Keifer (jkeifer), Element 84
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cirrus-geo-0.9.0b0/src/cirrus_geo.egg-info/SOURCES.txt` & `cirrus-geo-0.9.0rc0/src/cirrus_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

